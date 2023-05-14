# Comparing `tmp/uuyoupinapi-0.0.2.tar.gz` & `tmp/uuyoupinapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uuyoupinapi-0.0.2.tar", last modified: Sat Apr 22 08:04:25 2023, max compression
+gzip compressed data, was "uuyoupinapi-0.0.3.tar", last modified: Sat May 13 15:07:36 2023, max compression
```

## Comparing `uuyoupinapi-0.0.2.tar` & `uuyoupinapi-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 08:04:25.091061 uuyoupinapi-0.0.2/
--rw-rw-rw-   0        0        0    35823 2023-04-22 06:02:59.000000 uuyoupinapi-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      432 2023-04-22 08:04:25.090060 uuyoupinapi-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-22 08:04:25.091061 uuyoupinapi-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      475 2023-04-22 08:04:03.000000 uuyoupinapi-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 08:04:25.085061 uuyoupinapi-0.0.2/uuyoupinapi/
--rw-rw-rw-   0        0        0     5093 2023-04-22 08:02:17.000000 uuyoupinapi-0.0.2/uuyoupinapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 08:04:25.089061 uuyoupinapi-0.0.2/uuyoupinapi.egg-info/
--rw-rw-rw-   0        0        0      432 2023-04-22 08:04:25.000000 uuyoupinapi-0.0.2/uuyoupinapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-04-22 08:04:25.000000 uuyoupinapi-0.0.2/uuyoupinapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 08:04:25.000000 uuyoupinapi-0.0.2/uuyoupinapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-22 08:04:25.000000 uuyoupinapi-0.0.2/uuyoupinapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-13 15:07:36.479343 uuyoupinapi-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-04-22 06:02:59.000000 uuyoupinapi-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      432 2023-05-13 15:07:36.479343 uuyoupinapi-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2023-05-13 15:05:54.000000 uuyoupinapi-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-13 15:07:36.480343 uuyoupinapi-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      475 2023-05-13 15:05:09.000000 uuyoupinapi-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-13 15:07:36.474343 uuyoupinapi-0.0.3/uuyoupinapi/
+-rw-rw-rw-   0        0        0     5186 2023-05-13 15:05:32.000000 uuyoupinapi-0.0.3/uuyoupinapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-13 15:07:36.478343 uuyoupinapi-0.0.3/uuyoupinapi.egg-info/
+-rw-rw-rw-   0        0        0      432 2023-05-13 15:07:36.000000 uuyoupinapi-0.0.3/uuyoupinapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-05-13 15:07:36.000000 uuyoupinapi-0.0.3/uuyoupinapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-13 15:07:36.000000 uuyoupinapi-0.0.3/uuyoupinapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-13 15:07:36.000000 uuyoupinapi-0.0.3/uuyoupinapi.egg-info/top_level.txt
```

### Comparing `uuyoupinapi-0.0.2/LICENSE` & `uuyoupinapi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uuyoupinapi-0.0.2/uuyoupinapi/__init__.py` & `uuyoupinapi-0.0.3/uuyoupinapi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,29 +96,29 @@
         """
         return self.call_api('POST', '/api/youpin/bff/trade/v1/order/query/detail', data={
             "orderNo": order_id
         }).json()['data']['tradeOfferId']
 
     def get_wait_deliver_list(self, game_id=730, return_offer_id=True):
         """
-        获取待发货列表
+        获取待发货列表（出售）
         :param return_offer_id: 默认为True，是否返回steam交易报价号
         :param game_id: 游戏ID，默认为730(CSGO)
         :return: 待发货列表，格式为[{'order_id': '订单号', 'item_name': '物品名称', 'offer_id': 'steam交易报价号'}... , ...]
         """
         data = self.call_api('POST', '/api/youpin/bff/trade/sell/page/v1/waitDeliver/waitDeliverList', data={
             "gameId": game_id,
             "pageIndex": 1,
             "pageSize": 1000
         })
         wait_deliver_list = data.json()['data']['waitDeliverList']
         data_to_return = []
         if wait_deliver_list is not None:
             for item in wait_deliver_list:
-                dict_to_append = dict()
-                dict_to_append['order_id'] = item['orderInfoVO']['orderNo']
-                dict_to_append['item_name'] = item['commodityInfoVO']['commodityName']
-                if return_offer_id:
-                    dict_to_append['offer_id'] = self.get_steam_offer_id_by_order_id(dict_to_append['order_id'])
-                data_to_return.append(dict_to_append)
+                if item['orderInfoVO']['orderType'] == 1:
+                    dict_to_append = dict()
+                    dict_to_append['order_id'] = item['orderInfoVO']['orderNo']
+                    dict_to_append['item_name'] = item['commodityInfoVO']['commodityName']
+                    if return_offer_id:
+                        dict_to_append['offer_id'] = self.get_steam_offer_id_by_order_id(dict_to_append['order_id'])
+                    data_to_return.append(dict_to_append)
         return data_to_return
-
```

