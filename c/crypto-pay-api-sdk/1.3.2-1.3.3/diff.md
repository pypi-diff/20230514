# Comparing `tmp/crypto_pay_api_sdk-1.3.2.tar.gz` & `tmp/crypto_pay_api_sdk-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto_pay_api_sdk-1.3.2.tar", last modified: Wed Jul 27 15:00:22 2022, max compression
+gzip compressed data, was "crypto_pay_api_sdk-1.3.3.tar", last modified: Sun May 14 15:03:12 2023, max compression
```

## Comparing `crypto_pay_api_sdk-1.3.2.tar` & `crypto_pay_api_sdk-1.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-07-27 15:00:22.044871 crypto_pay_api_sdk-1.3.2/
--rw-rw-rw-   0        0        0     1083 2022-07-27 14:50:22.000000 crypto_pay_api_sdk-1.3.2/LICENSE
--rw-rw-rw-   0        0        0     7039 2022-07-27 15:00:22.045872 crypto_pay_api_sdk-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     6346 2022-07-27 14:50:22.000000 crypto_pay_api_sdk-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2022-07-27 15:00:22.038905 crypto_pay_api_sdk-1.3.2/crypto_pay_api_sdk/
--rw-rw-rw-   0        0        0       24 2022-07-27 14:50:22.000000 crypto_pay_api_sdk-1.3.2/crypto_pay_api_sdk/__init__.py
--rw-rw-rw-   0        0        0     6227 2022-07-27 14:56:22.000000 crypto_pay_api_sdk-1.3.2/crypto_pay_api_sdk/cryptopay.py
-drwxrwxrwx   0        0        0        0 2022-07-27 15:00:22.044871 crypto_pay_api_sdk-1.3.2/crypto_pay_api_sdk.egg-info/
--rw-rw-rw-   0        0        0     7039 2022-07-27 15:00:21.000000 crypto_pay_api_sdk-1.3.2/crypto_pay_api_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2022-07-27 15:00:21.000000 crypto_pay_api_sdk-1.3.2/crypto_pay_api_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-27 15:00:21.000000 crypto_pay_api_sdk-1.3.2/crypto_pay_api_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-07-27 15:00:21.000000 crypto_pay_api_sdk-1.3.2/crypto_pay_api_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-07-27 15:00:21.000000 crypto_pay_api_sdk-1.3.2/crypto_pay_api_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-07-27 14:50:22.000000 crypto_pay_api_sdk-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0      818 2022-07-27 15:00:22.046873 crypto_pay_api_sdk-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      893 2022-07-27 14:57:21.000000 crypto_pay_api_sdk-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 15:03:12.566464 crypto_pay_api_sdk-1.3.3/
+-rw-rw-rw-   0        0        0     1083 2022-07-27 14:50:22.000000 crypto_pay_api_sdk-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0     7157 2023-05-14 15:03:12.567439 crypto_pay_api_sdk-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6489 2023-05-14 15:03:02.000000 crypto_pay_api_sdk-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 15:03:12.496152 crypto_pay_api_sdk-1.3.3/crypto_pay_api_sdk/
+-rw-rw-rw-   0        0        0       24 2022-07-27 14:50:22.000000 crypto_pay_api_sdk-1.3.3/crypto_pay_api_sdk/__init__.py
+-rw-rw-rw-   0        0        0     6172 2023-05-14 14:55:06.000000 crypto_pay_api_sdk-1.3.3/crypto_pay_api_sdk/cryptopay.py
+drwxrwxrwx   0        0        0        0 2023-05-14 15:03:12.564509 crypto_pay_api_sdk-1.3.3/crypto_pay_api_sdk.egg-info/
+-rw-rw-rw-   0        0        0     7157 2023-05-14 15:03:12.000000 crypto_pay_api_sdk-1.3.3/crypto_pay_api_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-14 15:03:12.000000 crypto_pay_api_sdk-1.3.3/crypto_pay_api_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 15:03:12.000000 crypto_pay_api_sdk-1.3.3/crypto_pay_api_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 15:03:12.000000 crypto_pay_api_sdk-1.3.3/crypto_pay_api_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-14 15:03:12.000000 crypto_pay_api_sdk-1.3.3/crypto_pay_api_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-07-27 14:50:22.000000 crypto_pay_api_sdk-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0      816 2023-05-14 15:03:12.568419 crypto_pay_api_sdk-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      892 2023-05-14 14:57:41.000000 crypto_pay_api_sdk-1.3.3/setup.py
```

### Comparing `crypto_pay_api_sdk-1.3.2/LICENSE` & `crypto_pay_api_sdk-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crypto_pay_api_sdk-1.3.2/PKG-INFO` & `crypto_pay_api_sdk-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: crypto_pay_api_sdk
-Version: 1.3.2
+Version: 1.3.3
 Summary: API for CryptoBot
-Home-page: https://github.com/althonos/crypto-pay-api-sdk
+Home-page: https://github.com/sllavon/crypto-pay-api-sdk
 Author: Vyacheslav Zhigulin
 Author-email: muxellexum@gmail.com
 License: MIT
-Project-URL: Bug Tracker, https://github.com/althonos/crypto-pay-api-sdk/issues
-Platform: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/sllavon/crypto-pay-api-sdk/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![](https://raw.githubusercontent.com/sllavon/crypto-pay-api-sdk/3e83818c975a47f4ca61209b478f2508224058db/media/header.svg)
 # @muxel/crypto-pay-api-sdk
 ## [SDK for working with Crypto Bot](https://t.me/CryptoBot)
 
-![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master) [![TON](https://camo.githubusercontent.com/862a7c69bd3b8a405bdd94557b8e6d5a90702f363058e59fd8dadda3adb60a97/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2546302539462539322538452d544f4e2d677265656e)](https://ton.org) [![license - MIT](https://camo.githubusercontent.com/63691059c8dda9856bd568ef8bb0b326677b863d8b1fc9237cc096b6fd18a205/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f737461732d70726f6b6f706965762f697079776964676574735f746f67676c655f627574746f6e73)](https://github.com/sllavon/crypto-pay-api-sdk/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/crypto-pay-api-sdk?period=month&units=international_system&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/crypto-pay-api-sdk) [![TON](https://camo.githubusercontent.com/862a7c69bd3b8a405bdd94557b8e6d5a90702f363058e59fd8dadda3adb60a97/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2546302539462539322538452d544f4e2d677265656e)](https://ton.org) [![license - MIT](https://camo.githubusercontent.com/63691059c8dda9856bd568ef8bb0b326677b863d8b1fc9237cc096b6fd18a205/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f737461732d70726f6b6f706965762f697079776964676574735f746f67676c655f627574746f6e73)](https://github.com/sllavon/crypto-pay-api-sdk/blob/main/LICENSE) 
 
 # Installation
 ```sh
 pip install crypto-pay-api-sdk
 ```
 
 # Explanation
@@ -177,9 +176,7 @@
 
 ```python
 Crypto.getCurrencies()
 ```
 
 ## License
 MIT
-
-
```

### Comparing `crypto_pay_api_sdk-1.3.2/README.md` & `crypto_pay_api_sdk-1.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ![](https://raw.githubusercontent.com/sllavon/crypto-pay-api-sdk/3e83818c975a47f4ca61209b478f2508224058db/media/header.svg)
 # @muxel/crypto-pay-api-sdk
 ## [SDK for working with Crypto Bot](https://t.me/CryptoBot)
 
-![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master) [![TON](https://camo.githubusercontent.com/862a7c69bd3b8a405bdd94557b8e6d5a90702f363058e59fd8dadda3adb60a97/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2546302539462539322538452d544f4e2d677265656e)](https://ton.org) [![license - MIT](https://camo.githubusercontent.com/63691059c8dda9856bd568ef8bb0b326677b863d8b1fc9237cc096b6fd18a205/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f737461732d70726f6b6f706965762f697079776964676574735f746f67676c655f627574746f6e73)](https://github.com/sllavon/crypto-pay-api-sdk/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/crypto-pay-api-sdk?period=month&units=international_system&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/crypto-pay-api-sdk) [![TON](https://camo.githubusercontent.com/862a7c69bd3b8a405bdd94557b8e6d5a90702f363058e59fd8dadda3adb60a97/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2546302539462539322538452d544f4e2d677265656e)](https://ton.org) [![license - MIT](https://camo.githubusercontent.com/63691059c8dda9856bd568ef8bb0b326677b863d8b1fc9237cc096b6fd18a205/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f737461732d70726f6b6f706965762f697079776964676574735f746f67676c655f627574746f6e73)](https://github.com/sllavon/crypto-pay-api-sdk/blob/main/LICENSE) 
 
 # Installation
 ```sh
 pip install crypto-pay-api-sdk
 ```
 
 # Explanation
```

### Comparing `crypto_pay_api_sdk-1.3.2/crypto_pay_api_sdk/cryptopay.py` & `crypto_pay_api_sdk-1.3.3/crypto_pay_api_sdk/cryptopay.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,36 +87,36 @@
         return post(f'{self.url}/transfer',
                         headers = self.headers,
                         json = {'user_id': user_id,
                                 'asset': asset,
                                 'amount': amount,
                                 'spend_id': spend_id,
                                 **params}
-                        ).json() 
+                        ).json()
 
-    def getInvoices(self) -> (dict):
+    def getInvoices(self, params={}) -> (dict):
         """Use this method to get invoices of your app
-        
+
         Args:
-            asset - Optional. Currency code.
+            asset -- Optional. Currency code.
             Supported assets: `BTC`, `TON`, `ETH` (only testnet), `USDT`, `USDC`, `BUSD`. Default: all assets
-            
+
             invoice_ids {string} - Optional. Invoice `IDs` separated by comma
-            
+
             status {string} - Optional. Status of invoices. Available statusses: active or paid. `Default: all statusses`
-            
+
             offset {number} - Optional. Offset needed to return a specific subset of invoices. `Default 0`
-            
+
             count {number} - Optional. Number of invoices to return. `Default 100, max 1000`
-            
+
         Returns:
             Array of invoices
         """
-        return get(f'{self.url}/getInvoices', headers=self.headers).json()        
-       
+        return get(f'{self.url}/getInvoices', headers=self.headers, json={**params}).json()
+
     def getBalance(self) -> (dict):
         """Use this method to get balance of your app
 
         Args:
             Requires no parameters.
             
         Returns:
```

### Comparing `crypto_pay_api_sdk-1.3.2/crypto_pay_api_sdk.egg-info/PKG-INFO` & `crypto_pay_api_sdk-1.3.3/crypto_pay_api_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: crypto-pay-api-sdk
-Version: 1.3.2
+Version: 1.3.3
 Summary: API for CryptoBot
-Home-page: https://github.com/althonos/crypto-pay-api-sdk
+Home-page: https://github.com/sllavon/crypto-pay-api-sdk
 Author: Vyacheslav Zhigulin
 Author-email: muxellexum@gmail.com
 License: MIT
-Project-URL: Bug Tracker, https://github.com/althonos/crypto-pay-api-sdk/issues
-Platform: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/sllavon/crypto-pay-api-sdk/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![](https://raw.githubusercontent.com/sllavon/crypto-pay-api-sdk/3e83818c975a47f4ca61209b478f2508224058db/media/header.svg)
 # @muxel/crypto-pay-api-sdk
 ## [SDK for working with Crypto Bot](https://t.me/CryptoBot)
 
-![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master) [![TON](https://camo.githubusercontent.com/862a7c69bd3b8a405bdd94557b8e6d5a90702f363058e59fd8dadda3adb60a97/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2546302539462539322538452d544f4e2d677265656e)](https://ton.org) [![license - MIT](https://camo.githubusercontent.com/63691059c8dda9856bd568ef8bb0b326677b863d8b1fc9237cc096b6fd18a205/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f737461732d70726f6b6f706965762f697079776964676574735f746f67676c655f627574746f6e73)](https://github.com/sllavon/crypto-pay-api-sdk/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/crypto-pay-api-sdk?period=month&units=international_system&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/crypto-pay-api-sdk) [![TON](https://camo.githubusercontent.com/862a7c69bd3b8a405bdd94557b8e6d5a90702f363058e59fd8dadda3adb60a97/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2546302539462539322538452d544f4e2d677265656e)](https://ton.org) [![license - MIT](https://camo.githubusercontent.com/63691059c8dda9856bd568ef8bb0b326677b863d8b1fc9237cc096b6fd18a205/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f737461732d70726f6b6f706965762f697079776964676574735f746f67676c655f627574746f6e73)](https://github.com/sllavon/crypto-pay-api-sdk/blob/main/LICENSE) 
 
 # Installation
 ```sh
 pip install crypto-pay-api-sdk
 ```
 
 # Explanation
@@ -177,9 +176,7 @@
 
 ```python
 Crypto.getCurrencies()
 ```
 
 ## License
 MIT
-
-
```

### Comparing `crypto_pay_api_sdk-1.3.2/setup.cfg` & `crypto_pay_api_sdk-1.3.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 7279 7074 6f5f 7061 795f 6170   = crypto_pay_ap
 00000020: 695f 7364 6b0d 0a76 6572 7369 6f6e 203d  i_sdk..version =
-00000030: 2031 2e33 2e32 0d0a 6175 7468 6f72 203d   1.3.2..author =
+00000030: 2031 2e33 2e33 0d0a 6175 7468 6f72 203d   1.3.3..author =
 00000040: 2056 7961 6368 6573 6c61 7620 5a68 6967   Vyacheslav Zhig
 00000050: 756c 696e 0d0a 6175 7468 6f72 5f65 6d61  ulin..author_ema
 00000060: 696c 203d 206d 7578 656c 6c65 7875 6d40  il = muxellexum@
 00000070: 676d 6169 6c2e 636f 6d0d 0a75 726c 203d  gmail.com..url =
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000090: 636f 6d2f 616c 7468 6f6e 6f73 2f63 7279  com/althonos/cry
-000000a0: 7074 6f2d 7061 792d 6170 692d 7364 6b0d  pto-pay-api-sdk.
-000000b0: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
-000000c0: 5049 2066 6f72 2043 7279 7074 6f42 6f74  PI for CryptoBot
-000000d0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000000e0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-000000f0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
-00000100: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-00000110: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
-00000120: 6f77 6e0d 0a6c 6963 656e 7365 203d 204d  own..license = M
-00000130: 4954 0d0a 636c 6173 7369 6669 6572 7320  IT..classifiers 
-00000140: 3d20 0d0a 0949 6e74 656e 6465 6420 4175  = ...Intended Au
-00000150: 6469 656e 6365 203a 3a20 4465 7665 6c6f  dience :: Develo
-00000160: 7065 7273 0d0a 094c 6963 656e 7365 203a  pers...License :
-00000170: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000180: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
-00000190: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-000001a0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-000001b0: 6e74 0d0a 0950 726f 6772 616d 6d69 6e67  nt...Programming
-000001c0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000001d0: 686f 6e20 3a3a 2033 0d0a 0954 6f70 6963  hon :: 3...Topic
-000001e0: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-000001f0: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
-00000200: 6172 6965 7320 3a3a 2050 7974 686f 6e20  aries :: Python 
-00000210: 4d6f 6475 6c65 730d 0a70 726f 6a65 6374  Modules..project
-00000220: 5f75 726c 7320 3d20 0d0a 0942 7567 2054  _urls = ...Bug T
-00000230: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
-00000240: 2f67 6974 6875 622e 636f 6d2f 616c 7468  /github.com/alth
-00000250: 6f6e 6f73 2f63 7279 7074 6f2d 7061 792d  onos/crypto-pay-
-00000260: 6170 692d 7364 6b2f 6973 7375 6573 0d0a  api-sdk/issues..
-00000270: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 616b  ..[options]..pak
-00000280: 6167 655f 6469 7220 3d20 0d0a 093d 2063  age_dir = ...= c
-00000290: 7279 7074 6f5f 7061 795f 6170 695f 7364  rypto_pay_api_sd
-000002a0: 6b0d 0a70 6163 6b61 6765 7320 3d20 6669  k..packages = fi
-000002b0: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
-000002c0: 6972 6573 203d 203e 3d20 332e 360d 0a0d  ires = >= 3.6...
-000002d0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000002e0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-000002f0: 3d20 6372 7970 746f 5f70 6179 5f61 7069  = crypto_pay_api
-00000300: 5f73 646b 0d0a 0d0a 5b65 6767 5f69 6e66  _sdk....[egg_inf
-00000310: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000320: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000330: 0d0a                                     ..
+00000090: 636f 6d2f 736c 6c61 766f 6e2f 6372 7970  com/sllavon/cryp
+000000a0: 746f 2d70 6179 2d61 7069 2d73 646b 0d0a  to-pay-api-sdk..
+000000b0: 6465 7363 7269 7074 696f 6e20 3d20 4150  description = AP
+000000c0: 4920 666f 7220 4372 7970 746f 426f 740d  I for CryptoBot.
+000000d0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000e0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000f0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
+00000100: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+00000110: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+00000120: 776e 0d0a 6c69 6365 6e73 6520 3d20 4d49  wn..license = MI
+00000130: 540d 0a63 6c61 7373 6966 6965 7273 203d  T..classifiers =
+00000140: 200d 0a09 496e 7465 6e64 6564 2041 7564   ...Intended Aud
+00000150: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+00000160: 6572 730d 0a09 4c69 6365 6e73 6520 3a3a  ers...License ::
+00000170: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000180: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
+00000190: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000001a0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000001b0: 740d 0a09 5072 6f67 7261 6d6d 696e 6720  t...Programming 
+000001c0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001d0: 6f6e 203a 3a20 330d 0a09 546f 7069 6320  on :: 3...Topic 
+000001e0: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
+000001f0: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
+00000200: 7269 6573 203a 3a20 5079 7468 6f6e 204d  ries :: Python M
+00000210: 6f64 756c 6573 0d0a 7072 6f6a 6563 745f  odules..project_
+00000220: 7572 6c73 203d 200d 0a09 4275 6720 5472  urls = ...Bug Tr
+00000230: 6163 6b65 7220 3d20 6874 7470 733a 2f2f  acker = https://
+00000240: 6769 7468 7562 2e63 6f6d 2f73 6c6c 6176  github.com/sllav
+00000250: 6f6e 2f63 7279 7074 6f2d 7061 792d 6170  on/crypto-pay-ap
+00000260: 692d 7364 6b2f 6973 7375 6573 0d0a 0d0a  i-sdk/issues....
+00000270: 5b6f 7074 696f 6e73 5d0d 0a70 616b 6167  [options]..pakag
+00000280: 655f 6469 7220 3d20 0d0a 093d 2063 7279  e_dir = ...= cry
+00000290: 7074 6f5f 7061 795f 6170 695f 7364 6b0d  pto_pay_api_sdk.
+000002a0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+000002b0: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+000002c0: 6573 203d 203e 3d20 332e 360d 0a0d 0a5b  es = >= 3.6....[
+000002d0: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+000002e0: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+000002f0: 6372 7970 746f 5f70 6179 5f61 7069 5f73  crypto_pay_api_s
+00000300: 646b 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  dk....[egg_info]
+00000310: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000320: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `crypto_pay_api_sdk-1.3.2/setup.py` & `crypto_pay_api_sdk-1.3.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from io import open
 from setuptools import setup
 
-version = '1.3.2'
+version = '1.3.3'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name = 'crypto_pay_api_sdk',
     author = 'Vyacheslav Zhigulin',
     author_email = 'muxellexum@gmail.com',
-    url = 'https://github.com/althonos/crypto-pay-api-sdk',
+    url = 'https://github.com/sllavon/crypto-pay-api-sdk',
     description = 'API for CryptoBot',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     license = 'MIT',
     classifiers = [
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

