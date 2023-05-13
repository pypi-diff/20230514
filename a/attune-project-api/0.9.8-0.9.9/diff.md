# Comparing `tmp/attune-project-api-0.9.8.tar.gz` & `tmp/attune-project-api-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attune-project-api-0.9.8.tar", last modified: Mon Mar  6 02:26:45 2023, max compression
+gzip compressed data, was "attune-project-api-0.9.9.tar", last modified: Mon Mar  6 02:46:17 2023, max compression
```

## Comparing `attune-project-api-0.9.8.tar` & `attune-project-api-0.9.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:26:45.112128 attune-project-api-0.9.8/
--rw-r--r--   0 jchesney   (501) staff       (20)      262 2023-03-06 02:26:45.112336 attune-project-api-0.9.8/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)       60 2021-12-30 21:22:50.000000 attune-project-api-0.9.8/README.rst
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:26:45.076720 attune-project-api-0.9.8/attune_project_api/
--rw-r--r--   0 jchesney   (501) staff       (20)      692 2022-10-03 05:25:18.000000 attune-project-api-0.9.8/attune_project_api/Exceptions.py
--rw-r--r--   0 jchesney   (501) staff       (20)    28139 2023-03-06 02:26:35.000000 attune-project-api-0.9.8/attune_project_api/ObjectStorageContext.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4257 2022-02-24 06:08:44.000000 attune-project-api-0.9.8/attune_project_api/RelationField.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4299 2023-02-09 04:10:25.000000 attune-project-api-0.9.8/attune_project_api/StorageTuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2113 2022-01-07 01:53:29.000000 attune-project-api-0.9.8/attune_project_api/TupleFieldValidators.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2820 2022-01-12 10:25:43.000000 attune-project-api-0.9.8/attune_project_api/TupleValidators.py
--rw-r--r--   0 jchesney   (501) staff       (20)      315 2023-03-06 02:26:44.000000 attune-project-api-0.9.8/attune_project_api/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:26:45.080747 attune-project-api-0.9.8/attune_project_api/_contexts/
--rw-r--r--   0 jchesney   (501) staff       (20)    30967 2023-03-02 23:49:09.000000 attune-project-api-0.9.8/attune_project_api/_contexts/GitLibMixin.py
--rw-r--r--   0 jchesney   (501) staff       (20)    29528 2023-03-06 02:26:35.000000 attune-project-api-0.9.8/attune_project_api/_contexts/GitObjectStorageContext.py
--rw-r--r--   0 jchesney   (501) staff       (20)       39 2021-12-30 21:22:50.000000 attune-project-api-0.9.8/attune_project_api/_contexts/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:26:45.086933 attune-project-api-0.9.8/attune_project_api/_private/
--rw-r--r--   0 jchesney   (501) staff       (20)     1142 2022-01-07 01:53:29.000000 attune-project-api-0.9.8/attune_project_api/_private/RelationGraph.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-12-30 21:22:50.000000 attune-project-api-0.9.8/attune_project_api/_private/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3241 2022-05-23 00:41:40.000000 attune-project-api-0.9.8/attune_project_api/_private/archive_format.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3428 2023-02-28 01:54:20.000000 attune-project-api-0.9.8/attune_project_api/_private/archive_get_file_content.py
--rw-r--r--   0 jchesney   (501) staff       (20)      596 2022-01-07 03:41:18.000000 attune-project-api-0.9.8/attune_project_api/_private/archive_hasher.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3019 2022-05-23 00:41:40.000000 attune-project-api-0.9.8/attune_project_api/_private/archive_list_files.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3683 2022-07-01 03:12:12.000000 attune-project-api-0.9.8/attune_project_api/_private/large_file_http_downloader.py
--rw-r--r--   0 jchesney   (501) staff       (20)      661 2022-01-25 22:57:26.000000 attune-project-api-0.9.8/attune_project_api/_private/large_file_http_downloader_test.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1677 2023-02-03 06:38:08.000000 attune-project-api-0.9.8/attune_project_api/_private/readme_compiler.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:26:45.092435 attune-project-api-0.9.8/attune_project_api/_private/templates/
--rw-r--r--   0 jchesney   (501) staff       (20)     1357 2023-02-26 22:18:39.000000 attune-project-api-0.9.8/attune_project_api/_private/templates/ProjectReadme.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      868 2023-02-10 03:43:12.000000 attune-project-api-0.9.8/attune_project_api/_private/templates/ProjectReadmeAttune.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      267 2023-02-10 03:43:12.000000 attune-project-api-0.9.8/attune_project_api/_private/templates/ProjectReadmeBlueprints.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)     1608 2023-02-26 22:18:39.000000 attune-project-api-0.9.8/attune_project_api/_private/templates/ProjectReadmeCloneInstructions.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      787 2023-02-26 22:18:39.000000 attune-project-api-0.9.8/attune_project_api/_private/templates/ProjectReadmeContribute.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      185 2023-02-10 03:43:12.000000 attune-project-api-0.9.8/attune_project_api/_private/templates/ProjectReadmeFiles.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)      312 2023-02-10 03:43:12.000000 attune-project-api-0.9.8/attune_project_api/_private/templates/ProjectReadmeParameters.md.mako
--rw-r--r--   0 jchesney   (501) staff       (20)       27 2022-10-21 00:47:49.000000 attune-project-api-0.9.8/attune_project_api/_private/templates/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)      544 2023-01-23 02:29:43.000000 attune-project-api-0.9.8/attune_project_api/_private/utils.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2948 2022-05-04 02:21:42.000000 attune-project-api-0.9.8/attune_project_api/alembic.ini
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:26:45.094266 attune-project-api-0.9.8/attune_project_api/alembic_migrations/
--rw-r--r--   0 jchesney   (501) staff       (20)       38 2022-05-04 02:21:42.000000 attune-project-api-0.9.8/attune_project_api/alembic_migrations/README
--rw-r--r--   0 jchesney   (501) staff       (20)     2038 2022-05-04 02:21:42.000000 attune-project-api-0.9.8/attune_project_api/alembic_migrations/env.py
--rw-r--r--   0 jchesney   (501) staff       (20)      494 2022-05-04 02:21:42.000000 attune-project-api-0.9.8/attune_project_api/alembic_migrations/script.py.mako
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:26:45.097418 attune-project-api-0.9.8/attune_project_api/alembic_migrations/versions/
--rw-r--r--   0 jchesney   (501) staff       (20)     1115 2023-02-03 04:14:24.000000 attune-project-api-0.9.8/attune_project_api/alembic_migrations/versions/0aa489aa66b2_store_name_in_project_metadata.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1173 2023-02-10 02:46:44.000000 attune-project-api-0.9.8/attune_project_api/alembic_migrations/versions/145c6dc54454_rename_comment_md_to_readme_md_for_items.py
--rw-r--r--   0 jchesney   (501) staff       (20)      417 2022-05-04 02:21:42.000000 attune-project-api-0.9.8/attune_project_api/alembic_migrations/versions/16e34a42a9a1_attune_v5_starting_point.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1859 2022-05-04 02:21:42.000000 attune-project-api-0.9.8/attune_project_api/alembic_migrations/versions/58b1656aac40_move_sql_to_script_txt_file_in_oracle_.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1332 2023-02-03 04:14:24.000000 attune-project-api-0.9.8/attune_project_api/alembic_migrations/versions/ba6a8e4d7e2b_move_metadata_json_file_to_project_.py
--rw-r--r--   0 jchesney   (501) staff       (20)      215 2023-02-03 04:14:24.000000 attune-project-api-0.9.8/attune_project_api/context_project_info.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:26:45.099430 attune-project-api-0.9.8/attune_project_api/items/
--rw-r--r--   0 jchesney   (501) staff       (20)      489 2022-01-07 01:53:29.000000 attune-project-api-0.9.8/attune_project_api/items/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:26:45.101892 attune-project-api-0.9.8/attune_project_api/items/file_archive_tuples/
--rw-r--r--   0 jchesney   (501) staff       (20)      163 2022-01-07 01:53:29.000000 attune-project-api-0.9.8/attune_project_api/items/file_archive_tuples/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4776 2023-03-06 02:26:35.000000 attune-project-api-0.9.8/attune_project_api/items/file_archive_tuples/file_archive_large_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2548 2023-03-06 02:26:35.000000 attune-project-api-0.9.8/attune_project_api/items/file_archive_tuples/file_archive_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     6158 2023-03-06 02:26:35.000000 attune-project-api-0.9.8/attune_project_api/items/file_archive_tuples/file_archive_versioned_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)      482 2022-02-28 06:52:20.000000 attune-project-api-0.9.8/attune_project_api/items/file_archive_tuples/file_tuple_constants.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3087 2022-01-07 01:53:29.000000 attune-project-api-0.9.8/attune_project_api/items/parameter_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)      645 2023-02-03 04:14:24.000000 attune-project-api-0.9.8/attune_project_api/items/project_metadata_tuple.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:26:45.110113 attune-project-api-0.9.8/attune_project_api/items/step_tuples/
--rw-r--r--   0 jchesney   (501) staff       (20)      928 2022-01-12 10:38:07.000000 attune-project-api-0.9.8/attune_project_api/items/step_tuples/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1210 2022-01-07 01:53:29.000000 attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_bootstrap_linux_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2855 2022-01-13 14:55:18.000000 attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_group_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2791 2023-01-23 02:29:49.000000 attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_project_link_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2706 2022-02-24 06:08:31.000000 attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_push_design_file_compiled_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1692 2022-10-26 23:25:34.000000 attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_push_design_file_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1786 2022-01-14 07:57:32.000000 attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_sql_oracle_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1040 2022-01-07 01:53:29.000000 attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_ssh_prompted_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2086 2022-01-07 01:53:29.000000 attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_ssh_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1250 2022-01-07 01:53:29.000000 attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_tcp_ping_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2190 2023-02-03 06:38:08.000000 attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2499 2022-01-07 01:53:29.000000 attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_winrm_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4079 2023-02-28 01:54:20.000000 attune-project-api-0.9.8/attune_project_api/migration.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:26:45.111569 attune-project-api-0.9.8/attune_project_api/tuples/
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-12-30 21:22:50.000000 attune-project-api-0.9.8/attune_project_api/tuples/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)      366 2022-01-07 01:53:29.000000 attune-project-api-0.9.8/attune_project_api/tuples/git_commit_tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1123 2023-01-23 02:29:43.000000 attune-project-api-0.9.8/attune_project_api/tuples/project_modified_tuple.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:26:45.078877 attune-project-api-0.9.8/attune_project_api.egg-info/
--rw-r--r--   0 jchesney   (501) staff       (20)      262 2023-03-06 02:26:44.000000 attune-project-api-0.9.8/attune_project_api.egg-info/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)     3773 2023-03-06 02:26:45.000000 attune-project-api-0.9.8/attune_project_api.egg-info/SOURCES.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-03-06 02:26:45.000000 attune-project-api-0.9.8/attune_project_api.egg-info/dependency_links.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-03-06 02:26:44.000000 attune-project-api-0.9.8/attune_project_api.egg-info/not-zip-safe
--rw-r--r--   0 jchesney   (501) staff       (20)      134 2023-03-06 02:26:45.000000 attune-project-api-0.9.8/attune_project_api.egg-info/requires.txt
--rw-r--r--   0 jchesney   (501) staff       (20)       19 2023-03-06 02:26:45.000000 attune-project-api-0.9.8/attune_project_api.egg-info/top_level.txt
--rw-r--r--   0 jchesney   (501) staff       (20)       80 2023-03-06 02:26:45.112879 attune-project-api-0.9.8/setup.cfg
--rw-r--r--   0 jchesney   (501) staff       (20)     2202 2023-03-06 02:26:44.000000 attune-project-api-0.9.8/setup.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:46:17.200623 attune-project-api-0.9.9/
+-rw-r--r--   0 jchesney   (501) staff       (20)      262 2023-03-06 02:46:17.200831 attune-project-api-0.9.9/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)       60 2021-12-30 21:22:50.000000 attune-project-api-0.9.9/README.rst
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:46:17.174643 attune-project-api-0.9.9/attune_project_api/
+-rw-r--r--   0 jchesney   (501) staff       (20)      692 2022-10-03 05:25:18.000000 attune-project-api-0.9.9/attune_project_api/Exceptions.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    28139 2023-03-06 02:26:35.000000 attune-project-api-0.9.9/attune_project_api/ObjectStorageContext.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4257 2022-02-24 06:08:44.000000 attune-project-api-0.9.9/attune_project_api/RelationField.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4299 2023-02-09 04:10:25.000000 attune-project-api-0.9.9/attune_project_api/StorageTuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2113 2022-01-07 01:53:29.000000 attune-project-api-0.9.9/attune_project_api/TupleFieldValidators.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2820 2022-01-12 10:25:43.000000 attune-project-api-0.9.9/attune_project_api/TupleValidators.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      315 2023-03-06 02:46:16.000000 attune-project-api-0.9.9/attune_project_api/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:46:17.178403 attune-project-api-0.9.9/attune_project_api/_contexts/
+-rw-r--r--   0 jchesney   (501) staff       (20)    30967 2023-03-02 23:49:09.000000 attune-project-api-0.9.9/attune_project_api/_contexts/GitLibMixin.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    29528 2023-03-06 02:26:35.000000 attune-project-api-0.9.9/attune_project_api/_contexts/GitObjectStorageContext.py
+-rw-r--r--   0 jchesney   (501) staff       (20)       39 2021-12-30 21:22:50.000000 attune-project-api-0.9.9/attune_project_api/_contexts/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:46:17.182147 attune-project-api-0.9.9/attune_project_api/_private/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1142 2022-01-07 01:53:29.000000 attune-project-api-0.9.9/attune_project_api/_private/RelationGraph.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-12-30 21:22:50.000000 attune-project-api-0.9.9/attune_project_api/_private/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3241 2022-05-23 00:41:40.000000 attune-project-api-0.9.9/attune_project_api/_private/archive_format.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3428 2023-02-28 01:54:20.000000 attune-project-api-0.9.9/attune_project_api/_private/archive_get_file_content.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      596 2022-01-07 03:41:18.000000 attune-project-api-0.9.9/attune_project_api/_private/archive_hasher.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3019 2022-05-23 00:41:40.000000 attune-project-api-0.9.9/attune_project_api/_private/archive_list_files.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3683 2022-07-01 03:12:12.000000 attune-project-api-0.9.9/attune_project_api/_private/large_file_http_downloader.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      661 2022-01-25 22:57:26.000000 attune-project-api-0.9.9/attune_project_api/_private/large_file_http_downloader_test.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1677 2023-02-03 06:38:08.000000 attune-project-api-0.9.9/attune_project_api/_private/readme_compiler.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:46:17.185577 attune-project-api-0.9.9/attune_project_api/_private/templates/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1357 2023-02-26 22:18:39.000000 attune-project-api-0.9.9/attune_project_api/_private/templates/ProjectReadme.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      868 2023-02-10 03:43:12.000000 attune-project-api-0.9.9/attune_project_api/_private/templates/ProjectReadmeAttune.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      267 2023-02-10 03:43:12.000000 attune-project-api-0.9.9/attune_project_api/_private/templates/ProjectReadmeBlueprints.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)     1608 2023-02-26 22:18:39.000000 attune-project-api-0.9.9/attune_project_api/_private/templates/ProjectReadmeCloneInstructions.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      787 2023-02-26 22:18:39.000000 attune-project-api-0.9.9/attune_project_api/_private/templates/ProjectReadmeContribute.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      185 2023-02-10 03:43:12.000000 attune-project-api-0.9.9/attune_project_api/_private/templates/ProjectReadmeFiles.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)      312 2023-02-10 03:43:12.000000 attune-project-api-0.9.9/attune_project_api/_private/templates/ProjectReadmeParameters.md.mako
+-rw-r--r--   0 jchesney   (501) staff       (20)       27 2022-10-21 00:47:49.000000 attune-project-api-0.9.9/attune_project_api/_private/templates/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      544 2023-01-23 02:29:43.000000 attune-project-api-0.9.9/attune_project_api/_private/utils.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2948 2022-05-04 02:21:42.000000 attune-project-api-0.9.9/attune_project_api/alembic.ini
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:46:17.186901 attune-project-api-0.9.9/attune_project_api/alembic_migrations/
+-rw-r--r--   0 jchesney   (501) staff       (20)       38 2022-05-04 02:21:42.000000 attune-project-api-0.9.9/attune_project_api/alembic_migrations/README
+-rw-r--r--   0 jchesney   (501) staff       (20)     2038 2022-05-04 02:21:42.000000 attune-project-api-0.9.9/attune_project_api/alembic_migrations/env.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      494 2022-05-04 02:21:42.000000 attune-project-api-0.9.9/attune_project_api/alembic_migrations/script.py.mako
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:46:17.189127 attune-project-api-0.9.9/attune_project_api/alembic_migrations/versions/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1115 2023-02-03 04:14:24.000000 attune-project-api-0.9.9/attune_project_api/alembic_migrations/versions/0aa489aa66b2_store_name_in_project_metadata.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1173 2023-02-10 02:46:44.000000 attune-project-api-0.9.9/attune_project_api/alembic_migrations/versions/145c6dc54454_rename_comment_md_to_readme_md_for_items.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      417 2022-05-04 02:21:42.000000 attune-project-api-0.9.9/attune_project_api/alembic_migrations/versions/16e34a42a9a1_attune_v5_starting_point.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1859 2022-05-04 02:21:42.000000 attune-project-api-0.9.9/attune_project_api/alembic_migrations/versions/58b1656aac40_move_sql_to_script_txt_file_in_oracle_.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1332 2023-02-03 04:14:24.000000 attune-project-api-0.9.9/attune_project_api/alembic_migrations/versions/ba6a8e4d7e2b_move_metadata_json_file_to_project_.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      215 2023-02-03 04:14:24.000000 attune-project-api-0.9.9/attune_project_api/context_project_info.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:46:17.190296 attune-project-api-0.9.9/attune_project_api/items/
+-rw-r--r--   0 jchesney   (501) staff       (20)      489 2022-01-07 01:53:29.000000 attune-project-api-0.9.9/attune_project_api/items/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:46:17.192414 attune-project-api-0.9.9/attune_project_api/items/file_archive_tuples/
+-rw-r--r--   0 jchesney   (501) staff       (20)      163 2022-01-07 01:53:29.000000 attune-project-api-0.9.9/attune_project_api/items/file_archive_tuples/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4776 2023-03-06 02:26:35.000000 attune-project-api-0.9.9/attune_project_api/items/file_archive_tuples/file_archive_large_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2548 2023-03-06 02:26:35.000000 attune-project-api-0.9.9/attune_project_api/items/file_archive_tuples/file_archive_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     6158 2023-03-06 02:26:35.000000 attune-project-api-0.9.9/attune_project_api/items/file_archive_tuples/file_archive_versioned_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      482 2022-02-28 06:52:20.000000 attune-project-api-0.9.9/attune_project_api/items/file_archive_tuples/file_tuple_constants.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3087 2022-01-07 01:53:29.000000 attune-project-api-0.9.9/attune_project_api/items/parameter_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      645 2023-02-03 04:14:24.000000 attune-project-api-0.9.9/attune_project_api/items/project_metadata_tuple.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:46:17.198825 attune-project-api-0.9.9/attune_project_api/items/step_tuples/
+-rw-r--r--   0 jchesney   (501) staff       (20)      928 2022-01-12 10:38:07.000000 attune-project-api-0.9.9/attune_project_api/items/step_tuples/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1210 2022-01-07 01:53:29.000000 attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_bootstrap_linux_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2855 2022-01-13 14:55:18.000000 attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_group_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2791 2023-01-23 02:29:49.000000 attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_project_link_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2706 2022-02-24 06:08:31.000000 attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_push_design_file_compiled_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1692 2022-10-26 23:25:34.000000 attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_push_design_file_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1786 2022-01-14 07:57:32.000000 attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_sql_oracle_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1040 2022-01-07 01:53:29.000000 attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_ssh_prompted_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2086 2022-01-07 01:53:29.000000 attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_ssh_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1250 2022-01-07 01:53:29.000000 attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_tcp_ping_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2190 2023-02-03 06:38:08.000000 attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2499 2022-01-07 01:53:29.000000 attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_winrm_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4079 2023-02-28 01:54:20.000000 attune-project-api-0.9.9/attune_project_api/migration.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:46:17.199821 attune-project-api-0.9.9/attune_project_api/tuples/
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2021-12-30 21:22:50.000000 attune-project-api-0.9.9/attune_project_api/tuples/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      366 2022-01-07 01:53:29.000000 attune-project-api-0.9.9/attune_project_api/tuples/git_commit_tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1123 2023-01-23 02:29:43.000000 attune-project-api-0.9.9/attune_project_api/tuples/project_modified_tuple.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-03-06 02:46:17.176894 attune-project-api-0.9.9/attune_project_api.egg-info/
+-rw-r--r--   0 jchesney   (501) staff       (20)      262 2023-03-06 02:46:17.000000 attune-project-api-0.9.9/attune_project_api.egg-info/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)     3773 2023-03-06 02:46:17.000000 attune-project-api-0.9.9/attune_project_api.egg-info/SOURCES.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-03-06 02:46:17.000000 attune-project-api-0.9.9/attune_project_api.egg-info/dependency_links.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-03-06 02:46:17.000000 attune-project-api-0.9.9/attune_project_api.egg-info/not-zip-safe
+-rw-r--r--   0 jchesney   (501) staff       (20)      134 2023-03-06 02:46:17.000000 attune-project-api-0.9.9/attune_project_api.egg-info/requires.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)       19 2023-03-06 02:46:17.000000 attune-project-api-0.9.9/attune_project_api.egg-info/top_level.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)       80 2023-03-06 02:46:17.201581 attune-project-api-0.9.9/setup.cfg
+-rw-r--r--   0 jchesney   (501) staff       (20)     2202 2023-03-06 02:46:16.000000 attune-project-api-0.9.9/setup.py
```

### Comparing `attune-project-api-0.9.8/attune_project_api/Exceptions.py` & `attune-project-api-0.9.9/attune_project_api/Exceptions.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/ObjectStorageContext.py` & `attune-project-api-0.9.9/attune_project_api/ObjectStorageContext.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/RelationField.py` & `attune-project-api-0.9.9/attune_project_api/RelationField.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/StorageTuple.py` & `attune-project-api-0.9.9/attune_project_api/StorageTuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/TupleFieldValidators.py` & `attune-project-api-0.9.9/attune_project_api/TupleFieldValidators.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/TupleValidators.py` & `attune-project-api-0.9.9/attune_project_api/TupleValidators.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_contexts/GitLibMixin.py` & `attune-project-api-0.9.9/attune_project_api/_contexts/GitLibMixin.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_contexts/GitObjectStorageContext.py` & `attune-project-api-0.9.9/attune_project_api/_contexts/GitObjectStorageContext.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/RelationGraph.py` & `attune-project-api-0.9.9/attune_project_api/_private/RelationGraph.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/archive_format.py` & `attune-project-api-0.9.9/attune_project_api/_private/archive_format.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/archive_get_file_content.py` & `attune-project-api-0.9.9/attune_project_api/_private/archive_get_file_content.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/archive_hasher.py` & `attune-project-api-0.9.9/attune_project_api/_private/archive_hasher.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/archive_list_files.py` & `attune-project-api-0.9.9/attune_project_api/_private/archive_list_files.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/large_file_http_downloader.py` & `attune-project-api-0.9.9/attune_project_api/_private/large_file_http_downloader.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/large_file_http_downloader_test.py` & `attune-project-api-0.9.9/attune_project_api/_private/large_file_http_downloader_test.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/readme_compiler.py` & `attune-project-api-0.9.9/attune_project_api/_private/readme_compiler.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/templates/ProjectReadme.md.mako` & `attune-project-api-0.9.9/attune_project_api/_private/templates/ProjectReadme.md.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/templates/ProjectReadmeAttune.md.mako` & `attune-project-api-0.9.9/attune_project_api/_private/templates/ProjectReadmeAttune.md.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/templates/ProjectReadmeCloneInstructions.md.mako` & `attune-project-api-0.9.9/attune_project_api/_private/templates/ProjectReadmeCloneInstructions.md.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/templates/ProjectReadmeContribute.md.mako` & `attune-project-api-0.9.9/attune_project_api/_private/templates/ProjectReadmeContribute.md.mako`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/_private/utils.py` & `attune-project-api-0.9.9/attune_project_api/_private/utils.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/alembic.ini` & `attune-project-api-0.9.9/attune_project_api/alembic.ini`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/alembic_migrations/env.py` & `attune-project-api-0.9.9/attune_project_api/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/alembic_migrations/versions/0aa489aa66b2_store_name_in_project_metadata.py` & `attune-project-api-0.9.9/attune_project_api/alembic_migrations/versions/0aa489aa66b2_store_name_in_project_metadata.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/alembic_migrations/versions/145c6dc54454_rename_comment_md_to_readme_md_for_items.py` & `attune-project-api-0.9.9/attune_project_api/alembic_migrations/versions/145c6dc54454_rename_comment_md_to_readme_md_for_items.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/alembic_migrations/versions/58b1656aac40_move_sql_to_script_txt_file_in_oracle_.py` & `attune-project-api-0.9.9/attune_project_api/alembic_migrations/versions/58b1656aac40_move_sql_to_script_txt_file_in_oracle_.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/alembic_migrations/versions/ba6a8e4d7e2b_move_metadata_json_file_to_project_.py` & `attune-project-api-0.9.9/attune_project_api/alembic_migrations/versions/ba6a8e4d7e2b_move_metadata_json_file_to_project_.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/file_archive_tuples/file_archive_large_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/file_archive_tuples/file_archive_large_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/file_archive_tuples/file_archive_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/file_archive_tuples/file_archive_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/file_archive_tuples/file_archive_versioned_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/file_archive_tuples/file_archive_versioned_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/parameter_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/parameter_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/project_metadata_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/project_metadata_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/step_tuples/__init__.py` & `attune-project-api-0.9.9/attune_project_api/items/step_tuples/__init__.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_bootstrap_linux_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_bootstrap_linux_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_group_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_group_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_project_link_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_project_link_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_push_design_file_compiled_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_push_design_file_compiled_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_push_design_file_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_push_design_file_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_sql_oracle_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_sql_oracle_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_ssh_prompted_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_ssh_prompted_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_ssh_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_ssh_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_tcp_ping_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_tcp_ping_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/items/step_tuples/step_winrm_tuple.py` & `attune-project-api-0.9.9/attune_project_api/items/step_tuples/step_winrm_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/migration.py` & `attune-project-api-0.9.9/attune_project_api/migration.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api/tuples/project_modified_tuple.py` & `attune-project-api-0.9.9/attune_project_api/tuples/project_modified_tuple.py`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/attune_project_api.egg-info/SOURCES.txt` & `attune-project-api-0.9.9/attune_project_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `attune-project-api-0.9.8/setup.py` & `attune-project-api-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 
 from setuptools import find_packages
 from setuptools import setup
 
 pip_package_name = "attune-project-api"
 py_package_folder = "attune_project_api"
-package_version = '0.9.8'
+package_version = '0.9.9'
 
 egg_info = "%s.egg-info" % pip_package_name
 if os.path.isdir(egg_info):
     shutil.rmtree(egg_info)
 
 if os.path.isfile("MANIFEST"):
     os.remove("MANIFEST")
```

