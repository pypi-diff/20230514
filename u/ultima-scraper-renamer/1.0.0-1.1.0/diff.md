# Comparing `tmp/ultima_scraper_renamer-1.0.0.tar.gz` & `tmp/ultima_scraper_renamer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_renamer-1.0.0.tar", max compression
+gzip compressed data, was "ultima_scraper_renamer-1.1.0.tar", max compression
```

## Comparing `ultima_scraper_renamer-1.0.0.tar` & `ultima_scraper_renamer-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.0.0/README.md
--rw-r--r--   0        0        0      674 2023-04-20 23:22:36.713797 ultima_scraper_renamer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.0.0/ultima_scraper_renamer/__init__.py
--rw-r--r--   0        0        0        0 2022-12-06 16:13:32.768074 ultima_scraper_renamer-1.0.0/ultima_scraper_renamer/py.typed
--rw-r--r--   0        0        0     8793 2023-03-07 05:09:45.193613 ultima_scraper_renamer-1.0.0/ultima_scraper_renamer/reformat.py
--rw-r--r--   0        0        0     8413 2023-03-25 23:23:34.019541 ultima_scraper_renamer-1.0.0/ultima_scraper_renamer/renamer.py
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 ultima_scraper_renamer-1.0.0/setup.py
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 ultima_scraper_renamer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.0/README.md
+-rw-r--r--   0        0        0      681 2023-05-14 20:41:21.269502 ultima_scraper_renamer-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.0/ultima_scraper_renamer/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-06 16:13:32.768074 ultima_scraper_renamer-1.1.0/ultima_scraper_renamer/py.typed
+-rw-r--r--   0        0        0    17508 2023-05-14 14:58:06.653713 ultima_scraper_renamer-1.1.0/ultima_scraper_renamer/reformat.py
+-rw-r--r--   0        0        0     7872 2023-05-14 17:44:23.086692 ultima_scraper_renamer-1.1.0/ultima_scraper_renamer/renamer.py
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 ultima_scraper_renamer-1.1.0/PKG-INFO
```

### Comparing `ultima_scraper_renamer-1.0.0/pyproject.toml` & `ultima_scraper_renamer-1.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ultima-scraper-renamer"
-version = "1.0.0"
+version = "1.1.0"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 readme = "README.md"
 packages = [{include = "ultima_scraper_renamer"}]
 include = ["ultima_scraper_renamer/py.typed"]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10,<3.12"
 tqdm = "^4.64.1"
 orjson = "^3.8.3"
-ultima-scraper-api = "^1.0.0"
-ultima-scraper-collection = "^1.0.0"
+ultima-scraper-api = "^1.1.0"
+ultima-scraper-collection = "^1.1.0"
 
 
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.2"
 
 [tool.semantic_release]
```

### Comparing `ultima_scraper_renamer-1.0.0/ultima_scraper_renamer/renamer.py` & `ultima_scraper_renamer-1.1.0/ultima_scraper_renamer/renamer.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,26 +64,26 @@
             date_format = site_settings.date_format
             text_length = site_settings.text_length
             download_path = directory_manager.root_download_directory
             option = {}
             option["site_name"] = api.site_name
             option["post_id"] = post_id
             option["media_id"] = media_id
-            option["profile_username"] = authed.username
-            option["model_username"] = subscription.username
-            option["api_type"] = final_api_type
-            option["media_type"] = media.media_type
             option["filename"] = original_filename
             option["ext"] = ext
+            option["api_type"] = final_api_type
+            option["media_type"] = media.media_type
             option["text"] = post.text
-            option["postedAt"] = media.created_at
-            option["price"] = post.price
+            option["profile_username"] = authed.username
+            option["model_username"] = subscription.username
             option["date_format"] = date_format
+            option["postedAt"] = media.created_at
             option["text_length"] = text_length
             option["directory"] = download_path
+            option["price"] = post.price
             option["preview"] = media.preview
             option["archived"] = post.archived
             prepared_format = prepare_reformat(option)
             file_directory = await prepared_format.reformat_2(file_directory_format)
             prepared_format.directory = file_directory
             old_filepath = ""
             if media.linked:
@@ -170,38 +170,24 @@
 
 async def start(
     subscription: user_types,
     directory_manager: DirectoryManager,
     api_type: str,
     Session: sessionmaker[Session],
 ):
-    authed = subscription.get_authed()
-    api_table_ = user_database.table_picker(api_type)
-    database_session = Session()
-    site_settings = authed.api.get_site_settings()
-    # Slow
-    authed_username = authed.username
-    subscription_username = subscription.username
-    site_name = authed.api.site_name
-    p_r = prepare_reformat()
-    p_r = await p_r.standard(
-        site_name=site_name,
-        profile_username=authed_username,
-        user_username=subscription_username,
-        date=datetime.today(),
-        date_format=site_settings.date_format,
-        text_length=site_settings.text_length,
-        directory=directory_manager.root_metadata_directory,
-    )
-    p_r.api_type = api_type
-    result: list[ApiModel] = database_session.query(api_table_).all()
     metadata = getattr(subscription.scrape_manager.scraped, api_type)
-
-    await fix_directories(
-        result,
-        subscription,
-        directory_manager,
-        database_session,
-        api_type,
-    )
-    database_session.close()
     return metadata
+    try:
+        api_table_ = user_database.table_picker(api_type)
+        database_session = Session()
+        result: list[ApiModel] = database_session.query(api_table_).all()
+
+        await fix_directories(
+            result,
+            subscription,
+            directory_manager,
+            database_session,
+            api_type,
+        )
+        database_session.close()
+    except Exception as _e:
+        pass
```

### Comparing `ultima_scraper_renamer-1.0.0/PKG-INFO` & `ultima_scraper_renamer-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-renamer
-Version: 1.0.0
+Version: 1.1.0
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: ultima-scraper-api (>=1.0.0,<2.0.0)
-Requires-Dist: ultima-scraper-collection (>=1.0.0,<2.0.0)
+Requires-Dist: ultima-scraper-api (>=1.1.0,<2.0.0)
+Requires-Dist: ultima-scraper-collection (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
```

