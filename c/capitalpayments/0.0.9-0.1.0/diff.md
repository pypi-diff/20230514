# Comparing `tmp/capitalpayments-0.0.9.tar.gz` & `tmp/capitalpayments-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capitalpayments-0.0.9.tar", last modified: Fri May 12 00:59:04 2023, max compression
+gzip compressed data, was "capitalpayments-0.1.0.tar", last modified: Sun May 14 05:16:30 2023, max compression
```

## Comparing `capitalpayments-0.0.9.tar` & `capitalpayments-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-12 00:59:04.695207 capitalpayments-0.0.9/
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1066 2023-05-11 21:44:06.000000 capitalpayments-0.0.9/LICENSE
--rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-12 00:59:04.695053 capitalpayments-0.0.9/PKG-INFO
--rw-r--r--   0 javierfernandez   (501) staff       (20)     2677 2023-05-12 00:01:07.000000 capitalpayments-0.0.9/README.md
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-12 00:59:04.694119 capitalpayments-0.0.9/capitalpayments/
--rw-r--r--   0 javierfernandez   (501) staff       (20)       36 2023-05-12 00:50:40.000000 capitalpayments-0.0.9/capitalpayments/__init__.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)     4177 2023-05-12 00:58:50.000000 capitalpayments-0.0.9/capitalpayments/capitalpaymentscore.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)      620 2023-05-11 23:35:08.000000 capitalpayments-0.0.9/capitalpayments/ipn.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)      977 2023-05-12 00:58:48.000000 capitalpayments-0.0.9/capitalpayments/url_manager.py
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-12 00:59:04.694860 capitalpayments-0.0.9/capitalpayments.egg-info/
--rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-12 00:59:04.000000 capitalpayments-0.0.9/capitalpayments.egg-info/PKG-INFO
--rw-r--r--   0 javierfernandez   (501) staff       (20)      341 2023-05-12 00:59:04.000000 capitalpayments-0.0.9/capitalpayments.egg-info/SOURCES.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-05-12 00:59:04.000000 capitalpayments-0.0.9/capitalpayments.egg-info/dependency_links.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)        9 2023-05-12 00:59:04.000000 capitalpayments-0.0.9/capitalpayments.egg-info/requires.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)       16 2023-05-12 00:59:04.000000 capitalpayments-0.0.9/capitalpayments.egg-info/top_level.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)       38 2023-05-12 00:59:04.695251 capitalpayments-0.0.9/setup.cfg
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1091 2023-05-12 00:50:47.000000 capitalpayments-0.0.9/setup.py
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-14 05:16:30.311008 capitalpayments-0.1.0/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1066 2023-05-11 21:44:06.000000 capitalpayments-0.1.0/LICENSE
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-14 05:16:30.310810 capitalpayments-0.1.0/PKG-INFO
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     2677 2023-05-12 00:01:07.000000 capitalpayments-0.1.0/README.md
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-14 05:16:30.309745 capitalpayments-0.1.0/capitalpayments/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       36 2023-05-12 00:50:40.000000 capitalpayments-0.1.0/capitalpayments/__init__.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     4177 2023-05-12 00:58:50.000000 capitalpayments-0.1.0/capitalpayments/capitalpaymentscore.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      620 2023-05-11 23:35:08.000000 capitalpayments-0.1.0/capitalpayments/ipn.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      977 2023-05-14 05:15:35.000000 capitalpayments-0.1.0/capitalpayments/url_manager.py
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-14 05:16:30.310520 capitalpayments-0.1.0/capitalpayments.egg-info/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-14 05:16:30.000000 capitalpayments-0.1.0/capitalpayments.egg-info/PKG-INFO
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      341 2023-05-14 05:16:30.000000 capitalpayments-0.1.0/capitalpayments.egg-info/SOURCES.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-05-14 05:16:30.000000 capitalpayments-0.1.0/capitalpayments.egg-info/dependency_links.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        9 2023-05-14 05:16:30.000000 capitalpayments-0.1.0/capitalpayments.egg-info/requires.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       16 2023-05-14 05:16:30.000000 capitalpayments-0.1.0/capitalpayments.egg-info/top_level.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       38 2023-05-14 05:16:30.311053 capitalpayments-0.1.0/setup.cfg
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1091 2023-05-14 05:16:28.000000 capitalpayments-0.1.0/setup.py
```

### Comparing `capitalpayments-0.0.9/LICENSE` & `capitalpayments-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.0.9/PKG-INFO` & `capitalpayments-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capitalpayments
-Version: 0.0.9
+Version: 0.1.0
 Summary: For Api Capital Payments
 Author: Javier (leqjl93)
 Author-email: <javier.fernandez.pa93@gmail.com>
 Keywords: python,capitalpayments,paymentprocessor,usdt.trc20
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `capitalpayments-0.0.9/README.md` & `capitalpayments-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.0.9/capitalpayments/capitalpaymentscore.py` & `capitalpayments-0.1.0/capitalpayments/capitalpaymentscore.py`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.0.9/capitalpayments/ipn.py` & `capitalpayments-0.1.0/capitalpayments/ipn.py`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.0.9/capitalpayments/url_manager.py` & `capitalpayments-0.1.0/capitalpayments/url_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 url_manager = {
-    'get_environment': 'https://www.capitalpayments.co/app/api/getEnvironment',
-    'get_account': 'https://www.capitalpayments.co/app/api/getAccount',
-    'login': 'https://www.capitalpayments.co/app/api/login',
+    'get_environment': 'https://www.capitalpayments.me/app/api/getEnvironment',
+    'get_account': 'https://www.capitalpayments.me/app/api/getAccount',
+    'login': 'https://www.capitalpayments.me/app/api/login',
 
     # invoices
-    'create_invoice': 'https://www.capitalpayments.co/app/api/createInvoice',
-    'get_invoice_status': 'https://www.capitalpayments.co/app/api/getInvoiceStatus',
-    'cancel_invoice': 'https://www.capitalpayments.co/app/api/cancelInvoice',
+    'create_invoice': 'https://www.capitalpayments.me/app/api/createInvoice',
+    'get_invoice_status': 'https://www.capitalpayments.me/app/api/getInvoiceStatus',
+    'cancel_invoice': 'https://www.capitalpayments.me/app/api/cancelInvoice',
     
     # payouts
-    'create_payout': 'https://www.capitalpayments.co/app/api/createPayout',
-    'get_payout_status': 'https://www.capitalpayments.co/app/api/getPayoutStatus',
-    'cancel_payout': 'https://www.capitalpayments.co/app/api/cancelPayout',
+    'create_payout': 'https://www.capitalpayments.me/app/api/createPayout',
+    'get_payout_status': 'https://www.capitalpayments.me/app/api/getPayoutStatus',
+    'cancel_payout': 'https://www.capitalpayments.me/app/api/cancelPayout',
 
     # wallet
-    'get_balance': 'https://www.capitalpayments.co/app/api/getBalance',
-    'get_main_wallet': 'https://www.capitalpayments.co/app/api/getMainWallet',
-    'get_wallets': 'https://www.capitalpayments.co/app/api/getWallets'
+    'get_balance': 'https://www.capitalpayments.me/app/api/getBalance',
+    'get_main_wallet': 'https://www.capitalpayments.me/app/api/getMainWallet',
+    'get_wallets': 'https://www.capitalpayments.me/app/api/getWallets'
 }
```

### Comparing `capitalpayments-0.0.9/capitalpayments.egg-info/PKG-INFO` & `capitalpayments-0.1.0/capitalpayments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capitalpayments
-Version: 0.0.9
+Version: 0.1.0
 Summary: For Api Capital Payments
 Author: Javier (leqjl93)
 Author-email: <javier.fernandez.pa93@gmail.com>
 Keywords: python,capitalpayments,paymentprocessor,usdt.trc20
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `capitalpayments-0.0.9/setup.py` & `capitalpayments-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'For Api Capital Payments'
 LONG_DESCRIPTION = 'This SDK connects to Capital Payments Payment Processor Api.'
 
 # Setting up
 setup(
     name="capitalpayments",
     version=VERSION,
```

