# Comparing `tmp/kynaylibs-7.1.1.tar.gz` & `tmp/kynaylibs-7.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-7.1.1.tar", last modified: Sun May 14 21:32:22 2023, max compression
+gzip compressed data, was "kynaylibs-7.1.2.tar", last modified: Sun May 14 21:46:29 2023, max compression
```

## Comparing `kynaylibs-7.1.1.tar` & `kynaylibs-7.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:32:22.611345 kynaylibs-7.1.1/
--rw-r--r--   0 root         (0) root         (0)    35182 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 21:32:22.611345 kynaylibs-7.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:32:22.611345 kynaylibs-7.1.1/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)     1447 2023-05-14 21:32:06.000000 kynaylibs-7.1.1/kynaylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:32:22.611345 kynaylibs-7.1.1/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)      704 2023-05-14 21:32:06.000000 kynaylibs-7.1.1/kynaylibs/nan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:32:22.611345 kynaylibs-7.1.1/kynaylibs/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-14 20:20:56.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-14 21:32:06.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:32:22.611345 kynaylibs-7.1.1/kynaylibs/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)     8093 2023-05-14 21:32:06.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-05-14 21:04:54.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17782 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 20:20:56.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/kynaylibs/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 21:32:06.000000 kynaylibs-7.1.1/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:32:22.611345 kynaylibs-7.1.1/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 21:32:22.000000 kynaylibs-7.1.1/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      838 2023-05-14 21:32:22.000000 kynaylibs-7.1.1/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 21:32:22.000000 kynaylibs-7.1.1/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      335 2023-05-14 21:32:22.000000 kynaylibs-7.1.1/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-14 21:32:22.000000 kynaylibs-7.1.1/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 21:32:22.611345 kynaylibs-7.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1547 2023-05-14 19:46:25.000000 kynaylibs-7.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:46:29.949216 kynaylibs-7.1.2/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-05-14 21:46:05.000000 kynaylibs-7.1.2/kynaylibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)      704 2023-05-14 21:32:06.000000 kynaylibs-7.1.2/kynaylibs/nan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/kynaylibs/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-14 20:20:56.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-14 21:32:06.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/kynaylibs/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)     8093 2023-05-14 21:32:06.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-14 21:04:54.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/pilter.py
+-rw-r--r--   0 root         (0) root         (0)    17782 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-14 20:20:56.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/kynaylibs/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-14 21:46:05.000000 kynaylibs-7.1.2/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-05-14 21:46:29.000000 kynaylibs-7.1.2/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      838 2023-05-14 21:46:29.000000 kynaylibs-7.1.2/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 21:46:29.000000 kynaylibs-7.1.2/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      335 2023-05-14 21:46:29.000000 kynaylibs-7.1.2/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-14 21:46:29.000000 kynaylibs-7.1.2/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 21:46:29.953216 kynaylibs-7.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-05-14 19:46:25.000000 kynaylibs-7.1.2/setup.py
```

### Comparing `kynaylibs-7.1.1/LICENSE` & `kynaylibs-7.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/PKG-INFO` & `kynaylibs-7.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 7.1.1
+Version: 7.1.2
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-7.1.1/README.md` & `kynaylibs-7.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/__init__.py` & `kynaylibs-7.1.2/kynaylibs/nan/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/PyroHelpers.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/adminHelpers.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/ai.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/ai.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/aiohttp_helper.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/basic.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/basic.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/constants.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/constants.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/db/__init__.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/db/permit.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/function.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/function.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/inline.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/inline.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/interval.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/interval.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/misc.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/parser.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/parser.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/pilter.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/tools.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/tools.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/unpack.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs/nan/utils/utility.py` & `kynaylibs-7.1.2/kynaylibs/nan/utils/utility.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-7.1.2/kynaylibs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 7.1.1
+Version: 7.1.2
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-7.1.1/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-7.1.2/kynaylibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-7.1.1/setup.py` & `kynaylibs-7.1.2/setup.py`

 * *Files identical despite different names*

