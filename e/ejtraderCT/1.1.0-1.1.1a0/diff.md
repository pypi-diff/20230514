# Comparing `tmp/ejtraderCT-1.1.0.tar.gz` & `tmp/ejtraderCT-1.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejtraderCT-1.1.0.tar", last modified: Thu Apr 27 18:57:04 2023, max compression
+gzip compressed data, was "ejtraderCT-1.1.1a0.tar", last modified: Sat May 13 22:04:55 2023, max compression
```

## Comparing `ejtraderCT-1.1.0.tar` & `ejtraderCT-1.1.1a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:57:04.942202 ejtraderCT-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-27 18:57:04.942202 ejtraderCT-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:57:04.942202 ejtraderCT-1.1.0/ejtraderCT/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:57:04.942202 ejtraderCT-1.1.0/ejtraderCT/api/
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/api/Symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/api/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17077 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/api/ctrader.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/api/fix.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/ejtraderCT/api/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:57:04.942202 ejtraderCT-1.1.0/ejtraderCT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-27 18:57:04.000000 ejtraderCT-1.1.0/ejtraderCT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-27 18:57:04.000000 ejtraderCT-1.1.0/ejtraderCT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:57:04.000000 ejtraderCT-1.1.0/ejtraderCT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 18:57:04.000000 ejtraderCT-1.1.0/ejtraderCT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 18:57:04.946202 ejtraderCT-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:57:04.942202 ejtraderCT-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-27 18:56:50.000000 ejtraderCT-1.1.0/test/test_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:55.612561 ejtraderCT-1.1.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-13 22:04:55.612561 ejtraderCT-1.1.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:55.612561 ejtraderCT-1.1.1a0/ejtraderCT/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:55.612561 ejtraderCT-1.1.1a0/ejtraderCT/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/api/Symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/api/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/api/ctrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25737 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/api/fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/api/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:55.612561 ejtraderCT-1.1.1a0/ejtraderCT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-13 22:04:55.000000 ejtraderCT-1.1.1a0/ejtraderCT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-13 22:04:55.000000 ejtraderCT-1.1.1a0/ejtraderCT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 22:04:55.000000 ejtraderCT-1.1.1a0/ejtraderCT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-13 22:04:55.000000 ejtraderCT-1.1.1a0/ejtraderCT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-13 22:04:55.616561 ejtraderCT-1.1.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:55.612561 ejtraderCT-1.1.1a0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/test/test_math.py
```

### Comparing `ejtraderCT-1.1.0/LICENSE` & `ejtraderCT-1.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.1.0/PKG-INFO` & `ejtraderCT-1.1.1a0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,11 @@
-Metadata-Version: 2.1
-Name: ejtraderCT
-Version: 1.1.0
-Summary: Ctrader Fix API
-Home-page: https://ejtraderCT.readthedocs.io/
-Download-URL: https://ejtrader.com
-Author: Emerson Pedroso & Douglas Barros
-Author-email: support@ejtrader.com
-License: MIT License
-Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderCT/issues
-Project-URL: Source, https://github.com/traderpedroso/ejtraderCT
-Project-URL: Documentation, https://ejtraderCT.readthedocs.io/
-Keywords: ctrader,fix-api,historical-data,financial-data,stocks,funds,etfs,indices,currency crosses,bonds,commodities,crypto currencies
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Office/Business :: Financial
-Classifier: Topic :: Office/Business :: Financial :: Investment
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![Pypi Publish](https://github.com/ejtraderLabs/ejtraderCT/actions/workflows/python-publish.yml/badge.svg)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderCT)
+[![License](https://img.shields.io/github/license/ejtraderLabs/ejtraderCT)](https://github.com/ejtraderLabs/ejtraderCT/blob/master/LICENSE)
+[![PyPi downloads](https://img.shields.io/pypi/dm/ejtraderCT?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/ejtraderCT/)
 
 # Python Ctrader Fix API
 
 ### ToDo
 
 - [ ] Account Information "not possible fix limitation"
 - [x] Market Position buy and sell
@@ -52,140 +27,158 @@
 ```
 git clone https://github.com/ejtraderLabs/ejtraderCT
 cd ejtraderCT
 python setup.py install
 
 ```
 
-### Import librarys 
+## Accessing the Ctrader FIX API
 
-```python
-from ejtraderCT import Ctrader
 
-import time
-import logging
-from datetime import datetime
+To access your API, follow these simple steps:
+
+1. Open the cTrader desktop or web platform.
+2. In the bottom left corner of the platform, you will find the **Settings** option. Click on it.
+3. A popup window will appear. In the menu of the popup, look for the last option: **FIX API**.
+4. First, click on the **Change Password** button. Make sure to add a numeric password of at least 8 digits.
+5. After changing the password, click on the **Copy to Clipboard** button from  **Trade Connection**.
+6. Now, let's move to the **Trade Connection** section. Here, you will receive your data in the following format (this is an example with IC Markets for a real account):
+
+   - Host name: (Current IP address 168.205.95.20 can be changed without notice)
+   - Port: 5212 (SSL), 5202 (Plain text)
+   - Password: (a/c 1104928 password)
+   - SenderCompID: live.icmarkets.1104926 or demo.icmarkets.1104926  or live2.icmarkets.1104926 
+   - TargetCompID: cServer
+   - SenderSubID: TRADE
 
-logging.getLogger().setLevel(logging.INFO)
 
 
+
+
+### Import libraries
+
+```python
+from ejtraderCT import Ctrader
 ```
 
-### Fix login account and details
+### Fix account login and details
 
 ```python
-server="h8.p.c-trader.cn" # Host name
-broker="icmarkets" 
-account="3152339"
-password="393214"
-currency="EUR"
+server="168.205.95.20" # - Host name: (Current IP address 168.205.95.20 can be changed without notice)
+account="live.icmarkets.1104926" #  - SenderCompID: live.icmarkets.1104928
+password="12345678" # - The password you configured
 
-api = Ctrader(server,broker,account,password,currency)
+api = Ctrader(server,account,password)
 
 ```
 
-##### to Disconnect logout from account 
+##### To disconnect and logout from the account
 ```python
 api.logout()
 ```
 
-### Real time quote
+### Real-time quote
 
-##### Subscribe to symbol 
+##### Subscribe to symbols
 ```python
 api.subscribe("EURUSD", "GBPUSD")
 ```
-##### All symbols quote list
+##### List of quotes for all symbols
 ```python
 quote = api.quote()
 print(quote)
 
 # Output
 
 {'EURUSD': {'bid': 1.02616, 'ask': 1.02618}, 'GBPUSD': {'bid': 1.21358, 'ask': 1.21362}}
 ```
 
-#### Single symbol quote 
+#### Quote for a single symbol 
 ```python
 quote = api.quote("EURUSD")
 print(quote)
 
 # Output
 
 {'bid': 1.02612, 'ask': 1.02614}
 
 ```
-### Market position and pending order.
+### Market position and pending orders.
 
-##### Market Position
+##### Market position
 
 ```python
 # Buy position
 
 symbol = "EURUSD"
-volume = 0.01 # position size
+volume = 0.01 # position size:
 stoploss =  1.18
 takeprofit = 1.19
 
-api.buy(symbol, volume, stoploss, takeprofit)
+id = api.buy(symbol, volume, stoploss, takeprofit)
+print(f"Position: {id}")
 
 # sell position 
 
 symbol = "EURUSD"
 volume = 0.01 # position size
 stoploss = 1.19
 takeprofit = 1.18
 
-api.sell(symbol, volume, stoploss, takeprofit)
+id = api.sell(symbol, volume, stoploss, takeprofit)
+print(f"Position: {id}")
 ```
 
-##### Limit Orders 
+##### Limit Orders
 
 ```python
 
 # Buy limit order
 
 symbol = "EURUSD"
-volume = 0.01 # position size
+volume = 0.01 # order size
 stoploss = 1.17
 takeprofit = 1.19
 price = 1.18 # entry price 
 
-api.buyLimit(symbol, volume, stoploss, takeprofit, price)
+id = api.buyLimit(symbol, volume, stoploss, takeprofit, price)
+print(f"Order: {id}")
 
 
 # Sell limit order
 
 symbol = "EURUSD"
-volume = 0.01 # position size
+volume = 0.01 # Order size
 stoploss = 1.23
 takeprofit = 1.17
 price = 1.22 # entry price 
 
-api.sellLimit(symbol, volume, stoploss, takeprofit, price)
+id = api.sellLimit(symbol, volume, stoploss, takeprofit, price)
+print(f"Order: {id}")
 ```
 
 #### Stop Orders
 
 ```python
 
 # Buy stop order
 
 symbol = "EURUSD"
-volume = 0.01 # position size
+volume = 0.01 # order size
 stoploss = 1.20
 takeprofit = 1.24
 price = 1.22 # entry price
 
-api.buyStop(symbol, volume, stoploss, takeprofit, price)
+id = api.buyStop(symbol, volume, stoploss, takeprofit, price)
+print(f"Order: {id}")
 
 # Sell stop order
 
 symbol = "EURUSD"
-volume = 0.01 # position size
+volume = 0.01 # order size
 stoploss = 1.19
 takeprofit = 1.17
 price = 1.18 # entry price 
 
 api.sellStop(symbol, volume, stoploss, takeprofit, price)
 
 ```
@@ -200,15 +193,15 @@
 #### List limit and stop Orders
 
 ```python
 orders = api.orders()
 print(orders)
 
 ```
-#### Cancle order by id
+#### Cancel order by id
 
 ```python
 orders = api.orders()
 for order in orders:
     api.orderCancelById(order['ord_id'])
 
 ```
@@ -216,42 +209,46 @@
 
 ```python
 for position in positions:
     api.positionCloseById(position['pos_id'], position['amount'])
 
 ```
 
-#### cancel all Orders
+#### Cancel all orders
 
 ```python
 api.cancel_all()
 ```
 
-#### close all positions
+#### Close all positions
 
 ```python
 api.close_all()
 ```
-#### Modify Position SL and TP
+#### Modify position SL and TP
 ```python
 id = "position id "
 stoploss = "stop loss price""
 takeprofit "stop gain price"
 
 api.positionModify(id, stoploss, takeprofit)
 
 ```
 
-#### Modify order Order SL and TP and entry price
+#### Modify order SL and TP and entry price
 ```python
 id = "order id "
 stoploss = "stop loss price""
 takeprofit= "stop gain price"
 price = "limit or stop entry price"
 
 api.orderModify(id, stoploss, takeprofit, price)
 
 ```
+## Contributors:
+
+<!-- CONTRIBUTORS:START -->
+<!-- CONTRIBUTORS:END -->
+
+## Acknowledgements
 
-# Thanks for 
-@HarukaMa
-@douglasbarros
+I would like to express my gratitude to [@HarukaMa](https://github.com/HarukaMa) for creating the initial project. Their work has been an invaluable starting point for my modifications and improvements.
```

### Comparing `ejtraderCT-1.1.0/ejtraderCT/api/Symbol.py` & `ejtraderCT-1.1.1a0/ejtraderCT/api/Symbol.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.1.0/ejtraderCT/api/ctrader.py` & `ejtraderCT-1.1.1a0/ejtraderCT/api/ctrader.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 import random
 import os
 from operator import itemgetter
 from .fix import FIX, Side, OrderType
 from .Symbol import SYMBOLSLIST
 class Ctrader:
 
-    def __init__(self,server,broker,login,password,currency):
+    def __init__(self,server,account,password,debug=False):
         """AI is creating summary for __init__
 
         Args:
             server ([str]): [example h8.p.c-trader.cn]
-            broker ([str]): [icmarkets]
-            login ([str]): [3152339]
-            password ([str]): [example 123456 need to setup when you create api on ctrader platform]
-            currency ([str]): [EUR deprecating won need anymore for next version]
+            account ([str]): [live.icmarkets.1104926 or demo.icmarkets.1104926]
+            password ([str]): [example 12345678 need to setup when you create api on ctrader platform]
         """
+        if debug:
+            logging.getLogger().setLevel(logging.INFO)
+        split_string = account.split(".")
+        broker = split_string[0] + "." + split_string[1]
+        login = split_string[2]
+        currency = "EUR"
         self.client = c = {
             '_id': '1',
             'server': server,
             'broker': broker,
             'login': login,
             'password': password,
             'currency': currency,
@@ -416,7 +420,8 @@
         self.fix.close_all()
     
     def cancel_all(self):
         self.fix.cancel_all()
         
     def logout(self):
         self.fix.logout()
+
```

### Comparing `ejtraderCT-1.1.0/ejtraderCT/api/fix.py` & `ejtraderCT-1.1.1a0/ejtraderCT/api/fix.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,90 +186,95 @@
                 cksm = sum(data.replace("|", "\x01").encode()) % 256
                 data += "10=%03d|" % cksm
             return data
 
         def __repr__(self):
             return pformat([(k.name, v) for k, v in self.fields])
 
-    def __init__(self, server: str, broker: str, login: str, password: str, currency: str, client_id: str, position_list_callback, order_list_callback):
-        self.qstream = Buffer()
-        self.qs = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.qs.connect((server, 5201))
-        self.tstream = Buffer()
-        self.ts = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.ts.connect((server, 5202))
-        self.broker = broker
-        self.login = login
-        self.password = password
-        self.currency = currency
-        self.client_id = client_id
-        self.qseq = 1
-        self.tseq = 1
-        self.qtest_seq = 1
-        self.ttest_seq = 1
-        self.market_seq = 1
-        self.subscribed_symbol = [-1, -1, -1]
-        self.qworker_thread = threading.Thread(target=self.qworker)
-        self.qworker_thread.start()
-        self.tworker_thread = threading.Thread(target=self.tworker)
-        self.tworker_thread.start()
-        self.ping_qworker_thread = None
-        self.ping_tworker_thread = None
-        self.sec_list_callback = None
-        self.market_callback = None
-        self.sec_id_table = {}
-        self.sec_name_table = {}
-        self.position_list_callback = position_list_callback
-        self.order_list_callback = order_list_callback
-        self.market_data = {}
-        self.position_list = {}
-        self.spot_request_list = set()
-        self.spot_price_list = {}
-        self.base_convert_request_list = set()
-        self.base_convert_list = {}
-        self.order_list = {}
-        self.origin_to_pos_id = {}
-        self.origin_to_ord_id = {}
-        self.logged = False
-        self.logon()
-        self.sec_list_evt = threading.Event()
-        self.thread_sec_list = threading.Thread(target=self.sec_list)
-        self.thread_sec_list.start()
-        self.sec_list_evt.wait()
+    def __init__(self, server: str, broker: str, login: str, password: str, currency: str, client_id: str, position_list_callback, order_list_callback,update_fix_status=None):
+        try:
+            self.qstream = Buffer()
+            self.qs = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            self.qs.connect((server, 5201))
+            self.tstream = Buffer()
+            self.ts = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            self.ts.connect((server, 5202))
+            self.broker = broker
+            self.login = login
+            self.password = password
+            self.currency = currency
+            self.client_id = client_id
+            self.qseq = 1
+            self.tseq = 1
+            self.qtest_seq = 1
+            self.ttest_seq = 1
+            self.market_seq = 1
+            self.subscribed_symbol = [-1, -1, -1]
+            self.qworker_thread = threading.Thread(target=self.qworker)
+            self.qworker_thread.start()
+            self.tworker_thread = threading.Thread(target=self.tworker)
+            self.tworker_thread.start()
+            self.ping_qworker_thread = None
+            self.ping_tworker_thread = None
+            self.sec_list_callback = None
+            self.market_callback = None
+            self.sec_id_table = {}
+            self.sec_name_table = {}
+            self.position_list_callback = position_list_callback
+            self.order_list_callback = order_list_callback
+            self.update_fix_status = update_fix_status
+            self.market_data = {}
+            self.position_list = {}
+            self.spot_request_list = set()
+            self.spot_price_list = {}
+            self.base_convert_request_list = set()
+            self.base_convert_list = {}
+            self.order_list = {}
+            self.origin_to_pos_id = {}
+            self.origin_to_ord_id = {}
+            self.logged = False
+            self.logon()
+            self.sec_list_evt = threading.Event()
+            self.thread_sec_list = threading.Thread(target=self.sec_list)
+            self.thread_sec_list.start()
+            self.sec_list_evt.wait()
+        except Exception as e:
+            # Code to handle the exception
+            logging.error(f"{e}")
 
     def qworker(self):
         while True:
             try:
                 data = self.qs.recv(65535)
             except:
                 break
             if len(data) == 0:
-                logging.error("Disconnected")
+                print("Quote Logged out")
                 break
             try:
                 self.qstream.write(data)
                 self.parse_quote_message()
             except:
                 print("Market is Close or Disconnected")
                 break
 
     def tworker(self):
         while True:
             try:
                 data = self.ts.recv(65535)
-            except:
+            except Exception as e:
                 break
             if len(data) == 0:
-                logging.error("Disconnected")
+                print("Trade Logged out")
                 break
             try:
                 self.tstream.write(data)
                 self.parse_trade_message()
-            except:
-                print("Market is Close or Disconnected")
+            except Exception as e:
+                print(f"Market is Close or Logged out {e}")
                 break
 
     def parse_quote_message(self):
         while len(self.qstream) > 0:
             match = re.search(rb"10=\d{3}\x01", self.qstream.peek(self.qstream.count()))
             if match:
                 msg = FIX.Message()
@@ -316,17 +321,19 @@
     def process_test(self, msg):
         if msg[Field.SenderSubID] == "QUOTE":
             self.qheartbeat(msg[Field.TestReqID])
         elif msg[Field.SenderSubID] == "TRADE":
             self.theartbeat(msg[Field.TestReqID])
 
     def process_logout(self, msg):
-        logging.error("Logged out: %s" % msg[Field.Text])
         if msg[Field.Text] == None:
             self.logged = False
+        self.update_fix_status(self.client_id, self.logged)
+            
+       
 
     def process_exec_report(self, msg):
         if msg[Field.ExecType] == "F":
             self.position_list = {}
             self.position_request()
             self.order_list = {}
             self.origin_to_pos_id[msg[Field.ClOrdId]] = msg[Field.PosMaintRptID]
@@ -362,20 +369,20 @@
                     self.order_list[msg[Field.OrderID]]["price"] = float(msg[Field.StopPx])
             if name not in self.spot_request_list:
                 self.spot_market_request(name)
             self.order_list_callback(self.order_list, self.spot_price_list, self.client_id)
 
     def process_logon(self, msg):
         if msg[Field.SenderSubID] == "QUOTE":
-            logging.info("Quote logged on - client_id %s" % self.client_id)
+            print("Quote logged on")
             self.ping_qworker_thread = threading.Thread(target=self.ping_qworker, args=[int(msg[Field.HeartBtInt])])
             self.ping_qworker_thread.start()
             self.logged = True
         elif msg[Field.SenderSubID] == "TRADE":
-            logging.info("Trade logged on - client_id %s" % self.client_id)
+            print("Trade logged on")
             self.ping_tworker_thread = threading.Thread(target=self.ping_tworker, args=[int(msg[Field.HeartBtInt])])
             self.ping_tworker_thread.start()
 
     def process_market_data(self, msg: Message):
         name = self.sec_id_table[int(msg[Field.Symbol])]["name"]
         digits = self.sec_id_table[int(msg[Field.Symbol])]["digits"]
         entries = msg.get_repeating_groups(Field.NoMDEntries, Field.MDEntryType)
@@ -461,16 +468,20 @@
             self.position_list[msg[Field.PosMaintRptID]]["convert"] = pair
             self.position_list[msg[Field.PosMaintRptID]]["convert_dir"] = conv_dir
             if pair not in self.spot_request_list:
                 self.spot_market_request(pair)
         self.position_list_callback(self.position_list, self.spot_price_list, self.client_id)
 
     def process_reject(self, msg):
-        logging.error(msg[Field.Text])
-
+        checkOrders = msg[Field.Text].split(":")[1]
+        if checkOrders == "no orders found":
+            print("No Orders")
+        else:
+            logging.error(checkOrders)
+       
     message_dispatch = {
         "0": process_ping,
         "1": process_test,
         "3": process_reject,
         "5": process_logout,
         "8": process_exec_report,
         "9": process_reject,
@@ -617,15 +628,14 @@
         msg[Field.Side] = side.value
         msg[Field.TransactTime] = get_time()
         msg[Field.OrderQty] = size
         msg[Field.OrdType] = OrderType.Market.value
         msg[Field.Designation] = "test label"
         if pos_id:
             msg[Field.PosMaintRptID] = pos_id
-        print(msg)
         self.send_message(msg)
 
     def close_position(self, pos_id: str, lots):
         if pos_id not in self.position_list:
             return
 
         # remove referencia ao server ord_id da tabela de-para
```

### Comparing `ejtraderCT-1.1.0/ejtraderCT/api/math.py` & `ejtraderCT-1.1.1a0/ejtraderCT/api/math.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.1.0/ejtraderCT.egg-info/PKG-INFO` & `ejtraderCT-1.1.1a0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ejtraderCT
-Version: 1.1.0
+Version: 1.1.1a0
 Summary: Ctrader Fix API
 Home-page: https://ejtraderCT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso & Douglas Barros
 Author-email: support@ejtrader.com
-License: MIT License
+License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderCT/issues
 Project-URL: Source, https://github.com/traderpedroso/ejtraderCT
 Project-URL: Documentation, https://ejtraderCT.readthedocs.io/
 Keywords: ctrader,fix-api,historical-data,financial-data,stocks,funds,etfs,indices,currency crosses,bonds,commodities,crypto currencies
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -23,14 +23,17 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Pypi Publish](https://github.com/ejtraderLabs/ejtraderCT/actions/workflows/python-publish.yml/badge.svg)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderCT)
+[![License](https://img.shields.io/github/license/ejtraderLabs/ejtraderCT)](https://github.com/ejtraderLabs/ejtraderCT/blob/master/LICENSE)
+[![PyPi downloads](https://img.shields.io/pypi/dm/ejtraderCT?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/ejtraderCT/)
 
 # Python Ctrader Fix API
 
 ### ToDo
 
 - [ ] Account Information "not possible fix limitation"
 - [x] Market Position buy and sell
@@ -52,140 +55,158 @@
 ```
 git clone https://github.com/ejtraderLabs/ejtraderCT
 cd ejtraderCT
 python setup.py install
 
 ```
 
-### Import librarys 
+## Accessing the Ctrader FIX API
 
-```python
-from ejtraderCT import Ctrader
 
-import time
-import logging
-from datetime import datetime
+To access your API, follow these simple steps:
+
+1. Open the cTrader desktop or web platform.
+2. In the bottom left corner of the platform, you will find the **Settings** option. Click on it.
+3. A popup window will appear. In the menu of the popup, look for the last option: **FIX API**.
+4. First, click on the **Change Password** button. Make sure to add a numeric password of at least 8 digits.
+5. After changing the password, click on the **Copy to Clipboard** button from  **Trade Connection**.
+6. Now, let's move to the **Trade Connection** section. Here, you will receive your data in the following format (this is an example with IC Markets for a real account):
+
+   - Host name: (Current IP address 168.205.95.20 can be changed without notice)
+   - Port: 5212 (SSL), 5202 (Plain text)
+   - Password: (a/c 1104928 password)
+   - SenderCompID: live.icmarkets.1104926 or demo.icmarkets.1104926  or live2.icmarkets.1104926 
+   - TargetCompID: cServer
+   - SenderSubID: TRADE
 
-logging.getLogger().setLevel(logging.INFO)
 
 
+
+
+### Import libraries
+
+```python
+from ejtraderCT import Ctrader
 ```
 
-### Fix login account and details
+### Fix account login and details
 
 ```python
-server="h8.p.c-trader.cn" # Host name
-broker="icmarkets" 
-account="3152339"
-password="393214"
-currency="EUR"
+server="168.205.95.20" # - Host name: (Current IP address 168.205.95.20 can be changed without notice)
+account="live.icmarkets.1104926" #  - SenderCompID: live.icmarkets.1104928
+password="12345678" # - The password you configured
 
-api = Ctrader(server,broker,account,password,currency)
+api = Ctrader(server,account,password)
 
 ```
 
-##### to Disconnect logout from account 
+##### To disconnect and logout from the account
 ```python
 api.logout()
 ```
 
-### Real time quote
+### Real-time quote
 
-##### Subscribe to symbol 
+##### Subscribe to symbols
 ```python
 api.subscribe("EURUSD", "GBPUSD")
 ```
-##### All symbols quote list
+##### List of quotes for all symbols
 ```python
 quote = api.quote()
 print(quote)
 
 # Output
 
 {'EURUSD': {'bid': 1.02616, 'ask': 1.02618}, 'GBPUSD': {'bid': 1.21358, 'ask': 1.21362}}
 ```
 
-#### Single symbol quote 
+#### Quote for a single symbol 
 ```python
 quote = api.quote("EURUSD")
 print(quote)
 
 # Output
 
 {'bid': 1.02612, 'ask': 1.02614}
 
 ```
-### Market position and pending order.
+### Market position and pending orders.
 
-##### Market Position
+##### Market position
 
 ```python
 # Buy position
 
 symbol = "EURUSD"
-volume = 0.01 # position size
+volume = 0.01 # position size:
 stoploss =  1.18
 takeprofit = 1.19
 
-api.buy(symbol, volume, stoploss, takeprofit)
+id = api.buy(symbol, volume, stoploss, takeprofit)
+print(f"Position: {id}")
 
 # sell position 
 
 symbol = "EURUSD"
 volume = 0.01 # position size
 stoploss = 1.19
 takeprofit = 1.18
 
-api.sell(symbol, volume, stoploss, takeprofit)
+id = api.sell(symbol, volume, stoploss, takeprofit)
+print(f"Position: {id}")
 ```
 
-##### Limit Orders 
+##### Limit Orders
 
 ```python
 
 # Buy limit order
 
 symbol = "EURUSD"
-volume = 0.01 # position size
+volume = 0.01 # order size
 stoploss = 1.17
 takeprofit = 1.19
 price = 1.18 # entry price 
 
-api.buyLimit(symbol, volume, stoploss, takeprofit, price)
+id = api.buyLimit(symbol, volume, stoploss, takeprofit, price)
+print(f"Order: {id}")
 
 
 # Sell limit order
 
 symbol = "EURUSD"
-volume = 0.01 # position size
+volume = 0.01 # Order size
 stoploss = 1.23
 takeprofit = 1.17
 price = 1.22 # entry price 
 
-api.sellLimit(symbol, volume, stoploss, takeprofit, price)
+id = api.sellLimit(symbol, volume, stoploss, takeprofit, price)
+print(f"Order: {id}")
 ```
 
 #### Stop Orders
 
 ```python
 
 # Buy stop order
 
 symbol = "EURUSD"
-volume = 0.01 # position size
+volume = 0.01 # order size
 stoploss = 1.20
 takeprofit = 1.24
 price = 1.22 # entry price
 
-api.buyStop(symbol, volume, stoploss, takeprofit, price)
+id = api.buyStop(symbol, volume, stoploss, takeprofit, price)
+print(f"Order: {id}")
 
 # Sell stop order
 
 symbol = "EURUSD"
-volume = 0.01 # position size
+volume = 0.01 # order size
 stoploss = 1.19
 takeprofit = 1.17
 price = 1.18 # entry price 
 
 api.sellStop(symbol, volume, stoploss, takeprofit, price)
 
 ```
@@ -200,15 +221,15 @@
 #### List limit and stop Orders
 
 ```python
 orders = api.orders()
 print(orders)
 
 ```
-#### Cancle order by id
+#### Cancel order by id
 
 ```python
 orders = api.orders()
 for order in orders:
     api.orderCancelById(order['ord_id'])
 
 ```
@@ -216,42 +237,46 @@
 
 ```python
 for position in positions:
     api.positionCloseById(position['pos_id'], position['amount'])
 
 ```
 
-#### cancel all Orders
+#### Cancel all orders
 
 ```python
 api.cancel_all()
 ```
 
-#### close all positions
+#### Close all positions
 
 ```python
 api.close_all()
 ```
-#### Modify Position SL and TP
+#### Modify position SL and TP
 ```python
 id = "position id "
 stoploss = "stop loss price""
 takeprofit "stop gain price"
 
 api.positionModify(id, stoploss, takeprofit)
 
 ```
 
-#### Modify order Order SL and TP and entry price
+#### Modify order SL and TP and entry price
 ```python
 id = "order id "
 stoploss = "stop loss price""
 takeprofit= "stop gain price"
 price = "limit or stop entry price"
 
 api.orderModify(id, stoploss, takeprofit, price)
 
 ```
+## Contributors:
+
+<!-- CONTRIBUTORS:START -->
+<!-- CONTRIBUTORS:END -->
+
+## Acknowledgements
 
-# Thanks for 
-@HarukaMa
-@douglasbarros
+I would like to express my gratitude to [@HarukaMa](https://github.com/HarukaMa) for creating the initial project. Their work has been an invaluable starting point for my modifications and improvements.
```

### Comparing `ejtraderCT-1.1.0/setup.py` & `ejtraderCT-1.1.1a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
         for line in f.readlines():
             reqs.append(line.strip())
     return reqs
 
 
 setup(
     name='ejtraderCT',
-    version='1.1.0',
+    version='1.1.1a',
     packages=find_packages(),
     url='https://ejtraderCT.readthedocs.io/',
     download_url='https://ejtrader.com',
-    license='MIT License',
+    license='GPL-3.0',
     author='Emerson Pedroso & Douglas Barros',
     author_email='support@ejtrader.com',
     description='Ctrader Fix API',
     long_description=readme(),
     long_description_content_type='text/markdown',
     install_requires=requirements(filename='requirements.txt'),
     include_package_data=True,
```

### Comparing `ejtraderCT-1.1.0/test/test_math.py` & `ejtraderCT-1.1.1a0/test/test_math.py`

 * *Files identical despite different names*

