# Comparing `tmp/kynaylibs-7.0.6.tar.gz` & `tmp/kynaylibs-7.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-7.0.6.tar", last modified: Sun May 14 20:54:36 2023, max compression
+gzip compressed data, was "kynaylibs-7.0.7.tar", last modified: Sun May 14 20:58:51 2023, max compression
```

## Comparing `kynaylibs-7.0.6.tar` & `kynaylibs-7.0.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 20:54:36.711633 kynaylibs-7.0.6/
--rw-r--r--   0 root         (0) root         (0)    35182 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 20:54:36.711633 kynaylibs-7.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 20:54:36.707632 kynaylibs-7.0.6/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)     3438 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1331 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/config.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 20:54:36.707632 kynaylibs-7.0.6/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)     2071 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 20:54:36.711633 kynaylibs-7.0.6/kynaylibs/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-14 20:20:56.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 20:54:36.711633 kynaylibs-7.0.6/kynaylibs/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)     8088 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/pilter..py
--rw-r--r--   0 root         (0) root         (0)    17782 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 20:20:56.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/kynaylibs/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 20:53:16.000000 kynaylibs-7.0.6/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 20:54:36.707632 kynaylibs-7.0.6/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 20:54:36.000000 kynaylibs-7.0.6/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      902 2023-05-14 20:54:36.000000 kynaylibs-7.0.6/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 20:54:36.000000 kynaylibs-7.0.6/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      335 2023-05-14 20:54:36.000000 kynaylibs-7.0.6/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-14 20:54:36.000000 kynaylibs-7.0.6/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 20:54:36.711633 kynaylibs-7.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1547 2023-05-14 19:46:25.000000 kynaylibs-7.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 20:58:51.634802 kynaylibs-7.0.7/
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 20:58:51.634802 kynaylibs-7.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 20:58:51.630802 kynaylibs-7.0.7/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)     3438 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/config.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 20:58:51.630802 kynaylibs-7.0.7/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 20:58:51.634802 kynaylibs-7.0.7/kynaylibs/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-14 20:20:56.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-14 20:58:24.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 20:58:51.634802 kynaylibs-7.0.7/kynaylibs/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)     8104 2023-05-14 20:58:24.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/pilter..py
+-rw-r--r--   0 root         (0) root         (0)    17782 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 20:20:56.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/kynaylibs/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 20:58:24.000000 kynaylibs-7.0.7/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 20:58:51.630802 kynaylibs-7.0.7/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 20:58:51.000000 kynaylibs-7.0.7/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      902 2023-05-14 20:58:51.000000 kynaylibs-7.0.7/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 20:58:51.000000 kynaylibs-7.0.7/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      335 2023-05-14 20:58:51.000000 kynaylibs-7.0.7/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-14 20:58:51.000000 kynaylibs-7.0.7/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 20:58:51.634802 kynaylibs-7.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-05-14 19:46:25.000000 kynaylibs-7.0.7/setup.py
```

### Comparing `kynaylibs-7.0.6/LICENSE` & `kynaylibs-7.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/PKG-INFO` & `kynaylibs-7.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 7.0.6
+Version: 7.0.7
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-7.0.6/README.md` & `kynaylibs-7.0.7/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/__init__.py` & `kynaylibs-7.0.7/kynaylibs/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/__main__.py` & `kynaylibs-7.0.7/kynaylibs/__main__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/config.py` & `kynaylibs-7.0.7/kynaylibs/config.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/logging.py` & `kynaylibs-7.0.7/kynaylibs/logging.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/__init__.py` & `kynaylibs-7.0.7/kynaylibs/nan/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/PyroHelpers.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/adminHelpers.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/ai.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/ai.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import openai
-from config import OPENAI_API
+
+from kynaylibs.config import OPENAI_API
 
 
 class OpenAi:
     def Text(question):
         openai.api_key = OPENAI_API
         response = openai.Completion.create(
             model="text-davinci-003",
```

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/aiohttp_helper.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/basic.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/basic.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/constants.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/constants.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/db/__init__.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/db/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import asyncio
 from datetime import datetime, timedelta
 from platform import python_version as py
 from typing import Dict, List, Union
 
 import pymongo.errors
 import requests
-from config import *
 from dateutil.relativedelta import relativedelta
 from motor.motor_asyncio import AsyncIOMotorClient as MongoCli
-from naya import *
 from pyrogram import Client
 from pyrogram import __version__ as pyro
 from pyrogram import filters
 from pyrogram.filters import chat
 from pyrogram.types import Message
 
+from kynaylibs import *
+from kynaylibs.config import *
+
 mongo = MongoCli(MONGO_URL)
 db = mongo.naya
 
 coupledb = db.couple
 notesdb = db.notes
 filtersdb = db.filters
 accesdb = db.acces
```

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/db/permit.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/function.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/function.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/inline.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/inline.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/interval.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/interval.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/misc.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/parser.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/parser.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/pilter..py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/pilter..py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/tools.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/tools.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/unpack.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs/nan/utils/utility.py` & `kynaylibs-7.0.7/kynaylibs/nan/utils/utility.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-7.0.7/kynaylibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 7.0.6
+Version: 7.0.7
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-7.0.6/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-7.0.7/kynaylibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.6/setup.py` & `kynaylibs-7.0.7/setup.py`

 * *Files identical despite different names*

