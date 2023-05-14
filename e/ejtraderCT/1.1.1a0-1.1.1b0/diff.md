# Comparing `tmp/ejtraderCT-1.1.1a0.tar.gz` & `tmp/ejtraderCT-1.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejtraderCT-1.1.1a0.tar", last modified: Sat May 13 22:04:55 2023, max compression
+gzip compressed data, was "ejtraderCT-1.1.1b0.tar", last modified: Sun May 14 04:36:05 2023, max compression
```

## Comparing `ejtraderCT-1.1.1a0.tar` & `ejtraderCT-1.1.1b0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:55.612561 ejtraderCT-1.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-13 22:04:55.612561 ejtraderCT-1.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:55.612561 ejtraderCT-1.1.1a0/ejtraderCT/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:55.612561 ejtraderCT-1.1.1a0/ejtraderCT/api/
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/api/Symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/api/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/api/ctrader.py
--rw-r--r--   0 runner    (1001) docker     (123)    25737 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/api/fix.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/ejtraderCT/api/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:55.612561 ejtraderCT-1.1.1a0/ejtraderCT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-13 22:04:55.000000 ejtraderCT-1.1.1a0/ejtraderCT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-13 22:04:55.000000 ejtraderCT-1.1.1a0/ejtraderCT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 22:04:55.000000 ejtraderCT-1.1.1a0/ejtraderCT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-13 22:04:55.000000 ejtraderCT-1.1.1a0/ejtraderCT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-13 22:04:55.616561 ejtraderCT-1.1.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:04:55.612561 ejtraderCT-1.1.1a0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-13 22:04:42.000000 ejtraderCT-1.1.1a0/test/test_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:36:05.963381 ejtraderCT-1.1.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-14 04:36:05.963381 ejtraderCT-1.1.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:36:05.959381 ejtraderCT-1.1.1b0/ejtraderCT/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:36:05.963381 ejtraderCT-1.1.1b0/ejtraderCT/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/api/Symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/api/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/api/ctrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26527 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/api/fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/ejtraderCT/api/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:36:05.959381 ejtraderCT-1.1.1b0/ejtraderCT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-14 04:36:05.000000 ejtraderCT-1.1.1b0/ejtraderCT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-14 04:36:05.000000 ejtraderCT-1.1.1b0/ejtraderCT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 04:36:05.000000 ejtraderCT-1.1.1b0/ejtraderCT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-14 04:36:05.000000 ejtraderCT-1.1.1b0/ejtraderCT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-14 04:36:05.963381 ejtraderCT-1.1.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 04:36:05.963381 ejtraderCT-1.1.1b0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-14 04:35:48.000000 ejtraderCT-1.1.1b0/test/test_math.py
```

### Comparing `ejtraderCT-1.1.1a0/LICENSE` & `ejtraderCT-1.1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.1.1a0/PKG-INFO` & `ejtraderCT-1.1.1b0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderCT
-Version: 1.1.1a0
+Version: 1.1.1b0
 Summary: Ctrader Fix API
 Home-page: https://ejtraderCT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso & Douglas Barros
 Author-email: support@ejtrader.com
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderCT/issues
@@ -12,14 +12,16 @@
 Project-URL: Documentation, https://ejtraderCT.readthedocs.io/
 Keywords: ctrader,fix-api,historical-data,financial-data,stocks,funds,etfs,indices,currency crosses,bonds,commodities,crypto currencies
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
@@ -29,38 +31,43 @@
 ![Pypi Publish](https://github.com/ejtraderLabs/ejtraderCT/actions/workflows/python-publish.yml/badge.svg)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderCT)
 [![License](https://img.shields.io/github/license/ejtraderLabs/ejtraderCT)](https://github.com/ejtraderLabs/ejtraderCT/blob/master/LICENSE)
 [![PyPi downloads](https://img.shields.io/pypi/dm/ejtraderCT?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/ejtraderCT/)
 
 # Python Ctrader Fix API
 
-### ToDo
+`ejtraderCT` is a Python library to access the Ctrader trading platform's FIX API.
+
+## Features
 
-- [ ] Account Information "not possible fix limitation"
 - [x] Market Position buy and sell
-- [x] Peding orders limit and stop 
+- [x] Pending orders limit and stop 
 - [x] Partial close
 - [x] Stop loss & Take profit
 - [x] Modify Orders 
 - [x] Modify position 
-- [x] real time bid & ask
+- [x] Real-time bid & ask
+- [x] Check connection status
+- [ ] Rest API server (in development)
+- [ ] Webhook for Tradingviewer (in development)
+
+## Prerequisites
 
+The library has been tested on Python 3.7 to 3.9.
 
 ## Installation
-#### Tested on python 3.7 to 3.9
-```
-pip install ejtraderCT -U
-```
-#### Or install from source
 
-```
-git clone https://github.com/ejtraderLabs/ejtraderCT
-cd ejtraderCT
-python setup.py install
+To install the latest version of `ejtraderCT`, you can use pip:
 
+```shell
+pip install ejtraderCT -U
+```
+Or if you want to install from source, you can use:
+```shell
+pip install git+https://github.com/ejtraderLabs/ejtraderCT.git
 ```
 
 ## Accessing the Ctrader FIX API
 
 
 To access your API, follow these simple steps:
 
@@ -94,21 +101,24 @@
 server="168.205.95.20" # - Host name: (Current IP address 168.205.95.20 can be changed without notice)
 account="live.icmarkets.1104926" #  - SenderCompID: live.icmarkets.1104928
 password="12345678" # - The password you configured
 
 api = Ctrader(server,account,password)
 
 ```
-
-##### To disconnect and logout from the account
+##### Check the connection status
+```python
+api.isconnected()
+```
+##### Logout 
 ```python
 api.logout()
 ```
 
-### Real-time quote
+#### Real-time quote
 
 ##### Subscribe to symbols
 ```python
 api.subscribe("EURUSD", "GBPUSD")
 ```
 ##### List of quotes for all symbols
 ```python
@@ -268,15 +278,20 @@
 stoploss = "stop loss price""
 takeprofit= "stop gain price"
 price = "limit or stop entry price"
 
 api.orderModify(id, stoploss, takeprofit, price)
 
 ```
-## Contributors:
+## Contributing
 
-<!-- CONTRIBUTORS:START -->
-<!-- CONTRIBUTORS:END -->
+We welcome any contribution to `ejtraderCT`. Here are some ways to contribute:
+
+1. Report issues or suggest improvements by opening an [issue](https://github.com/ejtraderLabs/ejtraderCT/issues).
+2. Contribute with code to fix issues or add features via a [Pull Request](https://github.com/ejtraderLabs/ejtraderCT/pulls).
+
+Before submitting a pull request, please make sure your codes are well formatted and tested.
 
 ## Acknowledgements
 
 I would like to express my gratitude to [@HarukaMa](https://github.com/HarukaMa) for creating the initial project. Their work has been an invaluable starting point for my modifications and improvements.
+
```

### Comparing `ejtraderCT-1.1.1a0/README.md` & `ejtraderCT-1.1.1b0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 ![Pypi Publish](https://github.com/ejtraderLabs/ejtraderCT/actions/workflows/python-publish.yml/badge.svg)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderCT)
 [![License](https://img.shields.io/github/license/ejtraderLabs/ejtraderCT)](https://github.com/ejtraderLabs/ejtraderCT/blob/master/LICENSE)
 [![PyPi downloads](https://img.shields.io/pypi/dm/ejtraderCT?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/ejtraderCT/)
 
 # Python Ctrader Fix API
 
-### ToDo
+`ejtraderCT` is a Python library to access the Ctrader trading platform's FIX API.
+
+## Features
 
-- [ ] Account Information "not possible fix limitation"
 - [x] Market Position buy and sell
-- [x] Peding orders limit and stop 
+- [x] Pending orders limit and stop 
 - [x] Partial close
 - [x] Stop loss & Take profit
 - [x] Modify Orders 
 - [x] Modify position 
-- [x] real time bid & ask
+- [x] Real-time bid & ask
+- [x] Check connection status
+- [ ] Rest API server (in development)
+- [ ] Webhook for Tradingviewer (in development)
+
+## Prerequisites
 
+The library has been tested on Python 3.7 to 3.9.
 
 ## Installation
-#### Tested on python 3.7 to 3.9
-```
-pip install ejtraderCT -U
-```
-#### Or install from source
 
-```
-git clone https://github.com/ejtraderLabs/ejtraderCT
-cd ejtraderCT
-python setup.py install
+To install the latest version of `ejtraderCT`, you can use pip:
 
+```shell
+pip install ejtraderCT -U
+```
+Or if you want to install from source, you can use:
+```shell
+pip install git+https://github.com/ejtraderLabs/ejtraderCT.git
 ```
 
 ## Accessing the Ctrader FIX API
 
 
 To access your API, follow these simple steps:
 
@@ -66,21 +71,24 @@
 server="168.205.95.20" # - Host name: (Current IP address 168.205.95.20 can be changed without notice)
 account="live.icmarkets.1104926" #  - SenderCompID: live.icmarkets.1104928
 password="12345678" # - The password you configured
 
 api = Ctrader(server,account,password)
 
 ```
-
-##### To disconnect and logout from the account
+##### Check the connection status
+```python
+api.isconnected()
+```
+##### Logout 
 ```python
 api.logout()
 ```
 
-### Real-time quote
+#### Real-time quote
 
 ##### Subscribe to symbols
 ```python
 api.subscribe("EURUSD", "GBPUSD")
 ```
 ##### List of quotes for all symbols
 ```python
@@ -240,15 +248,20 @@
 stoploss = "stop loss price""
 takeprofit= "stop gain price"
 price = "limit or stop entry price"
 
 api.orderModify(id, stoploss, takeprofit, price)
 
 ```
-## Contributors:
+## Contributing
 
-<!-- CONTRIBUTORS:START -->
-<!-- CONTRIBUTORS:END -->
+We welcome any contribution to `ejtraderCT`. Here are some ways to contribute:
+
+1. Report issues or suggest improvements by opening an [issue](https://github.com/ejtraderLabs/ejtraderCT/issues).
+2. Contribute with code to fix issues or add features via a [Pull Request](https://github.com/ejtraderLabs/ejtraderCT/pulls).
+
+Before submitting a pull request, please make sure your codes are well formatted and tested.
 
 ## Acknowledgements
 
 I would like to express my gratitude to [@HarukaMa](https://github.com/HarukaMa) for creating the initial project. Their work has been an invaluable starting point for my modifications and improvements.
+
```

### Comparing `ejtraderCT-1.1.1a0/ejtraderCT/api/Symbol.py` & `ejtraderCT-1.1.1b0/ejtraderCT/api/Symbol.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.1.1a0/ejtraderCT/api/ctrader.py` & `ejtraderCT-1.1.1b0/ejtraderCT/api/ctrader.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,15 +352,14 @@
     def quote(self, symbol=None): 
         if symbol and symbol not in self.fix.spot_price_list: 
             return "Symbol not Subscribed"
         elif symbol:
             return self.fix.spot_price_list[symbol]     
         return self.fix.spot_price_list
     
-
     def order_list_callback(self, data: dict, price_data: dict, client_id: str):
         orders = []
         for i, kv in enumerate(data.items()):
             ord_id = kv[0]
             name = kv[1]["name"]
             side = "Buy" if kv[1]["side"] == Side.Buy else "Sell"
             amount = kv[1]["amount"]
@@ -419,9 +418,18 @@
     def close_all(self):
         self.fix.close_all()
     
     def cancel_all(self):
         self.fix.cancel_all()
         
     def logout(self):
-        self.fix.logout()
+        if self.isconnected():
+            self.fix.logout()
+            logout = "Logged out"
+        else:
+            logout = "Not logged in"
+        return logout
+    
+    
+    def isconnected(self):
+        return self.fix.logged
```

### Comparing `ejtraderCT-1.1.1a0/ejtraderCT/api/fix.py` & `ejtraderCT-1.1.1b0/ejtraderCT/api/fix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import re
 import threading
-from datetime import datetime, timedelta
+from datetime import datetime
 import time
 from enum import IntEnum, Enum
 import socket
 from pprint import pformat
 from .buffer import Buffer
 
 
@@ -13,15 +13,15 @@
     AvgPx = 6
     BeginSeqNo = 7
     BeginString = 8
     BodyLength = 9
     CheckSum = 10
     ClOrdId = 11
     CumQty = 14
-    OrdQty = 32 # nao tem na DOC
+    OrdQty = 32  # nao tem na DOC
     MsgSeqNum = 34
     MsgType = 35
     OrderID = 37
     OrderQty = 38
     OrdStatus = 39
     OrdType = 40
     OrigClOrdID = 41
@@ -98,38 +98,42 @@
 class SubID(Enum):
     QUOTE = "QUOTE"
     TRADE = "TRADE"
 
     def __str__(self):
         return self.value
 
+
 class Side(IntEnum):
     Buy = 1
     Sell = 2
 
+
 class OrderType(IntEnum):
     Market = 1
     Limit = 2
     Stop = 3
 
+
 def get_time():
-        return datetime.utcnow().strftime('%Y%m%d-%H:%M:%S')
+    return datetime.utcnow().strftime("%Y%m%d-%H:%M:%S")
 
-class FIX:
 
+class FIX:
     class Message:
-
-        def __init__(self, sub: SubID = None, msg_type: str = None, parent = None):
+        def __init__(self, sub: SubID = None, msg_type: str = None, parent=None):
             self.fields = []
             if parent:
                 self.origin = True
                 self.fields.append((Field.BeginString, "FIX.4.4"))
                 self.fields.append((Field.BodyLength, 0))
                 self.fields.append((Field.MsgType, msg_type))
-                self.fields.append((Field.SenderCompID, parent.broker + "." + parent.login))
+                self.fields.append(
+                    (Field.SenderCompID, parent.broker + "." + parent.login)
+                )
                 self.fields.append((Field.SenderSubID, sub))
                 self.fields.append((Field.TargetCompID, "CSERVER"))
                 self.fields.append((Field.TargetSubID, sub))
                 if sub == SubID.QUOTE:
                     self.fields.append((Field.MsgSeqNum, parent.qseq))
                     parent.qseq += 1
                 elif sub == SubID.TRADE:
@@ -144,15 +148,15 @@
                 if k == item:
                     return v
             return None
 
         def __setitem__(self, key, value):
             self.fields.append((key, value))
 
-        def get_repeating_groups(self, count_key, repeating_start, repeating_end = None):
+        def get_repeating_groups(self, count_key, repeating_start, repeating_end=None):
             count = None
             result = []
             item = {}
             for k, v in self.fields[8:]:
                 if count == 0:
                     return result
                 if count is None:
@@ -186,15 +190,26 @@
                 cksm = sum(data.replace("|", "\x01").encode()) % 256
                 data += "10=%03d|" % cksm
             return data
 
         def __repr__(self):
             return pformat([(k.name, v) for k, v in self.fields])
 
-    def __init__(self, server: str, broker: str, login: str, password: str, currency: str, client_id: str, position_list_callback, order_list_callback,update_fix_status=None):
+    def __init__(
+        self,
+        server: str,
+        broker: str,
+        login: str,
+        password: str,
+        currency: str,
+        client_id: str,
+        position_list_callback,
+        order_list_callback,
+        update_fix_status=None,
+    ):
         try:
             self.qstream = Buffer()
             self.qs = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.qs.connect((server, 5201))
             self.tstream = Buffer()
             self.ts = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.ts.connect((server, 5202))
@@ -241,40 +256,42 @@
             # Code to handle the exception
             logging.error(f"{e}")
 
     def qworker(self):
         while True:
             try:
                 data = self.qs.recv(65535)
-            except:
+            except Exception as e:
+                logging.info(e)
                 break
             if len(data) == 0:
-                print("Quote Logged out")
+                logging.info("Quote Logged out")
                 break
             try:
                 self.qstream.write(data)
                 self.parse_quote_message()
-            except:
-                print("Market is Close or Disconnected")
+            except Exception as e:
+                logging.info(f"Market is Close or Disconnected {e}")
                 break
 
     def tworker(self):
         while True:
             try:
                 data = self.ts.recv(65535)
             except Exception as e:
+                logging.info(e)
                 break
             if len(data) == 0:
-                print("Trade Logged out")
+                logging.info("Trade Logged out")
                 break
             try:
                 self.tstream.write(data)
                 self.parse_trade_message()
             except Exception as e:
-                print(f"Market is Close or Logged out {e}")
+                logging.info(f"Market is Close or Logged out {e}")
                 break
 
     def parse_quote_message(self):
         while len(self.qstream) > 0:
             match = re.search(rb"10=\d{3}\x01", self.qstream.peek(self.qstream.count()))
             if match:
                 msg = FIX.Message()
@@ -321,19 +338,17 @@
     def process_test(self, msg):
         if msg[Field.SenderSubID] == "QUOTE":
             self.qheartbeat(msg[Field.TestReqID])
         elif msg[Field.SenderSubID] == "TRADE":
             self.theartbeat(msg[Field.TestReqID])
 
     def process_logout(self, msg):
-        if msg[Field.Text] == None:
+        if not msg[Field.Text]:
             self.logged = False
         self.update_fix_status(self.client_id, self.logged)
-            
-       
 
     def process_exec_report(self, msg):
         if msg[Field.ExecType] == "F":
             self.position_list = {}
             self.position_request()
             self.order_list = {}
             self.origin_to_pos_id[msg[Field.ClOrdId]] = msg[Field.PosMaintRptID]
@@ -351,52 +366,66 @@
                 "pos_id": msg[Field.PosMaintRptID],
                 "digits": self.sec_id_table[int(msg[Field.Symbol])]["digits"],
                 "clid": msg[Field.ClOrdId],
             }
 
             if int(msg[Field.OrdType]) == 1:
                 self.origin_to_pos_id[msg[Field.ClOrdId]] = msg[Field.PosMaintRptID]
-            else :
+            else:
                 if msg[Field.ClOrdId] not in self.origin_to_ord_id:
                     self.origin_to_ord_id[msg[Field.ClOrdId]] = []
                 if msg[Field.OrderID] not in self.origin_to_ord_id[msg[Field.ClOrdId]]:
                     self.origin_to_ord_id[msg[Field.ClOrdId]].append(msg[Field.OrderID])
 
             if int(msg[Field.OrdType]) > 1:
                 price = msg[Field.Price]
                 if price:
                     self.order_list[msg[Field.OrderID]]["price"] = float(price)
                 else:
-                    self.order_list[msg[Field.OrderID]]["price"] = float(msg[Field.StopPx])
+                    self.order_list[msg[Field.OrderID]]["price"] = float(
+                        msg[Field.StopPx]
+                    )
             if name not in self.spot_request_list:
                 self.spot_market_request(name)
-            self.order_list_callback(self.order_list, self.spot_price_list, self.client_id)
+            self.order_list_callback(
+                self.order_list, self.spot_price_list, self.client_id
+            )
 
     def process_logon(self, msg):
         if msg[Field.SenderSubID] == "QUOTE":
-            print("Quote logged on")
-            self.ping_qworker_thread = threading.Thread(target=self.ping_qworker, args=[int(msg[Field.HeartBtInt])])
+            logging.info("Quote logged on")
+            self.ping_qworker_thread = threading.Thread(
+                target=self.ping_qworker, args=[int(msg[Field.HeartBtInt])]
+            )
             self.ping_qworker_thread.start()
             self.logged = True
         elif msg[Field.SenderSubID] == "TRADE":
-            print("Trade logged on")
-            self.ping_tworker_thread = threading.Thread(target=self.ping_tworker, args=[int(msg[Field.HeartBtInt])])
+            logging.info("Trade logged on")
+            self.ping_tworker_thread = threading.Thread(
+                target=self.ping_tworker, args=[int(msg[Field.HeartBtInt])]
+            )
             self.ping_tworker_thread.start()
 
     def process_market_data(self, msg: Message):
         name = self.sec_id_table[int(msg[Field.Symbol])]["name"]
         digits = self.sec_id_table[int(msg[Field.Symbol])]["digits"]
         entries = msg.get_repeating_groups(Field.NoMDEntries, Field.MDEntryType)
         if not msg[Field.MDEntryID] and msg[Field.NoMDEntries] != "0":
             self.spot_price_list[name] = {}
             for e in entries:
                 self.spot_price_list[name]["time"] = int(round(time.time() * 1000))
-                self.spot_price_list[name]["bid" if e[Field.MDEntryType] == "0" else "ask"] = float(e[Field.MDEntryPx])
-            self.position_list_callback(self.position_list, self.spot_price_list, self.client_id)
-            self.order_list_callback(self.order_list, self.spot_price_list, self.client_id)
+                self.spot_price_list[name][
+                    "bid" if e[Field.MDEntryType] == "0" else "ask"
+                ] = float(e[Field.MDEntryPx])
+            self.position_list_callback(
+                self.position_list, self.spot_price_list, self.client_id
+            )
+            self.order_list_callback(
+                self.order_list, self.spot_price_list, self.client_id
+            )
             return
         self.market_data[name] = {}
         for e in entries:
             eid = e[Field.MDEntryID]
             self.market_data[name][eid] = {
                 "type": int(e[Field.MDEntryType]),
                 "price": float(e[Field.MDEntryPx]),
@@ -421,16 +450,22 @@
                 }
         # logging.debug(pformat(msg))
         self.market_callback(name, digits, self.market_data[name])
 
     def process_sec_list(self, msg):
         sec_list = msg.get_repeating_groups(Field.NoRelatedSym, Field.Symbol)
         for symbol in sec_list:
-            self.sec_id_table[int(symbol[Field.Symbol])] = {"name": symbol[Field.SymbolName], "digits": int(symbol[Field.SymbolDigits])}
-            self.sec_name_table[symbol[Field.SymbolName]] = {"id": int(symbol[Field.Symbol]), "digits": int(symbol[Field.SymbolDigits])}
+            self.sec_id_table[int(symbol[Field.Symbol])] = {
+                "name": symbol[Field.SymbolName],
+                "digits": int(symbol[Field.SymbolDigits]),
+            }
+            self.sec_name_table[symbol[Field.SymbolName]] = {
+                "id": int(symbol[Field.Symbol]),
+                "digits": int(symbol[Field.SymbolDigits]),
+            }
         if self.sec_list_callback is not None:
             self.sec_list_callback()
         self.position_request()
         self.order_request()
         self.sec_list_evt.set()
 
     def get_origin_from_pos_id(self, pos_id):
@@ -438,26 +473,25 @@
         values = list(self.origin_to_pos_id.values())
         if pos_id in values:
             return keys[values.index(pos_id)]
         else:
             return None
 
     def process_position_list(self, msg):
-        
         if msg[Field.PosReqResult] == "2":
             return
         name = self.sec_id_table[int(msg[Field.Symbol])]["name"]
         self.position_list[msg[Field.PosMaintRptID]] = {
             "pos_id": msg[Field.PosMaintRptID],
             "name": name,
             "long": float(msg[Field.LongQty]),
             "short": float(msg[Field.ShortQty]),
             "price": float(msg[Field.SettlPrice]),
             "digits": self.sec_id_table[int(msg[Field.Symbol])]["digits"],
-            "clid": self.get_origin_from_pos_id(msg[Field.PosMaintRptID])
+            "clid": self.get_origin_from_pos_id(msg[Field.PosMaintRptID]),
         }
 
         if name not in self.spot_request_list:
             self.spot_market_request(name)
         base = name[-3:]
         if base != self.currency:
             pair = "%s%s" % (base, self.currency)
@@ -465,23 +499,25 @@
             if not self.sec_name_table.get(pair, None):
                 pair = "%s%s" % (self.currency, base)
                 conv_dir = 1
             self.position_list[msg[Field.PosMaintRptID]]["convert"] = pair
             self.position_list[msg[Field.PosMaintRptID]]["convert_dir"] = conv_dir
             if pair not in self.spot_request_list:
                 self.spot_market_request(pair)
-        self.position_list_callback(self.position_list, self.spot_price_list, self.client_id)
+        self.position_list_callback(
+            self.position_list, self.spot_price_list, self.client_id
+        )
 
     def process_reject(self, msg):
         checkOrders = msg[Field.Text].split(":")[1]
         if checkOrders == "no orders found":
-            print("No Orders")
+            logging.info("No Orders")
         else:
             logging.error(checkOrders)
-       
+
     message_dispatch = {
         "0": process_ping,
         "1": process_test,
         "3": process_reject,
         "5": process_logout,
         "8": process_exec_report,
         "9": process_reject,
@@ -498,23 +534,25 @@
         FIX.message_dispatch[msg_type](self, msg)
 
     def send_message(self, msg: Message):
         if msg[Field.TargetSubID] == SubID.QUOTE:
             try:
                 self.qs.send(bytes(msg))
                 logging.debug("\033[36mSEND >>> %s\033[0m" % msg)
-            except:
-                logging.error("Error in QUOTE send. Closing connection. client_id: %s" % self.client_id)
+            except Exception as e:
+                logging.debug(f"QUOTE send error: {e}. client_id: {self.client_id}")
                 self.qs.close()
         elif msg[Field.TargetSubID] == SubID.TRADE:
             try:
                 self.ts.send(bytes(msg))
                 logging.debug("\033[96mSEND >>> %s\033[0m" % msg)
-            except:
-                logging.error("Error in TRADE send. Closing connection. client_id: %s" % self.client_id)
+            except Exception as e:
+                logging.debug(
+                    f"TRADE send error: {e} Closing connection. client_id:{self.client_id}"
+                )
                 self.ts.close()
 
     def qheartbeat(self, test_id: int = None):
         msg = FIX.Message(SubID.QUOTE, "0", self)
         if test_id:
             msg[Field.TestReqID] = test_id
         self.send_message(msg)
@@ -607,27 +645,29 @@
 
     def order_request(self):
         msg = FIX.Message(SubID.TRADE, "AF", self)
         msg[Field.MassStatusReqID] = 1
         msg[Field.MassStatusReqType] = 7
         self.send_message(msg)
 
-    def sec_list(self, callback = None):
+    def sec_list(self, callback=None):
         msg = FIX.Message(SubID.QUOTE, "x", self)
         msg[Field.SecurityReqID] = 1
         msg[Field.SecurityListRequestType] = 0
         self.sec_list_callback = callback
         self.send_message(msg)
 
-    def new_market_order(self, symbol, side: Side, size: float, originId = None, pos_id = None):
+    def new_market_order(
+        self, symbol, side: Side, size: float, originId=None, pos_id=None
+    ):
         if symbol not in self.sec_name_table:
             return
-        
+
         msg = FIX.Message(SubID.TRADE, "D", self)
-        msg[Field.ClOrdId] = originId if originId != None else 'dt' + get_time()
+        msg[Field.ClOrdId] = originId if originId else "dt" + get_time()
         msg[Field.Symbol] = self.sec_name_table[symbol]["id"]
         msg[Field.Side] = side.value
         msg[Field.TransactTime] = get_time()
         msg[Field.OrderQty] = size
         msg[Field.OrdType] = OrderType.Market.value
         msg[Field.Designation] = "test label"
         if pos_id:
@@ -646,32 +686,53 @@
                     for cl_id in self.origin_to_ord_id[o]:
                         self.cancel_order(cl_id)
                 self.origin_to_pos_id.pop(o)
                 break
 
         msg = FIX.Message(SubID.TRADE, "D", self)
         msg[Field.ClOrdId] = get_time()
-        msg[Field.Symbol] = self.sec_name_table[self.position_list[pos_id]["name"]]["id"]
-        msg[Field.Side] = Side.Sell.value if self.position_list[pos_id]["long"] > 0 else Side.Buy.value
+        msg[Field.Symbol] = self.sec_name_table[self.position_list[pos_id]["name"]][
+            "id"
+        ]
+        msg[Field.Side] = (
+            Side.Sell.value
+            if self.position_list[pos_id]["long"] > 0
+            else Side.Buy.value
+        )
         msg[Field.TransactTime] = get_time()
-        msg[Field.OrderQty] = lots if lots is not None else self.position_list[pos_id]["long"] if msg[Field.Side] == Side.Sell else self.position_list[pos_id]["short"]
+        msg[Field.OrderQty] = (
+            lots
+            if lots is not None
+            else self.position_list[pos_id]["long"]
+            if msg[Field.Side] == Side.Sell
+            else self.position_list[pos_id]["short"]
+        )
         msg[Field.PosMaintRptID] = pos_id
         msg[Field.OrdType] = OrderType.Market.value
         self.send_message(msg)
 
     def close_all(self):
         for position in self.position_list:
             self.close_position(position, None)
 
-    def new_limit_order(self, symbol, side: Side, order_type: OrderType, size: float, price: float, originId = None, pos_id = None):
+    def new_limit_order(
+        self,
+        symbol,
+        side: Side,
+        order_type: OrderType,
+        size: float,
+        price: float,
+        originId=None,
+        pos_id=None,
+    ):
         if symbol not in self.sec_name_table:
             return
-        
+
         msg = FIX.Message(SubID.TRADE, "D", self)
-        msg[Field.ClOrdId] = originId if originId != None else 'dt' + get_time()
+        msg[Field.ClOrdId] = originId if originId else "dt" + get_time()
         msg[Field.Symbol] = self.sec_name_table[symbol]["id"]
         msg[Field.Side] = side.value
         msg[Field.TransactTime] = get_time()
         msg[Field.OrderQty] = size
         msg[Field.OrdType] = order_type.value
         if order_type == OrderType.Limit:
             msg[Field.Price] = price
@@ -685,15 +746,15 @@
         # remove referencia ao server ord_id da tabela de-para
         for o, p in self.origin_to_ord_id.items():
             if clid in p:
                 p.remove(clid)
                 if len(p) == 0:
                     self.origin_to_ord_id.pop(o)
                 break
-        
+
         msg = FIX.Message(SubID.TRADE, "F", self)
         msg[Field.OrigClOrdID] = clid
         msg[Field.OrderID] = clid
         msg[Field.ClOrdId] = clid
         self.send_message(msg)
 
     def cancel_all(self):
```

### Comparing `ejtraderCT-1.1.1a0/ejtraderCT/api/math.py` & `ejtraderCT-1.1.1b0/ejtraderCT/api/math.py`

 * *Files identical despite different names*

### Comparing `ejtraderCT-1.1.1a0/ejtraderCT.egg-info/PKG-INFO` & `ejtraderCT-1.1.1b0/ejtraderCT.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderCT
-Version: 1.1.1a0
+Version: 1.1.1b0
 Summary: Ctrader Fix API
 Home-page: https://ejtraderCT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso & Douglas Barros
 Author-email: support@ejtrader.com
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderCT/issues
@@ -12,14 +12,16 @@
 Project-URL: Documentation, https://ejtraderCT.readthedocs.io/
 Keywords: ctrader,fix-api,historical-data,financial-data,stocks,funds,etfs,indices,currency crosses,bonds,commodities,crypto currencies
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
@@ -29,38 +31,43 @@
 ![Pypi Publish](https://github.com/ejtraderLabs/ejtraderCT/actions/workflows/python-publish.yml/badge.svg)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/ejtraderLabs/ejtraderCT)
 [![License](https://img.shields.io/github/license/ejtraderLabs/ejtraderCT)](https://github.com/ejtraderLabs/ejtraderCT/blob/master/LICENSE)
 [![PyPi downloads](https://img.shields.io/pypi/dm/ejtraderCT?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/ejtraderCT/)
 
 # Python Ctrader Fix API
 
-### ToDo
+`ejtraderCT` is a Python library to access the Ctrader trading platform's FIX API.
+
+## Features
 
-- [ ] Account Information "not possible fix limitation"
 - [x] Market Position buy and sell
-- [x] Peding orders limit and stop 
+- [x] Pending orders limit and stop 
 - [x] Partial close
 - [x] Stop loss & Take profit
 - [x] Modify Orders 
 - [x] Modify position 
-- [x] real time bid & ask
+- [x] Real-time bid & ask
+- [x] Check connection status
+- [ ] Rest API server (in development)
+- [ ] Webhook for Tradingviewer (in development)
+
+## Prerequisites
 
+The library has been tested on Python 3.7 to 3.9.
 
 ## Installation
-#### Tested on python 3.7 to 3.9
-```
-pip install ejtraderCT -U
-```
-#### Or install from source
 
-```
-git clone https://github.com/ejtraderLabs/ejtraderCT
-cd ejtraderCT
-python setup.py install
+To install the latest version of `ejtraderCT`, you can use pip:
 
+```shell
+pip install ejtraderCT -U
+```
+Or if you want to install from source, you can use:
+```shell
+pip install git+https://github.com/ejtraderLabs/ejtraderCT.git
 ```
 
 ## Accessing the Ctrader FIX API
 
 
 To access your API, follow these simple steps:
 
@@ -94,21 +101,24 @@
 server="168.205.95.20" # - Host name: (Current IP address 168.205.95.20 can be changed without notice)
 account="live.icmarkets.1104926" #  - SenderCompID: live.icmarkets.1104928
 password="12345678" # - The password you configured
 
 api = Ctrader(server,account,password)
 
 ```
-
-##### To disconnect and logout from the account
+##### Check the connection status
+```python
+api.isconnected()
+```
+##### Logout 
 ```python
 api.logout()
 ```
 
-### Real-time quote
+#### Real-time quote
 
 ##### Subscribe to symbols
 ```python
 api.subscribe("EURUSD", "GBPUSD")
 ```
 ##### List of quotes for all symbols
 ```python
@@ -268,15 +278,20 @@
 stoploss = "stop loss price""
 takeprofit= "stop gain price"
 price = "limit or stop entry price"
 
 api.orderModify(id, stoploss, takeprofit, price)
 
 ```
-## Contributors:
+## Contributing
 
-<!-- CONTRIBUTORS:START -->
-<!-- CONTRIBUTORS:END -->
+We welcome any contribution to `ejtraderCT`. Here are some ways to contribute:
+
+1. Report issues or suggest improvements by opening an [issue](https://github.com/ejtraderLabs/ejtraderCT/issues).
+2. Contribute with code to fix issues or add features via a [Pull Request](https://github.com/ejtraderLabs/ejtraderCT/pulls).
+
+Before submitting a pull request, please make sure your codes are well formatted and tested.
 
 ## Acknowledgements
 
 I would like to express my gratitude to [@HarukaMa](https://github.com/HarukaMa) for creating the initial project. Their work has been an invaluable starting point for my modifications and improvements.
+
```

### Comparing `ejtraderCT-1.1.1a0/setup.py` & `ejtraderCT-1.1.1b0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,70 @@
 import io
 
 from setuptools import setup, find_packages
 
 
 def readme():
-    with io.open('README.md', encoding='utf-8') as f:
+    with io.open("README.md", encoding="utf-8") as f:
         return f.read()
 
+
 def requirements(filename):
     reqs = list()
-    with io.open(filename, encoding='utf-8') as f:
+    with io.open(filename, encoding="utf-8") as f:
         for line in f.readlines():
             reqs.append(line.strip())
     return reqs
 
 
 setup(
-    name='ejtraderCT',
-    version='1.1.1a',
+    name="ejtraderCT",
+    version="1.1.1b0",
     packages=find_packages(),
-    url='https://ejtraderCT.readthedocs.io/',
-    download_url='https://ejtrader.com',
-    license='GPL-3.0',
-    author='Emerson Pedroso & Douglas Barros',
-    author_email='support@ejtrader.com',
-    description='Ctrader Fix API',
+    url="https://ejtraderCT.readthedocs.io/",
+    download_url="https://ejtrader.com",
+    license="GPL-3.0",
+    author="Emerson Pedroso & Douglas Barros",
+    author_email="support@ejtrader.com",
+    description="Ctrader Fix API",
     long_description=readme(),
-    long_description_content_type='text/markdown',
-    install_requires=requirements(filename='requirements.txt'),
+    long_description_content_type="text/markdown",
+    install_requires=requirements(filename="requirements.txt"),
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Topic :: Office/Business :: Financial",
         "Topic :: Office/Business :: Financial :: Investment",
         "Topic :: Scientific/Engineering :: Information Analysis",
-        "Topic :: Software Development :: Libraries"
+        "Topic :: Software Development :: Libraries",
     ],
-    python_requires='>=3',
-    keywords=', '.join([
-        'ctrader', 'fix-api', 'historical-data',
-        'financial-data', 'stocks', 'funds', 'etfs',
-        'indices', 'currency crosses', 'bonds', 'commodities',
-        'crypto currencies'
-    ]),
+    python_requires=">=3",
+    keywords=", ".join(
+        [
+            "ctrader",
+            "fix-api",
+            "historical-data",
+            "financial-data",
+            "stocks",
+            "funds",
+            "etfs",
+            "indices",
+            "currency crosses",
+            "bonds",
+            "commodities",
+            "crypto currencies",
+        ]
+    ),
     project_urls={
-        'Bug Reports': 'https://github.com/traderpedroso/ejtraderCT/issues',
-        'Source': 'https://github.com/traderpedroso/ejtraderCT',
-        'Documentation': 'https://ejtraderCT.readthedocs.io/'
+        "Bug Reports": "https://github.com/traderpedroso/ejtraderCT/issues",
+        "Source": "https://github.com/traderpedroso/ejtraderCT",
+        "Documentation": "https://ejtraderCT.readthedocs.io/",
     },
 )
```

### Comparing `ejtraderCT-1.1.1a0/test/test_math.py` & `ejtraderCT-1.1.1b0/test/test_math.py`

 * *Files identical despite different names*

