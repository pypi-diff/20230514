# Comparing `tmp/tarvis-btb-0.9.5.tar.gz` & `tmp/tarvis-btb-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-btb-0.9.5.tar", last modified: Wed May  3 01:30:57 2023, max compression
+gzip compressed data, was "tarvis-btb-0.9.6.tar", last modified: Sun May 14 09:04:54 2023, max compression
```

## Comparing `tarvis-btb-0.9.5.tar` & `tarvis-btb-0.9.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:30:57.638990 tarvis-btb-0.9.5/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-03 01:30:57.638990 tarvis-btb-0.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 01:30:57.638990 tarvis-btb-0.9.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      759 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:30:57.630989 tarvis-btb-0.9.5/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:30:57.634990 tarvis-btb-0.9.5/tarvis/btb/
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/tarvis/btb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24506 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/tarvis/btb/basictradingbot.py
--rw-r--r--   0 root         (0) root         (0)     3978 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/tarvis/btb/btbs.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/tarvis/btb/exchangeaccount.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:30:57.634990 tarvis-btb-0.9.5/tarvis_btb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-03 01:30:57.000000 tarvis-btb-0.9.5/tarvis_btb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2023-05-03 01:30:57.000000 tarvis-btb-0.9.5/tarvis_btb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 01:30:57.000000 tarvis-btb-0.9.5/tarvis_btb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-03 01:30:57.000000 tarvis-btb-0.9.5/tarvis_btb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 01:30:57.000000 tarvis-btb-0.9.5/tarvis_btb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:30:57.638990 tarvis-btb-0.9.5/test/
--rw-r--r--   0 root         (0) root         (0)     3152 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/test/test_all.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:04:54.646407 tarvis-btb-0.9.6/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-14 09:04:41.000000 tarvis-btb-0.9.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-14 09:04:54.646407 tarvis-btb-0.9.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-14 09:04:41.000000 tarvis-btb-0.9.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 09:04:54.646407 tarvis-btb-0.9.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      759 2023-05-14 09:04:41.000000 tarvis-btb-0.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:04:54.642406 tarvis-btb-0.9.6/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:04:54.642406 tarvis-btb-0.9.6/tarvis/btb/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-14 09:04:41.000000 tarvis-btb-0.9.6/tarvis/btb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24286 2023-05-14 09:04:41.000000 tarvis-btb-0.9.6/tarvis/btb/basictradingbot.py
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-05-14 09:04:41.000000 tarvis-btb-0.9.6/tarvis/btb/btbs.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-05-14 09:04:41.000000 tarvis-btb-0.9.6/tarvis/btb/exchangeaccount.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:04:54.646407 tarvis-btb-0.9.6/tarvis_btb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-14 09:04:54.000000 tarvis-btb-0.9.6/tarvis_btb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2023-05-14 09:04:54.000000 tarvis-btb-0.9.6/tarvis_btb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:04:54.000000 tarvis-btb-0.9.6/tarvis_btb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 09:04:54.000000 tarvis-btb-0.9.6/tarvis_btb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 09:04:54.000000 tarvis-btb-0.9.6/tarvis_btb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:04:54.646407 tarvis-btb-0.9.6/test/
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-05-14 09:04:41.000000 tarvis-btb-0.9.6/test/test_all.py
```

### Comparing `tarvis-btb-0.9.5/LICENSE.txt` & `tarvis-btb-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.5/setup.py` & `tarvis-btb-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-btb",
-    version="0.9.5",
+    version="0.9.6",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Basic Trading Bot Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-btb-0.9.5/tarvis/btb/basictradingbot.py` & `tarvis-btb-0.9.6/tarvis/btb/basictradingbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,100 +140,100 @@
                 price_allowance = 1 - self._premium_limit
                 stop_loss_price_ratio = 1 + self._stop_loss
             case _:
                 raise ValueError("Indicator direction is invalid.")
 
         positions = exchange.get_positions()
         base_asset_position = positions.get(base_asset, 0)
-        orders = exchange.get_open_orders()
+        orders = exchange.get_open_orders(base_asset, quote_asset)
         quote_price = exchange.get_quote(base_asset, quote_asset)
         trading_policy = exchange.get_policy(base_asset, quote_asset)
         minimum_order_quantity = trading_policy.get_minimum_order_quantity(quote_price)
         flatten_vector = 0
         direction_vector = 0
         stop_loss_orders = []
         stop_loss_vector = 0
 
         for order in orders:
-            if order.quote_asset == quote_asset:
-                cancel_order = False
-                order_vector = order.get_quantity(quote_price) - order.filled_quantity
-
-                # Cancel all (except stop loss) orders placed before the indicator
-                if (order.creation_time < indicator.time) and (
-                    order.order_type != OrderType.STOP_LOSS_MARKET
-                ):
-                    cancel_order = True
+            cancel_order = False
+            order_vector = order.get_quantity(quote_price) - order.filled_quantity
 
-                # Cancel all orders that are not market orders if indicator is flat
-                elif (indicator.direction == MarketPosition.FLAT) and (
-                    order.order_type != OrderType.MARKET
-                ):
-                    cancel_order = True
+            # Cancel all (except stop loss) orders placed before the indicator
+            if (order.creation_time < indicator.time) and (
+                order.order_type != OrderType.STOP_LOSS
+            ):
+                cancel_order = True
 
-                # Cancel all stop loss orders that are not against the
-                elif (order.order_type == OrderType.STOP_LOSS_MARKET) and (
-                    order.side != order_side_opposing
-                ):
-                    cancel_order = True
+            # Cancel all orders that are not market orders if indicator is flat
+            elif (indicator.direction == MarketPosition.FLAT) and (
+                order.order_type != OrderType.MARKET
+            ):
+                cancel_order = True
+
+            # Cancel all stop loss orders that are not against the
+            elif (order.order_type == OrderType.STOP_LOSS) and (
+                order.side != order_side_opposing
+            ):
+                cancel_order = True
 
+            else:
+                if order.side == OrderSide.BUY:
+                    order_vector = order_vector
                 else:
-                    if order.side == OrderSide.BUY:
-                        order_vector = order_vector
+                    order_vector = -order_vector
+
+                # Only cancel the market orders that are not flattening
+                if order.order_type == OrderType.MARKET:
+                    # Cancel all sell orders if current position is short
+                    # Cancel all buy orders if current position is long
+                    # Tally the flattening orders
+                    if (
+                        (order.side == OrderSide.BUY) and (base_asset_position >= 0)
+                    ) or (
+                        (order.side == OrderSide.SELL) and (base_asset_position <= 0)
+                    ):
+                        cancel_order = True
                     else:
-                        order_vector = -order_vector
+                        flatten_vector += order_vector
 
-                    # Only cancel the market orders that are not flattening
-                    if order.order_type == OrderType.MARKET:
-                        # Cancel all sell orders if current position is short
-                        # Cancel all buy orders if current position is long
-                        # Tally the flattening orders
-                        if (
-                            (order.side == OrderSide.BUY) and (base_asset_position >= 0)
-                        ) or (
-                            (order.side == OrderSide.SELL)
-                            and (base_asset_position <= 0)
-                        ):
-                            cancel_order = True
-                        else:
-                            flatten_vector += order_vector
-
-                    # Tally the directional and stop loss orders
-                    elif order.order_type == OrderType.LIMIT:
-                        direction_vector += order_vector
-                    elif order.order_type == OrderType.STOP_LOSS_MARKET:
-                        stop_loss_orders.append(order)
-                        stop_loss_vector += order_vector
+                # Tally the directional and stop loss orders
+                elif order.order_type == OrderType.LIMIT:
+                    direction_vector += order_vector
+                elif order.order_type == OrderType.STOP_LOSS:
+                    stop_loss_orders.append(order)
+                    stop_loss_vector += order_vector
 
-                if cancel_order:
-                    # noinspection PyProtectedMember
-                    self._logger.info(
-                        "Cancelling order.",
-                        extra={
-                            **log_extra_iteration,
-                            "order_side": order.side.name,
-                            "order_type": order.order_type.name,
-                            "order_quantity": str(order._quantity),
-                            "order_amount": str(order._amount),
-                        },
-                    )
-                    exchange.cancel_order(order)
+            if cancel_order:
+                # noinspection PyProtectedMember
+                self._logger.info(
+                    "Cancelling order.",
+                    extra={
+                        **log_extra_iteration,
+                        "order_side": order.side.name,
+                        "order_type": order.order_type.name,
+                        "order_quantity": str(order._quantity),
+                        "order_amount": str(order._amount),
+                    },
+                )
+                exchange.cancel_order(order)
 
         opposing_position = base_asset_position + flatten_vector
         match indicator.direction:
             case MarketPosition.LONG:
                 if opposing_position > 0:
                     opposing_position = 0
             case MarketPosition.SHORT:
                 if opposing_position < 0:
                     opposing_position = 0
         flatten_quantity = abs(trading_policy.align_quantity(opposing_position))
 
         if (flatten_quantity != 0) and (flatten_quantity >= minimum_order_quantity):
-            flatten_quantity = trading_policy.limit_quantity_maximum(flatten_quantity)
+            flatten_quantity = trading_policy.limit_quantity_maximum(
+                flatten_quantity, quote_price
+            )
             if opposing_position > 0:
                 flatten_order_side = OrderSide.SELL
             else:
                 flatten_order_side = OrderSide.BUY
             self._logger.info(
                 "Placing flattening order.",
                 extra={
@@ -278,15 +278,15 @@
                     and (quote_price < (indicator.price * price_deviation_limit))
                 )
             ):
                 self._logger.info(
                     "Directional order not placed due to excessive price deviation.",
                     extra={
                         **log_extra_iteration,
-                        "quote_price": quote_price,
+                        "quote_price": str(quote_price),
                     },
                 )
                 direction_completed = True
 
             # Otherwise, attempt to move in the direction
             else:
                 quote_asset_position = positions.get(quote_asset, 0)
@@ -351,15 +351,15 @@
                     if self._stop_loss == 0:
                         stop_loss_price = None
                     else:
                         stop_loss_price = quote_price * stop_loss_price_ratio
                         stop_loss_price = trading_policy.align_price(stop_loss_price)
 
                     order_quantity = trading_policy.limit_quantity_maximum(
-                        order_quantity
+                        order_quantity, order_price
                     )
                     self._logger.info(
                         "Placing directional order.",
                         extra={
                             **log_extra_iteration,
                             "order_side": order_side.name,
                             "order_quantity": str(order_quantity),
@@ -426,15 +426,15 @@
                     )
                     exchange.cancel_order(order)
 
                 elif stop_loss_quantity >= minimum_order_quantity:
                     stop_loss_price = quote_price * stop_loss_price_ratio
                     stop_loss_price = trading_policy.align_price(stop_loss_price)
                     stop_loss_quantity = trading_policy.limit_quantity_maximum(
-                        stop_loss_quantity
+                        stop_loss_quantity, stop_loss_price
                     )
                     self._logger.info(
                         "Placing stop loss order.",
                         extra={
                             **log_extra_iteration,
                             "order_side": order_side_opposing.name,
                             "order_quantity": str(stop_loss_quantity),
@@ -442,15 +442,15 @@
                         },
                     )
                     exchange.place_order(
                         trading_policy,
                         base_asset,
                         quote_asset,
                         order_side_opposing,
-                        OrderType.STOP_LOSS_MARKET,
+                        OrderType.STOP_LOSS,
                         stop_loss_quantity,
                         stop_loss_price=stop_loss_price,
                         increasing_position=False,
                     )
 
             return direction_completed and stop_loss_completed
```

### Comparing `tarvis-btb-0.9.5/tarvis/btb/btbs.py` & `tarvis-btb-0.9.6/tarvis/btb/btbs.py`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.5/tarvis/btb/exchangeaccount.py` & `tarvis-btb-0.9.6/tarvis/btb/exchangeaccount.py`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.5/test/test_all.py` & `tarvis-btb-0.9.6/test/test_all.py`

 * *Files identical despite different names*

