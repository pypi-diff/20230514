# Comparing `tmp/sageworks-0.1.5.0.tar.gz` & `tmp/sageworks-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.1.5.0.tar", last modified: Tue May  9 15:35:16 2023, max compression
+gzip compressed data, was "sageworks-0.1.5.1.tar", last modified: Sun May 14 18:57:19 2023, max compression
```

## Comparing `sageworks-0.1.5.0.tar` & `sageworks-0.1.5.1.tar`

### file list

```diff
@@ -1,270 +1,270 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.836481 sageworks-0.1.5.0/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.813758 sageworks-0.1.5.0/.github/
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-04-03 17:04:32.000000 sageworks-0.1.5.0/.github/dependabot.yml
--rw-r--r--   0 briford    (501) staff       (20)     1899 2023-03-25 19:33:37.000000 sageworks-0.1.5.0/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      281 2023-03-28 23:51:00.000000 sageworks-0.1.5.0/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)     1080 2023-02-17 22:10:33.000000 sageworks-0.1.5.0/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1426 2023-04-30 02:31:13.000000 sageworks-0.1.5.0/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     5964 2023-05-09 15:35:16.836568 sageworks-0.1.5.0/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     5231 2023-05-06 21:24:25.000000 sageworks-0.1.5.0/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-04-03 17:04:32.000000 sageworks-0.1.5.0/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.808909 sageworks-0.1.5.0/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.813867 sageworks-0.1.5.0/applications/aws_dashboard/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.814077 sageworks-0.1.5.0/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12244 2023-04-30 02:31:13.000000 sageworks-0.1.5.0/applications/aws_dashboard/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-03-21 14:30:06.000000 sageworks-0.1.5.0/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     1081 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/aws_dashboard.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.814588 sageworks-0.1.5.0/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.815112 sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/
--rw-r--r--   0 briford    (501) staff       (20)     4530 2023-05-09 15:17:31.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)      937 2023-05-09 15:17:31.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)      984 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     1786 2023-05-09 15:17:31.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/main_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4766 2023-05-09 15:17:31.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/models_callbacks.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.815313 sageworks-0.1.5.0/applications/aws_dashboard/pages/data/
--rw-r--r--   0 briford    (501) staff       (20)     1867 2023-04-08 01:44:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/data/toy_data.csv
--rw-r--r--   0 briford    (501) staff       (20)      597 2023-04-05 23:27:13.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/data/toy_scores.json
--rw-r--r--   0 briford    (501) staff       (20)     2372 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/data_sources.py
--rw-r--r--   0 briford    (501) staff       (20)     1434 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     1535 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/feature_sets.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.815828 sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/
--rw-r--r--   0 briford    (501) staff       (20)     1458 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/data_sources_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1143 2023-04-09 22:27:31.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/endpoints_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1286 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/feature_sets_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1584 2023-04-07 15:53:06.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/main_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2436 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/models_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2124 2023-05-09 15:15:28.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/main.py
--rw-r--r--   0 briford    (501) staff       (20)     2556 2023-05-09 15:17:31.000000 sageworks-0.1.5.0/applications/aws_dashboard/pages/models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.816123 sageworks-0.1.5.0/applications/hello_world/
--rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/applications/hello_world/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2158 2023-05-01 19:48:59.000000 sageworks-0.1.5.0/applications/hello_world/hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)     1060 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/applications/hello_world/layout.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.816454 sageworks-0.1.5.0/applications/model_viewer/
--rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/applications/model_viewer/callbacks.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.816647 sageworks-0.1.5.0/applications/model_viewer/data/
--rw-r--r--   0 briford    (501) staff       (20)     1849 2023-03-12 02:23:08.000000 sageworks-0.1.5.0/applications/model_viewer/data/toy_data.csv
--rw-r--r--   0 briford    (501) staff       (20)      597 2023-03-12 02:23:08.000000 sageworks-0.1.5.0/applications/model_viewer/data/toy_scores.json
--rw-r--r--   0 briford    (501) staff       (20)     3069 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/applications/model_viewer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2525 2023-05-09 15:17:31.000000 sageworks-0.1.5.0/applications/model_viewer/model_viewer.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.817055 sageworks-0.1.5.0/applications/web_admin/
--rw-r--r--   0 briford    (501) staff       (20)      213 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/applications/web_admin/flask_test.py
--rw-r--r--   0 briford    (501) staff       (20)      201 2023-03-03 22:18:34.000000 sageworks-0.1.5.0/applications/web_admin/hello-world-http-test.ini
--rw-r--r--   0 briford    (501) staff       (20)      235 2023-03-03 22:19:17.000000 sageworks-0.1.5.0/applications/web_admin/hello-world.ini
--rw-r--r--   0 briford    (501) staff       (20)      399 2023-03-03 22:20:51.000000 sageworks-0.1.5.0/applications/web_admin/hello-world.service
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.817161 sageworks-0.1.5.0/applications/web_admin/nginx_conf/
--rw-r--r--   0 briford    (501) staff       (20)      486 2023-03-03 22:17:39.000000 sageworks-0.1.5.0/applications/web_admin/nginx_conf/nginx.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.817364 sageworks-0.1.5.0/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3315 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     4013 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/aws_setup/build_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.818053 sageworks-0.1.5.0/aws_setup/sageworks_cdk/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1028 2023-04-30 02:31:15.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1291 2023-04-30 16:18:03.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       70 2023-04-30 17:09:37.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.818242 sageworks-0.1.5.0/aws_setup/sageworks_cdk/stacks/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/stacks/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2304 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/stacks/sageworks_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.818339 sageworks-0.1.5.0/aws_setup/sageworks_cdk/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.818500 sageworks-0.1.5.0/aws_setup/sageworks_cdk/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      720 2023-04-30 02:31:15.000000 sageworks-0.1.5.0/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.818615 sageworks-0.1.5.0/config/
--rw-r--r--   0 briford    (501) staff       (20)      147 2023-04-30 02:43:00.000000 sageworks-0.1.5.0/config/sageworks_config.ini
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.819018 sageworks-0.1.5.0/data/
--rw-r--r--   0 briford    (501) staff       (20)   196156 2023-03-26 18:42:12.000000 sageworks-0.1.5.0/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)      829 2023-05-02 22:39:27.000000 sageworks-0.1.5.0/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-04-19 19:55:29.000000 sageworks-0.1.5.0/data/test_data.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.819306 sageworks-0.1.5.0/docs/
--rw-r--r--   0 briford    (501) staff       (20)     1770 2023-03-14 15:41:27.000000 sageworks-0.1.5.0/docs/admin_notes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.821205 sageworks-0.1.5.0/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2022-12-06 17:43:49.000000 sageworks-0.1.5.0/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-01-15 22:00:05.000000 sageworks-0.1.5.0/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-03-06 20:35:02.000000 sageworks-0.1.5.0/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-03-06 20:33:32.000000 sageworks-0.1.5.0/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-03-06 20:31:13.000000 sageworks-0.1.5.0/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-03-06 20:40:25.000000 sageworks-0.1.5.0/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-01-15 21:19:16.000000 sageworks-0.1.5.0/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-03-10 19:48:12.000000 sageworks-0.1.5.0/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-01-15 21:23:57.000000 sageworks-0.1.5.0/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-01-12 16:00:43.000000 sageworks-0.1.5.0/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2022-12-06 17:43:49.000000 sageworks-0.1.5.0/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)      667 2023-03-15 14:00:32.000000 sageworks-0.1.5.0/docs/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2023-03-13 14:45:22.000000 sageworks-0.1.5.0/docs/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.821506 sageworks-0.1.5.0/examples/
--rw-r--r--   0 briford    (501) staff       (20)     1240 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/examples/data_to_data_example.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.821605 sageworks-0.1.5.0/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)   236926 2023-05-06 21:30:24.000000 sageworks-0.1.5.0/notebooks/ML_Pipeline_with_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.822904 sageworks-0.1.5.0/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-04-14 22:52:23.000000 sageworks-0.1.5.0/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-04-14 22:50:14.000000 sageworks-0.1.5.0/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-04-14 23:47:56.000000 sageworks-0.1.5.0/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-04-15 00:30:02.000000 sageworks-0.1.5.0/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-04-15 16:18:02.000000 sageworks-0.1.5.0/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-04-15 16:17:49.000000 sageworks-0.1.5.0/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      211 2023-05-02 03:06:50.000000 sageworks-0.1.5.0/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.823290 sageworks-0.1.5.0/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     1373 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/scripts/data_source_tags.py
--rw-r--r--   0 briford    (501) staff       (20)     1717 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/scripts/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)     1306 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/scripts/list_data_sources.py
--rw-r--r--   0 briford    (501) staff       (20)      527 2023-05-09 15:35:16.837009 sageworks-0.1.5.0/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1787 2023-05-09 15:35:04.000000 sageworks-0.1.5.0/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.809909 sageworks-0.1.5.0/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.823403 sageworks-0.1.5.0/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)      853 2023-04-22 21:03:48.000000 sageworks-0.1.5.0/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.824047 sageworks-0.1.5.0/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.810141 sageworks-0.1.5.0/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.824136 sageworks-0.1.5.0/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-03-05 20:00:31.000000 sageworks-0.1.5.0/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.824238 sageworks-0.1.5.0/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-03-05 19:59:59.000000 sageworks-0.1.5.0/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.810304 sageworks-0.1.5.0/src/sageworks/algorithms/table/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.824339 sageworks-0.1.5.0/src/sageworks/algorithms/table/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      169 2023-03-05 20:04:10.000000 sageworks-0.1.5.0/src/sageworks/algorithms/table/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.824752 sageworks-0.1.5.0/src/sageworks/algorithms/table/light/
--rw-r--r--   0 briford    (501) staff       (20)       95 2023-03-05 20:05:08.000000 sageworks-0.1.5.0/src/sageworks/algorithms/table/light/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1751 2023-04-05 21:18:09.000000 sageworks-0.1.5.0/src/sageworks/algorithms/table/light/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     9476 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/src/sageworks/algorithms/table/light/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/src/sageworks/algorithms/table/light/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.825051 sageworks-0.1.5.0/src/sageworks/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      639 2023-03-05 21:06:58.000000 sageworks-0.1.5.0/src/sageworks/artifacts/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-01 03:28:03.000000 sageworks-0.1.5.0/src/sageworks/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     5749 2023-05-05 18:17:33.000000 sageworks-0.1.5.0/src/sageworks/artifacts/artifact.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.825459 sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    12779 2023-05-07 17:34:22.000000 sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2943 2023-05-05 22:50:09.000000 sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2467 2023-05-06 16:00:13.000000 sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/data_source_abstract.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.825675 sageworks-0.1.5.0/src/sageworks/artifacts/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/artifacts/endpoints/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9820 2023-05-05 17:05:57.000000 sageworks-0.1.5.0/src/sageworks/artifacts/endpoints/endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.825891 sageworks-0.1.5.0/src/sageworks/artifacts/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/artifacts/feature_sets/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    12888 2023-05-07 17:34:22.000000 sageworks-0.1.5.0/src/sageworks/artifacts/feature_sets/feature_set.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.826112 sageworks-0.1.5.0/src/sageworks/artifacts/models/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/artifacts/models/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4328 2023-05-05 17:05:57.000000 sageworks-0.1.5.0/src/sageworks/artifacts/models/model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.826350 sageworks-0.1.5.0/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     7633 2023-05-04 14:48:56.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)     7911 2023-05-07 17:26:56.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.827459 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-14 19:44:44.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4187 2023-04-30 18:15:05.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py
--rw-r--r--   0 briford    (501) staff       (20)     1512 2023-04-19 17:04:31.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     6063 2023-04-02 19:53:47.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     2722 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     7280 2023-04-09 21:30:08.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     3587 2023-04-09 21:30:08.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     2589 2023-04-30 02:50:10.000000 sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.827820 sageworks-0.1.5.0/src/sageworks/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2023-03-17 17:39:22.000000 sageworks-0.1.5.0/src/sageworks/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.810953 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.827955 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)     7367 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.828348 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)     2997 2023-04-14 22:16:23.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2483 2023-04-19 22:41:04.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4155 2023-04-30 02:50:10.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.828475 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.828581 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.828695 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:15:48.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.828825 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:16:45.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.829126 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2047 2023-04-19 22:49:17.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2346 2023-04-19 21:48:41.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.829256 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.829447 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     5843 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.829554 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:14.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.829659 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:14.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.829968 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2591 2023-05-05 22:47:42.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     3000 2023-04-18 02:49:29.000000 sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.830094 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 18:06:15.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.811754 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.830200 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:46.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.830308 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:46.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.830497 sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7866 2023-04-19 18:49:44.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.830713 sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)        8 2023-03-25 02:07:31.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)     5179 2023-04-18 16:01:35.000000 sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.830920 sageworks-0.1.5.0/src/sageworks/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.0/src/sageworks/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2818 2023-04-09 22:14:00.000000 sageworks-0.1.5.0/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.831513 sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)     2745 2023-04-13 18:18:49.000000 sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3144 2023-04-13 18:18:49.000000 sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     7029 2023-05-05 21:05:21.000000 sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)    10898 2023-05-05 22:58:13.000000 sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     4611 2023-04-19 22:02:24.000000 sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6568 2023-05-07 17:39:34.000000 sageworks-0.1.5.0/src/sageworks/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.832765 sageworks-0.1.5.0/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 02:34:19.000000 sageworks-0.1.5.0/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3962 2023-04-30 02:31:13.000000 sageworks-0.1.5.0/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)     5113 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     1121 2023-04-05 21:18:09.000000 sageworks-0.1.5.0/src/sageworks/utils/iso_8601.py
--rw-r--r--   0 briford    (501) staff       (20)     6532 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3618 2023-04-17 19:53:54.000000 sageworks-0.1.5.0/src/sageworks/utils/sageworks_config.py
--rw-r--r--   0 briford    (501) staff       (20)     3558 2023-04-12 15:59:21.000000 sageworks-0.1.5.0/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)      531 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2209 2023-04-02 19:53:47.000000 sageworks-0.1.5.0/src/sageworks/utils/sageworks_sqs.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.833445 sageworks-0.1.5.0/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)     9387 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/views/artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     1296 2023-04-19 17:02:05.000000 sageworks-0.1.5.0/src/sageworks/views/view.py
--rw-r--r--   0 briford    (501) staff       (20)    12447 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/views/web_artifacts_summary.py
--rw-r--r--   0 briford    (501) staff       (20)     7030 2023-05-06 16:08:21.000000 sageworks-0.1.5.0/src/sageworks/views/web_data_source_view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.834863 sageworks-0.1.5.0/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     1304 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/web_components/box_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     1661 2023-04-08 01:37:21.000000 sageworks-0.1.5.0/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     1247 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/src/sageworks/web_components/feature_details.py
--rw-r--r--   0 briford    (501) staff       (20)      815 2023-04-02 19:53:47.000000 sageworks-0.1.5.0/src/sageworks/web_components/feature_importance.py
--rw-r--r--   0 briford    (501) staff       (20)     1182 2023-04-07 23:04:10.000000 sageworks-0.1.5.0/src/sageworks/web_components/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)      837 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/src/sageworks/web_components/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     1507 2023-04-09 21:30:08.000000 sageworks-0.1.5.0/src/sageworks/web_components/model_data.py
--rw-r--r--   0 briford    (501) staff       (20)     1703 2023-04-02 19:53:47.000000 sageworks-0.1.5.0/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     1551 2023-04-09 21:27:30.000000 sageworks-0.1.5.0/src/sageworks/web_components/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2119 2023-05-07 21:37:50.000000 sageworks-0.1.5.0/src/sageworks/web_components/table.py
--rw-r--r--   0 briford    (501) staff       (20)     1944 2023-05-05 02:30:09.000000 sageworks-0.1.5.0/src/sageworks/web_components/violin_plot.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.823946 sageworks-0.1.5.0/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     5964 2023-05-09 15:35:16.000000 sageworks-0.1.5.0/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     8767 2023-05-09 15:35:16.000000 sageworks-0.1.5.0/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2023-05-09 15:35:16.000000 sageworks-0.1.5.0/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)      134 2023-05-09 15:35:16.000000 sageworks-0.1.5.0/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2023-05-09 15:35:16.000000 sageworks-0.1.5.0/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.834985 sageworks-0.1.5.0/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.835492 sageworks-0.1.5.0/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1159 2023-05-05 17:05:57.000000 sageworks-0.1.5.0/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1483 2023-04-11 20:37:15.000000 sageworks-0.1.5.0/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1075 2023-05-05 17:05:57.000000 sageworks-0.1.5.0/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2023-04-02 18:05:33.000000 sageworks-0.1.5.0/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.835753 sageworks-0.1.5.0/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)     1105 2023-05-05 02:37:56.000000 sageworks-0.1.5.0/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-05-05 02:38:20.000000 sageworks-0.1.5.0/tests/aws_account/aws_service_broker_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-19 17:23:07.000000 sageworks-0.1.5.0/tests/create_sageworks_objs_for_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-09 15:35:16.836338 sageworks-0.1.5.0/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      574 2023-04-09 22:14:00.000000 sageworks-0.1.5.0/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      704 2023-04-09 22:14:00.000000 sageworks-0.1.5.0/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      677 2023-04-09 22:14:00.000000 sageworks-0.1.5.0/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      662 2023-04-09 22:14:00.000000 sageworks-0.1.5.0/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      648 2023-04-09 22:03:48.000000 sageworks-0.1.5.0/tests/transforms/pandas_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      729 2023-05-05 02:35:30.000000 sageworks-0.1.5.0/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.902579 sageworks-0.1.5.1/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.853512 sageworks-0.1.5.1/.github/
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-04-03 17:04:32.000000 sageworks-0.1.5.1/.github/dependabot.yml
+-rw-r--r--   0 briford    (501) staff       (20)     1899 2023-03-25 19:33:37.000000 sageworks-0.1.5.1/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      281 2023-03-28 23:51:00.000000 sageworks-0.1.5.1/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2023-02-17 22:10:33.000000 sageworks-0.1.5.1/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-04-30 02:31:13.000000 sageworks-0.1.5.1/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     5964 2023-05-14 18:57:19.902666 sageworks-0.1.5.1/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     5231 2023-05-06 21:24:25.000000 sageworks-0.1.5.1/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-04-03 17:04:32.000000 sageworks-0.1.5.1/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.847615 sageworks-0.1.5.1/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.853692 sageworks-0.1.5.1/applications/aws_dashboard/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.854181 sageworks-0.1.5.1/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12244 2023-04-30 02:31:13.000000 sageworks-0.1.5.1/applications/aws_dashboard/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-03-21 14:30:06.000000 sageworks-0.1.5.1/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     1081 2023-05-14 18:49:45.000000 sageworks-0.1.5.1/applications/aws_dashboard/aws_dashboard.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.855502 sageworks-0.1.5.1/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.856599 sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/
+-rw-r--r--   0 briford    (501) staff       (20)     4713 2023-05-14 18:51:03.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)      928 2023-05-10 17:06:02.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)      975 2023-05-10 17:06:02.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     1777 2023-05-14 18:41:54.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/main_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4757 2023-05-10 17:06:02.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/models_callbacks.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.857085 sageworks-0.1.5.1/applications/aws_dashboard/pages/data/
+-rw-r--r--   0 briford    (501) staff       (20)     1867 2023-04-08 01:44:28.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/data/toy_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)      597 2023-04-05 23:27:13.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/data/toy_scores.json
+-rw-r--r--   0 briford    (501) staff       (20)     2518 2023-05-14 18:45:34.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/data_sources.py
+-rw-r--r--   0 briford    (501) staff       (20)     1425 2023-05-10 17:06:02.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     1526 2023-05-10 17:06:02.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/feature_sets.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.858483 sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/
+-rw-r--r--   0 briford    (501) staff       (20)     2847 2023-05-14 18:51:03.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/data_sources_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1143 2023-04-09 22:27:31.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/endpoints_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1286 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/feature_sets_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1584 2023-04-07 15:53:06.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/main_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2436 2023-05-09 15:15:28.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/models_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2115 2023-05-11 20:29:48.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/main.py
+-rw-r--r--   0 briford    (501) staff       (20)     2547 2023-05-10 17:06:02.000000 sageworks-0.1.5.1/applications/aws_dashboard/pages/models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.859183 sageworks-0.1.5.1/applications/hello_world/
+-rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/applications/hello_world/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2152 2023-05-10 22:36:25.000000 sageworks-0.1.5.1/applications/hello_world/hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)     1060 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/applications/hello_world/layout.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.859937 sageworks-0.1.5.1/applications/model_viewer/
+-rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/applications/model_viewer/callbacks.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.860376 sageworks-0.1.5.1/applications/model_viewer/data/
+-rw-r--r--   0 briford    (501) staff       (20)     1849 2023-03-12 02:23:08.000000 sageworks-0.1.5.1/applications/model_viewer/data/toy_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)      597 2023-03-12 02:23:08.000000 sageworks-0.1.5.1/applications/model_viewer/data/toy_scores.json
+-rw-r--r--   0 briford    (501) staff       (20)     3069 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/applications/model_viewer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2525 2023-05-09 15:17:31.000000 sageworks-0.1.5.1/applications/model_viewer/model_viewer.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.861192 sageworks-0.1.5.1/applications/web_admin/
+-rw-r--r--   0 briford    (501) staff       (20)      213 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/applications/web_admin/flask_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      201 2023-03-03 22:18:34.000000 sageworks-0.1.5.1/applications/web_admin/hello-world-http-test.ini
+-rw-r--r--   0 briford    (501) staff       (20)      235 2023-03-03 22:19:17.000000 sageworks-0.1.5.1/applications/web_admin/hello-world.ini
+-rw-r--r--   0 briford    (501) staff       (20)      399 2023-03-03 22:20:51.000000 sageworks-0.1.5.1/applications/web_admin/hello-world.service
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.861425 sageworks-0.1.5.1/applications/web_admin/nginx_conf/
+-rw-r--r--   0 briford    (501) staff       (20)      486 2023-03-03 22:17:39.000000 sageworks-0.1.5.1/applications/web_admin/nginx_conf/nginx.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.861846 sageworks-0.1.5.1/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3315 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     4013 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/aws_setup/build_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.863329 sageworks-0.1.5.1/aws_setup/sageworks_cdk/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-04-30 02:31:15.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1291 2023-04-30 16:18:03.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       70 2023-04-30 17:09:37.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.863569 sageworks-0.1.5.1/aws_setup/sageworks_cdk/stacks/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/stacks/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2304 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/stacks/sageworks_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.863697 sageworks-0.1.5.1/aws_setup/sageworks_cdk/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.863864 sageworks-0.1.5.1/aws_setup/sageworks_cdk/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-04-30 02:31:15.000000 sageworks-0.1.5.1/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.864008 sageworks-0.1.5.1/config/
+-rw-r--r--   0 briford    (501) staff       (20)      147 2023-04-30 02:43:00.000000 sageworks-0.1.5.1/config/sageworks_config.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.865055 sageworks-0.1.5.1/data/
+-rw-r--r--   0 briford    (501) staff       (20)   196156 2023-03-26 18:42:12.000000 sageworks-0.1.5.1/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)      829 2023-05-02 22:39:27.000000 sageworks-0.1.5.1/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-04-19 19:55:29.000000 sageworks-0.1.5.1/data/test_data.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.865736 sageworks-0.1.5.1/docs/
+-rw-r--r--   0 briford    (501) staff       (20)     1770 2023-05-09 15:36:49.000000 sageworks-0.1.5.1/docs/admin_notes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.871221 sageworks-0.1.5.1/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2022-12-06 17:43:49.000000 sageworks-0.1.5.1/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-01-15 22:00:05.000000 sageworks-0.1.5.1/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-03-06 20:35:02.000000 sageworks-0.1.5.1/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-03-06 20:33:32.000000 sageworks-0.1.5.1/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-03-06 20:31:13.000000 sageworks-0.1.5.1/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-03-06 20:40:25.000000 sageworks-0.1.5.1/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-01-15 21:19:16.000000 sageworks-0.1.5.1/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-03-10 19:48:12.000000 sageworks-0.1.5.1/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-01-15 21:23:57.000000 sageworks-0.1.5.1/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-01-12 16:00:43.000000 sageworks-0.1.5.1/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2022-12-06 17:43:49.000000 sageworks-0.1.5.1/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)      667 2023-03-15 14:00:32.000000 sageworks-0.1.5.1/docs/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2023-03-13 14:45:22.000000 sageworks-0.1.5.1/docs/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.872066 sageworks-0.1.5.1/examples/
+-rw-r--r--   0 briford    (501) staff       (20)     1240 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/examples/data_to_data_example.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.872325 sageworks-0.1.5.1/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)   236926 2023-05-06 21:30:24.000000 sageworks-0.1.5.1/notebooks/ML_Pipeline_with_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.876646 sageworks-0.1.5.1/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-04-14 22:52:23.000000 sageworks-0.1.5.1/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-04-14 22:50:14.000000 sageworks-0.1.5.1/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-04-14 23:47:56.000000 sageworks-0.1.5.1/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-04-15 00:30:02.000000 sageworks-0.1.5.1/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-04-15 16:18:02.000000 sageworks-0.1.5.1/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-04-15 16:17:49.000000 sageworks-0.1.5.1/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      211 2023-05-02 03:06:50.000000 sageworks-0.1.5.1/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.880700 sageworks-0.1.5.1/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     1373 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/scripts/data_source_tags.py
+-rw-r--r--   0 briford    (501) staff       (20)     1717 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/scripts/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     1306 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/scripts/list_data_sources.py
+-rw-r--r--   0 briford    (501) staff       (20)      527 2023-05-14 18:57:19.902952 sageworks-0.1.5.1/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1787 2023-05-14 18:53:19.000000 sageworks-0.1.5.1/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.848594 sageworks-0.1.5.1/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.880872 sageworks-0.1.5.1/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)      853 2023-04-22 21:03:48.000000 sageworks-0.1.5.1/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.881646 sageworks-0.1.5.1/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.848808 sageworks-0.1.5.1/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.881752 sageworks-0.1.5.1/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-03-05 20:00:31.000000 sageworks-0.1.5.1/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.882001 sageworks-0.1.5.1/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-03-05 19:59:59.000000 sageworks-0.1.5.1/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.849058 sageworks-0.1.5.1/src/sageworks/algorithms/table/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.882229 sageworks-0.1.5.1/src/sageworks/algorithms/table/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      169 2023-03-05 20:04:10.000000 sageworks-0.1.5.1/src/sageworks/algorithms/table/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.883333 sageworks-0.1.5.1/src/sageworks/algorithms/table/light/
+-rw-r--r--   0 briford    (501) staff       (20)       95 2023-03-05 20:05:08.000000 sageworks-0.1.5.1/src/sageworks/algorithms/table/light/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1751 2023-04-05 21:18:09.000000 sageworks-0.1.5.1/src/sageworks/algorithms/table/light/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     9476 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/src/sageworks/algorithms/table/light/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/src/sageworks/algorithms/table/light/row_tagger.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.883899 sageworks-0.1.5.1/src/sageworks/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2023-03-05 21:06:58.000000 sageworks-0.1.5.1/src/sageworks/artifacts/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-01 03:28:03.000000 sageworks-0.1.5.1/src/sageworks/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     5706 2023-05-14 17:23:33.000000 sageworks-0.1.5.1/src/sageworks/artifacts/artifact.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.884747 sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15504 2023-05-14 17:23:53.000000 sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     3129 2023-05-14 17:27:17.000000 sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2891 2023-05-14 15:23:51.000000 sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/data_source_abstract.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.885117 sageworks-0.1.5.1/src/sageworks/artifacts/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/artifacts/endpoints/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9792 2023-05-14 17:29:06.000000 sageworks-0.1.5.1/src/sageworks/artifacts/endpoints/endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.885487 sageworks-0.1.5.1/src/sageworks/artifacts/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/artifacts/feature_sets/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    13093 2023-05-14 17:29:06.000000 sageworks-0.1.5.1/src/sageworks/artifacts/feature_sets/feature_set.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.885860 sageworks-0.1.5.1/src/sageworks/artifacts/models/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/artifacts/models/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4419 2023-05-14 17:29:06.000000 sageworks-0.1.5.1/src/sageworks/artifacts/models/model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.886367 sageworks-0.1.5.1/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     7633 2023-05-04 14:48:56.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)     9590 2023-05-12 17:33:32.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.887846 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-14 19:44:44.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2501 2023-05-11 17:16:49.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     6066 2023-05-11 17:16:49.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     3325 2023-05-11 18:41:08.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     5772 2023-05-12 17:34:32.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     4297 2023-05-11 18:40:16.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     2949 2023-05-10 23:23:46.000000 sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.888448 sageworks-0.1.5.1/src/sageworks/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2023-03-17 17:39:22.000000 sageworks-0.1.5.1/src/sageworks/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.849778 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.888673 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)     7367 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.889365 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)     2997 2023-04-14 22:16:23.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2483 2023-04-19 22:41:04.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4155 2023-04-30 02:50:10.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.889576 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.889663 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.889751 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:15:48.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.889936 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:16:45.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.890458 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2231 2023-05-12 22:12:48.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2298 2023-05-12 21:29:54.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.890677 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.890838 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     5817 2023-05-12 17:46:07.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.891046 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:14.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.891282 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:14.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.891824 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2538 2023-05-12 17:52:28.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     2974 2023-05-12 17:46:07.000000 sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.892070 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 18:06:15.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.850562 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.892158 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:46.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.892428 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:46.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.892704 sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7840 2023-05-12 17:53:53.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.893192 sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)        8 2023-03-25 02:07:31.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)     5179 2023-04-18 16:01:35.000000 sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.893516 sageworks-0.1.5.1/src/sageworks/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.5.1/src/sageworks/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2800 2023-05-12 17:54:23.000000 sageworks-0.1.5.1/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.894522 sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     2745 2023-04-13 18:18:49.000000 sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3144 2023-04-13 18:18:49.000000 sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     7003 2023-05-12 21:36:54.000000 sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)    10872 2023-05-12 17:52:28.000000 sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     7517 2023-05-12 23:56:39.000000 sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6705 2023-05-14 17:33:24.000000 sageworks-0.1.5.1/src/sageworks/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.896498 sageworks-0.1.5.1/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 02:34:19.000000 sageworks-0.1.5.1/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3962 2023-04-30 02:31:13.000000 sageworks-0.1.5.1/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     5113 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     2417 2023-05-14 17:23:33.000000 sageworks-0.1.5.1/src/sageworks/utils/iso_8601.py
+-rw-r--r--   0 briford    (501) staff       (20)     6532 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3618 2023-04-17 19:53:54.000000 sageworks-0.1.5.1/src/sageworks/utils/sageworks_config.py
+-rw-r--r--   0 briford    (501) staff       (20)     3558 2023-04-12 15:59:21.000000 sageworks-0.1.5.1/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)      531 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2209 2023-04-02 19:53:47.000000 sageworks-0.1.5.1/src/sageworks/utils/sageworks_sqs.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.897473 sageworks-0.1.5.1/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)    11812 2023-05-12 17:36:11.000000 sageworks-0.1.5.1/src/sageworks/views/artifacts_text_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3063 2023-05-12 17:33:32.000000 sageworks-0.1.5.1/src/sageworks/views/artifacts_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     4206 2023-05-14 18:51:25.000000 sageworks-0.1.5.1/src/sageworks/views/data_source_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1296 2023-04-19 17:02:05.000000 sageworks-0.1.5.1/src/sageworks/views/view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.900206 sageworks-0.1.5.1/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     1304 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/src/sageworks/web_components/box_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     1661 2023-04-08 01:37:21.000000 sageworks-0.1.5.1/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     1015 2023-05-14 18:45:34.000000 sageworks-0.1.5.1/src/sageworks/web_components/data_source_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     1247 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/src/sageworks/web_components/feature_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      815 2023-04-02 19:53:47.000000 sageworks-0.1.5.1/src/sageworks/web_components/feature_importance.py
+-rw-r--r--   0 briford    (501) staff       (20)     1182 2023-04-07 23:04:10.000000 sageworks-0.1.5.1/src/sageworks/web_components/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)      837 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/src/sageworks/web_components/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     1507 2023-04-09 21:30:08.000000 sageworks-0.1.5.1/src/sageworks/web_components/model_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     1703 2023-04-02 19:53:47.000000 sageworks-0.1.5.1/src/sageworks/web_components/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     1551 2023-04-09 21:27:30.000000 sageworks-0.1.5.1/src/sageworks/web_components/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2227 2023-05-11 20:41:25.000000 sageworks-0.1.5.1/src/sageworks/web_components/table.py
+-rw-r--r--   0 briford    (501) staff       (20)     1944 2023-05-05 02:30:09.000000 sageworks-0.1.5.1/src/sageworks/web_components/violin_plot.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.881521 sageworks-0.1.5.1/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     5964 2023-05-14 18:57:19.000000 sageworks-0.1.5.1/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     8753 2023-05-14 18:57:19.000000 sageworks-0.1.5.1/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2023-05-14 18:57:19.000000 sageworks-0.1.5.1/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)      134 2023-05-14 18:57:19.000000 sageworks-0.1.5.1/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2023-05-14 18:57:19.000000 sageworks-0.1.5.1/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.900368 sageworks-0.1.5.1/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.901219 sageworks-0.1.5.1/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1250 2023-05-14 17:27:17.000000 sageworks-0.1.5.1/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1483 2023-04-11 20:37:15.000000 sageworks-0.1.5.1/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1155 2023-05-14 17:27:17.000000 sageworks-0.1.5.1/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2023-04-02 18:05:33.000000 sageworks-0.1.5.1/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.901644 sageworks-0.1.5.1/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)     1105 2023-05-05 02:37:56.000000 sageworks-0.1.5.1/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-05-05 02:38:20.000000 sageworks-0.1.5.1/tests/aws_account/aws_service_broker_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-19 17:23:07.000000 sageworks-0.1.5.1/tests/create_sageworks_objs_for_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-05-14 18:57:19.902432 sageworks-0.1.5.1/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      554 2023-05-12 17:46:18.000000 sageworks-0.1.5.1/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      682 2023-05-12 18:00:39.000000 sageworks-0.1.5.1/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      655 2023-05-12 18:01:20.000000 sageworks-0.1.5.1/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-05-12 17:46:18.000000 sageworks-0.1.5.1/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      628 2023-05-12 17:46:18.000000 sageworks-0.1.5.1/tests/transforms/pandas_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      729 2023-05-05 02:35:30.000000 sageworks-0.1.5.1/tox.ini
```

### Comparing `sageworks-0.1.5.0/.gitignore` & `sageworks-0.1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/LICENSE` & `sageworks-0.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/Makefile` & `sageworks-0.1.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/PKG-INFO` & `sageworks-0.1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.1.5.0
+Version: 0.1.5.1
 Summary: SageWorks: A Python WorkBench for creating and deploying SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sageworks-0.1.5.0/Readme.md` & `sageworks-0.1.5.1/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/assets/custom.css` & `sageworks-0.1.5.1/applications/aws_dashboard/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/aws_dashboard.py` & `sageworks-0.1.5.1/applications/aws_dashboard/aws_dashboard.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,34 @@
 """FeatureSets Callbacks: Callback within the DataSources Web User Interface"""
 from datetime import datetime
 import dash
 from dash import Dash
 from dash.dependencies import Input, Output
 
 # SageWorks Imports
-from sageworks.views.web_data_source_view import WebDataSourceView
-from sageworks.web_components import violin_plot
-
-# Cheese Sauce
-data_source_rows = WebDataSourceView().data_sources_summary()
-data_source_rows["id"] = data_source_rows.index
-
-"""
-def refresh_timer(app: Dash):
-    @app.callback(Output("last-updated-data-sources", "children"), Input("data-sources-updater", "n_intervals"))
-    def time_updated(_n):
-        return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
-"""
+from sageworks.views.data_source_web_view import DataSourceWebView
+from sageworks.web_components import data_source_details, violin_plot
 
 
-def refresh_data_broker(app: Dash, data_source_broker: WebDataSourceView):
+def refresh_data_timer(app: Dash):
     @app.callback(
         Output("last-updated-data-sources", "children"),
         Input("data-sources-updater", "n_intervals"),
     )
     def time_updated(_n):
-        global data_source_rows
-        data_source_broker.refresh()
-        data_source_rows = data_source_broker.data_sources_summary()
-        data_source_rows["id"] = data_source_rows.index
-        print(data_source_rows)
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
-def update_data_sources_table(app: Dash):
-    @app.callback(
-        Output("data_sources_table", "data"),
-        Input("data-sources-updater", "n_intervals"),
-        prevent_initial_call=True,
-    )
+def update_data_sources_table(app: Dash, data_source_broker: DataSourceWebView):
+    @app.callback(Output("data_sources_table", "data"), Input("data-sources-updater", "n_intervals"))
     def data_sources_update(_n):
         """Return the table data as a dictionary"""
-        global data_source_rows
+        data_source_broker.refresh()
+        data_source_rows = data_source_broker.data_sources_summary()
+        data_source_rows["id"] = data_source_rows.index
         return data_source_rows.to_dict("records")
 
 
 # Highlights the selected row in the table
 def table_row_select(app: Dash, table_name: str):
     @app.callback(
         Output(table_name, "style_data_conditional"),
@@ -62,60 +44,72 @@
                 "backgroundColor": "rgb(80, 80, 80)",
             }
             for i in selected_rows
         ]
         return row_style
 
 
-def update_sample_rows_header(app: Dash):
+# Updates the data source details when a row is selected in the summary
+def update_data_source_details(app: Dash, data_source_web_view: DataSourceWebView):
     @app.callback(
-        Output("sample_rows_header", "children"),
+        [Output("data_details_header", "children"), Output("data_source_details", "children")],
         Input("data_sources_table", "derived_viewport_selected_row_ids"),
-        prevent_initial_call=True,
     )
-    def update_sample_header(selected_rows):
-        return "Sampled Rows: Updating..."
+    def generate_new_markdown(selected_rows):
+        print(f"Selected Rows: {selected_rows}")
+        if not selected_rows or selected_rows[0] is None:
+            return dash.no_update
+        print("Calling DataSource Details...")
+        data_details = data_source_web_view.data_source_details(selected_rows[0])
+        data_details_markdown = data_source_details.create_markdown(data_details)
+
+        # Name of the data source for the Header
+        data_source_name = data_source_web_view.data_source_name(selected_rows[0])
+        header = f"Details: {data_source_name}"
 
+        # Return the details/markdown for these data details
+        return [header, data_details_markdown]
 
-def update_data_source_sample_rows(app: Dash, web_data_source_view: WebDataSourceView):
+
+def update_data_source_sample_rows(app: Dash, data_source_web_view: DataSourceWebView):
     @app.callback(
         [
-            Output("sample_rows_header", "children", allow_duplicate=True),
+            Output("sample_rows_header", "children"),
             Output("data_source_sample_rows", "columns"),
             Output("data_source_sample_rows", "data"),
         ],
         Input("data_sources_table", "derived_viewport_selected_row_ids"),
         prevent_initial_call=True,
     )
     def sample_rows_update(selected_rows):
         print(f"Selected Rows: {selected_rows}")
         if not selected_rows or selected_rows[0] is None:
             return dash.no_update
-        print("Calling DataSource Sample Rows Refresh...")
-        sample_rows = web_data_source_view.data_source_sample(selected_rows[0])
+        print("Calling DataSource Sample Rows...")
+        sample_rows = data_source_web_view.data_source_sample(selected_rows[0])
 
         # Name of the data source
-        data_source_name = web_data_source_view.data_source_name(selected_rows[0])
+        data_source_name = data_source_web_view.data_source_name(selected_rows[0])
         header = f"Sampled Rows: {data_source_name}"
 
         # The columns need to be in a special format for the DataTable
         column_setup = [{"name": c, "id": c, "presentation": "input"} for c in sample_rows.columns]
 
         # Return the columns and the data
         return [header, column_setup, sample_rows.to_dict("records")]
 
 
-def update_violin_plots(app: Dash, web_data_source_view: WebDataSourceView):
+def update_violin_plots(app: Dash, data_source_web_view: DataSourceWebView):
     """Updates the Violin Plots when a new data source is selected"""
 
     @app.callback(
         Output("violin_plot", "figure"),
         Input("data_sources_table", "derived_viewport_selected_row_ids"),
         prevent_initial_call=True,
     )
     def generate_new_violin_plot(selected_rows):
         print(f"Selected Rows: {selected_rows}")
         if not selected_rows or selected_rows[0] is None:
             return dash.no_update
         print("Calling DataSource Sample Rows Refresh...")
-        smart_sample_rows = web_data_source_view.data_source_smart_sample(selected_rows[0])
+        smart_sample_rows = data_source_web_view.data_source_smart_sample(selected_rows[0])
         return violin_plot.create_figure(smart_sample_rows)
```

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """FeatureSets Callbacks: Callback within the FeatureSets Web User Interface"""
 from datetime import datetime
 from dash import Dash
 from dash.dependencies import Input, Output
 
 # SageWorks Imports
-from sageworks.views.web_artifacts_summary import WebArtifactsSummary
+from sageworks.views.artifacts_web_view import ArtifactsWebView
 
 
 def update_last_updated(app: Dash):
     @app.callback(
         Output("last-updated-feature-sets", "children"),
         Input("feature-sets-updater", "n_intervals"),
     )
     def time_updated(n):
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
-def update_feature_sets_table(app: Dash, sageworks_artifacts: WebArtifactsSummary):
+def update_feature_sets_table(app: Dash, sageworks_artifacts: ArtifactsWebView):
     @app.callback(
         Output("FEATURE_SETS_DETAILS", "data"),
         Input("feature-sets-updater", "n_intervals"),
     )
     def data_sources_update(n):
         print("Calling FeatureSets Refresh...")
         sageworks_artifacts.refresh()
```

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/main_callbacks.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/main_callbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Callbacks/Connections in the Web User Interface"""
 from datetime import datetime
 from dash import Dash
 from dash.dependencies import Input, Output
 
 # SageWorks Imports
-from sageworks.views.web_artifacts_summary import WebArtifactsSummary
+from sageworks.views.artifacts_web_view import ArtifactsWebView
 
 # Cheese Sauce
 all_data = None
 
 
-def update_last_updated(app: Dash, sageworks_artifacts: WebArtifactsSummary):
+def update_last_updated(app: Dash, sageworks_artifacts: ArtifactsWebView):
     @app.callback(Output("last-updated", "children"), Input("main-updater", "n_intervals"))
     def time_updated(n):
         global all_data
         print("Calling ALL Artifact Refresh...")
         sageworks_artifacts.refresh()
         all_data = sageworks_artifacts.view_data()
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
```

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/callbacks/models_callbacks.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/callbacks/models_callbacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from sageworks.web_components.model_data import ModelData
 from sageworks.web_components import (
     feature_importance,
     confusion_matrix,
     model_details,
     feature_details,
 )
-from sageworks.views.web_artifacts_summary import WebArtifactsSummary
+from sageworks.views.artifacts_web_view import ArtifactsWebView
 
 
 def update_last_updated(app: Dash):
     @app.callback(
         Output("last-updated-models", "children"),
         Input("models-updater", "n_intervals"),
     )
     def time_updated(n):
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
-def update_models_table(app: Dash, sageworks_artifacts: WebArtifactsSummary):
+def update_models_table(app: Dash, sageworks_artifacts: ArtifactsWebView):
     @app.callback(Output("models_table", "data"), Input("models-updater", "n_intervals"))
     def data_sources_update(n):
         print("Calling Models Refresh...")
         sageworks_artifacts.refresh()
         models = sageworks_artifacts.models_summary()
         return models.to_dict("records")
```

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/data/toy_data.csv` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/data/toy_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/data/toy_scores.json` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/data/toy_scores.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/endpoints.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/endpoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Endpoints:  A SageWorks Web Interface to view, interact, and manage Endpoints"""
 from dash import register_page
 import dash
 
 # SageWorks Imports
 from sageworks.web_components import line_chart
-from sageworks.views.web_artifacts_summary import WebArtifactsSummary
+from sageworks.views.artifacts_web_view import ArtifactsWebView
 from sageworks.web_components import table
 
 # Local Imports
 from pages.layout.endpoints_layout import endpoints_layout
 import pages.callbacks.endpoints_callbacks as callbacks
 
 register_page(__name__, path="/endpoints")
 
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Grab a view that gives us a summary of all the artifacts currently in SageWorks
-sageworks_artifacts = WebArtifactsSummary()
+sageworks_artifacts = ArtifactsWebView()
 endpoints_summary = sageworks_artifacts.endpoints_summary()
 
 # Create a table to display the feature sets
 endpoints_table = table.create(
     "ENDPOINTS_DETAILS",
     endpoints_summary,
     header_color="rgb(100, 60, 100)",
```

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/feature_sets.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/feature_sets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """DataSources:  A SageWorks Web Interface to view, interact, and manage Data Sources"""
 from dash import register_page
 import dash
 
 # SageWorks Imports
 from sageworks.web_components import scatter_plot
-from sageworks.views.web_artifacts_summary import WebArtifactsSummary
+from sageworks.views.artifacts_web_view import ArtifactsWebView
 from sageworks.web_components import table
 
 # Local Imports
 from pages.layout.feature_sets_layout import feature_sets_layout
 import pages.callbacks.feature_sets_callbacks as callbacks
 
 register_page(__name__, path="/feature_sets")
 
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Grab a view that gives us a summary of all the artifacts currently in SageWorks
-sageworks_artifacts = WebArtifactsSummary()
+sageworks_artifacts = ArtifactsWebView()
 feature_sets_summary = sageworks_artifacts.feature_sets_summary()
 
 # Create a table to display the feature sets
 feature_sets_table = table.create(
     "FEATURE_SETS_DETAILS",
     feature_sets_summary,
     header_color="rgb(100, 100, 60)",
```

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/data_sources_layout.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/data_sources_layout.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,22 +18,52 @@
                             "fontSize": 15,
                             "padding": "0px 0px 0px 160px",
                         },
                     ),
                     dbc.Row(style={"padding": "30px 0px 0px 0px"}),
                 ]
             ),
+            # List out all the Data Sources
             dbc.Row(components["data_sources_table"]),
+            # Data Source Details, Sample Rows, and Violin Plots
+            # Row [ Column 1                       Column 2 ]
+            #       (Row(Data Source Details))     Row(Sample Rows)
+            #                                      Row(Violin Plots)
             dbc.Row(
-                html.H3("Sampled Rows", id="sample_rows_header"),
-                style={"padding": "30px 0px 10px 0px"},
-            ),
-            dbc.Row(
-                components["data_source_sample_rows"],
-                style={"padding": "0px 0px 30px 0px"},
+                [
+                    # Column 1: Data Source Details
+                    dbc.Col(
+                        [
+                            dbc.Row(
+                                html.H3("Details", id="data_details_header"),
+                                style={"padding": "30px 0px 10px 0px"},
+                            ),
+                            dbc.Row(
+                                components["data_source_details"],
+                                style={"padding": "0px 0px 30px 0px"},
+                            ),
+                        ],
+                        width=4,
+                    ),
+                    # Column 2: Sample Rows and Violin Plots
+                    dbc.Col(
+                        [
+                            dbc.Row(
+                                html.H3("Sampled Rows", id="sample_rows_header"),
+                                style={"padding": "30px 0px 10px 0px"},
+                            ),
+                            dbc.Row(
+                                components["data_source_sample_rows"],
+                                style={"padding": "0px 0px 30px 0px"},
+                            ),
+                            dbc.Row(components["violin_plot"]),
+                        ],
+                        width=8,
+                    ),
+                    # Just the auto updater
+                    dcc.Interval(id="data-sources-updater", interval=5000, n_intervals=0),
+                ]
             ),
-            dbc.Row(components["violin_plot"]),
-            dcc.Interval(id="data-sources-updater", interval=5000, n_intervals=0),
         ],
         style={"margin": "30px"},
     )
     return layout
```

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/endpoints_layout.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/endpoints_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/feature_sets_layout.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/feature_sets_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/main_layout.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/main_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/layout/models_layout.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/layout/models_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/main.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Main: The main SageWorks Web Interface to view, interact, and manage SageWorks Artifacts"""
 from dash import register_page
 import dash
 
 # SageWorks Imports
-from sageworks.views.web_artifacts_summary import WebArtifactsSummary
+from sageworks.views.artifacts_web_view import ArtifactsWebView
 from sageworks.web_components import table
 
 # Local Imports
 from pages.layout.main_layout import main_layout
 import pages.callbacks.main_callbacks as callbacks
 
 register_page(__name__, path="/")
 
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Grab a view that gives us a summary of all the artifacts currently in SageWorks
-web_artifacts_summary = WebArtifactsSummary()
+web_artifacts_summary = ArtifactsWebView()
 sageworks_artifacts = web_artifacts_summary.view_data()
 
 # Grab the Artifact Information DataFrame for each AWS Service and pass it to the table creation
 tables = dict()
 tables["INCOMING_DATA"] = table.create(
     "INCOMING_DATA",
     sageworks_artifacts["INCOMING_DATA"],
```

### Comparing `sageworks-0.1.5.0/applications/aws_dashboard/pages/models.py` & `sageworks-0.1.5.1/applications/aws_dashboard/pages/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 from sageworks.web_components import confusion_matrix, table, scatter_plot
 from sageworks.web_components import (
     feature_importance,
     model_data,
     model_details,
     feature_details,
 )
-from sageworks.views.web_artifacts_summary import WebArtifactsSummary
+from sageworks.views.artifacts_web_view import ArtifactsWebView
 
 # Local Imports
 from pages.layout.models_layout import models_layout
 import pages.callbacks.models_callbacks as callbacks
 
 register_page(__name__, path="/models")
 
 # Okay feels a bit weird but Dash pages just have a bunch of top level code (no classes/methods)
 
 # Put the components into 'dark' mode
 load_figure_template("darkly")
 
 # Grab a view that gives us a summary of all the artifacts currently in SageWorks
-web_artifacts_summary = WebArtifactsSummary()
+web_artifacts_summary = ArtifactsWebView()
 models_summary = web_artifacts_summary.models_summary(concise=True)
 
 # Read in our fake model data
 data_path = os.path.join(os.path.dirname(__file__), "data/toy_data.csv")
 fake_model_info = model_data.ModelData(data_path)
 
 # Create a table to display the models
```

### Comparing `sageworks-0.1.5.0/applications/hello_world/callbacks.py` & `sageworks-0.1.5.1/applications/hello_world/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/hello_world/hello_world.py` & `sageworks-0.1.5.1/applications/hello_world/hello_world.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """HelloWorld: A SageWorks HelloWorld Application"""
 from dash import Dash
 import dash_bootstrap_components as dbc
 
 
 # SageWorks Imports
-from sageworks.views.web_artifacts_summary import WebArtifactsSummary
+from sageworks.views.artifacts_web_view import ArtifactsWebView
 from sageworks.web_components import table
 
 
 # Local Imports
 import layout
 
 
@@ -22,26 +22,26 @@
 
 
 def setup_artifact_viewer():
     # Set Default Template for figures
     # load_figure_template('darkly')
 
     # Grab a view that gives us a summary of all the artifacts currently in SageWorks
-    sageworks_artifacts = WebArtifactsSummary()
+    sageworks_artifacts = ArtifactsWebView()
     web_artifacts_summary = sageworks_artifacts.view_data()
 
     # Just a bunch of tables for now :)
     tables = {}
     for service_category, artifact_info_df in web_artifacts_summary.items():
         # Grab the Artifact Information DataFrame for each AWS Service
         tables[service_category] = table.create(service_category, artifact_info_df)
 
     # Create our components
     components = {
-        "incoming_data": tables["INCOMING_DATA"],
+        "incoming_data": tables["INCOMING_DATA_S3"],
         "data_sources": tables["DATA_SOURCES"],
         "feature_sets": tables["FEATURE_SETS"],
         "models": tables["MODELS"],
         "endpoints": tables["ENDPOINTS"],
     }
 
     # Setup up our application layout
```

### Comparing `sageworks-0.1.5.0/applications/hello_world/layout.py` & `sageworks-0.1.5.1/applications/hello_world/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/model_viewer/callbacks.py` & `sageworks-0.1.5.1/applications/model_viewer/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/model_viewer/data/toy_data.csv` & `sageworks-0.1.5.1/applications/model_viewer/data/toy_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/model_viewer/data/toy_scores.json` & `sageworks-0.1.5.1/applications/model_viewer/data/toy_scores.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/model_viewer/layout.py` & `sageworks-0.1.5.1/applications/model_viewer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/applications/model_viewer/model_viewer.py` & `sageworks-0.1.5.1/applications/model_viewer/model_viewer.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/aws_setup/aws_account_check.py` & `sageworks-0.1.5.1/aws_setup/aws_account_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/aws_setup/build_ml_pipeline.py` & `sageworks-0.1.5.1/aws_setup/build_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/aws_setup/sageworks_cdk/README.md` & `sageworks-0.1.5.1/aws_setup/sageworks_cdk/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/aws_setup/sageworks_cdk/app.py` & `sageworks-0.1.5.1/aws_setup/sageworks_cdk/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/aws_setup/sageworks_cdk/cdk.json` & `sageworks-0.1.5.1/aws_setup/sageworks_cdk/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/aws_setup/sageworks_cdk/stacks/sageworks_stack.py` & `sageworks-0.1.5.1/aws_setup/sageworks_cdk/stacks/sageworks_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py` & `sageworks-0.1.5.1/aws_setup/sageworks_cdk/tests/unit/test_sageworks_sandbox_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/data/abalone.csv` & `sageworks-0.1.5.1/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/data/test_data.csv` & `sageworks-0.1.5.1/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/data/test_data.json` & `sageworks-0.1.5.1/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/admin_notes.md` & `sageworks-0.1.5.1/docs/admin_notes.md`

 * *Files 1% similar despite different names*

```diff
@@ -70,12 +70,12 @@
 $ twine upload dist/* -r pypi
 ```
 
 ### Push changes to Github
 
 ``` {.bash}
 $ git add setup.py
-$ get commit -m "sageworks version 1.8.7 (or whatever)"
+$ git commit -m "sageworks version 1.8.7 (or whatever)"
 $ git tag v1.8.7 (or whatever)
 $ git push --tags
 $ git push
 ```
```

### Comparing `sageworks-0.1.5.0/docs/images/big_spider.png` & `sageworks-0.1.5.1/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/images/graph_representation.png` & `sageworks-0.1.5.1/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/images/powered_aws_dark_blue.png` & `sageworks-0.1.5.1/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/images/powered_aws_transparent.png` & `sageworks-0.1.5.1/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/images/powered_aws_white.png` & `sageworks-0.1.5.1/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.1.5.1/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/images/sageworks.png` & `sageworks-0.1.5.1/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/images/sageworks_concepts.png` & `sageworks-0.1.5.1/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/images/scp.png` & `sageworks-0.1.5.1/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/images/scp_labs.png` & `sageworks-0.1.5.1/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/images/small_spider.png` & `sageworks-0.1.5.1/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/sageworks_classes_concepts.md` & `sageworks-0.1.5.1/docs/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/docs/scp_consulting.md` & `sageworks-0.1.5.1/docs/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/examples/data_to_data_example.py` & `sageworks-0.1.5.1/examples/data_to_data_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/notebooks/ML_Pipeline_with_SageWorks.ipynb` & `sageworks-0.1.5.1/notebooks/ML_Pipeline_with_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/notebooks/images/athena_query_aqsol.png` & `sageworks-0.1.5.1/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.1.5.1/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.1.5.1/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/notebooks/images/model_screenshot.png` & `sageworks-0.1.5.1/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/notebooks/images/sageworks_concepts.png` & `sageworks-0.1.5.1/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/notebooks/images/scp_labs.png` & `sageworks-0.1.5.1/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/scripts/data_source_tags.py` & `sageworks-0.1.5.1/scripts/data_source_tags.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/scripts/generate_jsonl_data.py` & `sageworks-0.1.5.1/scripts/generate_jsonl_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/scripts/list_data_sources.py` & `sageworks-0.1.5.1/scripts/list_data_sources.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/setup.cfg` & `sageworks-0.1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/setup.py` & `sageworks-0.1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """Simple directory walker"""
     return [(os.path.join(".", d), [os.path.join(d, f) for f in files]) for d, _, files in os.walk(dir_name)]
 
 
 setup(
     name="sageworks",
     # use_scm_version=True,
-    version="0.1.5.0",
+    version="0.1.5.1",
     description="SageWorks: A Python WorkBench for creating and deploying SageMaker Models",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="SuperCowPowers LLC",
     author_email="support@supercowpowers.com",
     url="https://github.com/SuperCowPowers/sageworks",
     packages=find_packages("src"),
```

### Comparing `sageworks-0.1.5.0/src/sageworks/__init__.py` & `sageworks-0.1.5.1/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/algorithms/table/light/data_source_eda.py` & `sageworks-0.1.5.1/src/sageworks/algorithms/table/light/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/algorithms/table/light/feature_spider.py` & `sageworks-0.1.5.1/src/sageworks/algorithms/table/light/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/algorithms/table/light/row_tagger.py` & `sageworks-0.1.5.1/src/sageworks/algorithms/table/light/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/artifacts/Readme.md` & `sageworks-0.1.5.1/src/sageworks/artifacts/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/artifacts/artifact.py` & `sageworks-0.1.5.1/src/sageworks/artifacts/artifact.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,41 +76,41 @@
 
     @abstractmethod
     def aws_url(self):
         """AWS console/web interface for this artifact"""
         pass
 
     @abstractmethod
-    def meta(self) -> dict:
+    def all_meta(self) -> dict:
         """Get the full AWS metadata for this artifact"""
         pass
 
     @abstractmethod
     def delete(self):
         """Delete this artifact including all related AWS objects"""
         pass
 
     def sageworks_meta(self) -> dict:
         """Get the SageWorks specific metadata for this Artifact
         Note: This functionality will work for FeatureSets, Models, and Endpoints
-              but not for DataSources. DataSources need to overwrite this method
+              but not for DataSources. The DataSource class overwrites this method.
         """
         aws_arn = self.arn()
         self.log.info(f"Retrieving SageWorks Metadata for Artifact: {aws_arn}...")
         aws_tags = self.sm_session.list_tags(aws_arn)
         meta = self._aws_tags_to_dict(aws_tags)
         return meta
 
     def upsert_sageworks_meta(self, new_meta: dict):
         """Add SageWorks specific metadata to this Artifact
         Args:
             new_meta (dict): Dictionary of new metadata to add
         Note:
             This functionality will work for FeatureSets, Models, and Endpoints
-            but not for DataSources. DataSources need to overwrite this method
+            but not for DataSources. The DataSource class overwrites this method.
         """
         aws_arn = self.arn()
         self.log.info(f"Upserting SageWorks Metadata for Artifact: {aws_arn}...")
         aws_tags = self._dict_to_aws_tags(new_meta)
         self.sm_session.sagemaker_client.add_tags(ResourceArn=aws_arn, Tags=aws_tags)
 
     def sageworks_tags(self) -> list:
@@ -127,15 +127,14 @@
             "uuid": self.uuid,
             "aws_arn": self.arn(),
             "aws_url": self.aws_url(),
             "size": self.size(),
             "created": self.created(),
             "modified": self.modified(),
             "sageworks_tags": self.sageworks_tags(),
-            "sageworks_meta": self.sageworks_meta(),
         }
 
     @staticmethod
     def _aws_tags_to_dict(aws_tags) -> dict:
         """Internal: AWS Tags are in an odd format, so convert to regular dictionary"""
         return {item["Key"]: item["Value"] for item in aws_tags if "sageworks" in item["Key"]}
```

### Comparing `sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/athena_source.py` & `sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/athena_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import awswrangler as wr
 from datetime import datetime
 import json
 
 # SageWorks Imports
 from sageworks.artifacts.data_sources.data_source_abstract import DataSourceAbstract
 from sageworks.aws_service_broker.aws_service_broker import ServiceCategory
+from sageworks.utils.iso_8601 import convert_all_to_iso8601
 
 
 class AthenaSource(DataSourceAbstract):
     """AthenaSource: SageWorks Data Source accessible through Athena
 
     Common Usage:
         my_data = AthenaSource(data_uuid, database="sageworks")
@@ -74,15 +75,15 @@
         account_id = self.aws_account_clamp.account_id()
         region = self.aws_account_clamp.region()
         arn = f"arn:aws:glue:{region}:{account_id}:table/{self.data_catalog_db}/{self.table_name}"
         return arn
 
     def sageworks_meta(self):
         """Get the SageWorks specific metadata for this Artifact"""
-        params = self.meta().get("Parameters", {})
+        params = self.all_meta().get("Parameters", {})
         return {key: value for key, value in params.items() if "sageworks" in key}
 
     def upsert_sageworks_meta(self, new_meta: dict):
         """Add SageWorks specific metadata to this Artifact
         Args:
             new_meta (dict): Dictionary of new metadata to add
         """
@@ -112,15 +113,15 @@
 
     def size(self) -> float:
         """Return the size of this data in MegaBytes"""
         size_in_bytes = sum(wr.s3.size_objects(self.s3_storage_location(), boto3_session=self.boto_session).values())
         size_in_mb = size_in_bytes / 1_000_000
         return size_in_mb
 
-    def meta(self) -> dict:
+    def all_meta(self) -> dict:
         """Get the FULL AWS metadata for this artifact"""
         return self.catalog_table_meta
 
     def aws_url(self):
         """The AWS URL for looking at/querying this data source"""
         return f"https://{self.aws_region}.console.aws.amazon.com/athena/home"
 
@@ -195,18 +196,18 @@
         # Store the sample_df in our SageWorks metadata
         rows_json = sample_df.to_json(orient="records", lines=True)
         self.upsert_sageworks_meta({"sageworks_sample_rows": rows_json})
 
         # Return the sample_df
         return sample_df
 
-    def quartiles(self, recompute=False) -> dict[dict]:
+    def quartiles(self, recompute: bool = False) -> dict[dict]:
         """Compute Quartiles for all the numeric columns in a DataSource
         Args:
-            recompute: Recompute the quartiles (default: False)
+            recompute(bool): Recompute the quartiles (default: False)
         Returns:
             dict(dict): A dictionary of quartiles for each column in the form
                  {'col1': {'min': 0, 'q1': 1, 'median': 2, 'q3': 3, 'max': 4},
                   'col2': ...}
         """
 
         # First check if we have already computed the quartiles
@@ -216,36 +217,91 @@
         # For every column in the table that is numeric, get the quartiles
         self.log.info("Computing Quartiles for all numeric columns (this may take a while)...")
         quartile_data = []
         for column, data_type in zip(self.column_names(), self.column_types()):
             print(column, data_type)
             if data_type in ["bigint", "double", "int", "smallint", "tinyint"]:
                 query = (
-                    f"SELECT MIN({column}) AS min, "
-                    f"approx_percentile({column}, 0.25) AS q1, "
-                    f"approx_percentile({column}, 0.5) AS median, "
-                    f"approx_percentile({column}, 0.75) AS q3, "
-                    f"MAX({column}) AS max FROM {self.table_name}"
+                    f'SELECT MIN("{column}") AS min, '
+                    f'approx_percentile("{column}", 0.25) AS q1, '
+                    f'approx_percentile("{column}", 0.5) AS median, '
+                    f'approx_percentile("{column}", 0.75) AS q3, '
+                    f'MAX("{column}") AS max FROM {self.table_name}'
                 )
                 result_df = self.query(query)
                 result_df["column_name"] = column
                 quartile_data.append(result_df)
-        quartile_data = pd.concat(quartile_data).set_index("column_name").to_dict(orient="index")
+        quartile_dict = pd.concat(quartile_data).set_index("column_name").to_dict(orient="index")
 
         # Push the quartile data into our DataSource Metadata
-        self.upsert_sageworks_meta({"sageworks_quartiles": quartile_data})
+        self.upsert_sageworks_meta({"sageworks_quartiles": quartile_dict})
 
         # Return the quartile data
-        return quartile_data
+        return quartile_dict
+
+    def value_counts(self, recompute: bool = False) -> dict[dict]:
+        """Compute 'value_counts' for all the string columns in a DataSource
+        Args:
+            recompute(bool): Recompute the value counts (default: False)
+        Returns:
+            dict(dict): A dictionary of value counts for each column in the form
+                 {'col1': {'value_1': X, 'value_2': Y, 'value_3': Z,...},
+                  'col2': ...}
+        """
+
+        # First check if we have already computed the quartiles
+        if self.sageworks_meta().get("sageworks_value_counts") and not recompute:
+            return json.loads(self.sageworks_meta()["sageworks_value_counts"])
+
+        # For every column in the table that is numeric, get the quartiles
+        self.log.info("Computing 'value_counts' for all string columns...")
+        value_count_dict = dict()
+        for column, data_type in zip(self.column_names(), self.column_types()):
+            print(column, data_type)
+            if data_type in ["string"]:
+                query = (
+                    f'SELECT "{column}", count(*) as count '
+                    f"FROM {self.table_name} "
+                    f'GROUP BY "{column}" ORDER BY count DESC limit 10'
+                )
+                # Convert int64 to int so that we can serialize to JSON
+                result_df = self.query(query)
+                result_df["count"] = result_df["count"].astype(int)
+
+                # Convert the result_df into a dictionary
+                value_count_dict[column] = dict(zip(result_df[column], result_df["count"]))
+
+        # Push the value_count data into our DataSource Metadata
+        self.upsert_sageworks_meta({"sageworks_value_counts": value_count_dict})
+
+        # Return the value_count data
+        return value_count_dict
+
+    def details(self, recompute: bool = False) -> dict[dict]:
+        """Additional Details about this AthenaSource Artifact
+        Args:
+            recompute(bool): Recompute the details (default: False)
+        Returns:
+            dict(dict): A dictionary of details about this AthenaSource
+        """
+
+        # First check if we have already computed the details
+        if self.sageworks_meta().get("sageworks_details") and not recompute:
+            return json.loads(self.sageworks_meta()["sageworks_details"])
 
-    def details(self) -> dict:
-        """Additional Details about this AthenaSource Artifact"""
         details = super().details()
         details["s3_storage_location"] = self.s3_storage_location()
-        details.update(self.meta())
+
+        # Convert any datetime fields to ISO-8601 strings
+        details = convert_all_to_iso8601(details)
+
+        # Push the details data into our DataSource Metadata
+        self.upsert_sageworks_meta({"sageworks_details": details})
+
+        # Return the details data
         return details
 
     def delete(self):
         """Delete the AWS Data Catalog Table and S3 Storage Objects"""
 
         # Make sure the Feature Group exists
         if not self.check():
@@ -261,15 +317,15 @@
 
 
 if __name__ == "__main__":
     """Exercise the AthenaSource Class"""
     from pprint import pprint
 
     # Retrieve a Data Source
-    my_data = AthenaSource("abalone_data")
+    my_data = AthenaSource("test_data")
 
     # Verify that the Athena Data Source exists
     assert my_data.check()
 
     # What's my SageWorks UUID
     print(f"UUID: {my_data.uuid}")
 
@@ -287,34 +343,42 @@
     print(f"Created: {my_data.created()}")
     print(f"Modified: {my_data.modified()}")
 
     # Column Names and Types
     print(f"Column Names: {my_data.column_names()}")
     print(f"Column Types: {my_data.column_types()}")
 
-    # Get Metadata and tags associated with this Artifact
-    print(f"Meta: {my_data.meta()}")
+    # Get Tags associated with this Artifact
     print(f"Tags: {my_data.sageworks_tags()}")
 
     # Get a sample of the data
     df = my_data.sample_df()
     print(f"Sample Data: {df.shape}")
     print(df)
 
     # Get the SageWorks Metadata for this Data Source
     meta = my_data.sageworks_meta()
-    print("SageWorks Meta")
+    print("\nSageWorks Meta")
     pprint(meta)
 
-    # Add some SageWorks Metadata to this Data Source
-    my_data.upsert_sageworks_meta({"sageworks_tags": "abalone:public"})
-    print("SageWorks Meta NEW")
-    pprint(my_data.sageworks_meta())
-
-    # Get quartiles for all the columns
-    quartile_info = my_data.quartiles()
-    print("Quartiles")
+    # Get details for this Data Source
+    my_details = my_data.details(recompute=True)
+    print("\nDetails")
+    pprint(my_details)
+
+    # Get quartiles for numeric columns
+    quartile_info = my_data.quartiles(recompute=True)
+    print("\nQuartiles")
     pprint(quartile_info)
 
+    # Get value_counts for string columns
+    value_count_info = my_data.value_counts(recompute=True)
+    print("\nValue Counts")
+    pprint(value_count_info)
+
+    # Get ALL Metadata associated with this Artifact
+    print("\n\nALL Meta")
+    pprint(my_data.all_meta())
+
     # Now delete the AWS artifacts associated with this DataSource
     # print('Deleting SageWorks Data Source...')
     # my_data.delete()
```

### Comparing `sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/data_source.py` & `sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,18 @@
         column_types(): Return the column types
         column_details(): Return the column details
         query(query: str): Returns a pd.DataFrame with the query results
         sample_df(): Returns a SAMPLED pd.DataFrame from this DataSource
         summary(): Returns a summary of this DataSource
         details(): Returns additional details about this DataSource
         quartiles(): Returns the quartiles for each numeric column in this DataSource
-        meta(): Returns ALL AWS Metadata for this DataSource
+        value_counts(): Returns the value counts for each string column in this DataSource
         sageworks_meta(): Returns the SageWorks Metadata for this DataSource
         sageworks_tags(): Returns the SageWorks Tags for this DataSource
+        all_meta(): Returns ALL AWS Metadata for this DataSource
     """
 
     def __new__(cls, uuid, data_source_type: str = "athena"):
         """DataSource: A Factory for DataSources (Athena, RDS, etc)
         Args:
             uuid: The UUID of the DataSource
             data_source_type: The type of DataSource (athena, rds, etc)
@@ -41,14 +42,15 @@
             return AthenaSource(uuid)
         else:
             raise NotImplementedError(f"DataSource type {data_source_type} not implemented")
 
 
 if __name__ == "__main__":
     """Exercise the DataSource Factory Class"""
+    from pprint import pprint
 
     # Retrieve a DataSource
     my_data = DataSource("abalone_data")
 
     # Verify that the Athena DataSource exists
     assert my_data.check()
 
@@ -69,13 +71,16 @@
     print(f"Created: {my_data.created()}")
     print(f"Modified: {my_data.modified()}")
 
     # Column Names and Types
     print(f"Column Names: {my_data.column_names()}")
     print(f"Column Types: {my_data.column_types()}")
 
-    # Get Metadata and tags associated with this Artifact
-    print(f"Meta: {my_data.meta()}")
+    # Get Tags associated with this Artifact
     print(f"Tags: {my_data.sageworks_tags()}")
 
+    # Get ALL Metadata associated with this Artifact
+    print("\n\nALL Meta")
+    pprint(my_data.all_meta())
+
     # Get a SAMPLE of the data
     print(f"Sample Data: {my_data.sample_df()}")
```

### Comparing `sageworks-0.1.5.0/src/sageworks/artifacts/data_sources/data_source_abstract.py` & `sageworks-0.1.5.1/src/sageworks/artifacts/data_sources/data_source_abstract.py`

 * *Files 19% similar despite different names*

```diff
@@ -60,15 +60,25 @@
         Returns:
             dict(dict): A dictionary of quartiles for each column in the form
                  {'col1': {'min': 0, 'q1': 1, 'median': 2, 'q3': 3, 'max': 4},
                   'col2': ...}
         """
         pass
 
+    def value_counts(self, recompute: bool = False) -> dict[dict]:
+        """Compute 'value_counts' for all the string columns in a DataSource
+        Args:
+            recompute(bool): Recompute the value counts (default: False)
+        Returns:
+            dict(dict): A dictionary of value counts for each column in the form
+                 {'col1': {'value_1': X, 'value_2': Y, 'value_3': Z,...},
+                  'col2': ...}
+        """
+        pass
+
     def details(self) -> dict:
         """Additional Details about this DataSourceAbstract Artifact"""
         details = self.summary()
         details["num_rows"] = self.num_rows()
         details["num_columns"] = self.num_columns()
         details["column_details"] = self.column_details()
-        details.update(self.meta())
         return details
```

### Comparing `sageworks-0.1.5.0/src/sageworks/artifacts/endpoints/endpoint.py` & `sageworks-0.1.5.1/src/sageworks/artifacts/endpoints/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,16 +156,16 @@
             error_df[column] = df[column].values
         return error_df
 
     def size(self) -> float:
         """Return the size of this data in MegaBytes"""
         return 0.0
 
-    def meta(self) -> dict:
-        """Get the metadata for this artifact"""
+    def all_meta(self) -> dict:
+        """Get ALL the metadata for this artifact"""
         return self.endpoint_meta
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for this artifact"""
         return self.endpoint_meta["EndpointArn"]
 
     def aws_url(self):
@@ -179,15 +179,14 @@
     def modified(self) -> datetime:
         """Return the datetime when this artifact was last modified"""
         return self.endpoint_meta["LastModifiedTime"]
 
     def details(self) -> dict:
         """Additional Details about this Endpoint"""
         details = self.summary()
-        details.update(self.meta())
         return details
 
     def performance_metrics(self, target: str, prediction_df: pd.DataFrame) -> dict:
         """Compute the performance metrics for this Endpoint"""
 
         # Compute the metrics
         metrics = {
```

### Comparing `sageworks-0.1.5.0/src/sageworks/artifacts/feature_sets/feature_set.py` & `sageworks-0.1.5.1/src/sageworks/artifacts/feature_sets/feature_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,17 @@
             self.data_source = None
             return
         else:
             self.record_id = self.feature_meta["RecordIdentifierFeatureName"]
             self.event_time = self.feature_meta["EventTimeFeatureName"]
 
             # Pull Athena and S3 Storage information from metadata
-            self.athena_database = self.feature_meta["sageworks"].get("athena_database")
-            self.athena_table = self.feature_meta["sageworks"].get("athena_table")
-            self.s3_storage = self.feature_meta["sageworks"].get("s3_storage")
+            self.athena_database = self.feature_meta["sageworks_meta"].get("athena_database")
+            self.athena_table = self.feature_meta["sageworks_meta"].get("athena_table")
+            self.s3_storage = self.feature_meta["sageworks_meta"].get("s3_storage")
 
             # Create our internal DataSource (hardcoded to Athena for now)
             self.data_source = AthenaSource(self.athena_table, self.athena_database)
 
         # Spin up our Feature Store
         self.feature_store = FeatureStore(self.sm_session)
 
@@ -74,16 +74,16 @@
     def check(self) -> bool:
         """Does the feature_set_name exist in the AWS Metadata?"""
         if self.feature_meta is None:
             self.log.info(f"FeatureSet.check() {self.feature_set_name} not found in AWS Metadata!")
             return False
         return True
 
-    def meta(self) -> dict:
-        """Get the full AWS metadata for this artifact"""
+    def all_meta(self) -> dict:
+        """Get ALL the metadata for this artifact"""
         return self.feature_meta
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for this artifact"""
         return self.feature_meta["FeatureGroupArn"]
 
     def size(self) -> float:
@@ -211,17 +211,14 @@
         # Column Details
         fs_details["column_details"] = self.column_details()
 
         # Underlying Storage Details
         fs_details["storage_type"] = "athena"  # TODO: Add RDS support
         fs_details["storage_uuid"] = self.data_source.uuid
 
-        # Full Metadata from AWS
-        fs_details.update(self.meta())
-
         # Return the details
         return fs_details
 
     def delete(self):
         """Delete the Feature Set: Feature Group, Catalog Table, and S3 Storage Objects"""
 
         # Delete the Feature Group and ensure that it gets deleted
@@ -249,24 +246,31 @@
                     break
                 else:
                     raise error
             time.sleep(1)
         self.log.info(f"FeatureSet {feature_group.name} successfully deleted")
 
     def quartiles(self) -> dict:
-        """Get the quartiles for all numeric columns of the underlying DataSource
+        """Get the quartiles for the numeric columns of the underlying DataSource
         Returns:
-            dict: A dictionary of quartiles for all numeric columns
+            dict: A dictionary of quartiles for the numeric columns
         """
         return self.data_source.quartiles()
 
     def sample_df(self) -> pd.DataFrame:
         """Get a sample of the data from the underlying DataSource"""
         return self.data_source.sample_df()
 
+    def value_counts(self) -> dict:
+        """Get the quartiles for the string columns of the underlying DataSource
+        Returns:
+            dict: A dictionary of value counts for the string columns
+        """
+        return self.data_source.value_counts()
+
 
 if __name__ == "__main__":
     """Exercise for FeatureSet Class"""
     from pprint import pprint
 
     # Setup Pandas output options
     pd.set_option("display.max_colwidth", 50)
```

### Comparing `sageworks-0.1.5.0/src/sageworks/artifacts/models/model.py` & `sageworks-0.1.5.1/src/sageworks/artifacts/models/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,16 +44,16 @@
             return False
         return True
 
     def size(self) -> float:
         """Return the size of this data in MegaBytes"""
         return 0.0
 
-    def meta(self) -> dict:
-        """Get the metadata for this artifact"""
+    def all_meta(self) -> dict:
+        """Get ALL the metadata for this artifact"""
         return self.latest_model
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for the Model Package Group"""
         return self.group_arn()
 
     def group_arn(self) -> str:
@@ -77,15 +77,14 @@
         return self.latest_model["CreationTime"]
 
     def details(self) -> dict:
         """Additional Details about this Endpoint"""
         details = self.summary()
         details["model_package_group_arn"] = self.group_arn()
         details["model_package_arn"] = self.model_arn()
-        details.update(self.meta())
         return details
 
     def delete(self):
         """Delete the Model Packages and the Model Group"""
 
         # If we don't have meta then the model probably doesn't exist
         if self.model_meta is None:
@@ -116,12 +115,15 @@
     # Get the ARN of the Model Group
     print(f"Model Group ARN: {my_model.group_arn()}")
     print(f"Model Package ARN: {my_model.arn()}")
 
     # Get the tags associated with this Model
     print(f"Tags: {my_model.sageworks_tags()}")
 
+    # Get the SageWorks metadata associated with this Model
+    print(f"SageWorks Meta: {my_model.sageworks_meta()}")
+
     # Get creation time
     print(f"Created: {my_model.created()}")
 
     # Delete the Model
     # my_model.delete()
```

### Comparing `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py` & `sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,106 +1,97 @@
-"""ArtifactInfo: Class to retrieve information (tags, meta, size) from an AWS Artifact"""
-import botocore
+"""S3ToDataSourceLight: Class to move LIGHT S3 Files into a SageWorks DataSource"""
 import awswrangler as wr
+import pandas as pd
+from pandas.errors import ParserError
 
+# Local imports
+from sageworks.transforms.transform import Transform, TransformInput, TransformOutput
+from sageworks.transforms.pandas_transforms.pandas_to_data import PandasToData
 
-# SageWorks Imports
-from sageworks.aws_service_broker.aws_service_connectors.connector import Connector
-from sageworks.utils.cache import Cache
 
+class S3ToDataSourceLight(Transform):
+    """S3ToDataSourceLight: Class to move LIGHT S3 Files into a SageWorks DataSource
 
-# Class to retrieve object/file information from an AWS S3 Bucket
-class ArtifactInfo(Connector):
-    """ArtifactInfo: Class to retrieve information (tags, meta, size) from an AWS Artifact"""
+    Common Usage:
+        s3_to_data = S3ToDataSourceLight(s3_path, data_uuid, datatype="csv/json")
+        s3_to_data.set_output_tags(["abalone", "whatever"])
+        s3_to_data.transform()
+    """
 
-    def __init__(self):
-        # Call SuperClass Initialization
-        super().__init__()
-
-        # Cache for information on AWS Artifacts (size, tags, metadata, etc)
-        self.artifact_info_cache = Cache(expire=60)
-
-    def check(self) -> bool:
-        """Can we connect to this AWS Service?"""
-        return True  # I'm great thx for asking!
-
-    def refresh_impl(self):
-        """Refresh the cache of AWS Artifact information"""
-        # The cache will handle the refresh
-        pass
-
-    def metadata(self) -> dict:
-        """Get all the metadata for this AWS connector"""
-        return {}
-
-    def s3_object_sizes(self, s3_path) -> int:
-        """Return the sum of all the s3 objects sizes for the given s3 path
+    def __init__(self, s3_path: str, data_uuid: str, datatype: str = "csv"):
+        """S3ToDataSourceLight Initialization
         Args:
-            s3_path (str): S3 Path for recursive aggregation
-        Returns:
-            int: Sum of object size in this s3 path in MegaBytes
+            s3_path (str): The S3 Path to the file to be transformed
+            data_uuid (str): The UUID of the SageWorks DataSource to be created
+            datatype (str): The datatype of the file to be transformed (defaults to "csv")
         """
-        size_in_mb = self.artifact_info_cache.get(s3_path)
-        if size_in_mb is None:
-            self.log.info(f"Computing S3 Object sizes: {s3_path}...")
-            size_in_bytes = sum(wr.s3.size_objects(s3_path, boto3_session=self.boto_session).values())
-            size_in_mb = f"{ (size_in_bytes/1_000_000):.1f}"
-            self.artifact_info_cache.set(s3_path, size_in_mb)
-        return size_in_mb
 
-    def get_sagemaker_obj_info(self, aws_arn) -> dict:
-        """Retrieve information on AWS *SageMaker* Objects (tags, metadata, etc)
-           This method will ONLY work for FeatureSets, Models, and Endpoints but fail for DataSources
-        Args:
-            aws_arn (str): AWS ARN for the artifact
-        Returns:
-            dict: Dictionary of AWS Artifact information
-        """
-        info = self.artifact_info_cache.get(aws_arn)
-        if info is None:
-            self.log.info(f"Retrieving Artifact Tags and Metadata: {aws_arn}...")
+        # Call superclass init
+        super().__init__(s3_path, data_uuid)
+
+        # Set up all my instance attributes
+        self.input_type = TransformInput.S3_OBJECT
+        self.output_type = TransformOutput.DATA_SOURCE
+        self.datatype = datatype
+
+    def input_size_mb(self) -> int:
+        """Get the size of the input S3 object in MBytes"""
+        size_in_bytes = wr.s3.size_objects(self.input_uuid, boto3_session=self.boto_session)[self.input_uuid]
+        size_in_mb = round(size_in_bytes / 1_000_000)
+        return size_in_mb
 
-            # This class will work for FeatureSets, Models, and Endpoints but fail for DataSources
+    def convert_object_columns(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Try to automatically convert object columns to datetime columns"""
+        for c in df.columns[df.dtypes == "object"]:  # Look at the object columns
             try:
-                aws_tags = self.sm_session.list_tags(aws_arn)
-                info = self._aws_tags_to_dict(aws_tags)
-            except botocore.exceptions.ClientError as exc:
-                if exc.response["Error"]["Code"] == "ValidationException":
-                    self.log.error(f"This method doesn't work on DataSources: {exc}")
-                    return {}
-                else:
-                    self.log.critical(f"Unknown Error: {exc}")
-                    raise exc
-
-            # Set the artifact info cache
-            self.artifact_info_cache.set(aws_arn, info)
-        return info
-
-    @staticmethod
-    def _aws_tags_to_dict(aws_tags):
-        """Internal: AWS Tags are in an odd format, so convert to regular dictionary"""
-        return {item["Key"]: item["Value"] for item in aws_tags if "sageworks" in item["Key"]}
+                df[c] = pd.to_datetime(df[c])
+            except (ParserError, ValueError, TypeError):
+                self.log.debug(f"Column {c} could not be converted to datetime...")
+
+                # Now try to convert object to string
+                try:
+                    df[c] = df[c].astype(str)
+                except (ParserError, ValueError, TypeError):
+                    self.log.info(f"Column {c} could not be converted to string...")
+        return df
+
+    def transform_impl(self, overwrite: bool = True):
+        """Convert the CSV data into Parquet Format in the SageWorks Data Sources Bucket, and
+        store the information about the data to the AWS Data Catalog sageworks database"""
+
+        # Sanity Check for S3 Object size
+        object_megabytes = self.input_size_mb()
+        if object_megabytes > 100:
+            self.log.error(f"S3 Object too big ({object_megabytes} MBytes): Use the S3ToDataSourceHeavy class!")
+            return
+
+        # Read in the S3 CSV as a Pandas DataFrame
+        if self.datatype == "csv":
+            df = wr.s3.read_csv(self.input_uuid, low_memory=False, boto3_session=self.boto_session)
+        else:
+            df = wr.s3.read_json(self.input_uuid, lines=True, boto3_session=self.boto_session)
+
+        # Convert object columns before sending to SageWorks Data Source
+        df = self.convert_object_columns(df)
+
+        # Use the SageWorks Pandas to Data Source class
+        pandas_to_data = PandasToData(self.output_uuid)
+        pandas_to_data.set_input(df)
+        pandas_to_data.set_output_tags(self.output_tags)
+        pandas_to_data.add_output_meta(self.output_meta)
+        pandas_to_data.transform()
 
 
 if __name__ == "__main__":
-    from pprint import pprint
-    from sageworks.artifacts.data_sources.athena_source import AthenaSource
-    from sageworks.artifacts.feature_sets.feature_set import FeatureSet
-
-    # Grab one of our test FeatureSets for something to test with
-    feature_set = FeatureSet("abalone_features")
-    details = feature_set.details()
-    arn = details["aws_arn"]
-    s3_location = details["s3_storage_location"]
-
-    # Create the class and get the info about the artifact
-    my_info = ArtifactInfo()
-    meta = my_info.get_sagemaker_obj_info(arn)
-    size = my_info.s3_object_sizes(s3_location)
-    pprint(meta)
-    print(f"Size: {size} MB")
-
-    # Grab one of our test DataSources for something to test with
-    data_source = AthenaSource("abalone_data")
-    details = data_source.details()
-    arn = details["aws_arn"]
-    s3_location = details["s3_storage_location"]
+    """Exercise the S3ToDataSourceLight Class"""
+    from sageworks.utils.sageworks_config import SageWorksConfig
+
+    # Create my Data Loader
+    sageworks_config = SageWorksConfig()
+    sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET_NAME")
+    input_path = "s3://" + sageworks_bucket + "/incoming-data/aqsol_public_data.csv"
+    output_uuid = "aqsol_data"
+    my_loader = S3ToDataSourceLight(input_path, output_uuid)
+    my_loader.set_output_tags(["aqsol", "public"])
+
+    # Store this data as a SageWorks DataSource
+    my_loader.transform()
```

### Comparing `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.1.5.1/src/sageworks/views/view.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,39 @@
-"""Connector: Abstract Base Class for pulling/refreshing AWS Service metadata"""
+"""View: View in the database sense: Pulls from the AWS Service Broker and does slice and dice"""
 from abc import ABC, abstractmethod
 
 import logging
-from typing import final
 
 # SageWorks Imports
+from sageworks.aws_service_broker.aws_service_broker import AWSServiceBroker
 from sageworks.aws_service_broker.aws_account_clamp import AWSAccountClamp
 from sageworks.utils.sageworks_logging import logging_setup
 
 # Set up logging
 logging_setup()
 
 
-class Connector(ABC):
-    # Class attributes
-    log = logging.getLogger(__name__)
-
-    # Set up our Boto3 and SageMaker Session and SageMaker Client
-    aws_account_clamp = AWSAccountClamp()
-    boto_session = aws_account_clamp.boto_session()
-    sm_session = aws_account_clamp.sagemaker_session(boto_session)
-    sm_client = aws_account_clamp.sagemaker_client(boto_session)
-
+class View(ABC):
     def __init__(self):
-        """Connector: Abstract Base Class for pulling/refreshing AWS Service metadata"""
+        """View: View in the database sense: Pulls from the AWS Service Broker and does slice and dice"""
         self.log = logging.getLogger(__name__)
 
+        # Grab an AWS Metadata Broker object for pulling AWS Service information
+        self.aws_broker = AWSServiceBroker()
+        self.aws_account_clamp = AWSAccountClamp()
+        self.boto_session = self.aws_account_clamp.boto_session()
+        self.sm_session = self.aws_account_clamp.sagemaker_session()
+
     @abstractmethod
     def check(self) -> bool:
-        """Can we connect to this service?"""
+        """Can we connect to this view/service?"""
         pass
 
     @abstractmethod
-    def refresh_impl(self):
-        """Abstract Method: Implement the AWS Service Data Refresh"""
-        pass
-
-    @final
     def refresh(self) -> bool:
-        """Refresh data/metadata associated with this service"""
-        # We could do something here to refresh the AWS Session or whatever
-
-        # Call the subclass Refresh method
-        return self.refresh_impl()
+        """Refresh data/metadata associated with this view"""
+        pass
 
     @abstractmethod
-    def metadata(self) -> dict:
-        """Return all the metadata for this service"""
+    def view_data(self) -> dict:
+        """Return all the data that's useful for this view"""
         pass
```

### Comparing `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             print(f"Reading Data Catalog Database: {database}...")
             table_list = wr.catalog.get_tables(database=database, boto3_session=self.boto_session)
 
             # Convert to a data structure with direct lookup
             self.data_catalog_metadata[database] = {table["Name"]: table for table in table_list}
 
     def metadata(self) -> dict:
-        """Get all the table information in this database"""
+        """Get all the information for this AWS Data Catalog"""
         return self.data_catalog_metadata
 
     def get_scoped_database_list(self):
         """Return a list of databases within the defined scope for this class"""
         all_databases = [db["Name"] for db in wr.catalog.get_databases(boto3_session=self.boto_session)]
         if self.database_scope == ["all"]:
             return all_databases
```

### Comparing `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,19 @@
         self.log.info("Reading Endpoints from SageMaker...")
         _endpoints = self.sm_client.list_endpoints()["Endpoints"]
         _end_names = [_endpoint["EndpointName"] for _endpoint in _endpoints]
 
         # Get the details for Endpoints and convert to a data structure with direct lookup
         self.endpoint_data = {name: self._retrieve_details(name) for name in _end_names}
 
+        # Additional details under the sageworks_meta section for each Model Group
+        for _end_name, end_info in self.endpoint_data.items():
+            sageworks_meta = self.sageworks_meta(end_info["EndpointArn"])
+            end_info["sageworks_meta"] = sageworks_meta
+
     def metadata(self) -> dict:
         """Get the full AWS metadata about endpoints"""
         return self.endpoint_data
 
     def endpoint_names(self) -> list:
         """Get all the endpoint names in AWS"""
         return list(self.endpoint_data.keys())
@@ -74,7 +79,16 @@
     print("Endpoints:")
     for end_name in my_endpoints.endpoint_names():
         print(f"\t{end_name}")
 
     # Get the details for a specific Endpoint
     endpoint_info = my_endpoints.endpoint_details(end_name)
     pprint(endpoint_info)
+
+    # Get the tags for this Endpoint
+    my_arn = endpoint_info["EndpointArn"]
+    my_tags = my_endpoints.sageworks_tags(my_arn)
+    print(f"Tags: {my_tags}")
+
+    # Get the SageWorks Metadata for this Endpoint
+    my_sageworks_meta = my_endpoints.sageworks_meta(my_arn)
+    print(f"SageWorks Metadata: {my_sageworks_meta}")
```

### Comparing `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,14 +34,21 @@
 
         # Grab the ModelPackageGroupArn (we store it in the model_data)
         self.model_package_group_arn = _model_groups[0]["ModelPackageGroupArn"] if _model_groups else None
 
         # Get the details for each Model Group and convert to a data structure with direct lookup
         self.model_data = {name: self._model_group_details(name) for name in _mg_names}
 
+        # Additional details under the sageworks_meta section for each Model Group
+        for mg_name in _mg_names:
+            sageworks_meta = self.sageworks_meta(self.model_package_group_arn)
+            # Model groups have a list of models
+            for model_info in self.model_data[mg_name]:
+                model_info["sageworks_meta"] = sageworks_meta
+
     def metadata(self) -> dict:
         """Get all the table information in this database"""
         return self.model_data
 
     def model_group_names(self) -> list:
         """Get all the feature group names in this database"""
         return list(self.model_data.keys())
@@ -87,7 +94,16 @@
     for my_group_name in model_registry.model_group_names():
         print(f"\t{my_group_name}")
 
     # Get the details for a specific Model Group
     my_group = "abalone-regression"
     group_info = model_registry.model_group_details(my_group)
     pprint(group_info)
+
+    # Get the tags for this Model Group
+    my_arn = model_registry.model_package_group_arn
+    my_tags = model_registry.sageworks_tags(my_arn)
+    print(f"Tags: {my_tags}")
+
+    # Get the SageWorks Metadata for this Model Group
+    my_sageworks_meta = model_registry.sageworks_meta(my_arn)
+    print(f"SageWorks Metadata: {my_sageworks_meta}")
```

### Comparing `sageworks-0.1.5.0/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.1.5.1/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,45 +28,55 @@
             return False
 
     def refresh_impl(self):
         """Load/reload the files in the bucket"""
         # Grab all the files in this bucket
         self.log.info(f"Reading S3 Bucket: {self.bucket}...")
         _aws_file_info = wr.s3.describe_objects(self.bucket, boto3_session=self.boto_session)
-        self.s3_bucket_data = {full_path.split("/")[-1]: info for full_path, info in _aws_file_info.items()}
+        self.s3_bucket_data = {full_path: info for full_path, info in _aws_file_info.items()}
 
     def metadata(self) -> dict:
         """Get all the metadata for the files in this bucket"""
         return self.s3_bucket_data
 
     def file_names(self) -> list:
         """Get all the file names in this bucket"""
         return list(self.s3_bucket_data.keys())
 
+    def bucket_size(self) -> list:
+        """For all the files in this bucket/prefix recursively SUM up the sizes"""
+        sizes = []
+        for file, info in self.s3_bucket_data.items():
+            sizes.append(info["ContentLength"])
+        return sum(sizes)
+
     def file_info(self, file: str) -> dict:
         """Get additional info about this specific file"""
         return self.s3_bucket_data[file]
 
 
 if __name__ == "__main__":
     """Exercises the S3Bucket Class"""
     from pprint import pprint
     from sageworks.utils.sageworks_config import SageWorksConfig
 
     # Grab out incoming data bucket for something to test with
     sageworks_config = SageWorksConfig()
     sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET_NAME")
-    incoming_data_bucket = "s3://" + sageworks_bucket + "/incoming-data"
+    incoming_data_bucket = "s3://" + sageworks_bucket + "/incoming-data/"
 
     # Create the class and check the functionality
     s3_bucket = S3Bucket(incoming_data_bucket)
     s3_bucket.check()
     s3_bucket.refresh()
 
     # List files in the bucket
     print(f"{s3_bucket.bucket}")
     for file_name in s3_bucket.file_names():
         print(f"\t{file_name}")
 
+    # Get the size of all the objects in this bucket
+    print(f"Bucket Size: {s3_bucket.bucket_size()}")
+
     # Get additional info for a specific file
     my_file_info = s3_bucket.file_info("abalone.csv")
     pprint(my_file_info)
```

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/Readme.md` & `sageworks-0.1.5.1/src/sageworks/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.1.5.1/src/sageworks/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/light/clean_data.py` & `sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/light/clean_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from sageworks.transforms.pandas_transforms import pandas_utils
 
 
 class CleanData(DataToDataLight):
     """CleanData:Class for filtering, sub-setting, and value constraints on Light DataSources
 
     Common Usage:
-        clean_data = DataToDataLight(input_data_uuid, output_data_uuid)
+        clean_data = CleanData(input_data_uuid, output_data_uuid)
         clean_data.set_output_tags(["abalone", "clean", "whatever"])
-        clean_data.transform(delete_existing=True/False)
+        clean_data.transform(drop_na="any", drop_outliers=True, drop_duplicates=True)
     """
 
     def __init__(self, input_data_uuid: str, output_data_uuid: str):
         """CleanData Initialization"""
 
         # Call superclass init
         super().__init__(input_data_uuid, output_data_uuid)
 
-    def transform_impl(self, drop_na="any", **kwargs):
+    def transform_impl(self, drop_na="any", drop_duplicates=True, drop_outliers=True, **kwargs):
         """Simple Clean Data, will improve later"""
 
         """
         Notes for later:
         Cleaning data typically involves two phases: Identification and Remediation.
 
         - Identification
@@ -37,21 +37,25 @@
             - Fill/Replace
             - Impute the value (using inference/context to fill in a value)
         """
 
         # Drop Rows that have NaNs in them
         self.output_df = pandas_utils.drop_nans(self.input_df, how=drop_na)
 
+        # Drop Duplicates
+        if drop_duplicates:
+            self.output_df = pandas_utils.drop_duplicates(self.output_df)
+
+        # Drop Outliers
+        if drop_outliers:
+            self.output_df = pandas_utils.drop_outliers_iqr(self.output_df, scale=2.0)
+
 
 if __name__ == "__main__":
     """Exercise the CleanData Class"""
 
     # Create the class with inputs and outputs and invoke the transform
     input_uuid = "test_data"
     output_uuid = "test_data_clean"
-    CleanData(input_uuid, output_uuid).transform(drop_na="any")
-
-    input_uuid = "test_data_json"
-    output_uuid = "test_data_json_clean"
     data_to_data = CleanData(input_uuid, output_uuid)
-    data_to_data.set_output_tags(["test", "json", "clean"])
+    data_to_data.set_output_tags(["test", "clean"])
     data_to_data.transform(drop_na="any")
```

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.1.5.1/src/sageworks/transforms/data_to_data/light/data_to_data_light.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class DataToDataLight(Transform):
     """DataToDataLight: Base Class for Light DataSource to DataSource using Pandas
 
     Common Usage:
         to_data = DataToDataLight(input_data_uuid, output_data_uuid)
         to_data.set_output_tags(["abalone", "public", "whatever"])
-        to_data.transform(delete_existing=True/False)
+        to_data.transform()
     """
 
     def __init__(self, input_data_uuid: str, output_data_uuid: str):
         """DataToDataLight Initialization"""
 
         # Call superclass init
         super().__init__(input_data_uuid, output_data_uuid)
@@ -37,23 +37,23 @@
         """Base Class is simply an identity transform"""
         self.output_df = self.input_df
 
     def post_transform(self, **kwargs):
         """At this point the output DataFrame should be populated, so publish it as a DataSource"""
 
         # Now publish to the output location
-        output_data_source = PandasToData(self.output_uuid, **kwargs)
+        output_data_source = PandasToData(self.output_uuid)
         output_data_source.set_input(self.output_df)
         output_data_source.set_output_tags(self.output_tags)
         output_data_source.add_output_meta(self.output_meta)
-        output_data_source.transform()
+        output_data_source.transform(**kwargs)
 
 
 if __name__ == "__main__":
     """Exercise the DataToDataLight Class"""
 
     # Create the class with inputs and outputs and invoke the transform
     input_uuid = "abalone_data"
     output_uuid = "abalone_data_copy"
     data_to_data = DataToDataLight(input_uuid, output_uuid)
     data_to_data.set_output_tags(["abalone", "public"])
-    data_to_data.transform(delete_existing=True)
+    data_to_data.transform()
```

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py` & `sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/heavy/data_to_features_heavy.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class DataToFeaturesHeavy(Transform):
     """DataToFeaturesHeavy: Class to Transform a DataSource into a FeatureSet (Athena/FeatureStore)
 
     Common Usage:
         to_features = DataToFeaturesHeavy(output_uuid)
         to_features.set_output_tags(["abalone", "heavy", "whatever"])
         to_features.set_input(df, id_column="id"/None, event_time_column="date"/None)
-        to_features.transform(delete_existing=True/False)
+        to_features.transform()
     """
 
     def __init__(self, input_uuid: str, output_uuid: str):
         """DataToFeaturesHeavy Initialization"""
 
         # Call superclass init
         super().__init__(input_uuid, output_uuid)
```

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/light/data_to_features_light.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,22 +33,22 @@
         # Grab the Input (Data Source)
         self.input_df = DataToPandas(self.input_uuid).get_output()  # Shorthand for transform, get_output
 
     def transform_impl(self, **kwargs):
         """Base Class is simply an identity transform"""
         self.output_df = self.input_df
 
-    def post_transform(self, id_column=None, event_time_column=None, delete_existing=True):
+    def post_transform(self, id_column=None, event_time_column=None):
         """At this point the output DataFrame should be populated, so publish it as a Feature Set"""
         # Now publish to the output location
         output_features = PandasToFeatures(self.output_uuid)
         output_features.set_input(self.output_df, id_column=id_column, event_time_column=event_time_column)
         output_features.set_output_tags(self.output_tags)
         output_features.add_output_meta(self.output_meta)
-        output_features.transform(delete_existing=delete_existing)
+        output_features.transform()
 
 
 if __name__ == "__main__":
     """Exercise the DataToFeaturesLight Class"""
 
     # Create the class with inputs and outputs and invoke the transform
     input_uuid = "abalone_data"
```

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py` & `sageworks-0.1.5.1/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class RDKitDescriptors(DataToFeaturesLight):
     """RDKitDescriptors: Create a FeatureSet (RDKit Descriptors) from a DataSource
 
     Common Usage:
         to_features = RDKitDescriptors(data_uuid, feature_uuid)
         to_features.set_output_tags(["aqsol", "rdkit", "whatever"])
-        to_features.transform(delete_existing=True/False)
+        to_features.transform()
     """
 
     def __init__(self, data_uuid: str, feature_uuid: str):
         """RDKitDescriptors Initialization"""
 
         # Call superclass init
         super().__init__(data_uuid, feature_uuid)
```

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/features_to_model.py` & `sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/features_to_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """FeaturesToModel: Train/Create a Model from a FeatureSet
 
     Common Usage:
         to_model = FeaturesToModel(feature_uuid, model_uuid)
         to_model.set_output_tags(["abalone", "public", "whatever"])
         to_model.transform(target="class_number_of_rings", description="Abalone Regression Model".
                            input_feature_list=<features>, model_type="regression/classification",
-                           delete_existing=True/False)
+                           )
     """
 
     def __init__(self, feature_uuid: str, model_uuid: str):
         """FeaturesToModel Initialization"""
 
         # Call superclass init
         super().__init__(feature_uuid, model_uuid)
```

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.1.5.1/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.1.5.1/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 
 class ModelToEndpoint(Transform):
     """ModelToEndpoint: Deploy an Endpoint for a Model
 
     Common Usage:
         to_endpoint = ModelToEndpoint(model_uuid, endpoint_uuid)
         to_endpoint.set_output_tags(["aqsol", "public", "whatever"])
-        to_endpoint.transform(delete_existing=True/False)
+        to_endpoint.transform()
     """
 
     def __init__(self, model_uuid: str, endpoint_uuid: str):
         """ModelToEndpoint Initialization"""
 
         # Call superclass init
         super().__init__(model_uuid, endpoint_uuid)
 
         # Set up all my instance attributes
         self.input_type = TransformInput.MODEL
         self.output_type = TransformOutput.ENDPOINT
 
-    def transform_impl(self, delete_existing=True):
+    def transform_impl(self, delete_existing: bool = True):
         """Compute a Feature Set based on RDKit Descriptors"""
 
         # Get the Model Package ARN for our input model
         model_package_arn = Model(self.input_uuid).model_arn()
 
         # Create a Model Package
         model_package = ModelPackage(role=self.sageworks_role_arn, model_package_arn=model_package_arn)
```

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/features_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/pandas_to_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 class PandasToData(Transform):
     """PandasToData: Class to publish a Pandas DataFrame as a DataSource
 
     Common Usage:
         df_to_data = PandasToData(output_uuid)
         df_to_data.set_output_tags(["test", "small"])
         df_to_data.set_input(test_df)
-        df_to_data.transform(delete_existing=True/False)
+        df_to_data.transform()
     """
 
-    def __init__(self, output_uuid: str, output_file_format: str = "parquet", **kwargs):
+    def __init__(self, output_uuid: str, output_file_format: str = "parquet"):
         """PandasToData Initialization
         Args:
             output_uuid (str): The UUID of the DataSource to create
             output_file_format (str): The file format to store the S3 object data in
         """
 
         # Call superclass init
@@ -63,15 +63,15 @@
         """Convert datetime columns to ISO-8601 string"""
         datetime_type = ["datetime", "datetime64", "datetime64[ns]", "datetimetz"]
         for c in df.select_dtypes(include=datetime_type).columns:
             df[c] = df[c].map(datetime_to_iso8601)
             df[c] = df[c].astype(pd.StringDtype())
         return df
 
-    def transform_impl(self, overwrite: bool = True):
+    def transform_impl(self, overwrite: bool = True, **kwargs):
         """Convert the Pandas DataFrame into Parquet Format in the SageWorks S3 Bucket, and
         store the information about the data to the AWS Data Catalog sageworks database
 
         Args:
             overwrite (bool): Overwrite the existing data in the SageWorks S3 Bucket
         """
```

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.1.5.1/src/sageworks/transforms/pandas_transforms/pandas_to_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class PandasToFeatures(Transform):
     """PandasToFeatures: Class to publish a Pandas DataFrame into a FeatureSet (Athena/FeatureStore)
 
     Common Usage:
         to_features = PandasToFeatures(output_uuid)
         to_features.set_output_tags(["abalone", "public", "whatever"])
         to_features.set_input(df, id_column="id"/None, event_time_column="date"/None)
-        to_features.transform(delete_existing=True/False)
+        to_features.transform()
     """
 
     def __init__(self, output_uuid: str):
         """PandasToFeatures Initialization"""
 
         # Call superclass init
         super().__init__("DataFrame", output_uuid)
```

### Comparing `sageworks-0.1.5.0/src/sageworks/transforms/transform.py` & `sageworks-0.1.5.1/src/sageworks/transforms/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,34 +84,38 @@
         """Perform any Pre-Transform operations"""
         self.log.debug("Pre-Transform...")
 
     def post_transform(self, **kwargs):
         """Perform any Post-Transform operations"""
         self.log.info("Post-Transform...")
 
-        # For DataSource and FeatureSet outputs we'll compute sample rows and quartiles
+        # For DataSource and FeatureSet we'll compute sample rows, quartiles, and value counts
         if self.output_type == TransformOutput.DATA_SOURCE:
-            self.log.info("Computing Sample Rows and Quartiles...")
+            self.log.info("Computing Details, Sample Rows, and Quartiles...")
             while not DataSource(self.output_uuid).check():
                 self.log.info("Waiting for DataSource to be created...")
                 sleep(1)
             ds = DataSource(self.output_uuid)
+            ds.refresh(force_fresh=True)
+            ds.details()
             ds.sample_df()
             ds.quartiles()
-            ds.refresh(force_fresh=True)
+            ds.value_counts()
 
         elif self.output_type == TransformOutput.FEATURE_SET:
-            self.log.info("Computing Sample Rows and Quartiles...")
+            self.log.info("Computing Details, Sample Rows, and Quartiles...")
             while not FeatureSet(self.output_uuid).check():
                 self.log.info("Waiting for FeatureSet to be created...")
                 sleep(1)
             fs = FeatureSet(self.output_uuid)
+            fs.refresh(force_fresh=True)
+            fs.details()
             fs.sample_df()
             fs.quartiles()
-            fs.refresh(force_fresh=True)
+            fs.value_counts()
 
     def set_output_tags(self, tags: list | str):
         """Set the tags that will be associated with the output object
         Args:
             tags (list | str): The list of tags or a ':' separated string of tags"""
         if isinstance(tags, list):
             self.output_tags = ":".join(tags)
```

### Comparing `sageworks-0.1.5.0/src/sageworks/utils/cache.py` & `sageworks-0.1.5.1/src/sageworks/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.1.5.1/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/utils/redis_cache.py` & `sageworks-0.1.5.1/src/sageworks/utils/redis_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/utils/sageworks_config.py` & `sageworks-0.1.5.1/src/sageworks/utils/sageworks_config.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.1.5.1/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.1.5.1/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.1.5.1/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/views/artifacts.py` & `sageworks-0.1.5.1/src/sageworks/views/artifacts_text_view.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-"""Artifacts pulls All the metadata from the AWS Service Broker and organizes/summarizes it"""
+"""ArtifactsTextView pulls All the metadata from the AWS Service Broker and organizes/summarizes it"""
 import sys
 import argparse
 import pandas as pd
 from termcolor import colored
 
 # SageWorks Imports
 from sageworks.views.view import View
 from sageworks.aws_service_broker.aws_service_broker import ServiceCategory
 
 
-class Artifacts(View):
+class ArtifactsTextView(View):
     def __init__(self):
-        """Artifacts pulls All the metadata from the AWS Service Broker and organizes/summarizes it"""
+        """ArtifactsTextView pulls All the metadata from the AWS Service Broker and organizes/summarizes it"""
         # Call SuperClass Initialization
         super().__init__()
 
         # Get AWS Service information for ALL the categories (data_source, feature_set, endpoints, etc)
-        self.aws_artifact_data = {}
-        self.refresh()
+        self.aws_artifact_data = self.aws_broker.get_all_metadata()
 
-        # Get a handle to the AWS Artifact Information class
-        self.artifact_info = self.aws_broker.artifact_info
+        # Get AWS Account Region
+        self.aws_region = self.aws_account_clamp.region()
 
         # Setup Pandas output options
         pd.set_option("display.max_colwidth", 50)
         pd.set_option("display.max_columns", 15)
         pd.set_option("display.width", 1000)
 
     def check(self) -> bool:
@@ -35,161 +34,235 @@
         """Refresh data/metadata associated with this view"""
         self.aws_artifact_data = self.aws_broker.get_all_metadata()
 
     def view_data(self) -> dict:
         """Get all the data that's useful for this view
 
         Returns:
-            dict: Dictionary of Pandas Dataframes, e.g. {'INCOMING_DATA': pd.DataFrame, ...}
+            dict: Dictionary of Pandas Dataframes, e.g. {'INCOMING_DATA_S3': pd.DataFrame, ...}
         """
 
         # We're filling in Summary Data for all the AWS Services
         summary_data = {
             "INCOMING_DATA": self.incoming_data_summary(),
             "DATA_SOURCES": self.data_sources_summary(),
             "FEATURE_SETS": self.feature_sets_summary(),
             "MODELS": self.models_summary(),
             "ENDPOINTS": self.endpoints_summary(),
         }
         return summary_data
 
-    def header_text(self, header_text: str) -> str:
+    @staticmethod
+    def header_text(header_text: str) -> str:
         """Colorize text for the terminal"""
         color_map = {
             "INCOMING_DATA": "cyan",
             "DATA_SOURCES": "red",
             "FEATURE_SETS": "yellow",
             "MODELS": "green",
             "ENDPOINTS": "magenta",
         }
         header = f"\n{'='*111}\n{header_text}\n{'='*111}"
         return colored(header, color_map[header_text])
 
-    def dump(self) -> None:
-        """Dump all the data to stdout"""
+    def summary(self) -> None:
+        """Give a summary of all the Artifact data to stdout"""
         for name, df in self.view_data().items():
             print(self.header_text(name))
             if df.empty:
-                print("\tNo Artifacts Found")
+                print("\tNo ArtifactsTextView Found")
             else:
                 print(df.to_string(index=False))
 
     def incoming_data_summary(self) -> pd.DataFrame:
         """Get summary data about data in the incoming-data S3 Bucket"""
-        data = self.aws_artifact_data[ServiceCategory.INCOMING_DATA]
+        data = self.aws_artifact_data[ServiceCategory.INCOMING_DATA_S3]
         data_summary = []
         for name, info in data.items():
             # Get the size of the S3 Storage Object(s)
             size = info.get("ContentLength") / 1_000_000
             summary = {
-                "Name": name,
-                "Size(MB)": f"{size:.1f}",
+                "Name": "/".join(name.split("/")[-2:]).replace("incoming-data/", ""),
+                "Size(MB)": f"{size:.2f}",
                 "Modified": self.datetime_string(info.get("LastModified", "-")),
                 "ContentType": str(info.get("ContentType", "-")),
                 "ServerSideEncryption": info.get("ServerSideEncryption", "-"),
                 "Tags": str(
                     info.get("tags", "-"),
                 ),
             }
             data_summary.append(summary)
-        return pd.DataFrame(data_summary)
+
+        # Make sure we have data else return just the column names
+        if data_summary:
+            return pd.DataFrame(data_summary)
+        else:
+            columns = ["Name", "Size(MB)", "Modified", "ContentType", "ServerSideEncryption", "Tags"]
+            return pd.DataFrame(columns=columns)
 
     def data_sources_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks DataSources"""
-        data = self.aws_artifact_data[ServiceCategory.DATA_CATALOG]
+        data_catalog = self.aws_artifact_data[ServiceCategory.DATA_CATALOG]
         data_summary = []
 
         # Get the SageWorks DataSources
-        if "sageworks" in data:
-            for name, info in data["sageworks"].items():  # Just the sageworks database (not sagemaker_featurestore)
+        if "sageworks" in data_catalog:
+            for name, info in data_catalog["sageworks"].items():  # Just the sageworks database
                 # Get the size of the S3 Storage Object(s)
-                size = self.artifact_info.s3_object_sizes(info["StorageDescriptor"]["Location"])
+                size = self.aws_broker.get_s3_object_sizes(
+                    ServiceCategory.DATA_SOURCES_S3, info["StorageDescriptor"]["Location"]
+                )
+                size = f"{size/1_000_000:.2f}"
                 summary = {
                     "Name": name,
                     "Ver": info.get("VersionId", "-"),
                     "Size(MB)": size,
+                    "Modified": self.datetime_string(info.get("UpdateTime")),
                     "Num Columns": self.num_columns(info),
+                    "DataLake": info.get("IsRegisteredWithLakeFormation", "-"),
                     "Tags": info.get("Parameters", {}).get("sageworks_tags", "-"),
                     "Input": str(
                         info.get("Parameters", {}).get("sageworks_input", "-"),
                     ),
                 }
                 data_summary.append(summary)
-        return pd.DataFrame(data_summary)
+
+        # Make sure we have data else return just the column names
+        if data_summary:
+            return pd.DataFrame(data_summary)
+        else:
+            columns = [
+                "Name",
+                "Ver",
+                "Size(MB)",
+                "Modified",
+                "Num Columns",
+                "DataLake",
+                "Tags",
+                "Input",
+            ]
+            return pd.DataFrame(columns=columns)
 
     def feature_sets_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks FeatureSets"""
         data = self.aws_artifact_data[ServiceCategory.FEATURE_STORE]
         data_summary = []
         for feature_group, group_info in data.items():
-            # Get the tags for this Feature Group
-            arn = group_info["FeatureGroupArn"]
-            sageworks_meta = self.artifact_info.get_sagemaker_obj_info(arn)
+            # Get the SageWorks metadata for this Feature Group
+            sageworks_meta = group_info.get("sageworks_meta", {})
 
             # Get the size of the S3 Storage Object(s)
-            size = self.artifact_info.s3_object_sizes(group_info["OfflineStoreConfig"]["S3StorageConfig"]["S3Uri"])
+            size = self.aws_broker.get_s3_object_sizes(
+                ServiceCategory.FEATURE_SETS_S3, group_info["OfflineStoreConfig"]["S3StorageConfig"]["S3Uri"]
+            )
+            size = f"{size / 1_000_000:.2f}"
             summary = {
                 "Feature Group": group_info["FeatureGroupName"],
                 "Size(MB)": size,
                 "Catalog DB": group_info["OfflineStoreConfig"].get("DataCatalogConfig", {}).get("Database", "-"),
                 "Athena Table": group_info["OfflineStoreConfig"].get("DataCatalogConfig", {}).get("TableName", "-"),
+                "Online": str(group_info.get("OnlineStoreConfig", {}).get("EnableOnlineStore", "False")),
+                "Created": self.datetime_string(group_info.get("CreationTime")),
                 "Tags": sageworks_meta.get("sageworks_tags", "-"),
                 "Input": sageworks_meta.get("sageworks_input", "-"),
             }
             data_summary.append(summary)
-        return pd.DataFrame(data_summary)
+
+        # Make sure we have data else return just the column names
+        if data_summary:
+            return pd.DataFrame(data_summary)
+        else:
+            columns = [
+                "Feature Group",
+                "Size(MB)",
+                "Catalog DB",
+                "Athena Table",
+                "Online",
+                "Created",
+                "Tags",
+                "Input",
+            ]
+            return pd.DataFrame(columns=columns)
 
     def models_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks Models"""
         data = self.aws_artifact_data[ServiceCategory.MODELS]
         model_summary = []
-        for model_group, model_list in data.items():
+        for model_group_info, model_list in data.items():
             # Special Case for Model Groups without any Models
             if not model_list:
-                summary = {"Model Group": model_group}
+                summary = {"Model Group": model_group_info}
                 model_summary.append(summary)
                 continue
 
             # Get Summary information for each model in the model_list
             for model in model_list:
-                # Get the tags for this Model Group
-                model_group_arn = model["ModelPackageGroupArn"]
-                sageworks_meta = self.artifact_info.get_sagemaker_obj_info(model_group_arn)
+                # Get the SageWorks metadata for this Model Group
+                sageworks_meta = model.get("sageworks_meta", {})
                 summary = {
                     "Model Group": model["ModelPackageGroupName"],
+                    "Ver": model["ModelPackageVersion"],
+                    "Status": model["ModelPackageStatus"],
                     "Description": model["ModelPackageDescription"],
                     "Created": self.datetime_string(model.get("CreationTime")),
                     "Tags": sageworks_meta.get("sageworks_tags", "-"),
                     "Input": sageworks_meta.get("sageworks_input", "-"),
                 }
                 model_summary.append(summary)
-        return pd.DataFrame(model_summary)
+
+        # Make sure we have data else return just the column names
+        if model_summary:
+            return pd.DataFrame(model_summary)
+        else:
+            columns = [
+                "Model Group",
+                "Ver",
+                "Status",
+                "Description",
+                "Created",
+                "Tags",
+                "Input",
+            ]
+            return pd.DataFrame(columns=columns)
 
     def endpoints_summary(self) -> pd.DataFrame:
         """Get summary data about the SageWorks Endpoints"""
         data = self.aws_artifact_data[ServiceCategory.ENDPOINTS]
         data_summary = []
 
         # Get Summary information for each endpoint
         for endpoint, endpoint_info in data.items():
-            # Get the tags for this Model Group
-            endpoint_arn = endpoint_info["EndpointArn"]
-            sageworks_meta = self.artifact_info.get_sagemaker_obj_info(endpoint_arn)
+            # Get the SageWorks metadata for this Endpoint
+            sageworks_meta = endpoint_info.get("sageworks_meta", {})
 
             summary = {
                 "Name": endpoint_info["EndpointName"],
                 "Status": endpoint_info["EndpointStatus"],
                 "Created": self.datetime_string(endpoint_info.get("CreationTime")),
                 "DataCapture": str(endpoint_info.get("DataCaptureConfig", {}).get("EnableCapture", "False")),
                 "Sampling(%)": str(endpoint_info.get("DataCaptureConfig", {}).get("CurrentSamplingPercentage", "-")),
                 "Tags": sageworks_meta.get("sageworks_tags", "-"),
                 "Input": sageworks_meta.get("sageworks_input", "-"),
             }
             data_summary.append(summary)
-        return pd.DataFrame(data_summary)
+
+        # Make sure we have data else return just the column names
+        if data_summary:
+            return pd.DataFrame(data_summary)
+        else:
+            columns = [
+                "Name",
+                "Status",
+                "Created",
+                "DataCapture",
+                "Sampling(%)",
+                "Tags",
+                "Input",
+            ]
+            return pd.DataFrame(columns=columns)
 
     @staticmethod
     def num_columns(data_info):
         """Helper: Compute the number of columns from the storage descriptor data"""
         try:
             return len(data_info["StorageDescriptor"]["Columns"])
         except KeyError:
@@ -211,17 +284,14 @@
 
     # Check for unknown args
     if commands:
         print("Unrecognized args: %s" % commands)
         sys.exit(1)
 
     # Create the class and get the AWS Model Registry details
-    artifacts = Artifacts()
+    artifacts = ArtifactsTextView()
 
-    # List the Endpoint Names
-    print("Artifacts:")
-    for category, df in artifacts.view_data().items():
-        print(f"\n{category}")
-        if df.empty:
-            print("\tNo Artifacts Found")
-        else:
-            print(df.head())
+    # Pull the data for all Artifacts in the AWS Account
+    artifacts.view_data()
+
+    # Give a text summary of all the Artifacts in the AWS Account
+    artifacts.summary()
```

### Comparing `sageworks-0.1.5.0/src/sageworks/web_components/box_plot.py` & `sageworks-0.1.5.1/src/sageworks/web_components/box_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.1.5.1/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/web_components/feature_details.py` & `sageworks-0.1.5.1/src/sageworks/web_components/feature_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/web_components/feature_importance.py` & `sageworks-0.1.5.1/src/sageworks/web_components/feature_importance.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/web_components/histogram.py` & `sageworks-0.1.5.1/src/sageworks/web_components/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/web_components/line_chart.py` & `sageworks-0.1.5.1/src/sageworks/web_components/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/web_components/model_data.py` & `sageworks-0.1.5.1/src/sageworks/web_components/model_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/web_components/model_details.py` & `sageworks-0.1.5.1/src/sageworks/web_components/model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/web_components/scatter_plot.py` & `sageworks-0.1.5.1/src/sageworks/web_components/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks/web_components/table.py` & `sageworks-0.1.5.1/src/sageworks/web_components/table.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     # To select rows we need to set up an ID for each row
     df["id"] = df.index
 
     # Only show these columns
     if not show_columns:
         show_columns = df.columns.to_list()
         show_columns.remove("id")
+        if "uuid" in show_columns:
+            show_columns.remove("uuid")
 
     # Column Setup with name, id, and presentation type
     column_setup = []
     for c in show_columns:
         presentation = "markdown" if markdown_columns and c in markdown_columns else "input"
         if columns_editable:
             column_setup.append({"name": c, "id": c, "deletable": True, "selectable": True})
@@ -47,14 +49,15 @@
         style_as_list_view=True,
         style_cell={
             "font-family": "HelveticaNeue",
             "padding": "5px",
             "overflow": "hidden",
             "textOverflow": "ellipsis",
             "maxWidth": 250,
+            "textAlign": "left",
         },
         style_header={
             "textAlign": "left",
             "fontSize": 16,
             "backgroundColor": header_color,
             "color": "rgb(200, 200, 200)",
         },
```

### Comparing `sageworks-0.1.5.0/src/sageworks/web_components/violin_plot.py` & `sageworks-0.1.5.1/src/sageworks/web_components/violin_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.1.5.1/src/sageworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.1.5.0
+Version: 0.1.5.1
 Summary: SageWorks: A Python WorkBench for creating and deploying SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sageworks-0.1.5.0/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.1.5.1/src/sageworks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,14 @@
 src/sageworks/artifacts/feature_sets/__init__.py
 src/sageworks/artifacts/feature_sets/feature_set.py
 src/sageworks/artifacts/models/__init__.py
 src/sageworks/artifacts/models/model.py
 src/sageworks/aws_service_broker/aws_account_clamp.py
 src/sageworks/aws_service_broker/aws_service_broker.py
 src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
-src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py
 src/sageworks/aws_service_broker/aws_service_connectors/connector.py
 src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
 src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
 src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
 src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
 src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
 src/sageworks/transforms/Readme.md
@@ -163,20 +162,21 @@
 src/sageworks/utils/df_to_endpoint.py
 src/sageworks/utils/iso_8601.py
 src/sageworks/utils/redis_cache.py
 src/sageworks/utils/sageworks_config.py
 src/sageworks/utils/sageworks_event_bridge.py
 src/sageworks/utils/sageworks_logging.py
 src/sageworks/utils/sageworks_sqs.py
-src/sageworks/views/artifacts.py
+src/sageworks/views/artifacts_text_view.py
+src/sageworks/views/artifacts_web_view.py
+src/sageworks/views/data_source_web_view.py
 src/sageworks/views/view.py
-src/sageworks/views/web_artifacts_summary.py
-src/sageworks/views/web_data_source_view.py
 src/sageworks/web_components/box_plot.py
 src/sageworks/web_components/confusion_matrix.py
+src/sageworks/web_components/data_source_details.py
 src/sageworks/web_components/feature_details.py
 src/sageworks/web_components/feature_importance.py
 src/sageworks/web_components/histogram.py
 src/sageworks/web_components/line_chart.py
 src/sageworks/web_components/model_data.py
 src/sageworks/web_components/model_details.py
 src/sageworks/web_components/scatter_plot.py
```

### Comparing `sageworks-0.1.5.0/tests/artifacts/data_source_tests.py` & `sageworks-0.1.5.1/tests/artifacts/data_source_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SageWorks Imports
 from sageworks.artifacts.data_sources.athena_source import AthenaSource
 
 
 def test():
     """Tests for the DataSource/AthenaSource functionality"""
+    from pprint import pprint
 
     # Retrieve our test Data Source
     my_data = AthenaSource("test_data")
 
     # Verify that the Athena Data Source exists
     assert my_data.check()
 
@@ -25,18 +26,21 @@
     # What's the size of the data?
     print(f"Size of Data (MB): {my_data.size()}")
 
     # When was it created and last modified?
     print(f"Created: {my_data.created()}")
     print(f"Modified: {my_data.modified()}")
 
-    # Get Metadata and tags associated with this Artifact
-    print(f"Meta: {my_data.meta()}")
+    # Get Tags associated with this Artifact
     print(f"Tags: {my_data.sageworks_tags()}")
 
+    # Get ALL Metadata associated with this Artifact
+    print("\n\nALL Meta")
+    pprint(my_data.all_meta())
+
     # Now delete the AWS artifacts associated with this DataSource
     # print('Deleting SageWorks Data Source...')
     # my_data.delete()
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `sageworks-0.1.5.0/tests/artifacts/endpoint_tests.py` & `sageworks-0.1.5.1/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/tests/artifacts/model_tests.py` & `sageworks-0.1.5.1/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/tests/aws_account/aws_account_clamp_tests.py` & `sageworks-0.1.5.1/tests/aws_account/aws_account_clamp_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.1.5.1/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/tests/create_sageworks_objs_for_tests.py` & `sageworks-0.1.5.1/tests/create_sageworks_objs_for_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.5.0/tests/transforms/data_to_data_tests.py` & `sageworks-0.1.5.1/tests/transforms/pandas_to_data_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-"""Tests for the Data to Data (light) Transforms"""
+"""Tests for the Pandas DataFrame to Data Transforms"""
 
 # Local imports
 from sageworks.transforms.data_to_data.light.data_to_data_light import DataToDataLight
 
 
 def test():
-    """Tests for the Data to Data (light) Transforms"""
+    """Tests for the Pandas DataFrame to Data Transforms"""
 
     # Create the class with inputs and outputs and invoke the transform
     input_uuid = "abalone_data"
     output_uuid = "abalone_data_copy"
     data_to_data = DataToDataLight(input_uuid, output_uuid)
     data_to_data.set_output_tags(["abalone", "public"])
-    data_to_data.transform(delete_existing=True)
+    data_to_data.add_output_meta({"sageworks_input": input_uuid})
+    data_to_data.transform()
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `sageworks-0.1.5.0/tests/transforms/data_to_features_tests.py` & `sageworks-0.1.5.1/tests/transforms/data_to_features_tests.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     """Tests for the Data to Features (light) Transforms"""
 
     # Create the class with inputs and outputs and invoke the transform
     input_uuid = "test_data"
     output_uuid = "test_feature_set"
     data_to_features = DataToFeaturesLight(input_uuid, output_uuid)
     data_to_features.set_output_tags(["test", "small"])
-    data_to_features.transform(id_column="id", event_time_column="date", delete_existing=True)
+    data_to_features.transform(id_column="id", event_time_column="date")
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `sageworks-0.1.5.0/tests/transforms/features_to_model_tests.py` & `sageworks-0.1.5.1/tests/transforms/features_to_model_tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     """Tests for the Features to Model Transforms"""
 
     # Create the class with inputs and outputs and invoke the transform
     input_uuid = "abalone_feature_set"
     output_uuid = "abalone-regression"
     to_model = FeaturesToModel(input_uuid, output_uuid)
     to_model.set_output_tags(["abalone", "public"])
-    to_model.transform(target="class_number_of_rings", delete_existing=True)
+    to_model.transform(target="class_number_of_rings")
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `sageworks-0.1.5.0/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.1.5.1/tests/transforms/model_to_endpoint_tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     """Tests for the Model to Endpoint Transforms"""
 
     # Create the class with inputs and outputs and invoke the transform
     input_uuid = "abalone-regression"
     output_uuid = "abalone-regression-endpoint"
     to_endpoint = ModelToEndpoint(input_uuid, output_uuid)
     to_endpoint.set_output_tags(["abalone", "public"])
-    to_endpoint.transform(delete_existing=True)
+    to_endpoint.transform()
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `sageworks-0.1.5.0/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.1.5.1/tests/transforms/data_to_data_tests.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-"""Tests for the Pandas DataFrame to Data Transforms"""
+"""Tests for the Data to Data (light) Transforms"""
 
 # Local imports
 from sageworks.transforms.data_to_data.light.data_to_data_light import DataToDataLight
 
 
 def test():
-    """Tests for the Pandas DataFrame to Data Transforms"""
+    """Tests for the Data to Data (light) Transforms"""
 
     # Create the class with inputs and outputs and invoke the transform
     input_uuid = "abalone_data"
     output_uuid = "abalone_data_copy"
     data_to_data = DataToDataLight(input_uuid, output_uuid)
     data_to_data.set_output_tags(["abalone", "public"])
-    data_to_data.add_output_meta({"sageworks_input": input_uuid})
-    data_to_data.transform(delete_existing=True)
+    data_to_data.transform()
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `sageworks-0.1.5.0/tox.ini` & `sageworks-0.1.5.1/tox.ini`

 * *Files identical despite different names*

