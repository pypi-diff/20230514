# Comparing `tmp/kynaylibs-7.0.8.tar.gz` & `tmp/kynaylibs-7.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-7.0.8.tar", last modified: Sun May 14 21:05:24 2023, max compression
+gzip compressed data, was "kynaylibs-7.0.9.tar", last modified: Sun May 14 21:08:34 2023, max compression
```

## Comparing `kynaylibs-7.0.8.tar` & `kynaylibs-7.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:05:24.330350 kynaylibs-7.0.8/
--rw-r--r--   0 root         (0) root         (0)    35182 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 21:05:24.330350 kynaylibs-7.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:05:24.330350 kynaylibs-7.0.8/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)     3438 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1331 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/config.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:05:24.330350 kynaylibs-7.0.8/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)     2071 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:05:24.330350 kynaylibs-7.0.8/kynaylibs/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-14 20:20:56.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-14 20:58:24.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:05:24.330350 kynaylibs-7.0.8/kynaylibs/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)     8104 2023-05-14 20:58:24.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-05-14 21:04:54.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17782 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 20:20:56.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/kynaylibs/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 21:04:54.000000 kynaylibs-7.0.8/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:05:24.330350 kynaylibs-7.0.8/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 21:05:24.000000 kynaylibs-7.0.8/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      901 2023-05-14 21:05:24.000000 kynaylibs-7.0.8/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 21:05:24.000000 kynaylibs-7.0.8/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      335 2023-05-14 21:05:24.000000 kynaylibs-7.0.8/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-14 21:05:24.000000 kynaylibs-7.0.8/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 21:05:24.330350 kynaylibs-7.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1547 2023-05-14 19:46:25.000000 kynaylibs-7.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:08:34.243925 kynaylibs-7.0.9/
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 21:08:34.243925 kynaylibs-7.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:08:34.239925 kynaylibs-7.0.9/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)     3438 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2023-05-14 21:08:11.000000 kynaylibs-7.0.9/kynaylibs/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/config.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:08:34.239925 kynaylibs-7.0.9/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:08:34.239925 kynaylibs-7.0.9/kynaylibs/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-14 20:20:56.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-14 20:58:24.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:08:34.243925 kynaylibs-7.0.9/kynaylibs/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)     8104 2023-05-14 20:58:24.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-14 21:04:54.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/pilter.py
+-rw-r--r--   0 root         (0) root         (0)    17782 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 20:20:56.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/kynaylibs/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 21:08:11.000000 kynaylibs-7.0.9/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:08:34.239925 kynaylibs-7.0.9/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 21:08:34.000000 kynaylibs-7.0.9/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      901 2023-05-14 21:08:34.000000 kynaylibs-7.0.9/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 21:08:34.000000 kynaylibs-7.0.9/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      335 2023-05-14 21:08:34.000000 kynaylibs-7.0.9/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-14 21:08:34.000000 kynaylibs-7.0.9/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 21:08:34.243925 kynaylibs-7.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-05-14 19:46:25.000000 kynaylibs-7.0.9/setup.py
```

### Comparing `kynaylibs-7.0.8/LICENSE` & `kynaylibs-7.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/PKG-INFO` & `kynaylibs-7.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 7.0.8
+Version: 7.0.9
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-7.0.8/README.md` & `kynaylibs-7.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/__init__.py` & `kynaylibs-7.0.9/kynaylibs/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/__main__.py` & `kynaylibs-7.0.9/kynaylibs/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from platform import python_version as py
 
 from modules import ALL_MODULES
 from pyrogram import __version__ as pyro
 from pyrogram import idle
 from uvloop import install
 
-from kynaylibs import LOGGER, aiosession, app, bots, ids
+from kynaylibs import *
 from kynaylibs.nan import *
-from kynaylibs.nan.db import *
+from kynaylibs.nan.utils.db import *
 
 from .version import __version__ as nay
 
 BOT_VER = "8.1.0"
 
 
 MSG_ON = """
```

### Comparing `kynaylibs-7.0.8/kynaylibs/config.py` & `kynaylibs-7.0.9/kynaylibs/config.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/logging.py` & `kynaylibs-7.0.9/kynaylibs/logging.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/__init__.py` & `kynaylibs-7.0.9/kynaylibs/nan/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/PyroHelpers.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/adminHelpers.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/ai.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/ai.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/aiohttp_helper.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/basic.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/basic.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/constants.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/constants.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/db/__init__.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/db/permit.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/function.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/function.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/inline.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/inline.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/interval.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/interval.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/misc.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/parser.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/parser.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/pilter.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/tools.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/tools.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/unpack.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs/nan/utils/utility.py` & `kynaylibs-7.0.9/kynaylibs/nan/utils/utility.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-7.0.9/kynaylibs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 7.0.8
+Version: 7.0.9
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-7.0.8/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-7.0.9/kynaylibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.0.8/setup.py` & `kynaylibs-7.0.9/setup.py`

 * *Files identical despite different names*

