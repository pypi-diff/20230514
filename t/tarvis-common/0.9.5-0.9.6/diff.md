# Comparing `tmp/tarvis-common-0.9.5.tar.gz` & `tmp/tarvis-common-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-common-0.9.5.tar", last modified: Wed May  3 01:28:13 2023, max compression
+gzip compressed data, was "tarvis-common-0.9.6.tar", last modified: Sun May 14 07:27:57 2023, max compression
```

## Comparing `tarvis-common-0.9.5.tar` & `tarvis-common-0.9.6.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.963436 tarvis-common-0.9.5/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-03 01:28:13.963436 tarvis-common-0.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 01:28:13.963436 tarvis-common-0.9.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/asyncio/
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/asyncio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/cache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/cache/local/
--rw-r--r--   0 root         (0) root         (0)     3885 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/cache/local/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/config/
--rw-r--r--   0 root         (0) root         (0)     1698 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/environ/
--rw-r--r--   0 root         (0) root         (0)     1987 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/environ/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/logging/
--rw-r--r--   0 root         (0) root         (0)     5793 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/monitoring/
--rw-r--r--   0 root         (0) root         (0)     3678 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/secrets/
--rw-r--r--   0 root         (0) root         (0)     2551 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/secrets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/time/
--rw-r--r--   0 root         (0) root         (0)     6201 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/time/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/trading/
--rw-r--r--   0 root         (0) root         (0)     8267 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.963436 tarvis-common-0.9.5/tarvis_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-03 01:28:13.000000 tarvis-common-0.9.5/tarvis_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      523 2023-05-03 01:28:13.000000 tarvis-common-0.9.5/tarvis_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 01:28:13.000000 tarvis-common-0.9.5/tarvis_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      208 2023-05-03 01:28:13.000000 tarvis-common-0.9.5/tarvis_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 01:28:13.000000 tarvis-common-0.9.5/tarvis_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.307687 tarvis-common-0.9.6/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-14 07:27:57.307687 tarvis-common-0.9.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 07:27:57.307687 tarvis-common-0.9.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.299687 tarvis-common-0.9.6/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.299687 tarvis-common-0.9.6/tarvis/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/asyncio/
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/asyncio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.299687 tarvis-common-0.9.6/tarvis/common/cache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/cache/local/
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/cache/local/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/config/
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/environ/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/environ/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/logging/
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/monitoring/
+-rw-r--r--   0 root         (0) root         (0)     3678 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/secrets/
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/secrets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/time/
+-rw-r--r--   0 root         (0) root         (0)     6436 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/time/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/trading/
+-rw-r--r--   0 root         (0) root         (0)     8778 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-14 07:27:57.000000 tarvis-common-0.9.6/tarvis_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      564 2023-05-14 07:27:57.000000 tarvis-common-0.9.6/tarvis_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 07:27:57.000000 tarvis-common-0.9.6/tarvis_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      208 2023-05-14 07:27:57.000000 tarvis-common-0.9.6/tarvis_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 07:27:57.000000 tarvis-common-0.9.6/tarvis_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.307687 tarvis-common-0.9.6/test/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/test/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/test/test_secrets.py
```

### Comparing `tarvis-common-0.9.5/LICENSE.txt` & `tarvis-common-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.5/setup.py` & `tarvis-common-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-common",
-    version="0.9.5",
+    version="0.9.6",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Common Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-common-0.9.5/tarvis/common/asyncio/__init__.py` & `tarvis-common-0.9.6/tarvis/common/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.5/tarvis/common/cache/local/__init__.py` & `tarvis-common-0.9.6/tarvis/common/cache/local/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.5/tarvis/common/config/__init__.py` & `tarvis-common-0.9.6/tarvis/common/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.5/tarvis/common/environ/__init__.py` & `tarvis-common-0.9.6/tarvis/common/environ/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.5/tarvis/common/logging/__init__.py` & `tarvis-common-0.9.6/tarvis/common/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.5/tarvis/common/monitoring/__init__.py` & `tarvis-common-0.9.6/tarvis/common/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.5/tarvis/common/secrets/__init__.py` & `tarvis-common-0.9.6/tarvis/common/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.5/tarvis/common/time/__init__.py` & `tarvis-common-0.9.6/tarvis/common/time/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,44 +8,53 @@
 import logging
 import math
 from tarvis.common import environ
 from tarvis.common.environ import DeploymentType
 import time as native_time
 from typing import Optional, Union
 
+_TIME_INTERVAL_DECIMALS = 3
+
 
 def span(
     weeks: float = 0,
     days: float = 0,
     hours: float = 0,
     minutes: float = 0,
     seconds: float = 0,
     milliseconds: float = 0,
 ) -> float:
-    return (
+    return round(
         (((((((weeks * 7) + days) * 24) + hours) * 60) + minutes) * 60)
         + seconds
-        + (0.001 * milliseconds)
+        + (0.001 * milliseconds),
+        _TIME_INTERVAL_DECIMALS,
     )
 
 
 def current_interval(timestamp: float, interval: float) -> float:
-    return interval * math.floor(timestamp / interval)
+    return round(
+        interval * math.floor(round(timestamp / interval, _TIME_INTERVAL_DECIMALS)),
+        _TIME_INTERVAL_DECIMALS,
+    )
 
 
 def next_interval(timestamp: float, interval: float) -> float:
     return current_interval(timestamp + interval, interval)
 
 
 def previous_interval(timestamp: float, interval: float) -> float:
     return current_interval(timestamp - interval, interval)
 
 
 def closest_interval(timestamp: float, interval: float) -> float:
-    return interval * round(timestamp / interval)
+    return round(
+        interval * round(timestamp / interval, _TIME_INTERVAL_DECIMALS),
+        _TIME_INTERVAL_DECIMALS,
+    )
 
 
 # noinspection PyPep8Naming
 class datetime(pendulum.DateTime):
     @classmethod
     def _clone(cls, dt) -> "datetime":
         return cls(
```

### Comparing `tarvis-common-0.9.5/tarvis/common/trading/__init__.py` & `tarvis-common-0.9.6/tarvis/common/trading/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     SELL = 1
 
 
 class OrderType(Enum):
     UNSUPPORTED = 0
     MARKET = 1
     LIMIT = 2
-    STOP_LOSS_MARKET = 3
+    STOP_LOSS = 3
 
 
 class MarketPosition(Enum):
     FLAT = 0
     LONG = 1
     SHORT = 2
 
@@ -85,41 +85,47 @@
         pass
 
 
 class TradingPolicy:
     def __init__(
         self,
         minimum_order_quantity: Decimal | float,
-        minimum_order_value: Decimal | float = None,
         maximum_order_quantity: Decimal | float = None,
+        minimum_order_value: Decimal | float = None,
+        maximum_order_value: Decimal | float = None,
         quantity_decimals: int = None,
         quantity_precision: Decimal = None,
         price_decimals: int = None,
         price_precision: Decimal = None,
     ):
         if (quantity_decimals is None) and quantity_precision:
             quantity_decimals = int(-math.log10(quantity_precision))
         self._quantity_decimals = quantity_decimals
 
         if (price_decimals is None) and price_precision:
             price_decimals = int(-math.log10(price_precision))
         self._price_decimals = price_decimals
 
-        # Ensure the minimum and maximum are aligned
+        # Ensure the minimum is aligned
         self._minimum_order_quantity = self.align_quantity(minimum_order_quantity)
 
+        if maximum_order_quantity is None:
+            self._maximum_order_quantity = None
+        else:
+            self._maximum_order_quantity = Decimal(maximum_order_quantity)
+
         if minimum_order_value is None:
-            self._minimum_order_value = None
+            self._minimum_order_value = 0
         else:
             self._minimum_order_value = Decimal(minimum_order_value)
 
-        if maximum_order_quantity is None:
-            self.maximum_order_quantity = None
+        if maximum_order_value is None:
+            self._maximum_order_value = None
         else:
-            self.maximum_order_quantity = self.align_quantity(maximum_order_quantity)
+            self._maximum_order_value = Decimal(maximum_order_value)
 
     @staticmethod
     def _align(value: Decimal | float | int, decimals: int | None, rounding) -> Decimal:
         value = Decimal(value)
         if decimals is not None:
             with decimal.localcontext() as ctx:
                 ctx.rounding = rounding
@@ -128,32 +134,37 @@
 
     def align_quantity(
         self, quantity: Decimal | float | int, rounding=decimal.ROUND_DOWN
     ) -> Decimal:
         return self._align(quantity, self._quantity_decimals, rounding)
 
     def get_minimum_order_quantity(self, price: Decimal) -> Decimal:
-        if self._minimum_order_value is None:
-            minimum_by_value = 0
-        else:
-            # Adjust slightly to prevent errors due to price fluctuations
-            minimum_by_value = (self._minimum_order_value / price) * Decimal("1.05")
+        # Adjust slightly to prevent errors due to price fluctuations
+        minimum_by_value = (self._minimum_order_value / price) * Decimal("1.01")
 
         if minimum_by_value > self._minimum_order_quantity:
             return self.align_quantity(minimum_by_value, decimal.ROUND_UP)
         else:
             return self._minimum_order_quantity
 
-    def limit_quantity_maximum(self, quantity: Decimal | float | int) -> Decimal:
-        if (self.maximum_order_quantity is not None) and (
-            quantity > self.maximum_order_quantity
+    def limit_quantity_maximum(
+        self, quantity: Decimal | float | int, price: Decimal
+    ) -> Decimal:
+        if self._maximum_order_value is not None:
+            # Adjust slightly to prevent errors due to price fluctuations
+            maximum_by_value = (self._maximum_order_value / price) * Decimal("0.99")
+            if quantity > maximum_by_value:
+                quantity = maximum_by_value
+
+        if (self._maximum_order_quantity is not None) and (
+            quantity > self._maximum_order_quantity
         ):
-            return self.maximum_order_quantity
-        else:
-            return Decimal(quantity)
+            quantity = self._maximum_order_quantity
+
+        return self.align_quantity(quantity)
 
     def align_price(
         self, price: Decimal | float | int, rounding=decimal.ROUND_HALF_EVEN
     ) -> Decimal:
         return self._align(price, self._price_decimals, rounding)
 
 
@@ -229,15 +240,15 @@
         """
         :return: dictionary with asset identifiers as keys and quantities as values
         Short positions are negative.
         """
         pass
 
     @abstractmethod
-    def get_open_orders(self) -> list[Order]:
+    def get_open_orders(self, base_asset: str, quote_asset: str) -> list[Order]:
         pass
 
     @abstractmethod
     def place_order(
         self,
         policy: TradingPolicy,
         base_asset: str,
@@ -264,11 +275,11 @@
         """
         pass
 
     @abstractmethod
     def cancel_order(self, order: Order):
         pass
 
-    def cancel_open_orders(self):
-        orders = self.get_open_orders()
+    def cancel_open_orders(self, base_asset: str, quote_asset: str):
+        orders = self.get_open_orders(base_asset, quote_asset)
         for order in orders:
             self.cancel_order(order)
```

### Comparing `tarvis-common-0.9.5/tarvis_common.egg-info/SOURCES.txt` & `tarvis-common-0.9.6/tarvis_common.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -10,8 +10,10 @@
 tarvis/common/secrets/__init__.py
 tarvis/common/time/__init__.py
 tarvis/common/trading/__init__.py
 tarvis_common.egg-info/PKG-INFO
 tarvis_common.egg-info/SOURCES.txt
 tarvis_common.egg-info/dependency_links.txt
 tarvis_common.egg-info/requires.txt
-tarvis_common.egg-info/top_level.txt
+tarvis_common.egg-info/top_level.txt
+test/test_config.py
+test/test_secrets.py
```

