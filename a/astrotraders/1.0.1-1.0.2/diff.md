# Comparing `tmp/astrotraders-1.0.1.tar.gz` & `tmp/astrotraders-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrotraders-1.0.1.tar", max compression
+gzip compressed data, was "astrotraders-1.0.2.tar", max compression
```

## Comparing `astrotraders-1.0.1.tar` & `astrotraders-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      917 2023-05-13 12:25:45.027449 astrotraders-1.0.1/README.md
--rw-r--r--   0        0        0       55 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/__init__.py
--rw-r--r--   0        0        0        0 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/__init__.py
--rw-r--r--   0        0        0     1181 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/client.py
--rw-r--r--   0        0        0      670 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/exceptions.py
--rw-r--r--   0        0        0      185 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/resources/__init__.py
--rw-r--r--   0        0        0      317 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/resources/agents.py
--rw-r--r--   0        0        0      160 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/resources/base.py
--rw-r--r--   0        0        0     1776 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/resources/contracts.py
--rw-r--r--   0        0        0      682 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/resources/factions.py
--rw-r--r--   0        0        0    11413 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/resources/fleet.py
--rw-r--r--   0        0        0     3227 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/resources/systems.py
--rw-r--r--   0        0        0    37202 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/schemas.py
--rw-r--r--   0        0        0      509 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/utils.py
--rw-r--r--   0        0        0     3020 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/api/wrapper.py
--rw-r--r--   0        0        0        0 2023-05-13 12:25:45.027449 astrotraders-1.0.1/astrotraders/py.typed
--rw-r--r--   0        0        0     1146 2023-05-13 12:25:45.027449 astrotraders-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 astrotraders-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1017 2023-05-14 00:18:14.619624 astrotraders-1.0.2/README.md
+-rw-r--r--   0        0        0       55 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/__init__.py
+-rw-r--r--   0        0        0     2668 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/client.py
+-rw-r--r--   0        0        0      698 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/exceptions.py
+-rw-r--r--   0        0        0      220 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/resources/__init__.py
+-rw-r--r--   0        0        0      317 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/resources/agents.py
+-rw-r--r--   0        0        0      160 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/resources/base.py
+-rw-r--r--   0        0        0     1776 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/resources/contracts.py
+-rw-r--r--   0        0        0      682 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/resources/factions.py
+-rw-r--r--   0        0        0    11413 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/resources/fleet.py
+-rw-r--r--   0        0        0      424 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/resources/server.py
+-rw-r--r--   0        0        0     3525 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/resources/systems.py
+-rw-r--r--   0        0        0    37913 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/schemas.py
+-rw-r--r--   0        0        0      509 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/utils.py
+-rw-r--r--   0        0        0     3039 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/api/wrapper.py
+-rw-r--r--   0        0        0        0 2023-05-14 00:18:14.619624 astrotraders-1.0.2/astrotraders/py.typed
+-rw-r--r--   0        0        0     1146 2023-05-14 00:18:14.619624 astrotraders-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1835 1970-01-01 00:00:00.000000 astrotraders-1.0.2/PKG-INFO
```

### Comparing `astrotraders-1.0.1/README.md` & `astrotraders-1.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -25,12 +25,15 @@
 After initializing client you can use API resources, for example:
 
 ```python
 agent = client.agents.info()
 systems = client.systems.list()
 contracts = client.contracts.list()
 factions = client.factions.list()
+# you can use undocumented endpoints!
+stats = client.server.stats()
+universe = client.systems.all()
 ```
 
 ## TODO
 1. "Game objects" with data caching and more pythonic usage
 2. CLI tool for manage fleet (and as example)
```

### Comparing `astrotraders-1.0.1/astrotraders/api/resources/contracts.py` & `astrotraders-1.0.2/astrotraders/api/resources/contracts.py`

 * *Files identical despite different names*

### Comparing `astrotraders-1.0.1/astrotraders/api/resources/factions.py` & `astrotraders-1.0.2/astrotraders/api/resources/factions.py`

 * *Files identical despite different names*

### Comparing `astrotraders-1.0.1/astrotraders/api/resources/fleet.py` & `astrotraders-1.0.2/astrotraders/api/resources/fleet.py`

 * *Files identical despite different names*

### Comparing `astrotraders-1.0.1/astrotraders/api/resources/systems.py` & `astrotraders-1.0.2/astrotraders/api/resources/systems.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List, cast
+
 from astrotraders.api.resources.base import BaseResource
 from astrotraders.api.schemas import (
     PaginatedObject,
     System,
     Waypoint,
     Market,
     Shipyard,
@@ -28,14 +30,21 @@
 
     def get(self, name: str) -> System:
         """
         Get the details of a system.
         """
         return self._client.request_to_model("GET", f"/systems/{name}", System)
 
+    def all(self) -> List[System]:
+        """
+        Get all systems with waypoints from undocumented endpoint
+        """
+        systems = cast(list[dict], self._client.raw_request("GET", "/systems.json"))
+        return [System(**system) for system in systems]
+
 
 class WaypointsResource(BaseResource):
     def list(
         self, system: str, limit: int = 20, page: int = 1
     ) -> PaginatedObject[Waypoint]:
         """
         Fetch all waypoints for a given system.
```

### Comparing `astrotraders-1.0.1/astrotraders/api/schemas.py` & `astrotraders-1.0.2/astrotraders/api/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1284,7 +1284,37 @@
     token: str = Field(
         ..., description="A Bearer token for accessing secured API endpoints."
     )
 
 
 class RegisterResponse(BaseModel):
     data: RegisterData
+
+
+class ServerStats(BaseModel):
+    agents: int
+    ships: int
+    systems: int
+    waypoints: int
+
+
+class LeaderboardsCreditTopItem(BaseModel):
+    agent: NonEmptyStr = Field(alias="agentSymbol")
+    credits: int
+
+
+class LeaderboardsSubmittedChartsTopItem(BaseModel):
+    agent: NonEmptyStr = Field(alias="agentSymbol")
+    chart_count: int = Field(alias="chartCount")
+
+
+class Leaderboards(BaseModel):
+    most_credits: list[LeaderboardsCreditTopItem] = Field(alias="mostCredits")
+    most_submitted_charts: list[LeaderboardsSubmittedChartsTopItem] = Field(
+        alias="mostSubmittedCharts"
+    )
+
+
+class ServerStatsResponse(BaseModel):
+    status: str
+    stats: ServerStats
+    leaderboards: Leaderboards
```

### Comparing `astrotraders-1.0.1/astrotraders/api/wrapper.py` & `astrotraders-1.0.2/astrotraders/api/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 class HttpxClientWrapper:
     def __init__(self, client: "Client"):
         self._client = client
 
     def raw_request(
         self, method: str, uri: str, **params: Unpack["HttpxRequestParams"]
-    ) -> Optional[dict[Any, Any]]:
+    ) -> Optional[Union[dict[Any, Any], list[dict]]]:
         # because httpx doesn't have default way to change json encoder
         if json_obj := params.get("json"):
             # it works as well with bytes
             params["data"] = orjson.dumps(json_obj)  # type: ignore[typeddict-item]
             params["headers"] = {"Content-Type": "application/json"}
             del params["json"]
         result = self._client.request(method, uri, **params)
```

### Comparing `astrotraders-1.0.1/pyproject.toml` & `astrotraders-1.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "astrotraders"
-version = "1.0.1"
+version = "1.0.2"
 description = "A typed, handwrited and powerful spacetraders API wrapper"
 authors = ["kiriharu <me@kiriha.ru>"]
 readme = "README.md"
 keywords = ["spacetraders", "spacetraders.io"]
 packages = [{include = "astrotraders"}]
 homepage = "https://github.com/kiriharu/astrotraders"
 repository = "https://github.com/kiriharu/astrotraders"
```

### Comparing `astrotraders-1.0.1/PKG-INFO` & `astrotraders-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrotraders
-Version: 1.0.1
+Version: 1.0.2
 Summary: A typed, handwrited and powerful spacetraders API wrapper
 Home-page: https://github.com/kiriharu/astrotraders
 Keywords: spacetraders,spacetraders.io
 Author: kiriharu
 Author-email: me@kiriha.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
@@ -47,13 +47,16 @@
 After initializing client you can use API resources, for example:
 
 ```python
 agent = client.agents.info()
 systems = client.systems.list()
 contracts = client.contracts.list()
 factions = client.factions.list()
+# you can use undocumented endpoints!
+stats = client.server.stats()
+universe = client.systems.all()
 ```
 
 ## TODO
 1. "Game objects" with data caching and more pythonic usage
 2. CLI tool for manage fleet (and as example)
```

