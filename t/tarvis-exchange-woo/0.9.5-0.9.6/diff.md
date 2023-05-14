# Comparing `tmp/tarvis-exchange-woo-0.9.5.tar.gz` & `tmp/tarvis-exchange-woo-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-exchange-woo-0.9.5.tar", last modified: Wed May  3 02:15:21 2023, max compression
+gzip compressed data, was "tarvis-exchange-woo-0.9.6.tar", last modified: Sun May 14 09:42:02 2023, max compression
```

## Comparing `tarvis-exchange-woo-0.9.5.tar` & `tarvis-exchange-woo-0.9.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:15:21.742359 tarvis-exchange-woo-0.9.5/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      404 2023-05-03 02:15:21.738359 tarvis-exchange-woo-0.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 02:15:21.742359 tarvis-exchange-woo-0.9.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      767 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:15:21.738359 tarvis-exchange-woo-0.9.5/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:15:21.738359 tarvis-exchange-woo-0.9.5/tarvis/exchange/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:15:21.738359 tarvis-exchange-woo-0.9.5/tarvis/exchange/woo/
--rw-r--r--   0 root         (0) root         (0)    10775 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/tarvis/exchange/woo/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11285 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/tarvis/exchange/woo/wooclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:15:21.738359 tarvis-exchange-woo-0.9.5/tarvis_exchange_woo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      404 2023-05-03 02:15:21.000000 tarvis-exchange-woo-0.9.5/tarvis_exchange_woo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-03 02:15:21.000000 tarvis-exchange-woo-0.9.5/tarvis_exchange_woo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 02:15:21.000000 tarvis-exchange-woo-0.9.5/tarvis_exchange_woo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-03 02:15:21.000000 tarvis-exchange-woo-0.9.5/tarvis_exchange_woo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 02:15:21.000000 tarvis-exchange-woo-0.9.5/tarvis_exchange_woo.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:15:21.738359 tarvis-exchange-woo-0.9.5/test/
--rw-r--r--   0 root         (0) root         (0)    11990 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/test/test_exchange_woo_margin.py
--rw-r--r--   0 root         (0) root         (0)    11996 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/test/test_exchange_woo_perpetual.py
--rw-r--r--   0 root         (0) root         (0)     6566 2023-05-03 02:15:10.000000 tarvis-exchange-woo-0.9.5/test/test_exchange_woo_spot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:42:02.912357 tarvis-exchange-woo-0.9.6/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      404 2023-05-14 09:42:02.912357 tarvis-exchange-woo-0.9.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 09:42:02.912357 tarvis-exchange-woo-0.9.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      767 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:42:02.908357 tarvis-exchange-woo-0.9.6/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:42:02.908357 tarvis-exchange-woo-0.9.6/tarvis/exchange/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:42:02.908357 tarvis-exchange-woo-0.9.6/tarvis/exchange/woo/
+-rw-r--r--   0 root         (0) root         (0)    11009 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/tarvis/exchange/woo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11285 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/tarvis/exchange/woo/wooclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:42:02.908357 tarvis-exchange-woo-0.9.6/tarvis_exchange_woo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      404 2023-05-14 09:42:02.000000 tarvis-exchange-woo-0.9.6/tarvis_exchange_woo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-14 09:42:02.000000 tarvis-exchange-woo-0.9.6/tarvis_exchange_woo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:42:02.000000 tarvis-exchange-woo-0.9.6/tarvis_exchange_woo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 09:42:02.000000 tarvis-exchange-woo-0.9.6/tarvis_exchange_woo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 09:42:02.000000 tarvis-exchange-woo-0.9.6/tarvis_exchange_woo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:42:02.912357 tarvis-exchange-woo-0.9.6/test/
+-rw-r--r--   0 root         (0) root         (0)    12337 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/test/test_exchange_woo_margin.py
+-rw-r--r--   0 root         (0) root         (0)    12343 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/test/test_exchange_woo_perpetual.py
+-rw-r--r--   0 root         (0) root         (0)     6777 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/test/test_exchange_woo_spot.py
```

### Comparing `tarvis-exchange-woo-0.9.5/LICENSE.txt` & `tarvis-exchange-woo-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.5/setup.py` & `tarvis-exchange-woo-0.9.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-exchange-woo",
-    version="0.9.5",
+    version="0.9.6",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Exchange Library for Woo",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-exchange-woo-0.9.5/tarvis/exchange/woo/__init__.py` & `tarvis-exchange-woo-0.9.6/tarvis/exchange/woo/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     _STANDARD_ORDER_TYPE_TO_TARVIS = dict(
         (value, key) for key, value in _STANDARD_ORDER_TYPE_TO_WOO.items()
     )
     _STANDARD_TARVIS_ORDER_TYPES = _STANDARD_ORDER_TYPE_TO_WOO.keys()
     _STANDARD_WOO_ORDER_TYPES = _STANDARD_ORDER_TYPE_TO_TARVIS.keys()
 
     _ALGO_ORDER_TYPE_TO_WOO = {
-        OrderType.STOP_LOSS_MARKET: ("STOP", "MARKET"),
+        OrderType.STOP_LOSS: ("STOP", "MARKET"),
     }
 
     def __init__(
         self,
         credentials_secret: str,
         version: str | WooVersion = WooVersion.SPOT,
     ):
@@ -82,16 +82,16 @@
         maximum_order_quantity = Decimal(market_data["base_max"])
         quantity_precision = Decimal(market_data["base_tick"])
         price_precision = Decimal(market_data["quote_tick"])
         minimum_order_value = float(market_data["min_notional"])
 
         return TradingPolicy(
             minimum_order_quantity=minimum_order_quantity,
-            minimum_order_value=minimum_order_value,
             maximum_order_quantity=maximum_order_quantity,
+            minimum_order_value=minimum_order_value,
             quantity_precision=quantity_precision,
             price_precision=price_precision,
         )
 
     def get_quote(self, base_asset: str, quote_asset: str) -> Decimal:
         market = self._convert_assets_to_market(base_asset, quote_asset)
         response = self._client.get_kline(market, "1m", 1)
@@ -125,23 +125,23 @@
                 base_quantity = results.get(base_asset, 0)
                 quote_quantity = results.get(quote_asset, 0)
                 results[base_asset] = base_quantity + quantity
                 results[quote_asset] = quote_quantity - (quantity * price)
 
         return results
 
-    def _get_open_orders_standard(self) -> list[Order]:
+    def _get_open_orders_standard(self, market: str) -> list[Order]:
         _PAGE_SIZE = 500
 
         results = {}
         page_order_count = _PAGE_SIZE
         page = 1
         while page_order_count == _PAGE_SIZE:
             response = self._client.get_orders(
-                status="INCOMPLETE", size=_PAGE_SIZE, page=page
+                symbol=market, status="INCOMPLETE", size=_PAGE_SIZE, page=page
             )
             woo_orders = response["rows"]
             page_order_count = len(woo_orders)
             page += 1
 
             for woo_order in woo_orders:
                 symbol = woo_order["symbol"]
@@ -180,47 +180,51 @@
                         meta_data=meta_data,
                     )
 
                     results[order_id] = order
 
         return list(results.values())
 
-    def _get_open_orders_algo(self) -> list[Order]:
+    def _get_open_orders_algo(self, market: str) -> list[Order]:
         _PAGE_SIZE = 25
 
         results = {}
         page_order_count = _PAGE_SIZE
         page = 1
         while page_order_count == _PAGE_SIZE:
             response = self._client.get_algo_orders(
-                algo_type="STOP", status="INCOMPLETE", size=_PAGE_SIZE, page=page
+                algo_type="STOP",
+                symbol=market,
+                status="INCOMPLETE",
+                size=_PAGE_SIZE,
+                page=page,
             )
             woo_orders = response["data"]["rows"]
             page_order_count = len(woo_orders)
             page += 1
 
             for woo_order in woo_orders:
                 symbol = woo_order["symbol"]
                 market_type, quote_asset, base_asset = self._convert_market_to_assets(
                     symbol
                 )
 
                 if market_type == self._market_type:
                     order_id = woo_order["algoOrderId"]
-                    quantity = woo_order.get("quantity", None)
-                    amount = woo_order.get("amount", None)
-                    price = woo_order["triggerPrice"]
+                    quantity = woo_order.get("quantity")
+                    amount = woo_order.get("amount")
+                    price = woo_order.get("triggerPrice")
                     side = woo_order["side"]
                     order_type = woo_order["type"]
                     creation_time = woo_order["createdTime"]
                     filled_quantity = woo_order.get("totalExecutedQuantity")
 
                     side = OrderSide[side]
                     if order_type == "MARKET":
-                        order_type = OrderType.STOP_LOSS_MARKET
+                        order_type = OrderType.STOP_LOSS
                     else:
                         order_type = OrderType.UNSUPPORTED
                     meta_data = {"order_id": order_id, "order_method": "algo"}
 
                     order = Order(
                         quote_asset,
                         base_asset,
@@ -234,16 +238,19 @@
                         meta_data=meta_data,
                     )
 
                     results[order_id] = order
 
         return list(results.values())
 
-    def get_open_orders(self) -> list[Order]:
-        return self._get_open_orders_standard() + self._get_open_orders_algo()
+    def get_open_orders(self, base_asset: str, quote_asset: str) -> list[Order]:
+        market = self._convert_assets_to_market(base_asset, quote_asset)
+        return self._get_open_orders_standard(market) + self._get_open_orders_algo(
+            market
+        )
 
     def place_order(
         self,
         policy: TradingPolicy,
         base_asset: str,
         quote_asset: str,
         side: OrderSide,
@@ -259,15 +266,15 @@
             standard_order = True
             algo_type = None
             woo_order_type = self._STANDARD_ORDER_TYPE_TO_WOO[order_type]
         else:
             standard_order = False
             algo_type, woo_order_type = self._ALGO_ORDER_TYPE_TO_WOO[order_type]
 
-        if order_type == OrderType.STOP_LOSS_MARKET:
+        if order_type == OrderType.STOP_LOSS:
             price = str(stop_loss_price)
         elif price is not None:
             price = str(price)
 
         if standard_order:
             self._client.post_order(
                 market,
```

### Comparing `tarvis-exchange-woo-0.9.5/tarvis/exchange/woo/wooclient.py` & `tarvis-exchange-woo-0.9.6/tarvis/exchange/woo/wooclient.py`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.5/test/test_exchange_woo_margin.py` & `tarvis-exchange-woo-0.9.6/test/test_exchange_woo_perpetual.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import common  # noqa
 from decimal import Decimal
 from tarvis.common import time
 from tarvis.common.trading import OrderSide, OrderType
 from tarvis.exchange.woo import WooExchange, WooVersion
 import pytest  # noqa
 
-_TEST_CREDENTIALS = "woo_margin_test_credentials"
+_TEST_CREDENTIALS = "woo_perpetual_test_credentials"
 
 _BASE_ASSET = "BTC"
 _QUOTE_ASSET = "USDT"
 
 _PRICE_RANGE_MIN = 1000
 _PRICE_RANGE_MAX = 1000000000
 
@@ -17,50 +17,50 @@
 _UNREALISTIC_SELL = Decimal("1.1")
 _STOP_LOSS_LONG = Decimal("0.8")
 _STOP_LOSS_SHORT = Decimal("1.2")
 
 _SETTLEMENT_DELAY = 5
 _ALLOWED_TIME_DIFFERENCE = 5
 
-exchange = WooExchange(_TEST_CREDENTIALS, WooVersion.MARGIN)
+exchange = WooExchange(_TEST_CREDENTIALS, WooVersion.PERPETUAL)
 price = exchange.get_quote(_BASE_ASSET, _QUOTE_ASSET)
 trading_policy = exchange.get_policy(_BASE_ASSET, _QUOTE_ASSET)
 minimum_order_quantity = trading_policy.get_minimum_order_quantity(price)
 
 
 def test_get_quote():
     assert price > _PRICE_RANGE_MIN
     assert price < _PRICE_RANGE_MAX
 
 
 def test_get_policy():
     assert minimum_order_quantity < (1.0 / _PRICE_RANGE_MIN)
     assert minimum_order_quantity > (1.0 / _PRICE_RANGE_MAX)
     # noinspection PyProtectedMember
-    assert trading_policy._quantity_decimals == 8
+    assert trading_policy._quantity_decimals == 4
     # noinspection PyProtectedMember
     assert trading_policy._price_decimals == 2
 
 
 def test_get_positions():
     positions = exchange.get_positions()
     assert positions is not None
     quote_position = positions.get(_QUOTE_ASSET, 0)
     assert quote_position > 0
 
 
 def test_get_open_orders():
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert orders is not None
 
 
 def test_long_market_order_completed():
-    exchange.cancel_open_orders()
+    exchange.cancel_open_orders(_BASE_ASSET, _QUOTE_ASSET)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
     positions = exchange.get_positions()
     base_position_start = positions.get(_BASE_ASSET, 0)
     quote_position_start = positions.get(_QUOTE_ASSET, 0)
 
     # Order twice as much as necessary to ensure success
@@ -74,15 +74,15 @@
         OrderType.MARKET,
         order_quantity,
         price=order_price,
     )
 
     time.sleep(_SETTLEMENT_DELAY)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
     positions = exchange.get_positions()
     base_position_end = positions.get(_BASE_ASSET, 0)
     quote_position_end = positions.get(_QUOTE_ASSET, 0)
     assert float(base_position_end - base_position_start) == pytest.approx(
         float(order_quantity), 0.01
@@ -103,45 +103,45 @@
     order_quantity = trading_policy.align_quantity(base_position)
     stop_loss_price = trading_policy.align_price(price * _STOP_LOSS_LONG)
     exchange.place_order(
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.SELL,
-        OrderType.STOP_LOSS_MARKET,
+        OrderType.STOP_LOSS,
         order_quantity,
         stop_loss_price=stop_loss_price,
     )
 
     end_time = time.time()
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
     order = orders[0]
     assert order.base_asset == _BASE_ASSET
     assert order.quote_asset == _QUOTE_ASSET
     # noinspection PyProtectedMember
     assert float(order._quantity) == pytest.approx(float(order_quantity))
     assert float(order.price) == pytest.approx(float(stop_loss_price))
     assert order.side == OrderSide.SELL
-    assert order.order_type == OrderType.STOP_LOSS_MARKET
+    assert order.order_type == OrderType.STOP_LOSS
     # Allow 1 second time inaccuracy
     assert order.creation_time > (start_time - _ALLOWED_TIME_DIFFERENCE)
     assert order.creation_time < (end_time + _ALLOWED_TIME_DIFFERENCE)
     assert order.filled_quantity == 0
 
     exchange.cancel_order(order)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
 
 def test_long_limit_order():
-    exchange.cancel_open_orders()
+    exchange.cancel_open_orders(_BASE_ASSET, _QUOTE_ASSET)
 
     start_time = time.time()
 
     # Create an unrealistic limit order that will not be filled
     order_price = trading_policy.align_price(price * _UNREALISTIC_BUY)
     order_quantity = trading_policy.get_minimum_order_quantity(order_price)
     exchange.place_order(
@@ -152,15 +152,15 @@
         OrderType.LIMIT,
         order_quantity,
         price=order_price,
     )
 
     end_time = time.time()
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
     order = orders[0]
     assert order.base_asset == _BASE_ASSET
     assert order.quote_asset == _QUOTE_ASSET
     # noinspection PyProtectedMember
     assert float(order._quantity) == pytest.approx(float(order_quantity))
@@ -170,15 +170,15 @@
     # Allow 1 second time inaccuracy
     assert order.creation_time > (start_time - _ALLOWED_TIME_DIFFERENCE)
     assert order.creation_time < (end_time + _ALLOWED_TIME_DIFFERENCE)
     assert order.filled_quantity == 0
 
     exchange.cancel_order(order)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
 
 def test_close_long_position():
     positions = exchange.get_positions()
     base_position_start = positions.get(_BASE_ASSET, 0)
     quote_position_start = positions.get(_QUOTE_ASSET, 0)
@@ -234,15 +234,15 @@
         OrderType.MARKET,
         order_quantity,
         price=order_price,
     )
 
     time.sleep(_SETTLEMENT_DELAY)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
     positions = exchange.get_positions()
     base_position_end = positions.get(_BASE_ASSET, 0)
     quote_position_end = positions.get(_QUOTE_ASSET, 0)
     assert quote_position_end > quote_position_start
     assert base_position_end < 0
@@ -267,45 +267,45 @@
     order_quantity = trading_policy.align_quantity(base_position)
     stop_loss_price = trading_policy.align_price(price * _STOP_LOSS_SHORT)
     exchange.place_order(
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.BUY,
-        OrderType.STOP_LOSS_MARKET,
+        OrderType.STOP_LOSS,
         order_quantity,
         stop_loss_price=stop_loss_price,
     )
 
     end_time = time.time()
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
     order = orders[0]
     assert order.base_asset == _BASE_ASSET
     assert order.quote_asset == _QUOTE_ASSET
     # noinspection PyProtectedMember
     assert float(order._quantity) == pytest.approx(float(order_quantity))
     assert float(order.price) == pytest.approx(float(stop_loss_price))
     assert order.side == OrderSide.BUY
-    assert order.order_type == OrderType.STOP_LOSS_MARKET
+    assert order.order_type == OrderType.STOP_LOSS
     # Allow 1 second time inaccuracy
     assert order.creation_time > (start_time - _ALLOWED_TIME_DIFFERENCE)
     assert order.creation_time < (end_time + _ALLOWED_TIME_DIFFERENCE)
     assert order.filled_quantity == 0
 
     exchange.cancel_order(order)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
 
 def test_short_limit_order():
-    exchange.cancel_open_orders()
+    exchange.cancel_open_orders(_BASE_ASSET, _QUOTE_ASSET)
 
     start_time = time.time()
 
     # Create an unrealistic limit order that will not be filled
     order_price = trading_policy.align_price(price * _UNREALISTIC_SELL)
     order_quantity = trading_policy.get_minimum_order_quantity(order_price)
     exchange.place_order(
@@ -316,15 +316,15 @@
         OrderType.LIMIT,
         order_quantity,
         price=order_price,
     )
 
     end_time = time.time()
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
     order = orders[0]
     assert order.base_asset == _BASE_ASSET
     assert order.quote_asset == _QUOTE_ASSET
     # noinspection PyProtectedMember
     assert float(order._quantity) == pytest.approx(float(order_quantity))
@@ -334,15 +334,15 @@
     # Allow 1 second time inaccuracy
     assert order.creation_time > (start_time - _ALLOWED_TIME_DIFFERENCE)
     assert order.creation_time < (end_time + _ALLOWED_TIME_DIFFERENCE)
     assert order.filled_quantity == 0
 
     exchange.cancel_order(order)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
 
 def test_close_short_position():
     positions = exchange.get_positions()
     base_position_start = positions.get(_BASE_ASSET, 0)
     quote_position_start = positions.get(_QUOTE_ASSET, 0)
```

### Comparing `tarvis-exchange-woo-0.9.5/test/test_exchange_woo_perpetual.py` & `tarvis-exchange-woo-0.9.6/test/test_exchange_woo_margin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import common  # noqa
 from decimal import Decimal
 from tarvis.common import time
 from tarvis.common.trading import OrderSide, OrderType
 from tarvis.exchange.woo import WooExchange, WooVersion
 import pytest  # noqa
 
-_TEST_CREDENTIALS = "woo_perpetual_test_credentials"
+_TEST_CREDENTIALS = "woo_margin_test_credentials"
 
 _BASE_ASSET = "BTC"
 _QUOTE_ASSET = "USDT"
 
 _PRICE_RANGE_MIN = 1000
 _PRICE_RANGE_MAX = 1000000000
 
@@ -17,50 +17,50 @@
 _UNREALISTIC_SELL = Decimal("1.1")
 _STOP_LOSS_LONG = Decimal("0.8")
 _STOP_LOSS_SHORT = Decimal("1.2")
 
 _SETTLEMENT_DELAY = 5
 _ALLOWED_TIME_DIFFERENCE = 5
 
-exchange = WooExchange(_TEST_CREDENTIALS, WooVersion.PERPETUAL)
+exchange = WooExchange(_TEST_CREDENTIALS, WooVersion.MARGIN)
 price = exchange.get_quote(_BASE_ASSET, _QUOTE_ASSET)
 trading_policy = exchange.get_policy(_BASE_ASSET, _QUOTE_ASSET)
 minimum_order_quantity = trading_policy.get_minimum_order_quantity(price)
 
 
 def test_get_quote():
     assert price > _PRICE_RANGE_MIN
     assert price < _PRICE_RANGE_MAX
 
 
 def test_get_policy():
     assert minimum_order_quantity < (1.0 / _PRICE_RANGE_MIN)
     assert minimum_order_quantity > (1.0 / _PRICE_RANGE_MAX)
     # noinspection PyProtectedMember
-    assert trading_policy._quantity_decimals == 4
+    assert trading_policy._quantity_decimals == 8
     # noinspection PyProtectedMember
     assert trading_policy._price_decimals == 2
 
 
 def test_get_positions():
     positions = exchange.get_positions()
     assert positions is not None
     quote_position = positions.get(_QUOTE_ASSET, 0)
     assert quote_position > 0
 
 
 def test_get_open_orders():
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert orders is not None
 
 
 def test_long_market_order_completed():
-    exchange.cancel_open_orders()
+    exchange.cancel_open_orders(_BASE_ASSET, _QUOTE_ASSET)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
     positions = exchange.get_positions()
     base_position_start = positions.get(_BASE_ASSET, 0)
     quote_position_start = positions.get(_QUOTE_ASSET, 0)
 
     # Order twice as much as necessary to ensure success
@@ -74,15 +74,15 @@
         OrderType.MARKET,
         order_quantity,
         price=order_price,
     )
 
     time.sleep(_SETTLEMENT_DELAY)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
     positions = exchange.get_positions()
     base_position_end = positions.get(_BASE_ASSET, 0)
     quote_position_end = positions.get(_QUOTE_ASSET, 0)
     assert float(base_position_end - base_position_start) == pytest.approx(
         float(order_quantity), 0.01
@@ -103,45 +103,45 @@
     order_quantity = trading_policy.align_quantity(base_position)
     stop_loss_price = trading_policy.align_price(price * _STOP_LOSS_LONG)
     exchange.place_order(
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.SELL,
-        OrderType.STOP_LOSS_MARKET,
+        OrderType.STOP_LOSS,
         order_quantity,
         stop_loss_price=stop_loss_price,
     )
 
     end_time = time.time()
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
     order = orders[0]
     assert order.base_asset == _BASE_ASSET
     assert order.quote_asset == _QUOTE_ASSET
     # noinspection PyProtectedMember
     assert float(order._quantity) == pytest.approx(float(order_quantity))
     assert float(order.price) == pytest.approx(float(stop_loss_price))
     assert order.side == OrderSide.SELL
-    assert order.order_type == OrderType.STOP_LOSS_MARKET
+    assert order.order_type == OrderType.STOP_LOSS
     # Allow 1 second time inaccuracy
     assert order.creation_time > (start_time - _ALLOWED_TIME_DIFFERENCE)
     assert order.creation_time < (end_time + _ALLOWED_TIME_DIFFERENCE)
     assert order.filled_quantity == 0
 
     exchange.cancel_order(order)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
 
 def test_long_limit_order():
-    exchange.cancel_open_orders()
+    exchange.cancel_open_orders(_BASE_ASSET, _QUOTE_ASSET)
 
     start_time = time.time()
 
     # Create an unrealistic limit order that will not be filled
     order_price = trading_policy.align_price(price * _UNREALISTIC_BUY)
     order_quantity = trading_policy.get_minimum_order_quantity(order_price)
     exchange.place_order(
@@ -152,15 +152,15 @@
         OrderType.LIMIT,
         order_quantity,
         price=order_price,
     )
 
     end_time = time.time()
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
     order = orders[0]
     assert order.base_asset == _BASE_ASSET
     assert order.quote_asset == _QUOTE_ASSET
     # noinspection PyProtectedMember
     assert float(order._quantity) == pytest.approx(float(order_quantity))
@@ -170,15 +170,15 @@
     # Allow 1 second time inaccuracy
     assert order.creation_time > (start_time - _ALLOWED_TIME_DIFFERENCE)
     assert order.creation_time < (end_time + _ALLOWED_TIME_DIFFERENCE)
     assert order.filled_quantity == 0
 
     exchange.cancel_order(order)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
 
 def test_close_long_position():
     positions = exchange.get_positions()
     base_position_start = positions.get(_BASE_ASSET, 0)
     quote_position_start = positions.get(_QUOTE_ASSET, 0)
@@ -234,15 +234,15 @@
         OrderType.MARKET,
         order_quantity,
         price=order_price,
     )
 
     time.sleep(_SETTLEMENT_DELAY)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
     positions = exchange.get_positions()
     base_position_end = positions.get(_BASE_ASSET, 0)
     quote_position_end = positions.get(_QUOTE_ASSET, 0)
     assert quote_position_end > quote_position_start
     assert base_position_end < 0
@@ -267,45 +267,45 @@
     order_quantity = trading_policy.align_quantity(base_position)
     stop_loss_price = trading_policy.align_price(price * _STOP_LOSS_SHORT)
     exchange.place_order(
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.BUY,
-        OrderType.STOP_LOSS_MARKET,
+        OrderType.STOP_LOSS,
         order_quantity,
         stop_loss_price=stop_loss_price,
     )
 
     end_time = time.time()
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
     order = orders[0]
     assert order.base_asset == _BASE_ASSET
     assert order.quote_asset == _QUOTE_ASSET
     # noinspection PyProtectedMember
     assert float(order._quantity) == pytest.approx(float(order_quantity))
     assert float(order.price) == pytest.approx(float(stop_loss_price))
     assert order.side == OrderSide.BUY
-    assert order.order_type == OrderType.STOP_LOSS_MARKET
+    assert order.order_type == OrderType.STOP_LOSS
     # Allow 1 second time inaccuracy
     assert order.creation_time > (start_time - _ALLOWED_TIME_DIFFERENCE)
     assert order.creation_time < (end_time + _ALLOWED_TIME_DIFFERENCE)
     assert order.filled_quantity == 0
 
     exchange.cancel_order(order)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
 
 def test_short_limit_order():
-    exchange.cancel_open_orders()
+    exchange.cancel_open_orders(_BASE_ASSET, _QUOTE_ASSET)
 
     start_time = time.time()
 
     # Create an unrealistic limit order that will not be filled
     order_price = trading_policy.align_price(price * _UNREALISTIC_SELL)
     order_quantity = trading_policy.get_minimum_order_quantity(order_price)
     exchange.place_order(
@@ -316,15 +316,15 @@
         OrderType.LIMIT,
         order_quantity,
         price=order_price,
     )
 
     end_time = time.time()
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
     order = orders[0]
     assert order.base_asset == _BASE_ASSET
     assert order.quote_asset == _QUOTE_ASSET
     # noinspection PyProtectedMember
     assert float(order._quantity) == pytest.approx(float(order_quantity))
@@ -334,15 +334,15 @@
     # Allow 1 second time inaccuracy
     assert order.creation_time > (start_time - _ALLOWED_TIME_DIFFERENCE)
     assert order.creation_time < (end_time + _ALLOWED_TIME_DIFFERENCE)
     assert order.filled_quantity == 0
 
     exchange.cancel_order(order)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
 
 def test_close_short_position():
     positions = exchange.get_positions()
     base_position_start = positions.get(_BASE_ASSET, 0)
     quote_position_start = positions.get(_QUOTE_ASSET, 0)
```

### Comparing `tarvis-exchange-woo-0.9.5/test/test_exchange_woo_spot.py` & `tarvis-exchange-woo-0.9.6/test/test_exchange_woo_spot.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,22 +45,22 @@
     positions = exchange.get_positions()
     assert positions is not None
     quote_position = positions.get(_QUOTE_ASSET, 0)
     assert quote_position > 0
 
 
 def test_get_open_orders():
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert orders is not None
 
 
 def test_long_market_order_completed():
-    exchange.cancel_open_orders()
+    exchange.cancel_open_orders(_BASE_ASSET, _QUOTE_ASSET)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
     positions = exchange.get_positions()
     base_position_start = positions.get(_BASE_ASSET, 0)
     quote_position_start = positions.get(_QUOTE_ASSET, 0)
     order_quantity = trading_policy.align_quantity(minimum_order_quantity * 2)
     order_price = trading_policy.align_price(price)
@@ -72,15 +72,15 @@
         OrderType.MARKET,
         order_quantity,
         price=order_price,
     )
 
     time.sleep(_SETTLEMENT_DELAY)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
     positions = exchange.get_positions()
     base_position_end = positions.get(_BASE_ASSET, 0)
     quote_position_end = positions.get(_QUOTE_ASSET, 0)
     assert float(base_position_end - base_position_start) == pytest.approx(
         float(order_quantity), 0.01
@@ -101,45 +101,45 @@
     order_quantity = trading_policy.align_quantity(base_position)
     stop_loss_price = trading_policy.align_price(price * _STOP_LOSS_LONG)
     exchange.place_order(
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.SELL,
-        OrderType.STOP_LOSS_MARKET,
+        OrderType.STOP_LOSS,
         order_quantity,
         stop_loss_price=stop_loss_price,
     )
 
     end_time = time.time()
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
     order = orders[0]
     assert order.base_asset == _BASE_ASSET
     assert order.quote_asset == _QUOTE_ASSET
     # noinspection PyProtectedMember
     assert float(order._quantity) == pytest.approx(float(order_quantity))
     assert float(order.price) == pytest.approx(float(stop_loss_price))
     assert order.side == OrderSide.SELL
-    assert order.order_type == OrderType.STOP_LOSS_MARKET
+    assert order.order_type == OrderType.STOP_LOSS
     # Allow 1 second time inaccuracy
     assert order.creation_time > (start_time - _ALLOWED_TIME_DIFFERENCE)
     assert order.creation_time < (end_time + _ALLOWED_TIME_DIFFERENCE)
     assert order.filled_quantity == 0
 
     exchange.cancel_order(order)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
 
 def test_long_limit_order():
-    exchange.cancel_open_orders()
+    exchange.cancel_open_orders(_BASE_ASSET, _QUOTE_ASSET)
 
     start_time = time.time()
 
     # Create an unrealistic limit order that will not be filled
     order_price = trading_policy.align_price(price * _UNREALISTIC_BUY)
     order_quantity = trading_policy.get_minimum_order_quantity(order_price)
     exchange.place_order(
@@ -150,15 +150,15 @@
         OrderType.LIMIT,
         order_quantity,
         price=order_price,
     )
 
     end_time = time.time()
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
     order = orders[0]
     assert order.base_asset == _BASE_ASSET
     assert order.quote_asset == _QUOTE_ASSET
     # noinspection PyProtectedMember
     assert float(order._quantity) == pytest.approx(float(order_quantity))
@@ -168,15 +168,15 @@
     # Allow 1 second time inaccuracy
     assert order.creation_time > (start_time - _ALLOWED_TIME_DIFFERENCE)
     assert order.creation_time < (end_time + _ALLOWED_TIME_DIFFERENCE)
     assert order.filled_quantity == 0
 
     exchange.cancel_order(order)
 
-    orders = exchange.get_open_orders()
+    orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
 
 def test_close_long_position():
     positions = exchange.get_positions()
     base_position_start = positions.get(_BASE_ASSET, 0)
     quote_position_start = positions.get(_QUOTE_ASSET, 0)
```

