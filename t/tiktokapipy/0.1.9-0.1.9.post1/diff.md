# Comparing `tmp/tiktokapipy-0.1.9.tar.gz` & `tmp/tiktokapipy-0.1.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktokapipy-0.1.9.tar", last modified: Thu Jan 12 02:26:46 2023, max compression
+gzip compressed data, was "tiktokapipy-0.1.9.post1.tar", last modified: Thu Jan 12 02:35:52 2023, max compression
```

## Comparing `tiktokapipy-0.1.9.tar` & `tiktokapipy-0.1.9.post1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:26:46.461314 tiktokapipy-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-12 02:26:36.000000 tiktokapipy-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-01-12 02:26:46.461314 tiktokapipy-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-01-12 02:26:36.000000 tiktokapipy-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-01-12 02:26:36.000000 tiktokapipy-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 02:26:46.461314 tiktokapipy-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:26:46.461314 tiktokapipy-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:26:46.461314 tiktokapipy-0.1.9/src/tiktokapipy/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-12 02:26:36.000000 tiktokapipy-0.1.9/src/tiktokapipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-01-12 02:26:36.000000 tiktokapipy-0.1.9/src/tiktokapipy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-01-12 02:26:36.000000 tiktokapipy-0.1.9/src/tiktokapipy/async_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:26:46.461314 tiktokapipy-0.1.9/src/tiktokapipy/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-01-12 02:26:36.000000 tiktokapipy-0.1.9/src/tiktokapipy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-01-12 02:26:36.000000 tiktokapipy-0.1.9/src/tiktokapipy/models/challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-01-12 02:26:36.000000 tiktokapipy-0.1.9/src/tiktokapipy/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-01-12 02:26:36.000000 tiktokapipy-0.1.9/src/tiktokapipy/models/raw_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-01-12 02:26:36.000000 tiktokapipy-0.1.9/src/tiktokapipy/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-01-12 02:26:36.000000 tiktokapipy-0.1.9/src/tiktokapipy/models/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:26:46.461314 tiktokapipy-0.1.9/src/tiktokapipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-01-12 02:26:46.000000 tiktokapipy-0.1.9/src/tiktokapipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-01-12 02:26:46.000000 tiktokapipy-0.1.9/src/tiktokapipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 02:26:46.000000 tiktokapipy-0.1.9/src/tiktokapipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-12 02:26:46.000000 tiktokapipy-0.1.9/src/tiktokapipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-12 02:26:46.000000 tiktokapipy-0.1.9/src/tiktokapipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:35:52.334649 tiktokapipy-0.1.9.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-01-12 02:35:52.330649 tiktokapipy-0.1.9.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 02:35:52.334649 tiktokapipy-0.1.9.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:35:52.330649 tiktokapipy-0.1.9.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:35:52.330649 tiktokapipy-0.1.9.post1/src/tiktokapipy/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17476 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/async_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:35:52.330649 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/raw_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-01-12 02:35:40.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy/models/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 02:35:52.330649 tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-01-12 02:35:52.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-01-12 02:35:52.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 02:35:52.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-12 02:35:52.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-12 02:35:52.000000 tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/top_level.txt
```

### Comparing `tiktokapipy-0.1.9/LICENSE` & `tiktokapipy-0.1.9.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.1.9/PKG-INFO` & `tiktokapipy-0.1.9.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktokapipy
-Version: 0.1.9
+Version: 0.1.9.post1
 Summary: Asyncio TikTok data scraping tool
 Author-email: Russell Newton <russell.newton01@gmail.com>
 Project-URL: Homepage, https://github.com/Russell-Newton/TikTokPy
 Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok scraper,asyncio,playwright-python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: tiktokapipy Version: 0.1.9 Summary: Asyncio TikTok
-data scraping tool Author-email: Russell Newton
+Metadata-Version: 2.1 Name: tiktokapipy Version: 0.1.9.post1 Summary: Asyncio
+TikTok data scraping tool Author-email: Russell Newton
 newton01@gmail.com> Project-URL: Homepage, https://github.com/Russell-Newton/
 TikTokPy Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok
 scraper,asyncio,playwright-python Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tiktokapipy-0.1.9/README.md` & `tiktokapipy-0.1.9.post1/README.md`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.1.9/pyproject.toml` & `tiktokapipy-0.1.9.post1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tiktokapipy"
-version = "0.1.9"
+version = "0.1.9.post1"
 authors = [
     { name="Russell Newton", email="russell.newton01@gmail.com" },
 ]
 description = "Asyncio TikTok data scraping tool"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `tiktokapipy-0.1.9/src/tiktokapipy/api.py` & `tiktokapipy-0.1.9.post1/src/tiktokapipy/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,16 +150,18 @@
         :param scroll_down_time: How much time (in seconds) should the page navigation include scrolling down. This can
             load more content from the page.
         :param headless: Whether to use headless browsing.
         :param data_dump_file: If the data scraped from TikTok should also be dumped to a JSON file before parsing,
             specify the name of the dump file (exluding '.json').
         :param emulate_mobile: Whether to emulate a mobile device during sraping. Required for retrieving data
             on slideshows.
-        :param navigator_type: Whether to launch Playwright with 'Chromium' or 'Firefox'
-            Note: 'Chromium' seems to make collecting comments on :ref:`Video`s impossible.
+        :param navigator_type: Whether to launch Playwright with 'Chromium' or 'Firefox'.
+            'Firefox' is incompatible with ``emulate_mobile=True``.
+            Note: 'Chromium' seems to make collecting comments on :ref:`Video`s impossible. Comments can't be collected
+            in mobile.
         :param navigation_timeout: How long (in milliseconds) page navigation should wait before timing out. Set to 0 to
             disable the timeout.
         :param navigation_retries: How many times to retry navigation if ``network_timeout`` is exceeded. Set to 0 to
             not retry navigation.
         :param context_kwargs: Any extra kwargs used to initialize the playwright browser context. For full details,
             see `Browser::new_context() <https://playwright.dev/python/docs/api/class-browser#browser-new-context>`_.
         :param kwargs: Any extra kwargs used to initialize the playwright browser (e.g.: proxy, etc.).
@@ -167,15 +169,15 @@
             `BrowserType::launch() <https://playwright.dev/python/docs/api/class-browsertype#browser-type-launch>`_.
         """
         self.scroll_down_time = scroll_down_time
         self.headless = headless
         self.data_dump_file = data_dump_file
         self.emulate_mobile = emulate_mobile
         self.context_kwargs = context_kwargs or {}
-        self.navigator_type = navigator_type
+        self.navigator_type = navigator_type if not emulate_mobile else "chromium"
         self.navigation_timeout = navigation_timeout * 1000
         self.navigation_retries = navigation_retries
 
     def __enter__(self) -> TikTokAPI:
         self._playwright = sync_playwright().start()
         if self.navigator_type.lower() == "firefox":
             self._browser = self.playwright.firefox.launch(headless=self.headless)
```

### Comparing `tiktokapipy-0.1.9/src/tiktokapipy/async_api.py` & `tiktokapipy-0.1.9.post1/src/tiktokapipy/async_api.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.1.9/src/tiktokapipy/models/__init__.py` & `tiktokapipy-0.1.9.post1/src/tiktokapipy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.1.9/src/tiktokapipy/models/challenge.py` & `tiktokapipy-0.1.9.post1/src/tiktokapipy/models/challenge.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.1.9/src/tiktokapipy/models/comment.py` & `tiktokapipy-0.1.9.post1/src/tiktokapipy/models/comment.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.1.9/src/tiktokapipy/models/raw_data.py` & `tiktokapipy-0.1.9.post1/src/tiktokapipy/models/raw_data.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.1.9/src/tiktokapipy/models/user.py` & `tiktokapipy-0.1.9.post1/src/tiktokapipy/models/user.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.1.9/src/tiktokapipy/models/video.py` & `tiktokapipy-0.1.9.post1/src/tiktokapipy/models/video.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.1.9/src/tiktokapipy.egg-info/PKG-INFO` & `tiktokapipy-0.1.9.post1/src/tiktokapipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktokapipy
-Version: 0.1.9
+Version: 0.1.9.post1
 Summary: Asyncio TikTok data scraping tool
 Author-email: Russell Newton <russell.newton01@gmail.com>
 Project-URL: Homepage, https://github.com/Russell-Newton/TikTokPy
 Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok scraper,asyncio,playwright-python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: tiktokapipy Version: 0.1.9 Summary: Asyncio TikTok
-data scraping tool Author-email: Russell Newton
+Metadata-Version: 2.1 Name: tiktokapipy Version: 0.1.9.post1 Summary: Asyncio
+TikTok data scraping tool Author-email: Russell Newton
 newton01@gmail.com> Project-URL: Homepage, https://github.com/Russell-Newton/
 TikTokPy Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok
 scraper,asyncio,playwright-python Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
```

