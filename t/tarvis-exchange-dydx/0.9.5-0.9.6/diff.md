# Comparing `tmp/tarvis-exchange-dydx-0.9.5.tar.gz` & `tmp/tarvis-exchange-dydx-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-exchange-dydx-0.9.5.tar", last modified: Wed May  3 01:40:50 2023, max compression
+gzip compressed data, was "tarvis-exchange-dydx-0.9.6.tar", last modified: Sun May 14 09:26:30 2023, max compression
```

## Comparing `tarvis-exchange-dydx-0.9.5.tar` & `tarvis-exchange-dydx-0.9.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:40:50.177733 tarvis-exchange-dydx-0.9.5/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-03 01:40:39.000000 tarvis-exchange-dydx-0.9.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      407 2023-05-03 01:40:50.177733 tarvis-exchange-dydx-0.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-03 01:40:39.000000 tarvis-exchange-dydx-0.9.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 01:40:50.177733 tarvis-exchange-dydx-0.9.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      769 2023-05-03 01:40:39.000000 tarvis-exchange-dydx-0.9.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:40:50.173732 tarvis-exchange-dydx-0.9.5/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:40:50.173732 tarvis-exchange-dydx-0.9.5/tarvis/exchange/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:40:50.177733 tarvis-exchange-dydx-0.9.5/tarvis/exchange/dydx/
--rw-r--r--   0 root         (0) root         (0)     8927 2023-05-03 01:40:39.000000 tarvis-exchange-dydx-0.9.5/tarvis/exchange/dydx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:40:50.177733 tarvis-exchange-dydx-0.9.5/tarvis_exchange_dydx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      407 2023-05-03 01:40:50.000000 tarvis-exchange-dydx-0.9.5/tarvis_exchange_dydx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-03 01:40:50.000000 tarvis-exchange-dydx-0.9.5/tarvis_exchange_dydx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 01:40:50.000000 tarvis-exchange-dydx-0.9.5/tarvis_exchange_dydx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-03 01:40:50.000000 tarvis-exchange-dydx-0.9.5/tarvis_exchange_dydx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 01:40:50.000000 tarvis-exchange-dydx-0.9.5/tarvis_exchange_dydx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:40:50.177733 tarvis-exchange-dydx-0.9.5/test/
--rw-r--r--   0 root         (0) root         (0)    12009 2023-05-03 01:40:39.000000 tarvis-exchange-dydx-0.9.5/test/test_exchange_dydx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:26:30.501865 tarvis-exchange-dydx-0.9.6/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-14 09:26:19.000000 tarvis-exchange-dydx-0.9.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      407 2023-05-14 09:26:30.497864 tarvis-exchange-dydx-0.9.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-14 09:26:19.000000 tarvis-exchange-dydx-0.9.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 09:26:30.501865 tarvis-exchange-dydx-0.9.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      769 2023-05-14 09:26:19.000000 tarvis-exchange-dydx-0.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:26:30.497864 tarvis-exchange-dydx-0.9.6/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:26:30.497864 tarvis-exchange-dydx-0.9.6/tarvis/exchange/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:26:30.497864 tarvis-exchange-dydx-0.9.6/tarvis/exchange/dydx/
+-rw-r--r--   0 root         (0) root         (0)     9045 2023-05-14 09:26:19.000000 tarvis-exchange-dydx-0.9.6/tarvis/exchange/dydx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:26:30.497864 tarvis-exchange-dydx-0.9.6/tarvis_exchange_dydx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-05-14 09:26:30.000000 tarvis-exchange-dydx-0.9.6/tarvis_exchange_dydx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-14 09:26:30.000000 tarvis-exchange-dydx-0.9.6/tarvis_exchange_dydx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:26:30.000000 tarvis-exchange-dydx-0.9.6/tarvis_exchange_dydx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-14 09:26:30.000000 tarvis-exchange-dydx-0.9.6/tarvis_exchange_dydx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 09:26:30.000000 tarvis-exchange-dydx-0.9.6/tarvis_exchange_dydx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:26:30.497864 tarvis-exchange-dydx-0.9.6/test/
+-rw-r--r--   0 root         (0) root         (0)    12356 2023-05-14 09:26:19.000000 tarvis-exchange-dydx-0.9.6/test/test_exchange_dydx.py
```

### Comparing `tarvis-exchange-dydx-0.9.5/LICENSE.txt` & `tarvis-exchange-dydx-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-dydx-0.9.5/setup.py` & `tarvis-exchange-dydx-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-exchange-dydx",
-    version="0.9.5",
+    version="0.9.6",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Exchange Library for dYdX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-exchange-dydx-0.9.5/tarvis/exchange/dydx/__init__.py` & `tarvis-exchange-dydx-0.9.6/tarvis/exchange/dydx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class DYDXExchange(Exchange):
     EXCHANGE_NAME = "dYdX"
 
     _ORDER_TYPE_TO_DYDX = {
         OrderType.MARKET: "MARKET",
         OrderType.LIMIT: "LIMIT",
-        OrderType.STOP_LOSS_MARKET: "STOP_MARKET",
+        OrderType.STOP_LOSS: "STOP_MARKET",
     }
     _ORDER_TYPE_TO_TARVIS = dict(
         (value, key) for key, value in _ORDER_TYPE_TO_DYDX.items()
     )
 
     def __init__(
         self,
@@ -122,22 +122,24 @@
 
             results[base_asset] = size
 
         results["USD"] = Decimal(response.data["account"]["quoteBalance"])
 
         return results
 
-    def get_open_orders(self) -> list[Order]:
+    def get_open_orders(self, base_asset: str, quote_asset: str) -> list[Order]:
         _PAGE_SIZE = 100
-        results = {}
 
+        results = {}
+        market = self._convert_assets_to_market(base_asset, quote_asset)
         page_order_count = _PAGE_SIZE
         start_datetime = None
         while page_order_count == _PAGE_SIZE:
             response = self._client.private.get_orders(
+                market=market,
                 status="PENDING,OPEN,UNTRIGGERED",
                 limit=_PAGE_SIZE,
                 created_before_or_at=start_datetime,
             )
 
             dydx_orders = response.data["orders"]
             page_order_count = len(dydx_orders)
@@ -198,27 +200,27 @@
         stop_loss_price: Decimal = None,
         increasing_position: bool = None,
     ):
         market = self._convert_assets_to_market(base_asset, quote_asset)
         dydx_order_type = self._ORDER_TYPE_TO_DYDX[order_type]
         expiration = int(time.time() + self._order_expiration)
 
-        if order_type == OrderType.STOP_LOSS_MARKET:
+        if order_type == OrderType.STOP_LOSS:
             if stop_loss_price is None:
                 raise ValueError("stop_loss_price is None.")
             if price is None:
                 price = stop_loss_price
             trigger_price = str(stop_loss_price)
         else:
             trigger_price = None
 
         # dYdX requires all orders, even market orders, to have a price
         if price is None:
             raise ValueError("price is None.")
-        if order_type in [OrderType.MARKET, OrderType.STOP_LOSS_MARKET]:
+        if order_type in [OrderType.MARKET, OrderType.STOP_LOSS]:
             if side == OrderSide.BUY:
                 price *= 1 + self._market_limit
             else:
                 price *= 1 - self._market_limit
             price = policy.align_price(price)
 
         if increasing_position is not None:
```

### Comparing `tarvis-exchange-dydx-0.9.5/test/test_exchange_dydx.py` & `tarvis-exchange-dydx-0.9.6/test/test_exchange_dydx.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,22 +47,22 @@
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
@@ -76,15 +76,15 @@
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
@@ -105,45 +105,45 @@
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
@@ -154,15 +154,15 @@
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
@@ -172,15 +172,15 @@
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
@@ -236,15 +236,15 @@
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
@@ -269,45 +269,45 @@
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
@@ -318,15 +318,15 @@
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
@@ -336,15 +336,15 @@
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

