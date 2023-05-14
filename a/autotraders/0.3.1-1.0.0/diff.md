# Comparing `tmp/autotraders-0.3.1.tar.gz` & `tmp/autotraders-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-0.3.1.tar", last modified: Fri May 12 22:29:28 2023, max compression
+gzip compressed data, was "autotraders-1.0.0.tar", last modified: Sat May 13 01:48:16 2023, max compression
```

## Comparing `autotraders-0.3.1.tar` & `autotraders-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:29:28.796717 autotraders-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-12 22:29:13.000000 autotraders-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-12 22:29:28.796717 autotraders-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-12 22:29:13.000000 autotraders-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:29:28.792716 autotraders-0.3.1/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 22:29:13.000000 autotraders-0.3.1/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-12 22:29:13.000000 autotraders-0.3.1/autotraders/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-12 22:29:13.000000 autotraders-0.3.1/autotraders/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-12 22:29:13.000000 autotraders-0.3.1/autotraders/faction.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-12 22:29:13.000000 autotraders-0.3.1/autotraders/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-12 22:29:13.000000 autotraders-0.3.1/autotraders/ship.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-12 22:29:13.000000 autotraders-0.3.1/autotraders/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-12 22:29:13.000000 autotraders-0.3.1/autotraders/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 22:29:13.000000 autotraders-0.3.1/autotraders/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-12 22:29:13.000000 autotraders-0.3.1/autotraders/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:29:28.796717 autotraders-0.3.1/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-12 22:29:28.000000 autotraders-0.3.1/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-12 22:29:28.000000 autotraders-0.3.1/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 22:29:28.000000 autotraders-0.3.1/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 22:29:28.000000 autotraders-0.3.1/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-12 22:29:13.000000 autotraders-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 22:29:28.796717 autotraders-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:48:16.935983 autotraders-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-13 01:48:04.000000 autotraders-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-13 01:48:16.935983 autotraders-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-13 01:48:04.000000 autotraders-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:48:16.931983 autotraders-1.0.0/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:48:16.931983 autotraders-1.0.0/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:48:16.935983 autotraders-1.0.0/autotraders/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-13 01:48:04.000000 autotraders-1.0.0/autotraders/waypoint_types/shipyard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:48:16.931983 autotraders-1.0.0/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-13 01:48:16.000000 autotraders-1.0.0/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-13 01:48:16.000000 autotraders-1.0.0/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 01:48:16.000000 autotraders-1.0.0/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-13 01:48:16.000000 autotraders-1.0.0/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-13 01:48:04.000000 autotraders-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 01:48:16.935983 autotraders-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 01:48:16.935983 autotraders-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-13 01:48:04.000000 autotraders-1.0.0/tests/test_util.py
```

### Comparing `autotraders-0.3.1/LICENSE` & `autotraders-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-0.3.1/PKG-INFO` & `autotraders-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 0.3.1
+Version: 1.0.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,28 +14,16 @@
 License-File: LICENSE
 
 # Autotraders
 A spacetraders API focused on automation and ease of use
 ## Usage
 First you need a client, which can be generated 
 ```python
-import requests
-
-
-class BearerAuth(requests.auth.AuthBase):
-    def __init__(self, token):
-        self.token = token
-
-    def __call__(self, r):
-        r.headers["authorization"] = "Bearer " + self.token
-        return r
-
-token = TOKEN_HERE
-s = requests.Session()
-s.auth = BearerAuth(token)
+from autotraders import session
+s = session.get_session("YOUR_TOKEN_HERE")
 ```
 And now you're all set to use they actual API.
 
 ## Ships
 
 ```python
 from autotraders.ship import Ship, get_all_ships
```

### Comparing `autotraders-0.3.1/README.md` & `autotraders-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,14 @@
 # Autotraders
 A spacetraders API focused on automation and ease of use
 ## Usage
 First you need a client, which can be generated 
 ```python
-import requests
-
-
-class BearerAuth(requests.auth.AuthBase):
-    def __init__(self, token):
-        self.token = token
-
-    def __call__(self, r):
-        r.headers["authorization"] = "Bearer " + self.token
-        return r
-
-token = TOKEN_HERE
-s = requests.Session()
-s.auth = BearerAuth(token)
+from autotraders import session
+s = session.get_session("YOUR_TOKEN_HERE")
 ```
 And now you're all set to use they actual API.
 
 ## Ships
 
 ```python
 from autotraders.ship import Ship, get_all_ships
```

### Comparing `autotraders-0.3.1/autotraders/agent.py` & `autotraders-1.0.0/autotraders/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import requests
+
 from autotraders.ship import get_all_ships
 from autotraders.contract import get_all_contracts
 
 
 class Agent:
-    def __init__(self, session, update=True):
+    def __init__(self, session: requests.Session, update=True):
         self.session = session
         if update:
             self.update()
 
     def update(self, data=None):
         if data is None:
             r = self.session.get("https://api.spacetraders.io/v2/my/agent")
```

### Comparing `autotraders-0.3.1/autotraders/contract.py` & `autotraders-1.0.0/autotraders/contract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,22 @@
+import requests
+
+from autotraders.util import parse_time
+
+
+class Deliver:
+    def __init__(self, data):
+        self.trade_symbol = data["tradeSymbol"]
+        self.destination_symbol = data["destinationSymbol"]
+        self.units_required = data["unitsRequired"]
+        self.units_fulfilled = data["unitsFulfilled"]
+
+
 class Contract:
-    def __init__(self, contract_id, session, update=True):
+    def __init__(self, contract_id, session: requests.Session, update=True):
         self.contract_id = contract_id
         self.session = session
         if update:
             self.update()
 
     def update(self, data=None):
         if data is None:
@@ -11,15 +24,18 @@
                 "https://api.spacetraders.io/v2/my/contracts/" + self.contract_id
             )
             data = r.json()["data"]
         self.on_accepted = data["terms"]["payment"]["onAccepted"]
         self.on_fulfilled = data["terms"]["payment"]["onFulfilled"]
         self.accepted = data["accepted"]
         self.fulfilled = data["fulfilled"]
-        self.deadline = data["terms"]["deadline"]
+        self.deadline = parse_time(data["terms"]["deadline"])
+        if "deliver" in data:
+            self.contract_type = "deliver"
+            self.contract_data = [Deliver(d) for d in data["deliver"]]
 
     def accept(self):
         j = self.session.post(
             "https://api.spacetraders.io/v2/my/contracts/"
             + self.contract_id
             + "/accept"
         ).json()
```

### Comparing `autotraders-0.3.1/autotraders/faction.py` & `autotraders-1.0.0/autotraders/faction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+import requests
+
 from autotraders.trait import Trait
 
 
 class Faction:
-    def __init__(self, symbol, session, update=True):
+    def __init__(self, symbol, session: requests.Session, update=True):
         self.symbol = symbol
         self.session = session
         if update:
             self.update()
 
     def update(self, data=None):
         if data is None:
-            r = self.session.get("https://api.spacetraders.io/v2/factions/" + self.symbol)
+            r = self.session.get(
+                "https://api.spacetraders.io/v2/factions/" + self.symbol
+            )
             data = r.json()["data"]
         self.name = data["name"]
         self.description = data["description"]
         self.headquarters = data["headquarters"]
         self.traits = []
         for trait in data["traits"]:
             self.traits.append(Trait(trait))
```

### Comparing `autotraders-0.3.1/autotraders/marketplace.py` & `autotraders-1.0.0/autotraders/waypoint_types/marketplace.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,46 @@
+import requests
+
+
+class TradeGood:
+    def __init__(self, data):
+        self.symbol = data["symbol"]
+        self.trade_volume = data["tradeVolume"]
+        self.supply = data["supply"]
+        self.purchase_price = data["purchasePrice"]
+        self.sell_price = data["sellPrice"]
+
+
 class Marketplace:
-    def __init__(self, waypoint: str, session, update=True):
+    def __init__(self, waypoint: str, session: requests.Session, update=True):
         self.location = waypoint
         self.session = session
         if update:
             self.update()
 
     def update(self, data: dict = None):
         if data is None:
             split = self.location.split("-")
             system_symbol = split[0] + "-" + split[1]
             waypoint_symbol = self.location
-            data = self.session.get("https://api.spacetraders.io/v2/systems/"
-                                    + system_symbol + "/waypoints/"
-                                    + waypoint_symbol + "/market").json()["data"]
+            data = self.session.get(
+                "https://api.spacetraders.io/v2/systems/"
+                + system_symbol
+                + "/waypoints/"
+                + waypoint_symbol
+                + "/market"
+            ).json()["data"]
         self.imports = []
         for i in data["imports"]:
             self.imports.append(i["symbol"])
         self.exports = []
         for i in data["exports"]:
             self.exports.append(i["symbol"])
         self.exchange = []
         for i in data["exchange"]:
             self.exchange.append(i["symbol"])
+
+        self.trade_goods = None
+        if "tradeGoods" in data:
+            self.trade_goods = []
+            for i in data["tradeGoods"]:
+                self.trade_goods.append(TradeGood(i))
```

### Comparing `autotraders-0.3.1/autotraders/shipyard.py` & `autotraders-1.0.0/autotraders/waypoint_types/jumpgate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-class Shipyard:
-    def __init__(self, waypoint: str, session, update=True):
+import requests
+
+
+class JumpGate:
+    def __init__(self, waypoint: str, session: requests.Session, update=True):
         self.location = waypoint
         self.session = session
+        self.faction_symbol = ""
         if update:
             self.update()
 
     def update(self, data: dict = None):
         if data is None:
             split = self.location.split("-")
             system_symbol = split[0] + "-" + split[1]
             waypoint_symbol = self.location
-            data = self.session.get("https://api.spacetraders.io/v2/systems/"
-                                    + system_symbol + "/waypoints/"
-                                    + waypoint_symbol + "/shipyard").json()["data"]
-        self.ship_types = []
-        for ship_type in data["shipTypes"]:
-            self.ship_types.append(ship_type["type"])
-
-    def purchase(self, ship_type: str):
-        self.session.post("https://api.spacetraders.io/v2/my/ships", data={
-            "shipType": ship_type,
-            "waypointSymbol": self.location
-        })
+            data = self.session.get(
+                "https://api.spacetraders.io/v2/systems/"
+                + system_symbol
+                + "/waypoints/"
+                + waypoint_symbol
+                + "/jump-gate"
+            ).json()["data"]
+        self.jump_range = data["jumpRange"]
+        if "factionSymbol" in data:
+            self.faction_symbol = data["factionSymbol"]
```

### Comparing `autotraders-0.3.1/autotraders/system.py` & `autotraders-1.0.0/autotraders/system.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import requests
+
 from autotraders.waypoint import Waypoint
 
 
 class System:
-    def __init__(self, symbol, session, update=True):
+    def __init__(self, symbol, session: requests.Session, update=True):
         self.session = session
         self.symbol = symbol
         self.waypoints = []
         if update:
             self.update()
 
     def update(self, data=None):
```

### Comparing `autotraders-0.3.1/autotraders/waypoint.py` & `autotraders-1.0.0/autotraders/waypoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import requests
+
 from autotraders.trait import Trait
 
 
 class Waypoint:
-    def __init__(self, symbol, session, update=True):
+    def __init__(self, symbol, session: requests.Session, update=True):
         self.session = session
         self.symbol = symbol
         self.marketplace = False
         self.shipyard = False
         if update:
             self.update()
 
@@ -28,16 +30,20 @@
             self.faction = data["faction"]["symbol"]
         else:
             self.faction = None
         self.traits = []
         if "traits" in data:
             for trait in data["traits"]:
                 self.traits.append(Trait(trait))
-        self.marketplace = len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
-        self.shipyard = len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
+        self.marketplace = (
+            len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
+        )
+        self.shipyard = (
+            len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
+        )
 
 
 def get_all_waypoints(system, session):
     r = session.get("https://api.spacetraders.io/v2/systems/" + system + "/waypoints")
     data = r.json()["data"]
     waypoints = []
     for w in data:
```

### Comparing `autotraders-0.3.1/autotraders.egg-info/PKG-INFO` & `autotraders-1.0.0/autotraders.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 0.3.1
+Version: 1.0.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,28 +14,16 @@
 License-File: LICENSE
 
 # Autotraders
 A spacetraders API focused on automation and ease of use
 ## Usage
 First you need a client, which can be generated 
 ```python
-import requests
-
-
-class BearerAuth(requests.auth.AuthBase):
-    def __init__(self, token):
-        self.token = token
-
-    def __call__(self, r):
-        r.headers["authorization"] = "Bearer " + self.token
-        return r
-
-token = TOKEN_HERE
-s = requests.Session()
-s.auth = BearerAuth(token)
+from autotraders import session
+s = session.get_session("YOUR_TOKEN_HERE")
 ```
 And now you're all set to use they actual API.
 
 ## Ships
 
 ```python
 from autotraders.ship import Ship, get_all_ships
```

### Comparing `autotraders-0.3.1/pyproject.toml` & `autotraders-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "0.3.1"
+version = "1.0.0"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

