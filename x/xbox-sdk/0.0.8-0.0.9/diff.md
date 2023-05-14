# Comparing `tmp/xbox-sdk-0.0.8.tar.gz` & `tmp/xbox-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbox-sdk-0.0.8.tar", last modified: Sun May 14 07:11:31 2023, max compression
+gzip compressed data, was "xbox-sdk-0.0.9.tar", last modified: Sun May 14 07:15:24 2023, max compression
```

## Comparing `xbox-sdk-0.0.8.tar` & `xbox-sdk-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 07:11:31.567791 xbox-sdk-0.0.8/
--rw-rw-rw-   0        0        0     1095 2023-04-21 22:02:29.000000 xbox-sdk-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      645 2023-05-14 07:11:31.567791 xbox-sdk-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-21 22:02:29.000000 xbox-sdk-0.0.8/README.md
--rw-rw-rw-   0        0        0      535 2023-04-21 22:02:29.000000 xbox-sdk-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1031 2023-05-14 07:11:31.568791 xbox-sdk-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 07:11:31.543258 xbox-sdk-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 07:11:31.550778 xbox-sdk-0.0.8/src/xbox_sdk/
--rw-rw-rw-   0        0        0       64 2023-05-14 04:20:49.000000 xbox-sdk-0.0.8/src/xbox_sdk/__init__.py
--rw-rw-rw-   0        0        0     2640 2023-05-14 06:30:51.000000 xbox-sdk-0.0.8/src/xbox_sdk/gamer.py
-drwxrwxrwx   0        0        0        0 2023-05-14 07:11:31.558790 xbox-sdk-0.0.8/src/xbox_sdk/lib/
--rw-rw-rw-   0        0        0        0 2023-05-14 03:42:03.000000 xbox-sdk-0.0.8/src/xbox_sdk/lib/__init__.py
--rw-rw-rw-   0        0        0     4634 2023-05-14 05:44:49.000000 xbox-sdk-0.0.8/src/xbox_sdk/lib/client.py
--rw-rw-rw-   0        0        0     1501 2023-05-14 05:30:27.000000 xbox-sdk-0.0.8/src/xbox_sdk/lib/errors.py
--rw-rw-rw-   0        0        0     1050 2023-05-14 03:32:00.000000 xbox-sdk-0.0.8/src/xbox_sdk/lib/timer.py
--rw-rw-rw-   0        0        0        0 2023-04-21 22:02:29.000000 xbox-sdk-0.0.8/src/xbox_sdk/py.typed
--rw-rw-rw-   0        0        0     4622 2023-04-21 22:02:29.000000 xbox-sdk-0.0.8/src/xbox_sdk/scraper.py
--rw-rw-rw-   0        0        0     8633 2023-05-14 06:33:43.000000 xbox-sdk-0.0.8/src/xbox_sdk/user.py
-drwxrwxrwx   0        0        0        0 2023-05-14 07:11:31.566792 xbox-sdk-0.0.8/src/xbox_sdk/xapi/
--rw-rw-rw-   0        0        0      474 2023-05-14 06:04:13.000000 xbox-sdk-0.0.8/src/xbox_sdk/xapi/__init__.py
--rw-rw-rw-   0        0        0      549 2023-05-14 05:22:01.000000 xbox-sdk-0.0.8/src/xbox_sdk/xapi/acheivements.py
--rw-rw-rw-   0        0        0      932 2023-05-14 05:20:04.000000 xbox-sdk-0.0.8/src/xbox_sdk/xapi/clubs.py
--rw-rw-rw-   0        0        0      695 2023-05-14 06:05:00.000000 xbox-sdk-0.0.8/src/xbox_sdk/xapi/content.py
--rw-rw-rw-   0        0        0     1001 2023-05-14 05:14:23.000000 xbox-sdk-0.0.8/src/xbox_sdk/xapi/marketplace.py
--rw-rw-rw-   0        0        0     1067 2023-05-14 05:48:35.000000 xbox-sdk-0.0.8/src/xbox_sdk/xapi/profile.py
--rw-rw-rw-   0        0        0     1827 2023-05-14 06:04:13.000000 xbox-sdk-0.0.8/src/xbox_sdk/xapi/profile_specific.py
--rw-rw-rw-   0        0        0      521 2023-05-14 05:05:39.000000 xbox-sdk-0.0.8/src/xbox_sdk/xapi/social.py
--rw-rw-rw-   0        0        0      215 2023-05-14 06:04:13.000000 xbox-sdk-0.0.8/src/xbox_sdk/xapi/stats.py
--rw-rw-rw-   0        0        0      838 2023-05-14 03:43:23.000000 xbox-sdk-0.0.8/src/xbox_sdk/xapi/xapi.py
-drwxrwxrwx   0        0        0        0 2023-05-14 07:11:31.555791 xbox-sdk-0.0.8/src/xbox_sdk.egg-info/
--rw-rw-rw-   0        0        0      645 2023-05-14 07:11:31.000000 xbox-sdk-0.0.8/src/xbox_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      745 2023-05-14 07:11:31.000000 xbox-sdk-0.0.8/src/xbox_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 07:11:31.000000 xbox-sdk-0.0.8/src/xbox_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2023-05-14 07:11:31.000000 xbox-sdk-0.0.8/src/xbox_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 07:11:31.000000 xbox-sdk-0.0.8/src/xbox_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 07:15:24.553230 xbox-sdk-0.0.9/
+-rw-rw-rw-   0        0        0     1095 2023-04-21 22:02:29.000000 xbox-sdk-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      645 2023-05-14 07:15:24.554229 xbox-sdk-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-21 22:02:29.000000 xbox-sdk-0.0.9/README.md
+-rw-rw-rw-   0        0        0      535 2023-04-21 22:02:29.000000 xbox-sdk-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1031 2023-05-14 07:15:24.555229 xbox-sdk-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 07:15:24.527341 xbox-sdk-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 07:15:24.534614 xbox-sdk-0.0.9/src/xbox_sdk/
+-rw-rw-rw-   0        0        0       64 2023-05-14 04:20:49.000000 xbox-sdk-0.0.9/src/xbox_sdk/__init__.py
+-rw-rw-rw-   0        0        0     2640 2023-05-14 06:30:51.000000 xbox-sdk-0.0.9/src/xbox_sdk/gamer.py
+drwxrwxrwx   0        0        0        0 2023-05-14 07:15:24.543231 xbox-sdk-0.0.9/src/xbox_sdk/lib/
+-rw-rw-rw-   0        0        0        0 2023-05-14 03:42:03.000000 xbox-sdk-0.0.9/src/xbox_sdk/lib/__init__.py
+-rw-rw-rw-   0        0        0     4634 2023-05-14 05:44:49.000000 xbox-sdk-0.0.9/src/xbox_sdk/lib/client.py
+-rw-rw-rw-   0        0        0     1502 2023-05-14 07:15:11.000000 xbox-sdk-0.0.9/src/xbox_sdk/lib/errors.py
+-rw-rw-rw-   0        0        0     1050 2023-05-14 03:32:00.000000 xbox-sdk-0.0.9/src/xbox_sdk/lib/timer.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 22:02:29.000000 xbox-sdk-0.0.9/src/xbox_sdk/py.typed
+-rw-rw-rw-   0        0        0     4622 2023-04-21 22:02:29.000000 xbox-sdk-0.0.9/src/xbox_sdk/scraper.py
+-rw-rw-rw-   0        0        0     8633 2023-05-14 06:33:43.000000 xbox-sdk-0.0.9/src/xbox_sdk/user.py
+drwxrwxrwx   0        0        0        0 2023-05-14 07:15:24.553230 xbox-sdk-0.0.9/src/xbox_sdk/xapi/
+-rw-rw-rw-   0        0        0      474 2023-05-14 06:04:13.000000 xbox-sdk-0.0.9/src/xbox_sdk/xapi/__init__.py
+-rw-rw-rw-   0        0        0      549 2023-05-14 05:22:01.000000 xbox-sdk-0.0.9/src/xbox_sdk/xapi/acheivements.py
+-rw-rw-rw-   0        0        0      932 2023-05-14 05:20:04.000000 xbox-sdk-0.0.9/src/xbox_sdk/xapi/clubs.py
+-rw-rw-rw-   0        0        0      695 2023-05-14 06:05:00.000000 xbox-sdk-0.0.9/src/xbox_sdk/xapi/content.py
+-rw-rw-rw-   0        0        0     1001 2023-05-14 05:14:23.000000 xbox-sdk-0.0.9/src/xbox_sdk/xapi/marketplace.py
+-rw-rw-rw-   0        0        0     1067 2023-05-14 05:48:35.000000 xbox-sdk-0.0.9/src/xbox_sdk/xapi/profile.py
+-rw-rw-rw-   0        0        0     1827 2023-05-14 06:04:13.000000 xbox-sdk-0.0.9/src/xbox_sdk/xapi/profile_specific.py
+-rw-rw-rw-   0        0        0      521 2023-05-14 05:05:39.000000 xbox-sdk-0.0.9/src/xbox_sdk/xapi/social.py
+-rw-rw-rw-   0        0        0      215 2023-05-14 06:04:13.000000 xbox-sdk-0.0.9/src/xbox_sdk/xapi/stats.py
+-rw-rw-rw-   0        0        0      838 2023-05-14 03:43:23.000000 xbox-sdk-0.0.9/src/xbox_sdk/xapi/xapi.py
+drwxrwxrwx   0        0        0        0 2023-05-14 07:15:24.539229 xbox-sdk-0.0.9/src/xbox_sdk.egg-info/
+-rw-rw-rw-   0        0        0      645 2023-05-14 07:15:24.000000 xbox-sdk-0.0.9/src/xbox_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      745 2023-05-14 07:15:24.000000 xbox-sdk-0.0.9/src/xbox_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 07:15:24.000000 xbox-sdk-0.0.9/src/xbox_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-05-14 07:15:24.000000 xbox-sdk-0.0.9/src/xbox_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 07:15:24.000000 xbox-sdk-0.0.9/src/xbox_sdk.egg-info/top_level.txt
```

### Comparing `xbox-sdk-0.0.8/LICENSE` & `xbox-sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/PKG-INFO` & `xbox-sdk-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbox-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: This application accesses the Xbox Live system.
 Home-page: https://github.com/mjlomeli/Xbox_SDK
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/Xbox_SDK/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `xbox-sdk-0.0.8/pyproject.toml` & `xbox-sdk-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/setup.cfg` & `xbox-sdk-0.0.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2078 626f 782d 7364 6b0d 0a76 6572   = xbox-sdk..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 7465  sion = 0.0.8..te
+00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 7465  sion = 0.0.9..te
 00000030: 7374 5f76 6572 7369 6f6e 203d 2030 2e30  st_version = 0.0
 00000040: 2e36 0d0a 7072 6f64 7563 7469 6f6e 5f76  .6..production_v
-00000050: 6572 7369 6f6e 203d 2030 2e30 2e38 0d0a  ersion = 0.0.8..
+00000050: 6572 7369 6f6e 203d 2030 2e30 2e39 0d0a  ersion = 0.0.9..
 00000060: 6175 7468 6f72 203d 204d 6175 7269 6369  author = Maurici
 00000070: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
 00000080: 3d20 6465 762e 6d61 7572 6963 696f 2e6c  = dev.mauricio.l
 00000090: 6f6d 656c 6940 676d 6169 6c2e 636f 6d0d  omeli@gmail.com.
 000000a0: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
 000000b0: 6869 7320 6170 706c 6963 6174 696f 6e20  his application 
 000000c0: 6163 6365 7373 6573 2074 6865 2058 626f  accesses the Xbo
```

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/gamer.py` & `xbox-sdk-0.0.9/src/xbox_sdk/gamer.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/lib/client.py` & `xbox-sdk-0.0.9/src/xbox_sdk/lib/client.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/lib/errors.py` & `xbox-sdk-0.0.9/src/xbox_sdk/lib/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,11 +31,11 @@
         raise requests.RequestException(f"{message}\n{hint}")
 
 
 def assert_success(response: Response):
     assert_response_is_ok(response)
     assert_response_is_json(response)
     #assert_response_is_xapi_data(response)
-    data = response.json()
+    #data = response.json()
 
     #if data['status'] != 'success':
     #    raise requests.RequestException(f"[XAPI Error]: {data['message']} ({response.url})")
```

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/lib/timer.py` & `xbox-sdk-0.0.9/src/xbox_sdk/lib/timer.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/scraper.py` & `xbox-sdk-0.0.9/src/xbox_sdk/scraper.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/user.py` & `xbox-sdk-0.0.9/src/xbox_sdk/user.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/xapi/acheivements.py` & `xbox-sdk-0.0.9/src/xbox_sdk/xapi/acheivements.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/xapi/clubs.py` & `xbox-sdk-0.0.9/src/xbox_sdk/xapi/clubs.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/xapi/content.py` & `xbox-sdk-0.0.9/src/xbox_sdk/xapi/content.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/xapi/marketplace.py` & `xbox-sdk-0.0.9/src/xbox_sdk/xapi/marketplace.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/xapi/profile.py` & `xbox-sdk-0.0.9/src/xbox_sdk/xapi/profile.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/xapi/profile_specific.py` & `xbox-sdk-0.0.9/src/xbox_sdk/xapi/profile_specific.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/xapi/social.py` & `xbox-sdk-0.0.9/src/xbox_sdk/xapi/social.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk/xapi/xapi.py` & `xbox-sdk-0.0.9/src/xbox_sdk/xapi/xapi.py`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk.egg-info/PKG-INFO` & `xbox-sdk-0.0.9/src/xbox_sdk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbox-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: This application accesses the Xbox Live system.
 Home-page: https://github.com/mjlomeli/Xbox_SDK
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/Xbox_SDK/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `xbox-sdk-0.0.8/src/xbox_sdk.egg-info/SOURCES.txt` & `xbox-sdk-0.0.9/src/xbox_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

