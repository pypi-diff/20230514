# Comparing `tmp/pymediatracker-0.1.0.tar.gz` & `tmp/pymediatracker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymediatracker-0.1.0.tar", max compression
+gzip compressed data, was "pymediatracker-0.1.1.tar", max compression
```

## Comparing `pymediatracker-0.1.0.tar` & `pymediatracker-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      707 2023-05-12 12:02:53.844662 pymediatracker-0.1.0/README.md
--rw-r--r--   0        0        0     3483 2023-05-12 12:02:53.841328 pymediatracker-0.1.0/pymediatracker/__init__.py
--rw-r--r--   0        0        0     1708 2023-05-12 12:02:53.841328 pymediatracker-0.1.0/pymediatracker/client.py
--rw-r--r--   0        0        0       46 2023-05-12 12:02:53.841328 pymediatracker-0.1.0/pymediatracker/const.py
--rw-r--r--   0        0        0      117 2023-05-12 12:02:53.841328 pymediatracker-0.1.0/pymediatracker/exceptions.py
--rw-r--r--   0        0        0       28 2023-05-12 12:02:53.844662 pymediatracker-0.1.0/pymediatracker/objects/__init__.py
--rw-r--r--   0        0        0      495 2023-05-12 12:02:53.844662 pymediatracker-0.1.0/pymediatracker/objects/base.py
--rw-r--r--   0        0        0     1777 2023-05-12 12:02:53.841328 pymediatracker-0.1.0/pymediatracker/objects/calendar.py
--rw-r--r--   0        0        0     1077 2023-05-12 12:02:53.844662 pymediatracker-0.1.0/pymediatracker/objects/config.py
--rw-r--r--   0        0        0    50070 2023-05-12 12:02:53.844662 pymediatracker-0.1.0/pymediatracker/objects/item.py
--rw-r--r--   0        0        0      742 2023-05-12 12:02:53.844662 pymediatracker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1548 1970-01-01 00:00:00.000000 pymediatracker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      707 2023-05-14 14:41:59.444552 pymediatracker-0.1.1/README.md
+-rw-r--r--   0        0        0     3541 2023-05-14 14:41:59.431218 pymediatracker-0.1.1/pymediatracker/__init__.py
+-rw-r--r--   0        0        0     1708 2023-05-14 14:41:59.431218 pymediatracker-0.1.1/pymediatracker/client.py
+-rw-r--r--   0        0        0       46 2023-05-14 14:41:59.431218 pymediatracker-0.1.1/pymediatracker/const.py
+-rw-r--r--   0        0        0      117 2023-05-14 14:41:59.431218 pymediatracker-0.1.1/pymediatracker/exceptions.py
+-rw-r--r--   0        0        0       28 2023-05-14 14:41:59.444552 pymediatracker-0.1.1/pymediatracker/objects/__init__.py
+-rw-r--r--   0        0        0      495 2023-05-14 14:41:59.444552 pymediatracker-0.1.1/pymediatracker/objects/base.py
+-rw-r--r--   0        0        0     1777 2023-05-14 14:41:59.444552 pymediatracker-0.1.1/pymediatracker/objects/calendar.py
+-rw-r--r--   0        0        0     1077 2023-05-14 14:41:59.444552 pymediatracker-0.1.1/pymediatracker/objects/config.py
+-rw-r--r--   0        0        0    50070 2023-05-14 14:41:59.444552 pymediatracker-0.1.1/pymediatracker/objects/item.py
+-rw-r--r--   0        0        0      742 2023-05-14 14:41:59.444552 pymediatracker-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1548 1970-01-01 00:00:00.000000 pymediatracker-0.1.1/PKG-INFO
```

### Comparing `pymediatracker-0.1.0/README.md` & `pymediatracker-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pymediatracker-0.1.0/pymediatracker/__init__.py` & `pymediatracker-0.1.1/pymediatracker/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,16 +18,19 @@
 
     def __init__(self, client: "MediaTrackerClient", host: str, token: str) -> None:
         """Initialize the appliance."""
         self._client = client
         self._host = host
         self._token = token
         self._config = MediaTrackerConfig
-        self._items: List[MediaTrackerItem] = []
-        self._calendar: List[MediaTrackerCalendar] = []
+        self._item: List[MediaTrackerItem] = []
+        self._item_dict: dict = {}
+        self._calendar_items: List[MediaTrackerCalendar] = []
+        self._calendar_items_dict: dict = {}
+
         self._entities = [
             {
                 "key": "audiobook",
                 "name": "Audiobooks",
             },
             {
                 "key": "book",
@@ -52,68 +55,72 @@
         return self._host
 
     @property
     def token(self) -> str:
         return self._token
 
     @property
-    def items(self) -> List[MediaTrackerItem]:
-        return self._items
+    def item(self) -> List[MediaTrackerItem]:
+        return self._item
+
+    @property
+    def calendar_items(self) -> List[MediaTrackerCalendar]:
+        return self._calendar_items
 
     @property
-    def calendar(self) -> List[MediaTrackerCalendar]:
-        return self._calendar
+    def calendar_items_dict(self) -> dict:
+        return self._calendar_items_dict
 
     @property
     def config(self) -> dict:
         return self._config
 
     @property
     def entities(self) -> dict:
         return self._entities
 
     async def fetch(self) -> None:
-        """Fetch data from MediaTracker."""
+        """Fetch some basic data from MediaTracker."""
         data: dict = {}
         data["config"] = await self.get_config()
-        data["items"] = await self.get_items()
         data["entities"] = self.entities
-        data["calendar"] = self.calendar
 
         return data
 
     async def get_config(self) -> MediaTrackerConfig:
-        """Get Config."""
+        """Get MediaTracker Configuration."""
         response: ClientResponse = await self._client.get(
             f"http://{self._host}/api/configuration?token={self._token}"
         )
         json = await response.json()
         self.logger.debug(json)
         config = [MediaTrackerConfig(self._client, json)]
 
         return config
 
-    async def get_items(self) -> MediaTrackerItem:
-        """Get Items."""
+
+    async def get_calendar_items(self, start, end) -> MediaTrackerCalendar:
+        """Get MediaTracker Calendar Items from Date Range."""
         response: ClientResponse = await self._client.get(
-            f"http://{self._host}/api/items?token={self._token}"
+            f"http://{self._host}/api/calendar?start={start}&end={end}&token={self._token}"
         )
         json = await response.json()
         self.logger.debug(json)
 
-        self._items = [MediaTrackerItem(self._client, item) for item in json or []]
-        self._items_dict: dict = {}
-        for item in self._items:
-            self._items_dict[item.id] = item
+        self._calendar_items = [
+            MediaTrackerCalendar(self._client, calendar_item) for calendar_item in json or []
+        ]
+
+        return self._calendar_items
 
-    async def get_by_media_type(self, media_type) -> MediaTrackerItem:
-        """Get Media."""
+
+    async def get_item(self, id) -> MediaTrackerItem:
+        """Get Item."""
         response: ClientResponse = await self._client.get(
-            f"http://{self._host}/api/items?mediaType={media_type}&token={self._token}"
+            f"http://{self._host}/api/details/{id}?token={self._token}"
         )
         json = await response.json()
         self.logger.debug(json)
 
-        self._items = [MediaTrackerItem(self._client, item) for item in json or []]
-        self._items_dict: dict = {}
-        for item in self._items:
-            self._items_dict[item.id] = item
+        self._item = MediaTrackerItem(self._client, json)
+
+        return self._item
```

### Comparing `pymediatracker-0.1.0/pymediatracker/client.py` & `pymediatracker-0.1.1/pymediatracker/client.py`

 * *Files identical despite different names*

### Comparing `pymediatracker-0.1.0/pymediatracker/objects/calendar.py` & `pymediatracker-0.1.1/pymediatracker/objects/calendar.py`

 * *Files identical despite different names*

### Comparing `pymediatracker-0.1.0/pymediatracker/objects/config.py` & `pymediatracker-0.1.1/pymediatracker/objects/config.py`

 * *Files identical despite different names*

### Comparing `pymediatracker-0.1.0/pymediatracker/objects/item.py` & `pymediatracker-0.1.1/pymediatracker/objects/item.py`

 * *Files identical despite different names*

### Comparing `pymediatracker-0.1.0/pyproject.toml` & `pymediatracker-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymediatracker"
-version = "0.1.0"
+version = "0.1.1"
 description = "Asynchronous python client for MediaTracker."
 authors = ["Jon Kristian Nilsen <hello@jonkristian.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jonkristian/pymediatracker"
 repository = "https://github.com/jonkristian/pymediatracker"
 documentation = "https://github.com/jonkristian/pymediatracker"
```

### Comparing `pymediatracker-0.1.0/PKG-INFO` & `pymediatracker-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymediatracker
-Version: 0.1.0
+Version: 0.1.1
 Summary: Asynchronous python client for MediaTracker.
 Home-page: https://github.com/jonkristian/pymediatracker
 License: MIT
 Keywords: mediatracker,api,async,client
 Author: Jon Kristian Nilsen
 Author-email: hello@jonkristian.no
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymediatracker Version: 0.1.0 Summary: Asynchronous
+Metadata-Version: 2.1 Name: pymediatracker Version: 0.1.1 Summary: Asynchronous
 python client for MediaTracker. Home-page: https://github.com/jonkristian/
 pymediatracker License: MIT Keywords: mediatracker,api,async,client Author: Jon
 Kristian Nilsen Author-email: hello@jonkristian.no Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

