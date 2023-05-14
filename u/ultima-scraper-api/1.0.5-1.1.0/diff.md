# Comparing `tmp/ultima_scraper_api-1.0.5.tar.gz` & `tmp/ultima_scraper_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_api-1.0.5.tar", max compression
+gzip compressed data, was "ultima_scraper_api-1.1.0.tar", max compression
```

## Comparing `ultima_scraper_api-1.0.5.tar` & `ultima_scraper_api-1.1.0.tar`

### file list

```diff
@@ -1,55 +1,59 @@
--rw-r--r--   0        0        0     1086 2023-04-21 23:52:29.844538 ultima_scraper_api-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.0.5/ultima_scraper_api/.readthedocs.yaml
--rw-r--r--   0        0        0     2140 2023-03-26 20:22:06.588147 ultima_scraper_api-1.0.5/ultima_scraper_api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.0.5/ultima_scraper_api/__main__.py
--rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/__init__.py
--rw-r--r--   0        0        0     6799 2023-03-25 23:19:49.924231 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/api_helper.py
--rw-r--r--   0        0        0     1694 2023-03-13 07:53:19.528681 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/api_streamliner.py
--rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/background_tasks.py
--rw-r--r--   0        0        0     2842 2023-04-09 16:10:08.954446 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/__init__.py
--rw-r--r--   0        0        0      164 2023-03-26 17:40:00.484637 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/__init__.py
--rw-r--r--   0        0        0    19219 2023-04-10 14:08:37.807384 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/auth_model.py
--rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/collection_model.py
--rw-r--r--   0        0        0    11370 2023-04-11 14:57:48.165435 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/extras.py
--rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
--rw-r--r--   0        0        0     6216 2023-04-11 15:11:13.965757 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/message_model.py
--rw-r--r--   0        0        0     6918 2023-04-09 17:42:13.567826 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/post_model.py
--rw-r--r--   0        0        0     3212 2023-03-26 19:02:31.325107 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/story_model.py
--rw-r--r--   0        0        0    27819 2023-04-21 19:38:11.534003 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/decorators/decorators.py
--rw-r--r--   0        0        0     3783 2023-04-11 14:58:58.366956 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/fansly.py
--rw-r--r--   0        0        0     2505 2023-04-09 16:10:03.007639 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/__init__.py
--rw-r--r--   0        0        0      153 2023-03-26 20:30:17.157147 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/__init__.py
--rw-r--r--   0        0        0    19791 2023-04-21 03:37:28.750604 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
--rw-r--r--   0        0        0    10554 2023-03-21 11:26:19.768761 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/extras.py
--rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
--rw-r--r--   0        0        0     2748 2023-03-27 06:43:37.105523 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/message_model.py
--rw-r--r--   0        0        0     3375 2023-03-27 00:23:55.042753 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/post_model.py
--rw-r--r--   0        0        0     1318 2023-04-09 10:09:44.773447 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/story_model.py
--rw-r--r--   0        0        0    26435 2023-04-21 19:37:21.105693 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
--rw-r--r--   0        0        0     3980 2023-03-28 02:35:06.221154 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/onlyfans.py
--rw-r--r--   0        0        0     2678 2023-03-12 07:58:39.963131 ultima_scraper_api-1.0.5/ultima_scraper_api/apis/user_streamliner.py
--rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.0.5/ultima_scraper_api/classes/__init__.py
--rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.0.5/ultima_scraper_api/classes/make_settings.py
--rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.0.5/ultima_scraper_api/classes/prepare_directories.py
--rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.5/ultima_scraper_api/classes/prepare_download.py
--rw-r--r--   0        0        0    13595 2023-04-11 15:12:54.204494 ultima_scraper_api-1.0.5/ultima_scraper_api/classes/prepare_metadata.py
--rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.0.5/ultima_scraper_api/classes/prepare_webhooks.py
--rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.0.5/ultima_scraper_api/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.0.5/ultima_scraper_api/docs/make.bat
--rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.0.5/ultima_scraper_api/docs/requirements.txt
--rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.0.5/ultima_scraper_api/docs/source/conf.py
--rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.0.5/ultima_scraper_api/docs/source/index.rst
--rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.0.5/ultima_scraper_api/helpers/__init__.py
--rw-r--r--   0        0        0    11368 2023-04-21 22:22:23.096800 ultima_scraper_api-1.0.5/ultima_scraper_api/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.0.5/ultima_scraper_api/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.0.5/ultima_scraper_api/managers/job_manager/__init__.py
--rw-r--r--   0        0        0     1791 2023-03-04 03:36:24.985587 ultima_scraper_api-1.0.5/ultima_scraper_api/managers/job_manager/job_manager.py
--rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.0.5/ultima_scraper_api/managers/job_manager/jobs/__init__.py
--rw-r--r--   0        0        0      704 2023-03-24 22:51:29.186132 ultima_scraper_api-1.0.5/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
--rw-r--r--   0        0        0     2181 2023-03-27 18:00:12.375116 ultima_scraper_api-1.0.5/ultima_scraper_api/managers/scrape_manager.py
--rw-r--r--   0        0        0    14873 2023-04-21 23:52:18.977804 ultima_scraper_api-1.0.5/ultima_scraper_api/managers/session_manager.py
--rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.0.5/ultima_scraper_api/py.typed
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 ultima_scraper_api-1.0.5/setup.py
--rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 ultima_scraper_api-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1193 2023-05-14 20:18:01.670537 ultima_scraper_api-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.1.0/ultima_scraper_api/.readthedocs.yaml
+-rw-r--r--   0        0        0     2286 2023-05-13 21:02:27.542962 ultima_scraper_api-1.1.0/ultima_scraper_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.1.0/ultima_scraper_api/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/__init__.py
+-rw-r--r--   0        0        0     6875 2023-05-10 16:14:24.886974 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/api_helper.py
+-rw-r--r--   0        0        0     3348 2023-05-08 16:02:24.472891 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/api_streamliner.py
+-rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/background_tasks.py
+-rw-r--r--   0        0        0     2895 2023-05-09 15:10:07.346536 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-13 20:33:08.152436 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/__init__.py
+-rw-r--r--   0        0        0    19412 2023-05-14 02:46:17.178578 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/auth_model.py
+-rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/collection_model.py
+-rw-r--r--   0        0        0    11370 2023-04-11 14:57:48.165435 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/extras.py
+-rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
+-rw-r--r--   0        0        0     6463 2023-05-13 21:26:45.672240 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/message_model.py
+-rw-r--r--   0        0        0     6918 2023-04-09 17:42:13.567826 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/post_model.py
+-rw-r--r--   0        0        0     3210 2023-05-14 02:55:01.328937 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/story_model.py
+-rw-r--r--   0        0        0      862 2023-05-14 01:36:53.261674 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/subscription_model.py
+-rw-r--r--   0        0        0    27819 2023-05-14 01:25:40.886202 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/decorators/decorators.py
+-rw-r--r--   0        0        0     2651 2023-05-14 13:27:19.560917 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/fansly.py
+-rw-r--r--   0        0        0     2784 2023-05-10 22:02:50.317100 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/__init__.py
+-rw-r--r--   0        0        0      191 2023-05-11 21:59:14.648026 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/__init__.py
+-rw-r--r--   0        0        0    18865 2023-05-14 01:48:23.829859 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
+-rw-r--r--   0        0        0    11378 2023-05-10 21:08:35.574644 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/extras.py
+-rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
+-rw-r--r--   0        0        0     2971 2023-05-10 21:01:08.286698 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/message_model.py
+-rw-r--r--   0        0        0     5698 2023-05-10 22:20:10.202315 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
+-rw-r--r--   0        0        0     3375 2023-03-27 00:23:55.042753 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/post_model.py
+-rw-r--r--   0        0        0     1318 2023-04-09 10:09:44.773447 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/story_model.py
+-rw-r--r--   0        0        0     1623 2023-05-13 21:04:18.608237 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
+-rw-r--r--   0        0        0    28372 2023-05-10 19:46:18.928115 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
+-rw-r--r--   0        0        0     2932 2023-05-14 13:27:38.918048 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/onlyfans.py
+-rw-r--r--   0        0        0     2763 2023-05-05 07:56:21.734680 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/user_streamliner.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.1.0/ultima_scraper_api/classes/__init__.py
+-rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.1.0/ultima_scraper_api/classes/make_settings.py
+-rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_directories.py
+-rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_download.py
+-rw-r--r--   0        0        0    13410 2023-05-07 21:56:21.760084 ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_metadata.py
+-rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_webhooks.py
+-rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.0/ultima_scraper_api/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.0/ultima_scraper_api/docs/make.bat
+-rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.1.0/ultima_scraper_api/docs/requirements.txt
+-rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.1.0/ultima_scraper_api/docs/source/conf.py
+-rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.1.0/ultima_scraper_api/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.1.0/ultima_scraper_api/helpers/__init__.py
+-rw-r--r--   0        0        0    11324 2023-05-09 19:08:54.838979 ultima_scraper_api-1.1.0/ultima_scraper_api/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/job_manager/__init__.py
+-rw-r--r--   0        0        0     1792 2023-05-13 20:28:21.224283 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/job_manager/job_manager.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/job_manager/jobs/__init__.py
+-rw-r--r--   0        0        0      767 2023-05-12 15:00:15.819155 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
+-rw-r--r--   0        0        0     2181 2023-03-27 18:00:12.375116 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/scrape_manager.py
+-rw-r--r--   0        0        0    17572 2023-05-13 13:21:06.845191 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/session_manager.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-1.1.0/ultima_scraper_api/models/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-11 21:44:11.005112 ultima_scraper_api-1.1.0/ultima_scraper_api/models/subscription_model.py
+-rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.1.0/ultima_scraper_api/py.typed
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 ultima_scraper_api-1.1.0/PKG-INFO
```

### Comparing `ultima_scraper_api-1.0.5/pyproject.toml` & `ultima_scraper_api-1.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 [tool.poetry]
 name = "ultima-scraper-api"
-version = "1.0.5"
+version = "1.1.0"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_api"}]
 include = ["ultima_scraper_api/py.typed"]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10,<3.12"
 requests = {extras = ["socks"], version = "2.28.2"}
 orjson = "^3.8.3"
 dill = "^0.3.6"
 python-socks = {extras = ["asyncio"], version = "2.2.0"}
 aiohttp = "^3.8.4"
-aiohttp-socks = "^0.7.1"
+aiohttp-socks = "^0.8.0"
 mergedeep = "^1.3.4"
 python-dateutil = "^2.8.2"
 user-agent = "^0.1.10"
 aiofiles = "^22.1.0"
 beautifulsoup4 = "^4.11.1"
-Sphinx = "^5.3.0"
-sphinx-autoapi = "^2.0.0"
-sphinx-rtd-theme = "^1.1.1"
 mypy = "^0.991"
 lxml =  "^4.9.1"
 win32-setctime = {version="^1.1.0", platform = 'win32'}
+pywidevine = "^1.6.0"
+xmltodict = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.2"
+black = {version = "^23.3.0", allow-prereleases = true}
+Sphinx = "^5.3.0"
+sphinx-autoapi = "^2.0.0"
+sphinx-rtd-theme = "^1.1.1"
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
 
 [project.urls]
 Homepage = "https://github.com/DIGITALCRIMINALS/UltimaScraperAPI"
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/__init__.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,20 @@
 post_types = (
     onlyfans_classes.post_model.create_post | fansly_classes.post_model.create_post
 )
 message_types = (
     onlyfans_classes.message_model.create_message
     | fansly_classes.message_model.create_message
 )
-content_types = story_types|post_types|message_types
+subscription_types = (
+    onlyfans_classes.subscription_model.SubscriptionModel
+    | fansly_classes.subscription_model.SubscriptionModel
+)
+
+content_types = story_types | post_types | message_types
 error_types = onlyfans_classes.extras.ErrorDetails | fansly_classes.extras.ErrorDetails
 
 
 def select_api(option: str, config: Config = Config()):
     """Allows you to select an API
 
     Args:
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/api_helper.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/api_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,7 +201,11 @@
         final_results.append(results)
     else:
         final_results = results
     final_results = [x for x in final_results if not isinstance(x, error_types)]
     if wrapped and final_results:
         final_results = final_results[0]
     return final_results
+
+
+async def extract_list(result: dict[str, Any]):
+    return result["list"]
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/background_tasks.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/__init__.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Literal
 from urllib.parse import urlparse
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.fansly.classes.user_model import (
         create_auth,
         create_user,
     )
 
+SubscriptionType = Literal["all", "active", "expired"]
+
 
 class SiteContent:
     def __init__(self, option: dict[str, Any], user: create_auth | create_user) -> None:
         self.id: int = int(option["id"])
         self.author = user
         self.media: list[dict[str, Any]] = option.get("media", [])
-        self.preview_ids:list[int] = []
+        self.preview_ids: list[int] = []
 
-    def url_picker(self, media_item:dict[str, Any],video_quality: str=""):
-        
+    def url_picker(self, media_item: dict[str, Any], video_quality: str = ""):
         # There are two media results at play here.
         # The top-level `media` element itself represents the original source quality.
         # It may also contain a `variants` list entry with alternate encoding qualities.
         # Each variant has a similar structure to the main media element.
         video_quality = (
             video_quality or self.author.get_api().get_site_settings().video_quality
         )
@@ -63,16 +64,17 @@
 
             # Return the first media <= the target quality.
             if media_quality <= int(quality_key):
                 return urlparse(media_url)
 
         # If all media was > target quality, return the lowest quality/last media.
         return urlparse(media_url)
-        
+
     def preview_url_picker(self, media_item: dict[str, Any]):
-        return  None
+        return None
+
     def get_author(self):
         return self.author
 
     async def refresh(self):
         func = await self.author.scrape_manager.handle_refresh(self)
         return await func(self.id)
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/auth_model.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/auth_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,21 +11,26 @@
     AuthDetails,
     ErrorDetails,
     create_headers,
     endpoint_links,
 )
 from ultima_scraper_api.apis.fansly.classes.message_model import create_message
 from ultima_scraper_api.apis.fansly.classes.post_model import create_post
+from ultima_scraper_api.apis.fansly.classes.subscription_model import SubscriptionModel
 from ultima_scraper_api.apis.fansly.classes.user_model import create_user
 from ultima_scraper_api.managers.session_manager import SessionManager
 from user_agent import generate_user_agent
+from ultima_scraper_api.apis.fansly import SubscriptionType
 
 if TYPE_CHECKING:
+    from ultima_scraper_api.apis.onlyfans.classes.only_drm import OnlyDRM
     from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
 
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+
 
 class create_auth(create_user):
     def __init__(
         self,
         api: FanslyAPI,
         option: dict[str, Any] = {},
         max_threads: int = -1,
@@ -36,25 +41,27 @@
         self.auth_details = auth_details
         self.session_manager = self._SessionManager(self, max_threads=max_threads)
         create_user.__init__(self, option, self)
         if not self.username:
             self.username = f"u{self.id}"
         self.lists = []
         self.links = api.ContentTypes()
-        self.subscriptions: list[create_user] = []
+        self.subscriptions: list[SubscriptionModel] = []
+        self.followed_users: list[create_user] = []
         self.chats = None
         self.archived_stories = {}
         self.mass_messages = []
         self.paid_content: list[create_message | create_post] = []
         self.auth_attempt = 0
         self.guest = False
         self.active: bool = False
         self.errors: list[ErrorDetails] = []
         self.extras: dict[str, Any] = {}
         self.blacklist: list[str] = []
+        self.drm: OnlyDRM | None = None
 
     class _SessionManager(SessionManager):
         def __init__(
             self,
             auth: create_auth,
             headers: dict[str, Any] = {},
             proxies: list[str] = [],
@@ -224,26 +231,29 @@
         if self.id in identifiers or self.username in identifiers:
             return True
         else:
             return False
 
     def find_user_by_identifier(self, identifier: int | str):
         user = [x for x in self.users if x.id == identifier or x.username == identifier]
-        return user
-
-    async def get_user(self, identifier: int | str) -> Union[create_user, ErrorDetails]:
-        link = endpoint_links().list_users([identifier])
-        response = await self.session_manager.json_request(link)
-        if not isinstance(response, ErrorDetails):
-            if response["response"]:
+        if user:
+            user = user[0]
+            return user
+
+    async def get_user(self, identifier: int | str):
+        valid_user = self.find_user_by_identifier(identifier)
+        if valid_user:
+            return valid_user
+        else:
+            link = endpoint_links(identifier).users
+            response = await self.session_manager.json_request(link)
+            if "error" not in response:
                 response["session_manager"] = self.session_manager
-                response = create_user(response["response"][0], self)
-            else:
-                response = ErrorDetails({"code": 69, "message": "User Doesn't Exist"})
-        return response
+                response = create_user(response, self)
+            return response
 
     async def get_lists_users(
         self,
         identifier: int | str,
         check: bool = False,
         limit: int = 100,
         offset: int = 0,
@@ -311,69 +321,65 @@
         for subscription in subscriptions:
             if identifier == subscription.username or identifier == subscription.id:
                 valid = subscription
                 break
         return valid
 
     async def get_subscriptions(
-        self, refresh: bool = True, identifiers: list[int | str] = []
-    ) -> list[create_user]:
+        self,
+        refresh: bool = True,
+        identifiers: list[int | str] = [],
+        sub_type: SubscriptionType = "all",
+    ):
         result, status = await api_helper.default_data(self, refresh)
         if status:
+            result: list[SubscriptionModel]
             return result
         subscriptions_link = endpoint_links().subscriptions
         temp_subscriptions = await self.session_manager.json_request(subscriptions_link)
-        subscriptions = temp_subscriptions["response"]["subscriptions"]
+        raw_subscriptions = temp_subscriptions["response"]["subscriptions"]
 
-        # If user is a creator, add them to the subscription list
-        results: list[list[create_user]] = []
-        if self.isPerformer:
-            subscription = await self.convert_to_user()
-            if isinstance(subscription, ErrorDetails):
-                return result
-            subscription.subscribedByData = {}
-            new_date = datetime.now() + relativedelta(years=1)
-            subscription.subscribedByData["expiredAt"] = new_date.isoformat()
-            subscriptions_ = [subscription]
-            results.append(subscriptions_)
-        if not identifiers:
-
-            async def multi(item: dict[str, Any]):
-                subscription = await self.get_user(item["accountId"])
-                valid_subscriptions: list[create_user] = []
-
-                if (
-                    isinstance(subscription, create_user)
-                    and subscription.following
-                    and not subscription.subscribedByData
-                ):
-                    new_date = datetime.now() + relativedelta(years=1)
-                    new_date = int(new_date.timestamp() * 1000)
-                    subscription.subscribedByData = {}
-                    subscription.subscribedByData["endsAt"] = new_date
-                    valid_subscriptions.append(subscription)
-                return valid_subscriptions
-
-            with self.get_pool() as pool:
-                tasks = pool.starmap(multi, product(subscriptions))
-                results += await asyncio.gather(*tasks)
-        else:
+        async def assign_user_to_sub(raw_subscription: Dict[str, Any]):
+            user = await self.get_user(raw_subscription["accountId"])
+            if isinstance(user, dict):
+                user = create_user(raw_subscription, self)
+                user.active = False
+            subscription_model = SubscriptionModel(raw_subscription, user, self)
+            return subscription_model
+
+        subscriptions: list[SubscriptionModel] = []
+        if identifiers:
+            found_raw_subscriptions: list[dict[str, Any]] = []
             for identifier in identifiers:
-                results_2 = await self.get_user(identifier)
-                results_2 = await api_helper.remove_errors(results_2)
-                if isinstance(results_2, create_user):
-                    x = [x for x in subscriptions if x["accountId"] == results_2.id]
-                    if x:
-                        results_2.subscribedByData = {}
-                        results_2.subscribedByData["endsAt"] = x[0]["endsAt"]
-                    results.append([results_2])
-        results = [x for x in results if x is not None]
-        results = list(chain(*results))
-        self.subscriptions = results
-        return results
+                for raw_subscription in raw_subscriptions:
+                    if (
+                        identifier == raw_subscription["id"]
+                        or identifier == raw_subscription["username"]
+                    ):
+                        found_raw_subscriptions.append(raw_subscription)
+                        break
+            raw_subscriptions = found_raw_subscriptions
+        with self.get_pool() as pool:
+            tasks = pool.starmap(assign_user_to_sub, product(raw_subscriptions))
+            subscriptions: list[SubscriptionModel] = await asyncio.gather(*tasks)
+
+        match sub_type:
+            case "all":
+                pass
+            case "active":
+                subscriptions = [
+                    x for x in subscriptions if x.ends_at > datetime.utcnow()
+                ]
+            case "expired":
+                subscriptions = [
+                    x for x in subscriptions if x.ends_at < datetime.utcnow()
+                ]
+            case _:
+                raise ValueError(f"Invalid subscription type: {sub_type}")
+        return subscriptions
 
     async def get_chats(
         self,
         links: list[str] = [],
         limit: int = 25,
         offset: int = 0,
         depth: int = 1,
@@ -477,7 +483,13 @@
     async def resolve_user(self, post_id: int | None = None):
         user = None
         if post_id:
             post = await self.get_post(post_id)
             if not isinstance(post, ErrorDetails):
                 user = post.author
         return user
+
+    async def get_scrapable_users(self):
+        followed_users = self.followed_users
+        subscription_users = [x.user for x in self.subscriptions]
+        unique_users = list(set(followed_users) | set(subscription_users))
+        return unique_users
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/collection_model.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/collection_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/extras.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/extras.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/message_model.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/message_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,29 @@
     from ultima_scraper_api.apis.fansly.classes.user_model import create_user
 
 
 class create_message(SiteContent):
     def __init__(
         self, option: dict[str, Any], user: create_user, extra: dict[Any, Any] = {}
     ) -> None:
-        author = user
+        author = user.get_authed().find_user_by_identifier(option["senderId"])
+        self.user = user
         SiteContent.__init__(self, option, author)
         self.responseType: Optional[str] = option.get("responseType")
         self.text: str = option["content"]
         self.lockedText: Optional[bool] = option.get("lockedText")
         self.isFree: Optional[bool] = option.get("isFree")
         self.price: Optional[float] = option.get("price")
         self.isMediaReady: Optional[bool] = option.get("isMediaReady")
         self.mediaCount: Optional[int] = option.get("mediaCount")
         self.media: list[Any] = option.get("attachments", [])
         self.previews: list[dict[str, Any]] = option.get("previews", [])
         self.isTip: Optional[bool] = option.get("isTip")
         self.isReportedByMe: Optional[bool] = option.get("isReportedByMe")
-        self.fromUser = user.get_authed().find_user_by_identifier(option["senderId"])[0]
+        self.fromUser = user.get_authed().find_user_by_identifier(option["senderId"])
         self.isFromQueue: Optional[bool] = option.get("isFromQueue")
         self.queueId: Optional[int] = option.get("queueId")
         self.canUnsendQueue: Optional[bool] = option.get("canUnsendQueue")
         self.unsendSecondsQueue: Optional[int] = option.get("unsendSecondsQueue")
         self.isOpened: Optional[bool] = option.get("isOpened")
         self.isNew: Optional[bool] = option.get("isNew")
         self.createdAt: Optional[str] = option.get("createdAt")
@@ -73,15 +74,21 @@
                             temp_media = account_media["media"]
                         if temp_media:
                             final_media.append(temp_media)
         self.media = final_media
         self.user = user
 
     def get_author(self):
-        return self.fromUser
+        return self.author
+
+    def get_receiver(self):
+        receiver = (
+            self.author.get_authed() if self.author.id == self.user.id else self.user
+        )
+        return receiver
 
     async def buy_message(self):
         """
         This function will buy a ppv message from a model.
         """
         message_price = self.price
         x = {
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/post_model.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/story_model.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/story_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING, Any
 
 from ultima_scraper_api.apis.fansly import SiteContent
 
 if TYPE_CHECKING:
-    from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
+    from ultima_scraper_api.apis.fansly.classes.user_model import create_user
 
 class create_story(SiteContent):
     def __init__(self, option: dict[str, Any], user: "create_user") -> None:
         SiteContent.__init__(self, option, user)
         self.userId: int = option.get("userId")
         self.createdAt: str = option.get("createdAt")
         self.expiredAt: str = option.get("expiredAt")
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/classes/user_model.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/user_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/fansly/fansly.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/fansly.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,40 +8,17 @@
 
 
 class FanslyAPI(StreamlinedAPI):
     def __init__(self, config: Config) -> None:
         self.site_name: Literal["Fansly"] = "Fansly"
         StreamlinedAPI.__init__(self, self, config)
         self.auths: list[create_auth] = []
-        self.subscriptions: list[create_user] = []
+        self.users: dict[int, create_user] = {}
         self.endpoint_links = endpoint_links
 
-    def add_auth(
-        self, auth_json: dict[str, Any] = {}, only_active: bool = False
-    ) -> create_auth:
-        """Creates and appends an auth object to auths property
-
-        Args:
-            auth_json (dict[str, str], optional): []. Defaults to {}.
-            only_active (bool, optional): [description]. Defaults to False.
-
-        Returns:
-            create_auth: [Auth object]
-        """
-        temp_auth_details = AuthDetails(**auth_json).upgrade_legacy(auth_json)
-        auth = create_auth(
-            self, max_threads=self.max_threads, auth_details=temp_auth_details
-        )
-        if only_active and not auth.auth_details.active:
-            return auth
-        auth.auth_details = temp_auth_details
-        auth.extras["settings"] = self.config
-        self.auths.append(auth)
-        return auth
-
     def get_auth(self, identifier: Union[str, int]) -> Optional[create_auth]:
         final_auth = None
         for auth in self.auths:
             if auth.id == identifier:
                 final_auth = auth
             elif auth.username == identifier:
                 final_auth = auth
@@ -58,25 +35,16 @@
         Returns:
             auth_details: [auth_details object]
         """
         return AuthDetails(**auth_json).upgrade_legacy(auth_json)
 
     class ContentTypes:
         def __init__(self) -> None:
-            class ArchivedTypes:
-                def __init__(self) -> None:
-                    self.Posts = []
-
-                def __iter__(self):
-                    for attr, value in self.__dict__.items():
-                        yield attr, value
-
             self.Stories = []
             self.Posts = []
-            # self.Archived = ArchivedTypes()
             self.Chats = []
             self.Messages = []
             self.Highlights = []
             self.MassMessages = []
 
         def __iter__(self):
             for attr, value in self.__dict__.items():
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/__init__.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Literal
 from urllib.parse import urlparse
 
+SubscriptionType = Literal["all", "active", "expired", "attention"]
+
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.onlyfans.classes.user_model import (
         create_auth,
         create_user,
     )
 
 
 class SiteContent:
     def __init__(self, option: dict[str, Any], user: create_auth | create_user) -> None:
         self.id: int = option["id"]
         self.author = user
         self.media: list[dict[str, Any]] = option.get("media", [])
-        self.preview_ids:list[int] = []
-
+        self.preview_ids: list[int] = []
 
     def url_picker(self, media_item: dict[str, Any], video_quality: str = ""):
+        authed = self.get_author().get_authed()
         video_quality = (
             video_quality or self.author.get_api().get_site_settings().video_quality
         )
         if not media_item["canView"]:
             return
         source: dict[str, Any] = {}
         media_type: str = ""
@@ -45,26 +47,31 @@
                 video_quality = video_quality.removesuffix("p")
                 if quality == video_quality:
                     if quality_link:
                         url = quality_link
                         break
         if "src" in media_item:
             url = media_item["src"]
+        if authed.drm:
+            has_drm = authed.drm.has_drm(media_item)
+            if has_drm:
+                url = has_drm
         return urlparse(url) if url else None
-        
+
     def preview_url_picker(self, media_item: dict[str, Any]):
+        preview_url = None
         if "files" in media_item:
             if (
                 "preview" in media_item["files"]
                 and "url" in media_item["files"]["preview"]
             ):
                 preview_url = media_item["files"]["preview"]["url"]
         else:
             preview_url = media_item["preview"]
-        return urlparse(preview_url) if preview_url else None
+            return urlparse(preview_url) if preview_url else None
 
     def get_author(self):
         return self.author
 
     async def refresh(self):
         func = await self.author.scrape_manager.handle_refresh(self)
         return await func(self.id)
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/auth_model.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/auth_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from __future__ import annotations
 
 import asyncio
 import math
-from asyncio.tasks import Task
-from datetime import datetime
 from itertools import chain, product
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
-from dateutil.relativedelta import relativedelta
 from ultima_scraper_api.apis import api_helper
 from ultima_scraper_api.apis.onlyfans.classes.extras import (
     AuthDetails,
     ErrorDetails,
     create_headers,
     endpoint_links,
 )
 from ultima_scraper_api.apis.onlyfans.classes.message_model import create_message
 from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
 from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 from ultima_scraper_api.managers.session_manager import SessionManager
 from user_agent import generate_user_agent
+from ultima_scraper_api.apis.onlyfans import SubscriptionType
+from ultima_scraper_api.apis.onlyfans.classes.subscription_model import (
+    SubscriptionModel,
+)
 
 if TYPE_CHECKING:
+    from ultima_scraper_api.apis.onlyfans.classes.only_drm import OnlyDRM
     from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
 
 # auth_model.py handles functions that only relate to the authenticated user
 # We can create a auth_streamliner that has a parent class of create_user instead
 
 
 class create_auth(create_user):
@@ -41,25 +43,26 @@
         self.auth_details = auth_details
         self.session_manager = self._SessionManager(self, max_threads=max_threads)
         create_user.__init__(self, option, self)
         if not self.username:
             self.username = f"u{self.id}"
         self.lists = []
         self.links = api.ContentTypes()
-        self.subscriptions: list[create_user] = []
+        self.subscriptions: list[SubscriptionModel] = []
         self.chats = None
         self.archived_stories = {}
         self.mass_messages = []
         self.paid_content: list[create_message | create_post] = []
         self.auth_attempt = 0
         self.guest = False
         self.active: bool = False
         self.errors: list[ErrorDetails] = []
         self.extras: dict[str, Any] = {}
         self.blacklist: list[str] = []
+        self.drm: OnlyDRM | None = None
 
     class _SessionManager(SessionManager):
         def __init__(
             self,
             auth: create_auth,
             headers: dict[str, Any] = {},
             proxies: list[str] = [],
@@ -101,22 +104,21 @@
         dynamic_rules = self.session_manager.dynamic_rules
         a: list[Any] = [dynamic_rules, auth_id, auth_items.x_bc, user_agent, link]
         self.session_manager.headers = create_headers(*a)
         if guest:
             self.guest = True
             return self
 
-        while self.auth_attempt < max_attempts + 1:
+        while self.auth_attempt < max_attempts:
             await self.process_auth()
             self.auth_attempt += 1
 
             async def resolve_auth(auth: create_auth):
                 if self.errors:
                     error = self.errors[-1]
-                    print(error.message)
                     if error.code == 101:
                         if auth_items.support_2fa:
                             link = f"https://onlyfans.com/api2/v2/users/otp/check"
                             count = 1
                             max_count = 3
                             while count < max_count + 1:
                                 print(
@@ -144,16 +146,14 @@
                     error_message = error.message
                     if "token" in error_message:
                         break
                     if "Code wrong" in error_message:
                         break
                     if "Please refresh" in error_message:
                         break
-                else:
-                    print("Auth 404'ed")
                 continue
             else:
                 break
         if not self.active:
             user = await self.get_user(auth_id)
             if isinstance(user, create_user):
                 self.update(user.__dict__)
@@ -187,15 +187,15 @@
         error_code = error.code
         if error_code == 0:
             pass
         elif error_code == 101:
             error_message = "Blocked by 2FA."
         elif error_code == 401:
             # Session/Refresh
-            pass
+            error_message = "Invalid Auth Info"
         error.code = error_code
         error.message = error_message
         match error_code:
             case 0:
                 pass
             case _:
                 await api_helper.handle_error_details(error)
@@ -230,24 +230,26 @@
         if self.id in identifiers or self.username in identifiers:
             return True
         else:
             return False
 
     def find_user_by_identifier(self, identifier: int | str):
         user = [x for x in self.users if x.id == identifier or x.username == identifier]
-        return user
+        if user:
+            user = user[0]
+            return user
 
-    async def get_user(self, identifier: int | str) -> Union[create_user, ErrorDetails]:
+    async def get_user(self, identifier: int | str):
         valid_user = self.find_user_by_identifier(identifier)
         if valid_user:
-            return valid_user[0]
+            return valid_user
         else:
             link = endpoint_links(identifier).users
             response = await self.session_manager.json_request(link)
-            if not isinstance(response, ErrorDetails):
+            if "error" not in response:
                 response["session_manager"] = self.session_manager
                 response = create_user(response, self)
             return response
 
     async def get_lists_users(
         self,
         identifier: int | str,
@@ -266,120 +268,95 @@
             results2 = await self.get_lists_users(
                 identifier, limit=limit, offset=limit + offset
             )
             results.extend(results2)
         return results
 
     async def get_subscription(
-        self, identifier: int | str = "", custom_list: list[create_user] = []
-    ) -> create_user | None:
+        self, identifier: int | str = "", custom_list: list[SubscriptionModel] = []
+    ) -> SubscriptionModel | None:
         subscriptions = (
             await self.get_subscriptions(refresh=False)
             if not custom_list
             else custom_list
         )
         valid = None
         for subscription in subscriptions:
-            if identifier == subscription.username or identifier == subscription.id:
+            if (
+                identifier == subscription.user.username
+                or identifier == subscription.user.id
+            ):
                 valid = subscription
                 break
         return valid
 
     async def get_subscriptions(
         self,
         refresh: bool = True,
         identifiers: list[int | str] = [],
-        extra_info: bool = True,
         limit: int = 20,
-    ) -> list[create_user]:
+        sub_type: SubscriptionType = "all",
+    ):
         result, status = await api_helper.default_data(self, refresh)
         if status:
+            result: list[SubscriptionModel]
             return result
-        # if self.subscribesCount > 900:
-        #     limit = 100
-        ceil = math.ceil(self.subscribesCount / limit)
+        url = endpoint_links().subscription_count
+        subscriptions_count = await self.session_manager.json_request(url)
+        subscriptions_info = subscriptions_count["subscriptions"]
+        match sub_type:
+            case "all":
+                subscription_type_count = subscriptions_info[sub_type]
+            case "active":
+                subscription_type_count = subscriptions_info[sub_type]
+            case "expired":
+                subscription_type_count = subscriptions_info[sub_type]
+            case _:
+                raise ValueError(f"Invalid subscription type: {sub_type}")
+        ceil = math.ceil(subscription_type_count / limit)
         a = list(range(ceil))
-        offset_array: list[str] = []
+        urls: list[str] = []
         for b in a:
             b = b * limit
-            link = endpoint_links(global_limit=limit, global_offset=b).subscriptions
-            offset_array.append(link)
-
-        results: list[list[create_user]] = []
-        if not identifiers:
-
-            async def multi(item: str):
-                link = item
-                subscriptions = await self.session_manager.json_request(link)
-                valid_subscriptions: list[create_user] = []
-                extras = {}
-                extras["auth_check"] = ""
-                if isinstance(subscriptions, ErrorDetails):
-                    return
-                subscriptions = [
-                    subscription
-                    for subscription in subscriptions
-                    if "error" != subscription
-                ]
-                tasks: list[Task[create_user | ErrorDetails]] = []
-                for subscription in subscriptions:
-                    subscription["session_manager"] = self.session_manager
-                    if extra_info:
-                        task = asyncio.create_task(
-                            self.get_user(subscription["username"])
-                        )
-                        tasks.append(task)
-                results2 = await asyncio.gather(*tasks)
-                for result in results2:
-                    if isinstance(result, ErrorDetails):
-                        continue
-                    if not result:
-                        pass
-                    subscription2: create_user = result
-                    for subscription in subscriptions:
-                        if subscription["id"] != subscription2.id:
-                            continue
-                        subscription = subscription | subscription2.__dict__
-                        subscription = create_user(subscription, self)
-                        if subscription.isBlocked:
-                            continue
-                        valid_subscriptions.append(subscription)
-                return valid_subscriptions
-
-            # If user is a creator, add them to the subscription list
-            if self.isPerformer:
-                subscription = await self.convert_to_user()
-                if isinstance(subscription, ErrorDetails):
-                    return result
-                subscription.subscribedByData = {}
-                new_date = datetime.now() + relativedelta(years=1)
-                subscription.subscribedByData["expiredAt"] = new_date.isoformat()
-                subscriptions = [subscription]
-                results.append(subscriptions)
-            with self.get_pool() as pool:
-                tasks = pool.starmap(multi, product(offset_array))
-                results2 = await asyncio.gather(*tasks)
-                results2 = list(filter(None, results2))
-                results.extend(results2)
-        else:
+            link = endpoint_links(
+                identifier=sub_type, global_limit=limit, global_offset=b
+            ).subscriptions
+            urls.append(link)
+
+        subscription_responses = await self.session_manager.bulk_json_requests(urls)
+        raw_subscriptions = [
+            raw_subscription
+            for temp_raw_subscriptions in subscription_responses
+            for raw_subscription in temp_raw_subscriptions
+        ]
+
+        async def assign_user_to_sub(raw_subscription: Dict[str, Any]):
+            user = await self.get_user(raw_subscription["username"])
+            if isinstance(user, dict):
+                user = create_user(raw_subscription, self)
+                user.active = False
+            subscription_model = SubscriptionModel(raw_subscription, user, self)
+            return subscription_model
+
+        subscriptions: list[SubscriptionModel] = []
+        if identifiers:
+            found_raw_subscriptions: list[dict[str, Any]] = []
             for identifier in identifiers:
-                if self.id == identifier or self.username == identifier:
-                    continue
-                link = endpoint_links(identifier=identifier).users
-                result = await self.session_manager.json_request(link)
-                if isinstance(result, ErrorDetails) or not result["subscribedBy"]:
-                    continue
-                subscription = create_user(result, self)
-                if subscription.isBlocked:
-                    continue
-                results.append([subscription])
-        final_results = [x for x in results if x is not None]
-        final_results = list(chain(*final_results))
-        self.subscriptions = final_results
-        return final_results
+                for raw_subscription in raw_subscriptions:
+                    if (
+                        identifier == raw_subscription["id"]
+                        or identifier == raw_subscription["username"]
+                    ):
+                        found_raw_subscriptions.append(raw_subscription)
+                        break
+            raw_subscriptions = found_raw_subscriptions
+        with self.get_pool() as pool:
+            tasks = pool.starmap(assign_user_to_sub, product(raw_subscriptions))
+            subscriptions: list[SubscriptionModel] = await asyncio.gather(*tasks)
+        return subscriptions
 
     async def get_chats(
         self,
         links: list[str] = [],
         limit: int = 100,
         offset: int = 0,
         depth: int = 1,
@@ -482,15 +459,17 @@
                 )
                 final_results.extend(results2)
             if not inside_loop:
                 temp: list[create_message | create_post] = []
                 for final_result in final_results:
                     content = None
                     if final_result["responseType"] == "message":
-                        user = create_user(final_result["fromUser"], self)
+                        user = await self.get_user(final_result["fromUser"]["id"])
+                        if not user:
+                            user = create_user(final_result["fromUser"], self)
                         content = create_message(final_result, user)
                     elif final_result["responseType"] == "post":
                         user = create_user(final_result["author"], self)
                         content = create_post(final_result, user)
                     if content:
                         temp.append(content)
                 final_results = temp
@@ -500,7 +479,11 @@
     async def resolve_user(self, post_id: int | None = None):
         user = None
         if post_id:
             post = await self.get_post(post_id)
             if not isinstance(post, ErrorDetails):
                 user = post.author
         return user
+
+    async def get_scrapable_users(self):
+        subscription_users = [x.user for x in self.subscriptions]
+        return subscription_users
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/extras.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/extras.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 import copy
 import math
 from itertools import chain
 from pathlib import Path
 from typing import Any, Literal, Optional, Union
+from urllib.parse import urlparse, parse_qs
 
 
 class AuthDetails:
-    def __init__(self, username:str="", cookie:str="", x_bc:str="",user_agent:str="",email:str="", password:str="", hashed:bool=False,support_2fa:bool=True, active:bool=True) -> None:
+    def __init__(
+        self,
+        username: str = "",
+        cookie: str = "",
+        x_bc: str = "",
+        user_agent: str = "",
+        email: str = "",
+        password: str = "",
+        hashed: bool = False,
+        support_2fa: bool = True,
+        active: bool = True,
+    ) -> None:
         self.username = username
         self.cookie = cookie_parser(cookie)
         self.x_bc = x_bc
         self.user_agent = user_agent
         self.email = email
         self.password = password
         self.hashed = hashed
@@ -18,21 +30,25 @@
         self.active = active
 
     def upgrade_legacy(self, options: dict[str, Any]):
         if "cookie" not in options:
             self = legacy_auth_details(options).upgrade(self)
         return self
 
-    def export(self):
+    def export(self, model: Any = None):
         new_dict = copy.copy(self.__dict__)
         cookie = self.cookie.convert()
         results = [
             x for x in cookie.replace(" ", "").split(";") if x and x.split("=")[1]
         ]
         new_dict["cookie"] = cookie if results else ""
+        if model:
+            for att in new_dict.copy():
+                if att not in model.__annotations__:
+                    del new_dict[att]
         return new_dict
 
 
 class legacy_auth_details:
     def __init__(self, option: dict[str, Any] = {}):
         self.username = option.get("username", "")
         self.auth_id = option.get("auth_id", "")
@@ -108,15 +124,15 @@
     ):
         domain = "https://onlyfans.com"
         api = "/api2/v2"
         full_url_path = f"{domain}{api}"
         self.full_url_path = full_url_path
         self.customer = f"https://onlyfans.com/api2/v2/users/me"
         self.users = f"https://onlyfans.com/api2/v2/users/{identifier}"
-        self.subscriptions = f"https://onlyfans.com/api2/v2/subscriptions/subscribes?limit={global_limit}&offset={global_offset}&type=active"
+        self.subscriptions = f"{full_url_path}/subscriptions/subscribes?limit={global_limit}&offset={global_offset}&type={identifier}"
         self.lists = f"https://onlyfans.com/api2/v2/lists?limit=100&offset=0"
         self.lists_users = f"https://onlyfans.com/api2/v2/lists/{identifier}/users?limit={global_limit}&offset={global_offset}&query="
         self.list_chats = f"https://onlyfans.com/api2/v2/chats?limit={global_limit}&offset={global_offset}&order=desc"
         self.post_by_id = f"https://onlyfans.com/api2/v2/posts/{identifier}"
         self.message_by_id = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages?limit=10&offset=0&firstId={identifier2}&order=desc&skip_users=all&skip_users_dups=1"
         self.search_chat = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages/search?query={text}"
         self.message_api = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages?limit={global_limit}&offset={global_offset}&order=desc"
@@ -133,15 +149,19 @@
         self.subscribe = f"https://onlyfans.com/api2/v2/users/{identifier}/subscribe"
         self.like = f"https://onlyfans.com/api2/v2/{identifier}/{identifier2}/like"
         self.favorite = f"https://onlyfans.com/api2/v2/{identifier}/{identifier2}/favorites/{identifier3}"
         self.transactions = (
             f"https://onlyfans.com/api2/v2/payments/all/transactions?limit=10&offset=0"
         )
         self.list_comments_api = f"{full_url_path}/{identifier}/{identifier2}/comments?limit={global_limit}&offset={global_offset}&sort={sort_order}"
-        self.two_factor = f"https://onlyfans.com/api2/v2/users/otp/check"
+        self.subscription_count = f"{full_url_path}/subscriptions/count/all"
+        self.socials = f"{full_url_path}/users/{identifier}/social/buttons"
+        self.spotify = f"{full_url_path}/users/{identifier}/social/spotify"
+        self.two_factor = f"{full_url_path}/users/otp/check"
+        self.drm_server = f"{full_url_path}/users/media/{identifier}/drm/{identifier2}/{identifier3}?type=widevine"
 
     def list_posts(
         self,
         content_id: Optional[int | str],
         global_limit: int = 10,
         global_offset: int = 0,
     ):
@@ -154,29 +174,32 @@
         global_limit: int = 10,
         global_offset: int = 0,
         sort_order: Literal["asc", "desc"] = "desc",
     ):
         content_type = f"{content_type}s" if content_type[0] != "s" else content_type
         return f"{self.full_url_path}/{content_type}/{content_id}/comments?limit={global_limit}&offset={global_offset}&sort={sort_order}"
 
-    def create_links(self, link: str, api_count: int, limit: int = 10, offset: int = 0):
+    def create_links(self, url: str, api_count: int, limit: int = 10, offset: int = 0):
         """
         This function will create a list of links depending on their content count.
 
         Example:\n
-        create_links(link="base_link", api_count=50) will return a list with 5 links.
+        create_links(link="base_link", api_count=50) will return a list with 5 links if limit=10.
         """
         final_links: list[str] = []
         if api_count:
             ceil = math.ceil(api_count / limit)
             numbers = list(range(ceil))
             for num in numbers:
                 num = num * limit
-                link = link.replace(f"limit={limit}", f"limit={limit}")
-                new_link = link.replace(f"offset={offset}", f"offset={num}")
+                parsed_url = urlparse(url)
+                query_params = parse_qs(parsed_url.query)
+                limit_value = query_params["limit"][0]
+                url = url.replace(f"limit={limit_value}", f"limit={limit}")
+                new_link = url.replace(f"offset={offset}", f"offset={num}")
                 final_links.append(new_link)
         return final_links
 
 
 class ErrorDetails:
     def __init__(self, result: dict[str, Any]) -> None:
         error = result["error"] if "error" in result else result
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/message_model.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/message_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 
 
 class create_message(SiteContent):
     def __init__(self, option: dict[str, Any], user: create_user) -> None:
 
-        author = user.get_authed().find_user_by_identifier(option["fromUser"]["id"])[0]
+        author = user.get_authed().find_user_by_identifier(option["fromUser"]["id"])
+        self.user = user
         SiteContent.__init__(self, option, author)
         self.responseType: Optional[str] = option.get("responseType")
-        self.text: str = option.get("text","")
+        self.text: str = option.get("text", "")
         self.lockedText: Optional[bool] = option.get("lockedText")
         self.isFree: Optional[bool] = option.get("isFree")
         self.price: Optional[float] = option.get("price")
         self.isMediaReady: Optional[bool] = option.get("isMediaReady")
         self.mediaCount: Optional[int] = option.get("mediaCount")
         self.media: list[dict[str, Any]] = option.get("media", [])
         self.previews: list[dict[str, Any]] = option.get("previews", [])
@@ -34,18 +35,25 @@
         self.createdAt: Optional[str] = option.get("createdAt")
         self.changedAt: Optional[str] = option.get("changedAt")
         self.cancelSeconds: Optional[int] = option.get("cancelSeconds")
         self.isLiked: Optional[bool] = option.get("isLiked")
         self.canPurchase: Optional[bool] = option.get("canPurchase")
         self.canPurchaseReason: Optional[str] = option.get("canPurchaseReason")
         self.canReport: Optional[bool] = option.get("canReport")
+        self.__raw__ = option
 
     def get_author(self):
         return self.author
 
+    def get_receiver(self):
+        receiver = (
+            self.author.get_authed() if self.author.id == self.user.id else self.user
+        )
+        return receiver
+
     async def buy_message(self):
         """
         This function will buy a ppv message from a model.
         """
         message_price = self.price
         x = {
             "amount": message_price,
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/post_model.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/story_model.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/classes/user_model.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/user_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,27 +59,27 @@
         self.joinDate: str = option.get("joinDate")
         self.isReferrerAllowed: bool = option.get("isReferrerAllowed")
         self.about: str = option.get("about")
         self.rawAbout: str = option.get("rawAbout")
         self.website: str = option.get("website")
         self.wishlist: str = option.get("wishlist")
         self.location: str = option.get("location")
-        self.postsCount: int = option.get("postsCount")
-        self.archivedPostsCount: int = option.get("archivedPostsCount")
-        self.photosCount: int = option.get("photosCount")
-        self.videosCount: int = option.get("videosCount")
-        self.audiosCount: int = option.get("audiosCount")
-        self.mediasCount: int = option.get("mediasCount")
+        self.postsCount: int = option.get("postsCount", 0)
+        self.archivedPostsCount: int = option.get("archivedPostsCount", 0)
+        self.photosCount: int = option.get("photosCount", 0)
+        self.videosCount: int = option.get("videosCount", 0)
+        self.audiosCount: int = option.get("audiosCount", 0)
+        self.mediasCount: int = option.get("mediasCount", 0)
         self.promotions: list[dict[str, Any]] = option.get("promotions", {})
         self.lastSeen: Any = option.get("lastSeen")
-        self.favoritesCount: int = option.get("favoritesCount")
-        self.favoritedCount: int = option.get("favoritedCount")
+        self.favoritesCount: int = option.get("favoritesCount", 0)
+        self.favoritedCount: int = option.get("favoritedCount", 0)
         self.showPostsInFeed: bool = option.get("showPostsInFeed")
         self.canReceiveChatMessage: bool = option.get("canReceiveChatMessage")
-        self.isPerformer: bool = option.get("isPerformer")
+        self.isPerformer: bool = option.get("isPerformer", False)
         self.isRealPerformer: bool = option.get("isRealPerformer")
         self.isSpotifyConnected: bool = option.get("isSpotifyConnected")
         self.subscribersCount: int = option.get("subscribersCount")
         self.hasPinnedPosts: bool = option.get("hasPinnedPosts")
         self.canChat: bool = option.get("canChat")
         self.callPrice: int = option.get("callPrice")
         self.isPrivateRestriction: bool = option.get("isPrivateRestriction")
@@ -285,27 +285,27 @@
             if not isinstance(result, error_types):
                 final_results = [create_story(x, self) for x in result["stories"]]
         return final_results
 
     async def get_posts(
         self,
         links: Optional[list[str]] = None,
-        limit: int = 10,
+        limit: int = 50,
         offset: int = 0,
         refresh: bool = True,
     ) -> list[create_post]:
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         if links is None:
             links = []
         if not links:
             epl = endpoint_links()
             link = epl.list_posts(self.id)
-            links = epl.create_links(link, self.postsCount)
+            links = epl.create_links(link, self.postsCount, limit=limit)
         results = await self.scrape_manager.bulk_scrape(links)
         final_results = self.finalize_content_set(results)
         self.scrape_manager.scraped.Posts = final_results
         return final_results
 
     async def get_post(
         self, identifier: Optional[int | str] = None, limit: int = 10, offset: int = 0
@@ -359,18 +359,23 @@
                 results2 = await self.get_messages(
                     limit=temp_limit,
                     offset=new_offset,
                     depth=depth + 1,
                 )
                 final_results.extend(results2)
             if depth == 1:
+                if len(final_results) > 1:
+                    last_link = f"{link}&id={final_results[-1]['id']}"
+                    first_message = await self.get_session_manager().json_request(
+                        last_link
+                    )
+                    final_results.extend(first_message["list"])
                 final_results = [
                     message_model.create_message(x, self) for x in final_results if x
                 ]
-                pass
             else:
                 final_results.sort(key=lambda x: x["fromUser"]["id"], reverse=True)
             self.scrape_manager.scraped.Messages = final_results
         return final_results
 
     async def get_message_by_id(
         self,
@@ -497,14 +502,17 @@
         if self.promotions:
             for promotion in self.promotions:
                 promotion_price: int = promotion["price"]
                 if promotion_price < subscription_price:
                     subscription_price = promotion_price
         return subscription_price
 
+    async def get_promotions(self):
+        return self.promotions
+
     async def buy_subscription(self):
         """
         This function will subscribe to a model. If the model has a promotion available, it will use it.
         """
         subscription_price = await self.subscription_price()
         x: dict[str, Any] = {
             "paymentType": "subscribe",
@@ -562,7 +570,51 @@
         return self.avatar
 
     async def get_header(self):
         return self.header
 
     async def is_subscribed(self):
         return not self.subscribedIsExpiredNow
+
+    async def get_paid_contents(self):
+        # REMINDER THAT YOU'LL HAVE TO REFRESH CONTENT
+        final_paid_content: list[create_post | message_model.create_message] = []
+        authed = self.get_authed()
+        for paid_content in authed.paid_content:
+            if paid_content.author.id == self.id:
+                final_paid_content.append(paid_content)
+        return final_paid_content
+
+    async def has_socials(self):
+        # If error message, this means the user has socials, but we have to subscribe to see them
+        result = bool(
+            await self.get_session_manager().json_request(
+                endpoint_links(self.id).socials
+            )
+        )
+        return result
+
+    async def get_socials(self):
+        result = await self.get_session_manager().json_request(
+            endpoint_links(self.id).socials
+        )
+        if "error" in result:
+            return []
+        return result
+
+    async def get_spotify(self):
+        if self.isSpotifyConnected:
+            result = await self.get_session_manager().json_request(
+                endpoint_links(self.id).spotify
+            )
+            if "error" in result:
+                return []
+            return result
+
+    async def has_socials(self):
+        # If error message, this means the user has socials, but we have to subscribe to see them
+        result = bool(
+            await self.get_session_manager().json_request(
+                endpoint_links(self.id).spotify
+            )
+        )
+        return result
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/onlyfans/onlyfans.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/onlyfans.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,39 +8,19 @@
 
 
 class OnlyFansAPI(StreamlinedAPI):
     def __init__(self, config: Config = Config()) -> None:
         self.site_name: Literal["OnlyFans"] = "OnlyFans"
         StreamlinedAPI.__init__(self, self, config)
         self.auths: list[create_auth] = []
-        self.subscriptions: list[create_user] = []
+        self.users: dict[int, create_user] = {}
         self.endpoint_links = endpoint_links
 
-    def add_auth(
-        self, auth_json: dict[str, Any] = {}, only_active: bool = False
-    ) -> create_auth:
-        """Creates and appends an auth object to auths property
-
-        Args:
-            auth_json (dict[str, str], optional): []. Defaults to {}.
-            only_active (bool, optional): [description]. Defaults to False.
-
-        Returns:
-            create_auth: [Auth object]
-        """
-        temp_auth_details = AuthDetails(**auth_json).upgrade_legacy(auth_json)
-        auth = create_auth(
-            self, max_threads=self.max_threads, auth_details=temp_auth_details
-        )
-        if only_active and not auth.auth_details.active:
-            return auth
-        auth.auth_details = temp_auth_details
-        auth.extras["settings"] = self.config
-        self.auths.append(auth)
-        return auth
+    def add_user(self, user: create_auth):
+        self.users[user.id] = user
 
     def get_auth(self, identifier: Union[str, int]) -> Optional[create_auth]:
         final_auth = None
         for auth in self.auths:
             if auth.id == identifier:
                 final_auth = auth
             elif auth.username == identifier:
@@ -58,52 +38,44 @@
         Returns:
             auth_details: [auth_details object]
         """
         return AuthDetails(**auth_json).upgrade_legacy(auth_json)
 
     class ContentTypes:
         def __init__(self) -> None:
-            class ArchivedTypes:
-                def __init__(self) -> None:
-                    self.Posts = []
-
-                def __iter__(self):
-                    for attr, value in self.__dict__.items():
-                        yield attr, value
-
             self.Stories = []
             self.Posts = []
-            # self.Archived = ArchivedTypes()
             self.Chats = []
             self.Messages = []
             self.Highlights = []
             self.MassMessages = []
 
         def __iter__(self):
             for attr, value in self.__dict__.items():
                 yield attr, value
 
         def get_keys(self):
             return [item[0] for item in self]
 
-        async def response_type_to_key(self, value:str):
+        async def response_type_to_key(self, value: str):
             result = [x[0] for x in self if x[0].lower() == f"{value}s"]
             if result:
                 return result[0]
 
     class MediaTypes:
         def __init__(self) -> None:
             self.Images = ["photo"]
             self.Videos = ["video", "stream", "gif"]
             self.Audios = ["audio"]
             self.Texts = ["text"]
 
         def get_keys(self):
             return [item[0] for item in self.__dict__.items()]
-        def find_by_value(self,value:str):
+
+        def find_by_value(self, value: str):
             final_media_type = None
             for media_type, alt_media_types in self.__dict__.items():
                 if value in alt_media_types:
                     final_media_type = media_type
             if not final_media_type:
                 raise Exception("No media type found")
-            return final_media_type
+            return final_media_type
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/apis/user_streamliner.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/user_streamliner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import copy
 from typing import TYPE_CHECKING
 
 import dill
-
 from ultima_scraper_api.managers.job_manager.jobs.custom_job import CustomJob
 
 if TYPE_CHECKING:
     import ultima_scraper_api.apis.fansly.classes as fansly_classes
     import ultima_scraper_api.apis.onlyfans.classes as onlyfans_classes
 
     auth_types = (
@@ -51,14 +50,15 @@
 
 class StreamlinedUser:
     def __init__(self, authed: auth_types) -> None:
         self.__authed = authed
         self.jobs: list[CustomJob] = []
         self.job_whitelist: list[int | str] = []
         self.scrape_whitelist: list[int | str] = []
+        self.active: bool = True
 
     def get_authed(self):
         return self.__authed
 
     def get_job(self, value: str):
         found_jobs = [x for x in self.jobs if x.title == value]
         found_job = None
@@ -89,7 +89,10 @@
         return data_string
 
     def get_session_manager(self):
         return self.__authed.session_manager
 
     def get_api(self):
         return self.__authed.api
+
+    def is_active(self):
+        return self.active
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/classes/make_settings.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/classes/make_settings.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/classes/prepare_directories.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_directories.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/classes/prepare_metadata.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 from typing import TYPE_CHECKING, Any, Optional
 
 import ultima_scraper_api
 from ultima_scraper_api.apis import api_helper
 from ultima_scraper_api.apis.onlyfans.classes.extras import media_types
 from ultima_scraper_api.helpers import main_helper
 
-if TYPE_CHECKING:
-    from ultima_scraper_api.classes.prepare_directories import DirectoryManager
-
-auth_types = ultima_scraper_api.auth_types
-user_types = ultima_scraper_api.user_types
 global_version = 2
 
 # Supports legacy metadata (.json and .db format) and converts it into the latest format (.db)
 class create_metadata(object):
     def __init__(
         self,
         metadata: list[dict[str, Any]] | dict[str, Any] = {},
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/classes/prepare_webhooks.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_webhooks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/docs/Makefile` & `ultima_scraper_api-1.1.0/ultima_scraper_api/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/docs/make.bat` & `ultima_scraper_api-1.1.0/ultima_scraper_api/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/docs/source/conf.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/helpers/main_helper.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/helpers/main_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 import ultima_scraper_api.classes.prepare_webhooks as prepare_webhooks
 
 if TYPE_CHECKING:
     pass
 
 api_types = ultima_scraper_api.api_types
 auth_types = ultima_scraper_api.auth_types
-user_types = ultima_scraper_api.user_types
 
 
 os_name = platform.system()
 
 if os_name == "Windows":
     import ctypes
 
@@ -104,15 +103,15 @@
     if "directories" in merged:
         for directory in merged["directories"]:
             await async_os.makedirs(directory, exist_ok=True)
         merged.pop("directories")
     return merged
 
 
-async def format_image(filepath: Path, timestamp: float, reformat_media: bool):
+async def format_file(filepath: Path, timestamp: float, reformat_media: bool):
     if reformat_media:
         while True:
             if os_name == "Windows":
                 from win32_setctime import setctime
 
                 setctime(filepath, timestamp)
                 # print(f"Updated Creation Time {filepath}")
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/managers/job_manager/job_manager.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/managers/job_manager/job_manager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,8 @@
         while True:
             job = await self.queue.get()
             # We can make jobs work in the background if we make waiting for inputs async
             await job.task
 
             self.queue.task_done()
 
-            # print(f'{job.type} has been processed')
+            # print(f'{job.type} has been processed')
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/managers/job_manager/jobs/custom_job.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/managers/job_manager/jobs/custom_job.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,17 +10,19 @@
         self.api_type = api_type
         self.media_types: list[str] = []
         self.min = 0
         self.task = None
         self.result = []
         self.done = False
         self.options: list[str] = []
-        self.blacklist:list[str] = []
+        self.blacklist: list[str] = []
 
     def add_media_type(self, media_type: str):
+        if media_type in self.media_types:
+            return
         self.media_types.append(media_type)
 
     def convert_to_dill(self):
         old = copy.copy(self)
         delattr(old, "task")
         data_string: bytes = dill.dumps(old)  # type: ignore
         return data_string, old
```

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/managers/scrape_manager.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/managers/scrape_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.0.5/ultima_scraper_api/managers/session_manager.py` & `ultima_scraper_api-1.1.0/ultima_scraper_api/managers/session_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,46 +9,69 @@
 from random import randint
 from typing import TYPE_CHECKING, Any
 from urllib.parse import urlparse
 
 import aiohttp
 import python_socks
 import requests
+import ultima_scraper_api
+import ultima_scraper_api.apis.api_helper as api_helper
 from aiohttp import ClientResponse, ClientSession
 from aiohttp.client_exceptions import (
     ClientConnectorError,
     ClientOSError,
     ClientPayloadError,
     ClientResponseError,
     ContentTypeError,
     ServerDisconnectedError,
 )
-from aiohttp_socks import (
-    ChainProxyConnector,
-    ProxyConnectionError,
-    ProxyError,
-    ProxyInfo,
-)
-
-import ultima_scraper_api
-import ultima_scraper_api.apis.api_helper as api_helper
+from aiohttp_socks import ProxyConnectionError, ProxyConnector, ProxyError, ProxyInfo
 
 if TYPE_CHECKING:
     auth_types = ultima_scraper_api.auth_types
 EXCEPTION_TEMPLATE = (
     ClientPayloadError,
     ContentTypeError,
     ClientOSError,
     ServerDisconnectedError,
     ProxyConnectionError,
     ConnectionResetError,
     asyncio.TimeoutError,
 )
 
 
+class ProxyManager:
+    def __init__(self, session_manager: SessionManager) -> None:
+        self.session_manager = session_manager
+        self.proxies = [
+            ProxyInfo(*python_socks.parse_proxy_url(proxy)) for proxy in self.session_manager.proxies  # type: ignore
+        ]
+        self.current_proxy_index = 0
+
+    def create_connection(self, proxy: ProxyInfo | None = None):
+        if proxy is None:
+            proxy = self.proxies[0]
+        return ProxyConnector(**proxy._asdict())  # type: ignore
+
+    def get_current_proxy(self):
+        return self.proxies[self.current_proxy_index]
+
+    async def proxy_switcher(self):
+        if self.proxies:
+            self.current_proxy_index = (self.current_proxy_index + 1) % len(
+                self.proxies
+            )
+            await self.session_manager.active_session.close()
+            self.session_manager.active_session = (
+                self.session_manager.create_client_session(
+                    False, self.get_current_proxy()
+                )
+            )
+
+
 class SessionManager:
     def __init__(
         self,
         auth: auth_types,
         headers: dict[str, Any] = {},
         proxies: list[str] = [],
         max_threads: int = -1,
@@ -56,15 +79,18 @@
     ) -> None:
         max_threads = api_helper.calculate_max_threads(max_threads)
         self.semaphore = asyncio.BoundedSemaphore(max_threads)
         self.max_threads = max_threads
         self.max_attempts = 10
         self.kill = False
         self.headers = headers
-        self.proxies: list[str] = proxies
+        self.proxies: list[str] = (
+            proxies if proxies else auth.api.config.settings.proxies
+        )
+        self.proxy_manager = ProxyManager(self)
         global_settings = auth.api.get_global_settings()
         dynamic_rules_link = (
             global_settings.dynamic_rules_link if global_settings else ""
         )
         dr_link = dynamic_rules_link
         dynamic_rules = requests.get(dr_link).json()  # type: ignore
         self.dynamic_rules = dynamic_rules
@@ -76,51 +102,49 @@
         # self.rate_limit_wait_minutes = 6
         self.rate_limit_check = False
         self.is_rate_limited = None
         self.time2sleep = 0
         asyncio.create_task(self.check_rate_limit())
 
     def get_cookies(self):
-
         import ultima_scraper_api.apis.fansly.classes as fansly_classes
 
         if isinstance(self.auth, fansly_classes.auth_model.create_auth):
             final_cookies: dict[str, Any] = {}
         else:
             final_cookies = self.auth.auth_details.cookie.format()
         return final_cookies
 
     def test_proxies(self, proxies: list[str] = []):
-
         final_proxies: list[str] = []
+
+        session = requests.Session()
         proxies = proxies if proxies else self.proxies
         for proxy in proxies:
             url = "https://checkip.amazonaws.com"
             temp_proxies = {"https": proxy}
             try:
-                resp = requests.get(url, proxies=temp_proxies)
+                resp = session.get(url, proxies=temp_proxies)
                 ip = resp.text
                 ip = ip.strip()
                 final_proxies.append(proxy)
             except Exception as _e:
                 continue
         return final_proxies
 
-    def create_client_session(self, test_proxies: bool = True):
+    def create_client_session(
+        self, test_proxies: bool = True, proxy: ProxyInfo | None = None
+    ):
         limit = 0
         if test_proxies and self.proxies:
             self.proxies = self.test_proxies()
             if not self.proxies:
                 raise Exception("Unable to create session due to invalid proxies")
-        proxies = [
-            ProxyInfo(*python_socks.parse_proxy_url(proxy)) for proxy in self.proxies  # type: ignore
-        ]
-
         connector = (
-            ChainProxyConnector(proxies, limit=limit)
+            self.proxy_manager.create_connection(proxy)
             if self.proxies
             else aiohttp.TCPConnector(limit=limit)
         )
         final_cookies = self.get_cookies()
         # Had to remove final_cookies and cookies=final_cookies due to it conflicting with headers
         client_session = ClientSession(
             connector=connector,
@@ -162,14 +186,18 @@
             while self.rate_limit_check:
                 async with lock:
                     try:
                         url = "https://onlyfans.com/api2/v2/init"
                         headers = await self.session_rules(url)
                         headers["accept"] = "application/json, text/plain, */*"
                         headers["Connection"] = "keep-alive"
+                        proxy_manager = self.proxy_manager
+                        if proxy_manager.proxies:
+                            await proxy_manager.proxy_switcher()
+                            print(proxy_manager.get_current_proxy().host)
 
                         result = await self.active_session.get(url, headers=headers)
                         result.raise_for_status()
                         self.rate_limit_check = False
                         self.is_rate_limited = None
                         break
                     except ClientResponseError as _e:
@@ -178,42 +206,60 @@
                             self.is_rate_limited = True
                             rate_limit_count += 1
                     except Exception as _e:
                         pass
                 await asyncio.sleep(self.time2sleep)
             await asyncio.sleep(5)
 
-    async def request(self, url: str, premade_settings: str = "json"):
+    async def request(
+        self,
+        url: str,
+        method: str = "GET",
+        data: Any = {},
+        premade_settings: str = "json",
+        custom_cookies: str = "",
+    ):
         while True:
             if self.rate_limit_check:
                 await asyncio.sleep(5)
                 continue
             headers = {}
             if premade_settings == "json":
                 headers = await self.session_rules(url)
                 headers["accept"] = "application/json, text/plain, */*"
                 headers["Connection"] = "keep-alive"
+            if custom_cookies:
+                headers = await self.session_rules(url, custom_cookies=custom_cookies)
+                pass
+
             # await self.limit_rate()
             try:
-                result = await self.active_session.get(url, headers=headers)
+                match method.upper():
+                    case "GET":
+                        result = await self.active_session.get(url, headers=headers)
+                    case "POST":
+                        result = await self.active_session.post(
+                            url, headers=headers, data=data
+                        )
             except EXCEPTION_TEMPLATE as _e:
                 continue
             except Exception as _e:
                 continue
             try:
                 result.raise_for_status()
                 return result
             except EXCEPTION_TEMPLATE as _e:
                 # Can retry
                 continue
             except ClientResponseError as _e:
                 match _e.status:
-                    case 403 | 404:
+                    case 400 | 401 | 403 | 404:
                         return result
                     case 429:
+                        pass
                         if self.is_rate_limited is None:
                             self.rate_limit_check = True
                         continue
                     case 500 | 503 | 504:
                         continue
                     case _:
                         raise Exception(
@@ -223,18 +269,22 @@
                 pass
 
     async def bulk_requests(self, urls: list[str]) -> list[ClientResponse | None]:
         return await asyncio.gather(*[self.request(url) for url in urls])
 
     async def json_request(self, url: str):
         response = await self.request(url)
-        json_resp = await response.json()
+        json_resp: dict[Any, Any] = {}
+        if response.status == 200:
+            json_resp = await response.json()
+        else:
+            json_resp["error"] = {"code": response.status, "message": response.reason}
         return json_resp
 
-    async def bulk_json_requests(self, urls: list[str]):
+    async def bulk_json_requests(self, urls: list[str]) -> list[dict[Any, Any]]:
         return await asyncio.gather(*[self.json_request(url) for url in urls])
 
     async def json_request_2(
         self,
         link: str,
         session: ClientSession | None = None,
         method: str = "GET",
@@ -285,15 +335,14 @@
                     if method == "HEAD":
                         result = response
                     else:
                         if json_format and not stream:
                             # qwsd = list(response.request_info.headers.items())
                             result = await response.json()
                             if "error" in result:
-
                                 extras: dict[str, Any] = {}
                                 extras["auth"] = self.auth
                                 extras["link"] = link
                                 if isinstance(
                                     self.auth, onlyfans_classes.auth_model.create_auth
                                 ):
                                     handle_error = onlyfans_classes.extras.ErrorDetails
@@ -322,43 +371,53 @@
                 except Exception as _exception:
                     pass
             if custom_session:
                 await session.close()
             return result
 
     async def session_rules(
-        self, link: str, signed_headers: dict[str, Any] = {}
+        self, link: str, signed_headers: dict[str, Any] = {}, custom_cookies: str = ""
     ) -> dict[str, Any]:
-
         import ultima_scraper_api.apis.fansly.classes as fansly_classes
         import ultima_scraper_api.apis.onlyfans.classes as onlyfans_classes
 
         headers: dict[str, Any] = {}
         headers |= self.headers
-        if "https://onlyfans.com/api2/v2/" in link and isinstance(
-            self.auth.auth_details, onlyfans_classes.extras.AuthDetails
-        ):
-            dynamic_rules = self.dynamic_rules
-            final_cookies = self.auth.auth_details.cookie.convert()
-            headers["app-token"] = dynamic_rules["app_token"]
-            headers["cookie"] = final_cookies
-            if self.auth.guest:
-                headers["x-bc"] = "".join(
-                    random.choice(string.digits + string.ascii_lowercase)
-                    for _ in range(40)
-                )
-            headers2 = self.create_signed_headers(link)
-            headers |= headers2
-            # t2s does not set for cdn links yet
-            self.time2sleep = 5
-        elif "https://apiv3.fansly.com" in link and isinstance(
-            self.auth.auth_details, fansly_classes.extras.AuthDetails
-        ):
-            headers["authorization"] = self.auth.auth_details.authorization
-            self.is_rate_limited = False
+        match self.auth.auth_details.__class__:
+            case onlyfans_classes.extras.AuthDetails:
+                if "https://onlyfans.com/api2/v2/" in link:
+                    dynamic_rules = self.dynamic_rules
+                    final_cookies = self.auth.auth_details.cookie.convert()
+                    headers["app-token"] = dynamic_rules["app_token"]
+                    headers["cookie"] = final_cookies
+                    if self.auth.guest:
+                        headers["x-bc"] = "".join(
+                            random.choice(string.digits + string.ascii_lowercase)
+                            for _ in range(40)
+                        )
+                    headers2 = self.create_signed_headers(link)
+                    headers |= headers2
+                    # t2s does not set for cdn links yet
+                    self.time2sleep = 5
+                elif ".mpd" in link:
+                    headers["cookie"] = custom_cookies
+                else:
+                    if "/files/" not in link:
+                        pass
+                    dynamic_rules = self.dynamic_rules
+                    final_cookies = (
+                        self.auth.auth_details.cookie.convert() + custom_cookies
+                    )
+                    headers["cookie"] = final_cookies
+            case fansly_classes.extras.AuthDetails:
+                if "https://apiv3.fansly.com" in link:
+                    headers["authorization"] = self.auth.auth_details.authorization
+                    self.is_rate_limited = False
+            case _:
+                pass
         return headers
 
     def create_signed_headers(
         self, link: str, auth_id: int = 0, time_: int | None = None
     ):
         # Users: 300000 | Creators: 301000
         headers: dict[str, Any] = {}
```

### Comparing `ultima_scraper_api-1.0.5/PKG-INFO` & `ultima_scraper_api-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-api
-Version: 1.0.5
+Version: 1.1.0
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Sphinx (>=5.3.0,<6.0.0)
 Requires-Dist: aiofiles (>=22.1.0,<23.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: aiohttp-socks (>=0.7.1,<0.8.0)
+Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: mypy (>=0.991,<0.992)
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-socks[asyncio] (==2.2.0)
+Requires-Dist: pywidevine (>=1.6.0,<2.0.0)
 Requires-Dist: requests[socks] (==2.28.2)
-Requires-Dist: sphinx-autoapi (>=2.0.0,<3.0.0)
-Requires-Dist: sphinx-rtd-theme (>=1.1.1,<2.0.0)
 Requires-Dist: user-agent (>=0.1.10,<0.2.0)
-Requires-Dist: win32-setctime (>=1.1.0,<2.0.0); sys_platform == "win32"
+Requires-Dist: win32-setctime (>=1.1.0,<2.0.0) ; sys_platform == "win32"
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
```

