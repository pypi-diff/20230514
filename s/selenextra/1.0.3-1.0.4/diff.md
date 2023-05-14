# Comparing `tmp/selenextra-1.0.3.tar.gz` & `tmp/selenextra-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-1.0.3.tar", last modified: Sun May 14 05:01:56 2023, max compression
+gzip compressed data, was "selenextra-1.0.4.tar", last modified: Sun May 14 05:07:44 2023, max compression
```

## Comparing `selenextra-1.0.3.tar` & `selenextra-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 05:01:56.034487 selenextra-1.0.3/
--rw-rw-rw-   0        0        0    35823 2023-05-14 04:52:24.000000 selenextra-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      627 2023-05-14 05:01:56.034487 selenextra-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-05-14 04:52:24.000000 selenextra-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 05:01:55.990605 selenextra-1.0.3/selenextra/
--rw-rw-rw-   0        0        0     4709 2023-05-14 04:59:16.000000 selenextra-1.0.3/selenextra/__init__.py
--rw-rw-rw-   0        0        0       46 2023-05-14 04:52:24.000000 selenextra-1.0.3/selenextra/exceptions.py
--rw-rw-rw-   0        0        0     1030 2023-05-14 04:59:02.000000 selenextra-1.0.3/selenextra/patcher.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:01:56.033490 selenextra-1.0.3/selenextra.egg-info/
--rw-rw-rw-   0        0        0      627 2023-05-14 05:01:55.000000 selenextra-1.0.3/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-14 05:01:55.000000 selenextra-1.0.3/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 05:01:55.000000 selenextra-1.0.3/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-14 05:01:55.000000 selenextra-1.0.3/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-14 05:01:55.000000 selenextra-1.0.3/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 05:01:56.034487 selenextra-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-05-14 04:59:54.000000 selenextra-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:07:44.561365 selenextra-1.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-05-14 05:05:34.000000 selenextra-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      627 2023-05-14 05:07:44.560364 selenextra-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-14 05:05:34.000000 selenextra-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 05:07:44.554380 selenextra-1.0.4/selenextra/
+-rw-rw-rw-   0        0        0     4757 2023-05-14 05:06:55.000000 selenextra-1.0.4/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-05-14 05:05:34.000000 selenextra-1.0.4/selenextra/exceptions.py
+-rw-rw-rw-   0        0        0     1030 2023-05-14 05:05:34.000000 selenextra-1.0.4/selenextra/patcher.py
+drwxrwxrwx   0        0        0        0 2023-05-14 05:07:44.560364 selenextra-1.0.4/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      627 2023-05-14 05:07:44.000000 selenextra-1.0.4/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-14 05:07:44.000000 selenextra-1.0.4/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 05:07:44.000000 selenextra-1.0.4/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-14 05:07:44.000000 selenextra-1.0.4/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-14 05:07:44.000000 selenextra-1.0.4/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 05:07:44.561365 selenextra-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-05-14 05:06:14.000000 selenextra-1.0.4/setup.py
```

### Comparing `selenextra-1.0.3/LICENSE` & `selenextra-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-1.0.3/PKG-INFO` & `selenextra-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 1.0.3
+Version: 1.0.4
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-1.0.3/selenextra/__init__.py` & `selenextra-1.0.4/selenextra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
         kwargs['driver_executable_path'] = self.custom_patcher.executable_path
         kwargs['seleniumwire_options'] = kwargs.get('seleniumwire_options', {})
         kwargs['seleniumwire_options']['mitm_http2'] = False
 
         super().__init__(
             version_main=version,
+            user_multi_procs=user_multi_procs,
             **kwargs
         )
 
     def get_user_agent(self) -> str:
         return self.execute_script('return navigator.userAgent')
 
     def get_cookie_string(self) -> str:
```

### Comparing `selenextra-1.0.3/selenextra/patcher.py` & `selenextra-1.0.4/selenextra/patcher.py`

 * *Files identical despite different names*

### Comparing `selenextra-1.0.3/selenextra.egg-info/PKG-INFO` & `selenextra-1.0.4/selenextra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 1.0.3
+Version: 1.0.4
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

