# Comparing `tmp/ultima_scraper_collection-1.0.3.tar.gz` & `tmp/ultima_scraper_collection-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_collection-1.0.3.tar", max compression
+gzip compressed data, was "ultima_scraper_collection-1.1.0.tar", max compression
```

## Comparing `ultima_scraper_collection-1.0.3.tar` & `ultima_scraper_collection-1.1.0.tar`

### file list

```diff
@@ -1,73 +1,72 @@
--rw-r--r--   0        0        0      701 2023-04-22 02:27:06.555309 ultima_scraper_collection-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-1.0.3/ultima_scraper_collection/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
--rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
--rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
--rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
--rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
--rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
--rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
--rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
--rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
--rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
--rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
--rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
--rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
--rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
--rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
--rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
--rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
--rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
--rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
--rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
--rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
--rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
--rw-r--r--   0        0        0     1611 2023-04-20 22:10:05.846209 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
--rw-r--r--   0        0        0     2764 2023-04-20 22:14:44.815046 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
--rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
--rw-r--r--   0        0        0     9406 2023-04-20 22:22:19.565161 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
--rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/database_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/datascraper_manager/__init__.py
--rw-r--r--   0        0        0     1558 2023-03-12 13:14:10.302489 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
--rw-r--r--   0        0        0    15824 2023-04-20 22:28:12.293022 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
--rw-r--r--   0        0        0     6714 2023-04-20 22:28:23.059323 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
--rw-r--r--   0        0        0     4759 2023-04-22 02:37:09.276671 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/download_manager.py
--rw-r--r--   0        0        0    13822 2023-04-21 23:41:49.647713 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/filesystem_manager.py
--rw-r--r--   0        0        0     6102 2023-03-05 04:29:30.964171 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/legacy_code.py
--rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/metadata_manager/__init__.py
--rw-r--r--   0        0        0    27544 2023-04-20 23:06:36.616983 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
--rw-r--r--   0        0        0     6673 2023-03-14 10:02:12.828825 ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/option_manager.py
--rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-1.0.3/ultima_scraper_collection/modules/__init__.py
--rw-r--r--   0        0        0    17953 2023-04-22 02:12:06.815554 ultima_scraper_collection-1.0.3/ultima_scraper_collection/modules/module_streamliner.py
--rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-1.0.3/ultima_scraper_collection/py.typed
--rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 ultima_scraper_collection-1.0.3/setup.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 ultima_scraper_collection-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      788 2023-05-14 20:46:02.767921 ultima_scraper_collection-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-1.1.0/ultima_scraper_collection/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
+-rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
+-rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
+-rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
+-rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
+-rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
+-rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
+-rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
+-rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
+-rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
+-rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
+-rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
+-rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
+-rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
+-rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
+-rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
+-rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
+-rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
+-rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
+-rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
+-rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
+-rw-r--r--   0        0        0     1611 2023-04-20 22:10:05.846209 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
+-rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
+-rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
+-rw-r--r--   0        0        0     9499 2023-05-14 03:29:16.005497 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
+-rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/database_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/__init__.py
+-rw-r--r--   0        0        0     1558 2023-03-12 13:14:10.302489 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
+-rw-r--r--   0        0        0     5390 2023-05-14 03:41:06.309010 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
+-rw-r--r--   0        0        0     5640 2023-05-14 03:41:28.928194 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
+-rw-r--r--   0        0        0    10135 2023-05-14 18:59:18.593115 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/download_manager.py
+-rw-r--r--   0        0        0    13669 2023-05-14 19:55:15.091076 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/filesystem_manager.py
+-rw-r--r--   0        0        0     6102 2023-03-05 04:29:30.964171 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/legacy_code.py
+-rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/metadata_manager/__init__.py
+-rw-r--r--   0        0        0    27818 2023-05-14 17:11:10.534764 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
+-rw-r--r--   0        0        0     6837 2023-05-14 02:04:39.528451 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/option_manager.py
+-rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-1.1.0/ultima_scraper_collection/modules/__init__.py
+-rw-r--r--   0        0        0    17809 2023-05-14 04:28:12.046662 ultima_scraper_collection-1.1.0/ultima_scraper_collection/modules/module_streamliner.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-1.1.0/ultima_scraper_collection/py.typed
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 ultima_scraper_collection-1.1.0/PKG-INFO
```

### Comparing `ultima_scraper_collection-1.0.3/pyproject.toml` & `ultima_scraper_collection-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "ultima-scraper-collection"
-version = "1.0.3"
+version = "1.1.0"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_collection"}]
 include = ["ultima_scraper_collection/py.typed"]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10,<3.12"
 
 sqlalchemy = "^2.0.1"
 psycopg2 = "^2.9.5"
 alembic = "^1.9.2"
 tqdm = "^4.65.0"
-ultima-scraper-api = "^1.0.0"
-ultima-scraper-renamer = "^1.0.0"
-
+ultima-scraper-api = "^1.1.0"
+ultima-scraper-renamer = "^1.1.0"
+ffmpeg-python = "^0.2.0"
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.2"
+black = {version = "^23.3.0", allow-prereleases = true}
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,17 +187,19 @@
                     and media_db.media_id
                 ):
                     media_id = media_db.media_id
 
                 media_db.media_id = media_id
                 media_db.post_id = post_id
                 media_db.size = media.size if media_db.size is None else media_db.size
-                media_db.link = media.urls[0]
+                media_db.link = media.urls[0] if media.urls else None
                 media_db.preview = media.preview
-                media_db.directory = media.directory.as_posix()
+                media_db.directory = (
+                    media.directory.as_posix() if media.directory else None
+                )
                 media_db.filename = media.filename
                 media_db.api_type = api_type
                 media_db.media_type = media.media_type
                 media_db.linked = media.linked
                 if date_object:
                     media_db.created_at = date_object
                 database_session.add(media_db)
```

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-import os
 from pathlib import Path
 from typing import Any, Union
-from urllib.parse import urlparse
 
 from ultima_scraper_api.apis.onlyfans.classes.auth_model import create_auth
 from ultima_scraper_api.apis.onlyfans.classes.hightlight_model import create_highlight
 from ultima_scraper_api.apis.onlyfans.classes.message_model import create_message
 from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
 from ultima_scraper_api.apis.onlyfans.classes.story_model import create_story
 from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
-
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
     ContentMetadata,
 )
 from ultima_scraper_collection.managers.option_manager import OptionManager
 from ultima_scraper_collection.modules.module_streamliner import StreamlinedDatascraper
+from ultima_scraper_renamer.reformat import ReformatManager
 
 
 class OnlyFansDataScraper(StreamlinedDatascraper):
     def __init__(self, api: OnlyFansAPI, option_manager: OptionManager) -> None:
         self.api = api
         self.option_manager = option_manager
         StreamlinedDatascraper.__init__(self, self)
 
     # Scrapes the API for content
-
     async def media_scraper(
         self,
         post_result: Union[create_story, create_post, create_message],
         subscription: create_user,
         formatted_directory: Path,
         api_type: str,
     ) -> dict[str, Any]:
-        from ultima_scraper_renamer.reformat import prepare_reformat
-
         authed = subscription.get_authed()
         api = authed.api
         site_settings = api.get_site_settings()
         if not site_settings:
             return {}
         new_set: dict[str, Any] = {"content": []}
         directories: list[Path] = []
@@ -46,64 +41,40 @@
             pass
         if api_type == "Archived":
             pass
         if api_type == "Posts":
             pass
         if api_type == "Messages":
             pass
-        download_path = formatted_directory
-        model_username = subscription.username
-        date_format = site_settings.date_format
         from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
             Extractor,
         )
 
         content_metadata = ContentMetadata(post_result.id, api_type)
         content_metadata.resolve_extractor(Extractor(post_result))
         matches = [
             s for s in site_settings.ignored_keywords if s in content_metadata.text
         ]
         if matches:
-            print("Ignoring - ", f"PostID: {content_metadata.id}")
-            return
+            print("Ignoring - ", f"PostID: {content_metadata.content_id}")
+            return {}
         for asset in content_metadata.medias:
-            filename = urlparse(asset.urls[0]).path.split("/")[-1]
-            name, ext = filename.rsplit(".", 1)
-            final_api_type = (
-                os.path.join("Archived", api_type)
-                if content_metadata.archived
-                else api_type
-            )
-            option: dict[str, Any] = {}
-            option = option | content_metadata.__dict__
-            option["site_name"] = api.site_name
-            option["media_id"] = asset.id
-            option["filename"] = name
-            option["api_type"] = final_api_type
-            option["media_type"] = asset.media_type
-            option["ext"] = ext
-            option["profile_username"] = authed.username
-            option["model_username"] = model_username
-            option["date_format"] = date_format
-            option["postedAt"] = asset.created_at
-            option["text_length"] = site_settings.text_length
-            option["directory"] = download_path
-            option["preview"] = asset.preview
-            option["archived"] = content_metadata.archived
-
-            prepared_format = prepare_reformat(option)
-            file_directory = await prepared_format.reformat_2(
-                site_settings.file_directory_format
-            )
-            prepared_format.directory = file_directory
-            file_path = await prepared_format.reformat_2(site_settings.filename_format)
-            asset.directory = file_directory
-            asset.filename = file_path.name
-            if file_directory not in directories:
-                directories.append(file_directory)
+            if asset.urls:
+                reformat_manager = ReformatManager(authed, self.filesystem_manager)
+                reformat_item = reformat_manager.prepare_reformat(asset)
+                file_directory = reformat_item.reformat(
+                    site_settings.file_directory_format
+                )
+                reformat_item.directory = file_directory
+                file_path = reformat_item.reformat(site_settings.filename_format)
+                asset.directory = file_directory
+                asset.filename = file_path.name
+
+                if file_directory not in directories:
+                    directories.append(file_directory)
         new_set["content"].append(content_metadata)
         new_set["directories"] = directories
         return new_set
 
     async def get_all_stories(self, subscription: create_user):
         """
         get_all_stories(subscription: create_user)
@@ -150,12 +121,12 @@
         authed (create_auth): An instance of the create_auth class.
         identifiers (list[int | str], optional): A list of identifiers (username or id) for the subscriptions. Defaults to an empty list.
         refresh (bool, optional): A flag indicating whether to refresh the list of subscriptions. Defaults to True.
 
         Returns:
         list[create_subscription]: A list of all subscriptions, sorted by expiredAt, from the authenticated user.
         """
-        results = await authed.get_subscriptions(
-            identifiers=identifiers, refresh=refresh
+        subscriptions = await authed.get_subscriptions(
+            identifiers=identifiers, refresh=refresh, sub_type="active"
         )
-        results.sort(key=lambda x: x.subscribedByData["expiredAt"])
-        return results
+        subscriptions.sort(key=lambda x: x.subscribed_by_expire_date)
+        return subscriptions
```

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/filesystem_manager.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/filesystem_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from typing import TYPE_CHECKING, Any, Generator, Literal
 
 import ultima_scraper_api
 from aiohttp.client_reqrep import ClientResponse
 from ultima_scraper_api.classes.prepare_directories import FormatTypes
 from ultima_scraper_api.helpers.main_helper import open_partial
 from ultima_scraper_api.managers.session_manager import EXCEPTION_TEMPLATE
-from ultima_scraper_renamer.reformat import prepare_reformat
+from ultima_scraper_renamer.reformat import ReformatItem
 
 if TYPE_CHECKING:
-
     api_types = ultima_scraper_api.api_types
     user_types = ultima_scraper_api.user_types
 
 
 class FilesystemManager:
     def __init__(self) -> None:
         self.user_data_directory = Path("__user_data__")
         self.trash_directory = self.user_data_directory.joinpath("trash")
         self.profiles_directory = self.user_data_directory.joinpath("profiles")
+        self.devices_directory = self.user_data_directory.joinpath("devices")
         self.settings_directory = Path("__settings__")
         self.ignore_files = ["desktop.ini", ".DS_Store", ".DS_store", "@eaDir"]
         self.directory_manager: DirectoryManager | None = None
         self.directory_manager_users: dict[int, DirectoryManager] = {}
         self.file_manager_users: dict[int, FileManager] = {}
 
     def __iter__(self):
@@ -75,15 +75,15 @@
 
     def trash(self):
         pass
 
     async def write_data(
         self, response: ClientResponse, download_path: Path, callback: Any = None
     ):
-        status_code = 0
+        status_code = None
         if response.status == 200:
             total_length = 0
             os.makedirs(os.path.dirname(download_path), exist_ok=True)
             partial_path: str | None = None
             try:
                 with open_partial(download_path) as f:
                     partial_path = f.name
@@ -114,15 +114,14 @@
             if response.content_length:
                 pass
                 # progress_bar.update_total_size(-response.content_length)
             status_code = 2
         return status_code
 
     async def create_directory_manager(self, api: api_types, user: user_types):
-
         # profile_directory = filesystem_directory_manager.profile.root_directory.joinpath(
         #     self.username
         # )
         if self.directory_manager:
             directory_manager = DirectoryManager(
                 api.get_site_settings(),
                 self.directory_manager.root_metadata_directory,
@@ -130,79 +129,64 @@
             )
             option = {
                 "site_name": api.site_name,
                 "profile_username": user.username,
                 "model_username": user.username,
                 "directory": directory_manager.root_download_directory,
             }
-            pr_rt_rd = prepare_reformat(option)
-            _f_d_p = await pr_rt_rd.remove_non_unique(
+            reformat_item_fd = ReformatItem(option)
+            _f_d_p = reformat_item_fd.remove_non_unique(
                 directory_manager, "file_directory_format"
             )
             # f_d_p.mkdir(parents=True, exist_ok=True)
             option["directory"] = self.directory_manager.root_metadata_directory
-            pr_rt_rm = prepare_reformat(option)
-            _f_d_p_2 = await pr_rt_rm.remove_non_unique(
+            reformat_item_md = ReformatItem(option)
+            _f_d_p_2 = reformat_item_md.remove_non_unique(
                 self.directory_manager, "metadata_directory_format"
             )
             # f_d_p_2.mkdir(parents=True, exist_ok=True)
             self.directory_manager_users[user.id] = directory_manager
             self.file_manager_users[user.id] = FileManager(directory_manager)
             return directory_manager
 
     async def format_directories(self, subscription: user_types) -> DirectoryManager:
-
         directory_manager = self.get_directory_manager(subscription.id)
         file_manager = self.get_file_manager(subscription.id)
         authed = subscription.get_authed()
         api = authed.api
         site_settings = authed.api.get_site_settings()
         if site_settings:
             authed_username = authed.username
             subscription_username = subscription.username
             site_name = authed.api.site_name
-            p_r = prepare_reformat()
-            prepared_metadata_format = await p_r.standard(
-                site_name,
-                authed_username,
-                subscription_username,
-                datetime.today(),
-                site_settings.date_format,
-                site_settings.text_length,
-                directory_manager.root_metadata_directory,
-            )
-            string = await prepared_metadata_format.reformat_2(
-                site_settings.metadata_directory_format
-            )
+            reformat_item = ReformatItem()
+            reformat_item.site_name = site_name
+            reformat_item.profile_username = authed_username
+            reformat_item.model_username = subscription_username
+            reformat_item.date = datetime.today()
+            reformat_item.date_format = site_settings.date_format
+            reformat_item.text_length = site_settings.text_length
+            reformat_item.directory = directory_manager.root_metadata_directory
+            string = reformat_item.reformat(site_settings.metadata_directory_format)
             directory_manager.user.metadata_directory = Path(string)
-            prepared_download_format = copy.copy(prepared_metadata_format)
-            prepared_download_format.directory = (
-                directory_manager.root_download_directory
-            )
-            string = await prepared_download_format.reformat_2(
-                site_settings.file_directory_format
-            )
-            formtatted_root_download_directory = (
-                await prepared_download_format.remove_non_unique(
-                    directory_manager, "file_directory_format"
-                )
+            reformat_item_2 = copy.copy(reformat_item)
+            reformat_item_2.directory = directory_manager.root_download_directory
+            string = reformat_item_2.reformat(site_settings.file_directory_format)
+            formtatted_root_download_directory = reformat_item_2.remove_non_unique(
+                directory_manager, "file_directory_format"
             )
             directory_manager.user.download_directory = (
                 formtatted_root_download_directory
             )
-            await file_manager.set_default_files(
-                prepared_metadata_format, prepared_download_format
-            )
+            await file_manager.set_default_files(reformat_item, reformat_item_2)
             _metadata_filepaths = await file_manager.find_metadata_files(
                 legacy_files=False
             )
             # I forgot why we need to set default file twice
-            await file_manager.set_default_files(
-                prepared_metadata_format, prepared_download_format
-            )
+            await file_manager.set_default_files(reformat_item, reformat_item_2)
             user_metadata_directory = directory_manager.user.metadata_directory
             _user_download_directory = directory_manager.user.download_directory
             legacy_metadata_directory = user_metadata_directory
             directory_manager.user.legacy_metadata_directories.append(
                 legacy_metadata_directory
             )
             items = api.ContentTypes().__dict__.items()
@@ -308,24 +292,24 @@
 class FileManager:
     def __init__(self, directory_manager: DirectoryManager) -> None:
         self.files: list[Path] = []
         self.directory_manager = directory_manager
 
     async def set_default_files(
         self,
-        prepared_metadata_format: prepare_reformat,
-        prepared_download_format: prepare_reformat,
+        prepared_metadata_format: ReformatItem,
+        prepared_download_format: ReformatItem,
     ):
         self.files = []
         await self.add_files(prepared_metadata_format, "metadata_directory_format")
         await self.add_files(prepared_download_format, "file_directory_format")
 
-    async def add_files(self, reformatter: prepare_reformat, format_key: str):
+    async def add_files(self, reformatter: ReformatItem, format_key: str):
         directory_manager = self.directory_manager
-        formatted_directory = await reformatter.remove_non_unique(
+        formatted_directory = reformatter.remove_non_unique(
             directory_manager, format_key
         )
         files: list[Path] = []
         files = await directory_manager.walk(formatted_directory)
         self.files.extend(files)
         return files
```

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/legacy_code.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/legacy_code.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-import shutil
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 from urllib.parse import ParseResult, urlparse
 
 import ultima_scraper_api
 from sqlalchemy import inspect
-from ultima_scraper_api.apis.onlyfans.classes.message_model import create_message
-from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
-from ultima_scraper_api.classes.prepare_metadata import legacy_metadata_fixer
+
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.sqlite_database import (
     DBCollection,
     SqliteDatabase,
 )
 from ultima_scraper_collection.managers.database_manager.database_manager import (
     DatabaseManager,
 )
 from ultima_scraper_collection.managers.filesystem_manager import (
-    DirectoryManager,
     FilesystemManager,
 )
-from ultima_scraper_renamer.reformat import prepare_reformat
 
 api_types = ultima_scraper_api.api_types
 user_types = ultima_scraper_api.user_types
 content_types = ultima_scraper_api.content_types
 from ultima_scraper_api.classes.prepare_metadata import format_content
 from ultima_scraper_api.helpers import main_helper
+
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.api_model import (
     ApiModel,
 )
+from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.user_database import (
+    messages_table,
+)
 
 
 class MetadataExtractor:
     def __init__(self, post_item: format_content.post_item) -> None:
         self.item = post_item
 
     def get_id(self):
@@ -54,15 +53,14 @@
 
     def get_date(self):
         return self.item.createdAt
 
     def get_medias(self, content_metadata: "ContentMetadata"):
         final_assets: list[MediaMetadata] = []
         for media in self.item.medias:
-
             new_asset = MediaMetadata(
                 media.media_id,
                 media.media_type,
                 content_metadata,
                 created_at=content_metadata.created_at_string,
             )
             new_asset.urls = media.links
@@ -71,14 +69,18 @@
             new_asset.size = media.size
             final_assets.append(new_asset)
         return final_assets
 
     def resolve_paid(self):
         return self.item.paid
 
+    def get_receiver_id(self):
+        if isinstance(self.item, messages_table):
+            return
+
 
 class Extractor:
     def __init__(self, item: content_types) -> None:
         self.item = item
 
     def get_id(self):
         return self.item.id
@@ -125,47 +127,44 @@
 
     def get_medias(self, content_metadata: "ContentMetadata"):
         final_assets: list[MediaMetadata] = []
         for asset_metadata in self.item.media:
             raw_media_type = asset_metadata["type"]
             if "mimetype" in asset_metadata:
                 raw_media_type: str = asset_metadata["mimetype"].split("/")[0]
-            media_type = (
-                self.item.get_author()
-                .get_api()
-                .MediaTypes()
-                .find_by_value(raw_media_type)
-            )
+            author = self.item.get_author()
+            media_type = author.get_api().MediaTypes().find_by_value(raw_media_type)
             new_asset = MediaMetadata(
                 asset_metadata["id"],
                 media_type,
                 content_metadata,
                 created_at=content_metadata.created_at_string,
             )
             main_url = self.item.url_picker(asset_metadata)
             preview_url = self.item.preview_url_picker(asset_metadata)
+            authed = author.get_authed()
+            if authed.drm:
+                new_asset.drm = bool(authed.drm.has_drm(asset_metadata))
             new_asset.urls = []
             matches = ["us", "uk", "ca", "ca2", "de"]
             for url in [main_url, preview_url].copy():
                 if url:
                     if url.hostname:
                         subdomain = url.hostname.split(".")[1]
                         if any(subdomain in nm for nm in matches):
                             subdomain = url.hostname.split(".")[1]
                             if "upload" in subdomain:
                                 continue
                             if "convert" in subdomain:
                                 continue
                     new_asset.urls.append(url.geturl())
-            if not new_asset.urls:
-                continue
 
             if int(new_asset.id) in content_metadata.preview_media_ids:
                 new_asset.preview = True
-            new_asset._raw_ = asset_metadata
+            new_asset.__raw__ = asset_metadata
             final_assets.append(new_asset)
         return final_assets
 
     def resolve_archived(self):
         archived = False
         if isinstance(self.item, ultima_scraper_api.post_types):
             archived = self.item.isArchived
@@ -173,46 +172,52 @@
 
     def resolve_paid(self):
         if getattr(self.item, "price", 0):
             if all(media["canView"] for media in self.item.media):
                 return True
         return False
 
+    def get_receiver_id(self):
+        if isinstance(self.item, ultima_scraper_api.message_types):
+            return self.item.get_receiver().id
+
 
 class ContentMetadata:
     def __init__(self, content_id: int, api_type: str) -> None:
         self.content_id = content_id
         self.user_id: int | None = None
+        self.receiver_id: int | None = None
         self.text: str = ""
         self.preview_media_ids: list[int] | list[dict[str, Any]] = []
         self.archived: bool = False
         self.created_at_string: str = ""
         self.medias: list[MediaMetadata] = []
         self.api_type = api_type
         self.price: float | None = None
         self.paid: bool = False
         self.deleted: bool = False
-        self._raw_: Any | None = None
-        self._soft_ = None
+        self.__raw__: Any | None = None
+        self.__soft__: Any = None
         self.__db_content__: ApiModel | None = None
         self.__legacy__ = False
 
     def resolve_extractor(self, result: Extractor | MetadataExtractor):
         self.content_id = result.get_id()
         self.user_id = result.get_user_id()
+        self.receiver_id = result.get_receiver_id()
         self.text = result.get_text()
         self.preview_media_ids = result.get_preview_ids()
         self.archived = result.resolve_archived()
         self.created_at_string = result.get_date()
         self.medias: list[MediaMetadata] = result.get_medias(self)
         self.price = getattr(result.item, "price", 0) or 0
         self.paid = result.resolve_paid()
         self.deleted = False
-        self._raw_: Any | None = None
-        self._soft_ = result.item
+        self.__raw__: Any | None = None
+        self.__soft__ = result.item
 
     def add_media(
         self, media_id: int, media_type: str, urls: list[str], preview: bool = False
     ):
         urls = [url for url in urls if url]
         new_media = MediaMetadata(media_id, media_type, urls, preview, self.created_at)
         self.medias.append(new_media)
@@ -248,25 +253,28 @@
         self,
         media_id: int,
         media_type: str,
         content_metadata: ContentMetadata,
         urls: list[str] = [],
         preview: bool = False,
         created_at: str = "",
+        drm: bool = False,
     ) -> None:
         self.id = int(media_id) if media_id is not None else None
         self.media_type = media_type
         self.urls: list[str] = urls
         self.preview = preview
         self.directory: Path | None = None
-        self.filename = ""
+        self.filename: str | None = None
         self.size = 0
         self.linked = None
+        self.drm = drm
+        self.key: str = ""
         self.created_at = created_at or content_metadata.created_at_string
-        self._raw_: Any | None = None
+        self.__raw__: Any | None = None
         self.__content_metadata__ = content_metadata
 
     def find_by_url(self, url: ParseResult):
         for media_url in self.urls:
             media_url = urlparse(media_url)
             url_path = url.path
             if "Protected" in url.path:
```

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/managers/option_manager.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/option_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,25 +77,29 @@
                 self.final_choices = [
                     key
                     for choice in final_list
                     for key in self.items
                     if choice.lower() == key.auth_details.username.lower()
                 ]
             case "subscriptions":
-                self.item_keys = [x.username for x in self.items]
+                subscription_users = [x for x in self.items]
+                self.item_keys = [x.username for x in subscription_users]
                 my_string = " | ".join(
-                    map(lambda x: f"{self.items.index(x)+1} = {x.username}", self.items)
+                    map(
+                        lambda x: f"{subscription_users.index(x)+1} = {x.username}",
+                        subscription_users,
+                    )
                 )
                 final_string = f"{final_string} | {my_string}"
                 self.string = final_string
                 final_list = await self.choose_option()
                 self.final_choices = [
                     key
                     for choice in final_list
-                    for key in self.items
+                    for key in subscription_users
                     if choice.lower() == key.username.lower()
                 ]
 
             case "contents":
                 self.item_keys = self.items
                 my_string = " | ".join(
                     map(lambda x: f"{self.items.index(x)+1} = {x}", self.items)
```

### Comparing `ultima_scraper_collection-1.0.3/ultima_scraper_collection/modules/module_streamliner.py` & `ultima_scraper_collection-1.1.0/ultima_scraper_collection/modules/module_streamliner.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,37 +4,40 @@
 from itertools import product
 from typing import Any, Optional
 
 import ultima_scraper_api
 import ultima_scraper_api.classes.make_settings as make_settings
 from sqlalchemy.exc import OperationalError
 from tqdm.asyncio import tqdm_asyncio
+from ultima_scraper_renamer import renamer
+
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.api_model import (
     ApiModel,
 )
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.sqlite_database import (
     DBCollection,
 )
 from ultima_scraper_collection.managers.database_manager.database_manager import (
     DatabaseManager,
 )
 from ultima_scraper_collection.managers.download_manager import DownloadManager
 from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
     MetadataManager,
 )
-from ultima_scraper_renamer import renamer
 
 auth_types = ultima_scraper_api.auth_types
 user_types = ultima_scraper_api.user_types
 message_types = ultima_scraper_api.message_types
 error_types = ultima_scraper_api.error_types
+subscription_types = ultima_scraper_api.subscription_types
 
 from typing import TYPE_CHECKING
 
+
 if TYPE_CHECKING:
     from ultima_scraper_collection.managers.datascraper_manager.datascrapers.fansly import (
         FanslyDataScraper,
     )
     from ultima_scraper_collection.managers.datascraper_manager.datascrapers.onlyfans import (
         OnlyFansDataScraper,
     )
@@ -120,15 +123,15 @@
                     for paid_content in paid_contents:
                         author = paid_content.get_author()
                         if identifiers:
                             found = await author.match_identifiers(identifiers)
                             if not found:
                                 continue
                         if author:
-                            performer = await authed.get_subscription(
+                            performer = authed.find_user_by_identifier(
                                 identifier=author.id,
                             )
                             if performer:
                                 performer.job_whitelist.append("PaidContents")
                                 performer.scrape_whitelist.clear()
                                 valid_user_list.add(performer)
         # Need to filter out own profile with is_performer,etc
@@ -141,41 +144,36 @@
         self.user_list = final_valid_user_set
         return final_valid_user_set
 
     # Prepares the API links to be scraped
 
     async def prepare_scraper(
         self,
-        subscription: user_types,
+        user: user_types,
         metadata_manager: MetadataManager,
         content_type: str,
         master_set: list[Any] = [],
     ):
-        authed = subscription.get_authed()
-        current_job = subscription.get_current_job()
+        authed = user.get_authed()
+        current_job = user.get_current_job()
         if not current_job:
             return
         temp_master_set: list[Any] = copy.copy(master_set)
         if not temp_master_set:
             match content_type:
                 case "Stories":
-                    temp_master_set.extend(
-                        await self.datascraper.get_all_stories(subscription)
-                    )
+                    temp_master_set.extend(await self.datascraper.get_all_stories(user))
                     pass
                 case "Posts":
-                    temp_master_set = await self.datascraper.get_all_posts(subscription)
-                    pass
+                    temp_master_set = await self.datascraper.get_all_posts(user)
                 case "Messages":
                     pass
-                    unrefined_set: list[
-                        message_types | Any
-                    ] = await subscription.get_messages()
+                    unrefined_set: list[message_types | Any] = await user.get_messages()
                     mass_messages = getattr(authed, "mass_messages")
-                    if subscription.is_me() and mass_messages:
+                    if user.is_me() and mass_messages:
                         mass_messages = getattr(authed, "mass_messages")
                         # Need access to a creator's account to fix this
                         # unrefined_set2 = await self.datascraper.process_mass_messages(
                         #     authed,
                         #     mass_messages,
                         # )
                         # unrefined_set += unrefined_set2
@@ -187,15 +185,15 @@
                 case "Highlights":
                     pass
                 case "MassMessages":
                     pass
                 case _:
                     raise Exception(f"{content_type} is an invalid choice")
         await self.process_scraped_content(
-            temp_master_set, content_type, subscription, metadata_manager
+            temp_master_set, content_type, user, metadata_manager
         )
         current_job.done = True
 
     async def process_scraped_content(
         self,
         master_set: list[dict[str, Any]],
         api_type: str,
@@ -232,15 +230,14 @@
             new_metadata = metadata_manager.merge_content_and_directories(unrefined_set)
             final_content, _final_directories = new_metadata
             metadata_path = formatted_metadata_directory.joinpath("user_data.db")
             metadata_manager.db_manager = DatabaseManager().get_sqlite_db(metadata_path)
             if new_metadata:
                 new_metadata_content = final_content
                 metadata_manager.content_metadatas.extend(new_metadata_content)
-                print("Processing metadata.")
                 subscription.scrape_manager.set_scraped(api_type, new_metadata_content)
                 if new_metadata_content:
                     import_status = metadata_manager.db_manager.import_metadata(
                         new_metadata_content, api_type
                     )
                     if import_status:
                         Session = metadata_manager.db_manager.session_factory
@@ -344,45 +341,45 @@
 
     async def manage_subscriptions(
         self,
         authed: auth_types,
         identifiers: list[int | str] = [],
         refresh: bool = True,
     ):
-        temp_subscriptions: list[user_types] = []
+        temp_subscriptions: list[subscription_types] = []
         results = await self.datascraper.get_all_subscriptions(
             authed, identifiers, refresh
         )
         site_settings = authed.api.get_site_settings()
         if not site_settings:
             return temp_subscriptions
         ignore_type = site_settings.ignore_type
-        results.sort(key=lambda x: x.is_me(), reverse=True)
+        results.sort(key=lambda x: x.user.is_me(), reverse=True)
         for result in results:
             # await result.create_directory_manager(user=True)
-            subscribePrice = result.subscribePrice
+            subscribe_price = result.get_price()
             if ignore_type in ["paid"]:
-                if subscribePrice > 0:
+                if subscribe_price > 0:
                     continue
             if ignore_type in ["free"]:
-                if subscribePrice == 0:
+                if subscribe_price == 0:
                     continue
             temp_subscriptions.append(result)
         authed.subscriptions = temp_subscriptions
         return authed.subscriptions
 
     async def account_setup(
         self,
         auth: auth_types,
         datascraper: datascraper_types,
         site_settings: make_settings.SiteSettings,
         identifiers: list[int | str] | list[str] = [],
     ) -> tuple[bool, list[user_types]]:
         status = False
-        subscriptions: list[user_types] = []
+        subscriptions: list[subscription_types] = []
         authed = await auth.login()
 
         if authed.active and site_settings:
             # metadata_filepath = (
             #     authed.directory_manager.profile.metadata_directory.joinpath(
             #         "Mass Messages.json"
             #     )
```

### Comparing `ultima_scraper_collection-1.0.3/PKG-INFO` & `ultima_scraper_collection-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-collection
-Version: 1.0.3
+Version: 1.1.0
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: alembic (>=1.9.2,<2.0.0)
+Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: ultima-scraper-api (>=1.0.0,<2.0.0)
-Requires-Dist: ultima-scraper-renamer (>=1.0.0,<2.0.0)
+Requires-Dist: ultima-scraper-api (>=1.1.0,<2.0.0)
+Requires-Dist: ultima-scraper-renamer (>=1.1.0,<2.0.0)
```

