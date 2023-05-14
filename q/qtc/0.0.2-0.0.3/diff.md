# Comparing `tmp/qtc-0.0.2.tar.gz` & `tmp/qtc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtc-0.0.2.tar", last modified: Sun Apr 30 15:12:40 2023, max compression
+gzip compressed data, was "qtc-0.0.3.tar", last modified: Sun May 14 07:44:49 2023, max compression
```

## Comparing `qtc-0.0.2.tar` & `qtc-0.0.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.668745 qtc-0.0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-04-28 00:35:58.000000 qtc-0.0.2/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2023-04-30 15:12:40.668745 qtc-0.0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-04-28 00:35:58.000000 qtc-0.0.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.648744 qtc-0.0.2/qtc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.652744 qtc-0.0.2/qtc/app_configs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:20.000000 qtc-0.0.2/qtc/app_configs/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.652744 qtc-0.0.2/qtc/app_configs/bq/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:25.000000 qtc-0.0.2/qtc/app_configs/bq/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2023-04-29 15:40:25.000000 qtc-0.0.2/qtc/app_configs/bq/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4648 2023-04-29 15:41:30.000000 qtc-0.0.2/qtc/app_configs/bq/params.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.652744 qtc-0.0.2/qtc/app_configs/bq_sim/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:22.000000 qtc-0.0.2/qtc/app_configs/bq_sim/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5745 2023-04-29 15:40:22.000000 qtc-0.0.2/qtc/app_configs/bq_sim/params.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.652744 qtc-0.0.2/qtc/calendar/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/calendar/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10261 2023-04-28 01:40:37.000000 qtc-0.0.2/qtc/calendar/calendar.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.652744 qtc-0.0.2/qtc/consts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/consts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-04-29 15:42:12.000000 qtc-0.0.2/qtc/consts/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2023-04-30 15:11:38.000000 qtc-0.0.2/qtc/env_config.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5371 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/env_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.656744 qtc-0.0.2/qtc/ext/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/ext/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1459 2023-04-28 01:41:03.000000 qtc-0.0.2/qtc/ext/configurable.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1145 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/ext/enum.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1992 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/ext/inspect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/ext/logging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/ext/multiprocessing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1037 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/ext/unittest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.656744 qtc-0.0.2/qtc/file/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/file/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9319 2023-04-28 01:57:29.000000 qtc-0.0.2/qtc/file/file_cache.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16376 2023-04-28 01:57:29.000000 qtc-0.0.2/qtc/file/file_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30307 2023-04-28 01:57:29.000000 qtc-0.0.2/qtc/file/file_serialization.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.656744 qtc-0.0.2/qtc/toolbox/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/toolbox/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5483 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/toolbox/calcs.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.660744 qtc-0.0.2/qtc/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/qtc/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2691 2023-04-28 02:42:24.000000 qtc-0.0.2/qtc/utils/cipher_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3944 2023-04-28 02:53:51.000000 qtc-0.0.2/qtc/utils/dash_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27303 2023-04-29 14:44:17.000000 qtc-0.0.2/qtc/utils/datetime_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30465 2023-04-28 01:46:30.000000 qtc-0.0.2/qtc/utils/db_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7567 2023-04-28 02:56:22.000000 qtc-0.0.2/qtc/utils/email_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4540 2023-04-28 01:49:03.000000 qtc-0.0.2/qtc/utils/endpoint_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6612 2023-04-28 03:01:16.000000 qtc-0.0.2/qtc/utils/file_system_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7840 2023-04-28 01:53:01.000000 qtc-0.0.2/qtc/utils/html_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6663 2023-04-28 01:57:29.000000 qtc-0.0.2/qtc/utils/misc_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11079 2023-04-28 01:57:29.000000 qtc-0.0.2/qtc/utils/notebook_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-04-28 01:40:20.000000 qtc-0.0.2/qtc/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.652744 qtc-0.0.2/qtc.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2023-04-30 15:12:40.000000 qtc-0.0.2/qtc.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1500 2023-04-30 15:12:40.000000 qtc-0.0.2/qtc.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-30 15:12:40.000000 qtc-0.0.2/qtc.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-29 14:49:44.000000 qtc-0.0.2/qtc.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-04-30 15:12:40.000000 qtc-0.0.2/qtc.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-04-30 15:12:40.000000 qtc-0.0.2/qtc.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-30 15:12:40.668745 qtc-0.0.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      763 2023-04-28 03:01:16.000000 qtc-0.0.2/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.664744 qtc-0.0.2/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.664744 qtc-0.0.2/tests/ext/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/ext/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1003 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/ext/test_enum.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/ext/test_inspect.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.664744 qtc-0.0.2/tests/file/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/file/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/file/test_file_cache.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3244 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/file/test_file_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5806 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/file/test_file_serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      431 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/test_env_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 15:12:40.668745 qtc-0.0.2/tests/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      558 2023-04-28 02:46:02.000000 qtc-0.0.2/tests/utils/test_cipher_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3939 2023-04-28 02:45:02.000000 qtc-0.0.2/tests/utils/test_datetime_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2604 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/utils/test_db_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1855 2023-04-28 00:35:58.000000 qtc-0.0.2/tests/utils/test_misc_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.515946 qtc-0.0.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-04-28 00:35:58.000000 qtc-0.0.3/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-05-14 07:44:49.515946 qtc-0.0.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-04-28 00:35:58.000000 qtc-0.0.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.495946 qtc-0.0.3/qtc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.495946 qtc-0.0.3/qtc/app_configs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:20.000000 qtc-0.0.3/qtc/app_configs/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.495946 qtc-0.0.3/qtc/app_configs/bq/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:25.000000 qtc-0.0.3/qtc/app_configs/bq/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2023-04-29 15:40:25.000000 qtc-0.0.3/qtc/app_configs/bq/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4648 2023-04-29 15:41:30.000000 qtc-0.0.3/qtc/app_configs/bq/params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.499945 qtc-0.0.3/qtc/app_configs/bq_sim/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:22.000000 qtc-0.0.3/qtc/app_configs/bq_sim/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5745 2023-04-29 15:40:22.000000 qtc-0.0.3/qtc/app_configs/bq_sim/params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.499945 qtc-0.0.3/qtc/calendar/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/calendar/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10261 2023-04-28 01:40:37.000000 qtc-0.0.3/qtc/calendar/calendar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.499945 qtc-0.0.3/qtc/consts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/consts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-04-29 15:42:12.000000 qtc-0.0.3/qtc/consts/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2023-04-30 15:11:38.000000 qtc-0.0.3/qtc/env_config.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5371 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/env_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.503945 qtc-0.0.3/qtc/ext/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/ext/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1459 2023-04-28 01:41:03.000000 qtc-0.0.3/qtc/ext/configurable.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1145 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/ext/enum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1992 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/ext/inspect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/ext/logging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/ext/multiprocessing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1037 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/ext/unittest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.503945 qtc-0.0.3/qtc/file/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/file/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9319 2023-04-28 01:57:29.000000 qtc-0.0.3/qtc/file/file_cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16376 2023-04-28 01:57:29.000000 qtc-0.0.3/qtc/file/file_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30307 2023-04-28 01:57:29.000000 qtc-0.0.3/qtc/file/file_serialization.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.503945 qtc-0.0.3/qtc/toolbox/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/toolbox/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-13 06:34:37.000000 qtc-0.0.3/qtc/toolbox/calcs.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.511946 qtc-0.0.3/qtc/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2639 2023-04-30 15:30:33.000000 qtc-0.0.3/qtc/utils/cipher_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3931 2023-04-30 15:30:33.000000 qtc-0.0.3/qtc/utils/dash_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27238 2023-04-30 15:30:33.000000 qtc-0.0.3/qtc/utils/datetime_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30426 2023-04-30 15:30:33.000000 qtc-0.0.3/qtc/utils/db_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7567 2023-04-28 02:56:22.000000 qtc-0.0.3/qtc/utils/email_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4540 2023-04-28 01:49:03.000000 qtc-0.0.3/qtc/utils/endpoint_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6612 2023-04-28 03:01:16.000000 qtc-0.0.3/qtc/utils/file_system_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7840 2023-04-28 01:53:01.000000 qtc-0.0.3/qtc/utils/html_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6663 2023-04-28 01:57:29.000000 qtc-0.0.3/qtc/utils/misc_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11079 2023-04-28 01:57:29.000000 qtc-0.0.3/qtc/utils/notebook_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-05-13 06:38:50.000000 qtc-0.0.3/qtc/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.495946 qtc-0.0.3/qtc.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-05-14 07:44:49.000000 qtc-0.0.3/qtc.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1500 2023-05-14 07:44:49.000000 qtc-0.0.3/qtc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-14 07:44:49.000000 qtc-0.0.3/qtc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-29 14:49:44.000000 qtc-0.0.3/qtc.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       66 2023-05-14 07:44:49.000000 qtc-0.0.3/qtc.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-05-14 07:44:49.000000 qtc-0.0.3/qtc.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-14 07:44:49.515946 qtc-0.0.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      724 2023-05-13 06:37:41.000000 qtc-0.0.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.511946 qtc-0.0.3/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.511946 qtc-0.0.3/tests/ext/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/ext/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1003 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/ext/test_enum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/ext/test_inspect.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.511946 qtc-0.0.3/tests/file/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/file/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/file/test_file_cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3244 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/file/test_file_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5806 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/file/test_file_serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      431 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/test_env_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.515946 qtc-0.0.3/tests/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      558 2023-04-28 02:46:02.000000 qtc-0.0.3/tests/utils/test_cipher_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3939 2023-04-28 02:45:02.000000 qtc-0.0.3/tests/utils/test_datetime_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2604 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/utils/test_db_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1855 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/utils/test_misc_utils.py
```

### Comparing `qtc-0.0.2/qtc/app_configs/bq/params.py` & `qtc-0.0.3/qtc/app_configs/bq/params.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/app_configs/bq_sim/params.py` & `qtc-0.0.3/qtc/app_configs/bq_sim/params.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/calendar/calendar.py` & `qtc-0.0.3/qtc/calendar/calendar.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/consts/enums.py` & `qtc-0.0.3/qtc/consts/enums.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/env_config.py` & `qtc-0.0.3/qtc/env_config.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/ext/configurable.py` & `qtc-0.0.3/qtc/ext/configurable.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/ext/enum.py` & `qtc-0.0.3/qtc/ext/enum.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/ext/inspect.py` & `qtc-0.0.3/qtc/ext/inspect.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/ext/logging.py` & `qtc-0.0.3/qtc/ext/logging.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/ext/multiprocessing.py` & `qtc-0.0.3/qtc/ext/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/ext/unittest.py` & `qtc-0.0.3/qtc/ext/unittest.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/file/file_cache.py` & `qtc-0.0.3/qtc/file/file_cache.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/file/file_manager.py` & `qtc-0.0.3/qtc/file/file_manager.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/file/file_serialization.py` & `qtc-0.0.3/qtc/file/file_serialization.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/utils/cipher_utils.py` & `qtc-0.0.3/qtc/utils/cipher_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import typing as T
 
 _BASE_SALT = 'QuantTrading'
 
 
 def intersperse(str1: str, str2: str) -> str:
     """Mixes together two strings.  If one string is longer, the shorter sting is cycled.
-    >>> import sysequity_common.utils.cipher_utils as cu
+    >>> import qtc.utils.cipher_utils as cu
     >>> cu.intersperse('foo', 'bar')
     'fboaor'
     >>> cu.intersperse('steven', '_-')
     's_t-e_v-e_n-'
     """
     piece_len = max(len(str1), len(str2))
     combined = [None] * 2 * piece_len
@@ -23,44 +23,44 @@
     combined[0::2] = itertools.islice(itertools.cycle(str1), piece_len) # type: ignore
     combined[1::2] = itertools.islice(itertools.cycle(str2), piece_len) # type: ignore
     return ''.join(map(str, combined))
 
 
 def scramble(secret: str, *, salt: str = 'AbCdEfG') -> bytes:
     """Apply a salt to a secret string using xor.
-    >>> import sysequity_common.utils.cipher_utils as cu
+    >>> import qtc.utils.cipher_utils as cu
     >>> str(cu.scramble('ABC', salt='ABC'))
     "b'\\\\x00\\\\x00\\\\x00'"
     >>> str(cu.scramble('ABCABC', salt='ABC'))
     "b'\\\\x00\\\\x00\\\\x00\\\\x00\\\\x00\\\\x00'"
     >>> str(cu.scramble('AAA', salt='ABC'))
     "b'\\\\x00\\\\x03\\\\x02'"
     >>> str(cu.scramble('AAAAAA', salt='ABC'))
     "b'\\\\x00\\\\x03\\\\x02\\\\x00\\\\x03\\\\x02'"
     """
     return bytes((ord(a) ^ ord(b)) for (a, b) in zip(secret, itertools.cycle(salt)))
 
 
 def to_salted(text: str, user: str = None) -> str:
     """Encode a text string by salt
-    >>> import sysequity_common.utils.cipher_utils as cu
+    >>> import qtc.utils.cipher_utils as cu
     >>> cu.to_salted(text='Hello World')
     '0a040d0403552e0e130417'
     """
     if user is None:
         user = getpass.getuser()
     salt = intersperse(_BASE_SALT, user)
     secret = scramble(text, salt=salt)
     secret_str = ''.join('{:02x}'.format(b) for b in secret)
     return secret_str
 
 
 def from_salted(secret_str: str, user: str = None) -> str:
     """Decodes a salted string
-    >>> import sysequity_common.utils.cipher_utils as cu
+    >>> import qtc.utils.cipher_utils as cu
     >>> cu.from_salted(secret_str='0a040d0403552e0e130417')
     'Hello World'
     """
     if user is None:
         user = getpass.getuser()
     salt = intersperse(_BASE_SALT, user)
     secret_chars = bytearray.fromhex(secret_str)
```

### Comparing `qtc-0.0.2/qtc/utils/dash_utils.py` & `qtc-0.0.3/qtc/utils/dash_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #     instead of in this python module
 ####################################################################
 
 DEFAULT_DASH_TABLE_STYLES = None
 def get_dash_table_styles(apply_defaults=True,
                           bold_cols=None):
     """
-    >>> import sysequity_common.utils.dash_utils as dashu
+    >>> import qtc.utils.dash_utils as dashu
     """
     global DEFAULT_DASH_TABLE_STYLES
     if apply_defaults:
         if DEFAULT_DASH_TABLE_STYLES is None:
             style_data_conditional = [{
                 'if': {'row_index': 'odd'},
                 # 'backgroundColor': 'rgb(220, 220, 220)',
```

### Comparing `qtc-0.0.2/qtc/utils/datetime_utils.py` & `qtc-0.0.3/qtc/utils/datetime_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
         ttm_start_date = date.replace(year=date.year-1, day=date.day-1)
 
     return normalize_date_to_dateid(date=ttm_start_date)
 
 
 def get_quarter_start_dateid(date):
     """
-    >>> import sysequity_common.utils.datetime_utils as dtu
+    >>> import qtc.utils.datetime_utils as dtu
     >>> dtu.get_quarter_start_dateid(date=20220630)
     20220401
     >>> dtu.get_quarter_start_dateid(date=20220715)
     20220701
     """
     date = parse_datetime(dt=date)
     quarter_start_date = datetime(date.year, 3 * ((date.month - 1) // 3) + 1, 1)
@@ -354,15 +354,15 @@
 
     return EXCHANGE_SESSIONS_CFG
 
 
 
 def get_exchange_sessions(date):
     """
-    >>> import sysequity_common.utils.datetime_utils as dtu
+    >>> import qtc.utils.datetime_utils as dtu
     >>> dtu.get_exchange_sessions(date=20220425)
         MIC Region          Timezone OpenTimeLocal CloseTimeLocal          OpenDateTimeLocal         CloseDateTimeLocal           OpenDateTimeUTC          CloseDateTimeUTC
     0  XASX     AP  Australia/Sydney      10:00:00       16:00:00  2022-04-25 10:00:00+10:00  2022-04-25 16:00:00+10:00 2022-04-25 00:00:00+00:00 2022-04-25 06:00:00+00:00
     1  XSES     AP    Asia/Singapore      09:00:00       17:00:00  2022-04-25 09:00:00+08:00  2022-04-25 17:00:00+08:00 2022-04-25 01:00:00+00:00 2022-04-25 09:00:00+00:00
     2  XHEL     EU   Europe/Helsinki      10:00:00       18:25:00  2022-04-25 10:00:00+03:00  2022-04-25 18:25:00+03:00 2022-04-25 07:00:00+00:00 2022-04-25 15:25:00+00:00
     3  XLIS     EU     Europe/Lisbon      08:00:00       16:30:00  2022-04-25 08:00:00+01:00  2022-04-25 16:30:00+01:00 2022-04-25 07:00:00+00:00 2022-04-25 15:30:00+00:00
     4  XNYS     US  America/New_York      09:30:00       16:00:00  2022-04-25 09:30:00-04:00  2022-04-25 16:00:00-04:00 2022-04-25 13:30:00+00:00 2022-04-25 20:00:00+00:00
@@ -397,15 +397,15 @@
     exchange_sessions['CloseDateTimeUTC'] = exchange_sessions['CloseDateTimeLocal'].apply(lambda x: x.astimezone(timezone.utc))
 
     return exchange_sessions
 
 
 def get_region_sessions(date):
     """
-    >>> import sysequity_common.utils.datetime_utils as dtu
+    >>> import qtc.utils.datetime_utils as dtu
     >>> dtu.get_region_sessions(date=20230425)
                     StartDateTimeUTC            EndDateTimeUTC
     Region
     AP     2023-04-25 00:00:00+00:00 2023-04-25 09:00:00+00:00
     EU     2023-04-25 07:00:00+00:00 2023-04-25 15:30:00+00:00
     US     2023-04-25 13:30:00+00:00 2023-04-25 20:00:00+00:00
     WW     2023-04-25 00:00:00+00:00 2023-04-25 20:00:00+00:00
@@ -440,15 +440,15 @@
     return region_sessions
 
 
 def infer_region_cutoff_dts(dateid=None, now=None,
                             region='WW',
                             ext_minutes=None):
     """
-    >>> import sysequity_common.utils.datetime_utils as dtu
+    >>> import qtc.utils.datetime_utils as dtu
     >>> dtu.infer_region_cutoff_dts(dateid=20240101)
     (Timestamp('2024-01-01 23:00:00+0000', tz='UTC'),
      Timestamp('2024-01-02 21:00:00+0000', tz='UTC'))
     >>> dtu.infer_region_cutoff_dts(dateid=20230422)
     (Timestamp('2023-04-24 00:00:00+0000', tz='UTC'),
      Timestamp('2023-04-24 20:00:00+0000', tz='UTC'))
     >>> dtu.infer_region_cutoff_dts(dateid=20230425)
@@ -538,15 +538,15 @@
 #     return TRADING_SESSIONS
 
 
 # def get_region_start_end_dt(dateid=None, region=None,
 #                             now=None,
 #                             ext_minutes=0):
 #     """
-#     >>> import sysequity_common.utils.datetime_utils as dtu
+#     >>> import qtc.utils.datetime_utils as dtu
 #     >>> dtu.get_region_start_end_dt(dateid=20230417)
 #     (Timestamp('2023-04-17 00:00:00+0000', tz='UTC'),
 #      Timestamp('2023-04-17 20:00:00+0000', tz='UTC'))
 #     >>> dtu.get_region_start_end_dt(dateid=20230416)
 #     (Timestamp('2023-04-17 00:00:00+0000', tz='UTC'),
 #      Timestamp('2023-04-17 20:00:00+0000', tz='UTC'))
 #     >>> dtu.get_region_start_end_dt(dateid=20230103)
```

### Comparing `qtc-0.0.2/qtc/utils/db_utils.py` & `qtc-0.0.3/qtc/utils/db_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,19 +343,19 @@
                   sql=None):
     """Infers the final columns based on all "available_cols", "required_cols"(usually key columns in the DB table)
     and user "expected_cols", which could overlap with "required_cols".
     If "required_cols" is not None, then the returned cols will have "required_cols" first and then other columns if more columns should be returned.
     If "expected_cols" is None, then return all "available_cols". Otherwise, return "required_cols"+"expected_cols".
 
     :param available_cols: All available columns. Please note that it cannot be None.
-    :type available_cols: str | int | Iterable. See :func:`sysequity_common.utils.misc.iterable_to_tuple`
+    :type available_cols: str | int | Iterable. See :func:`qtc.utils.misc.iterable_to_tuple`
     :param required_cols: Required columns. If not found in the available columns, exception handling will depend on 'raise_exception_on_not_found_required_cols'.
-    :type required_cols: str | int | Iterable. See :func:`sysequity_common.utils.misc.iterable_to_tuple`
+    :type required_cols: str | int | Iterable. See :func:`qtc.utils.misc.iterable_to_tuple`
     :param expected_cols: User expected columns.
-    :type expected_cols: str | int | Iterable. See :func:`sysequity_common.utils.misc.iterable_to_tuple`
+    :type expected_cols: str | int | Iterable. See :func:`qtc.utils.misc.iterable_to_tuple`
     :param raise_exception_on_not_found_required_cols: If True, throw exception if there are some required columns which cannot be found in available columns.
     :type raise_exception_on_not_found_required_cols: bool
     :return: list - Return columns.
 
     >>> import qtc.utils.db_utils as dbu
     >>> dbu._process_cols(available_cols='SecurityId,AxiomaId,BbergCode,NMV,Return', required_cols='SecurityId', expected_cols='NMV,Return')
     ['SecurityId', 'NMV', 'Return']
```

### Comparing `qtc-0.0.2/qtc/utils/email_utils.py` & `qtc-0.0.3/qtc/utils/email_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/utils/endpoint_utils.py` & `qtc-0.0.3/qtc/utils/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/utils/file_system_utils.py` & `qtc-0.0.3/qtc/utils/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/utils/html_utils.py` & `qtc-0.0.3/qtc/utils/html_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/utils/misc_utils.py` & `qtc-0.0.3/qtc/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc/utils/notebook_utils.py` & `qtc-0.0.3/qtc/utils/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/qtc.egg-info/SOURCES.txt` & `qtc-0.0.3/qtc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/setup.py` & `qtc-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,26 @@
 setup(
     name='qtc',
     version=__version__,
     url='',
     license='',
     author='Andrew Hu',
     author_email='AndrewWeiHu@gmail.com',
-    description='Quant Trading Common',
+    description='Quant Trading',
     packages=find_packages(exclude=['backup']),
     zip_safe=False,
     include_package_data=True,
     platforms='any',
     install_requires=[
-        'pandas>=1.3.4',
+        'pandas>=1.4.3',
         'joblib',
         'sqlalchemy',
+        # 'pymssql',
         'psycopg2',
         'pyarrow',
         'datatable',
-        'pytest-html',
         'pyyaml',
-        'requests-kerberos',
     ],
     tests_require=[
         'pytest'
     ],
 )
```

### Comparing `qtc-0.0.2/tests/ext/test_enum.py` & `qtc-0.0.3/tests/ext/test_enum.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/tests/ext/test_inspect.py` & `qtc-0.0.3/tests/ext/test_inspect.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/tests/file/test_file_cache.py` & `qtc-0.0.3/tests/file/test_file_cache.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/tests/file/test_file_manager.py` & `qtc-0.0.3/tests/file/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/tests/file/test_file_serialization.py` & `qtc-0.0.3/tests/file/test_file_serialization.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/tests/utils/test_cipher_utils.py` & `qtc-0.0.3/tests/utils/test_cipher_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/tests/utils/test_datetime_utils.py` & `qtc-0.0.3/tests/utils/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/tests/utils/test_db_utils.py` & `qtc-0.0.3/tests/utils/test_db_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.2/tests/utils/test_misc_utils.py` & `qtc-0.0.3/tests/utils/test_misc_utils.py`

 * *Files identical despite different names*

