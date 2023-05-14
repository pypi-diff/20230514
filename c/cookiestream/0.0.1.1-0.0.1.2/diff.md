# Comparing `tmp/cookiestream-0.0.1.1.tar.gz` & `tmp/cookiestream-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiestream-0.0.1.1.tar", last modified: Sun May 14 21:11:04 2023, max compression
+gzip compressed data, was "cookiestream-0.0.1.2.tar", last modified: Sun May 14 21:37:23 2023, max compression
```

## Comparing `cookiestream-0.0.1.1.tar` & `cookiestream-0.0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:11:04.259560 cookiestream-0.0.1.1/
--rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-10 23:11:22.000000 cookiestream-0.0.1.1/LICENCE
--rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-14 21:11:04.259560 cookiestream-0.0.1.1/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-10 23:11:22.000000 cookiestream-0.0.1.1/README.md
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:11:04.255560 cookiestream-0.0.1.1/configs/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.1/configs/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)      234 2023-05-11 21:21:05.000000 cookiestream-0.0.1.1/configs/base_config.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:11:04.255560 cookiestream-0.0.1.1/cookiestream/
--rw-rw-r--   0 zied      (1000) zied      (1000)       48 2023-05-11 21:26:51.000000 cookiestream-0.0.1.1/cookiestream/__init__.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:11:04.259560 cookiestream-0.0.1.1/cookiestream/src/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.1/cookiestream/src/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)      432 2023-05-11 22:08:24.000000 cookiestream-0.0.1.1/cookiestream/src/clone_template.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     1978 2023-05-11 22:46:42.000000 cookiestream-0.0.1.1/cookiestream/src/make_rename.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     2906 2023-05-14 17:49:27.000000 cookiestream-0.0.1.1/cookiestream/src/modify_yaml_content.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     3781 2023-05-14 20:22:06.000000 cookiestream-0.0.1.1/cookiestream/src/stream.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:11:04.255560 cookiestream-0.0.1.1/cookiestream.egg-info/
--rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-14 21:11:04.000000 cookiestream-0.0.1.1/cookiestream.egg-info/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)      525 2023-05-14 21:11:04.000000 cookiestream-0.0.1.1/cookiestream.egg-info/SOURCES.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-14 21:11:04.000000 cookiestream-0.0.1.1/cookiestream.egg-info/dependency_links.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       43 2023-05-14 21:11:04.000000 cookiestream-0.0.1.1/cookiestream.egg-info/entry_points.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       29 2023-05-14 21:11:04.000000 cookiestream-0.0.1.1/cookiestream.egg-info/requires.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       70 2023-05-14 21:11:04.000000 cookiestream-0.0.1.1/cookiestream.egg-info/top_level.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-14 21:11:04.259560 cookiestream-0.0.1.1/setup.cfg
--rw-rw-r--   0 zied      (1000) zied      (1000)     1994 2023-05-14 21:05:55.000000 cookiestream-0.0.1.1/setup.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:11:04.255560 cookiestream-0.0.1.1/utils/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.1/utils/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-10 23:11:22.000000 cookiestream-0.0.1.1/utils/util.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:37:23.606713 cookiestream-0.0.1.2/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-10 23:11:22.000000 cookiestream-0.0.1.2/LICENCE
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-14 21:37:23.606713 cookiestream-0.0.1.2/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-10 23:11:22.000000 cookiestream-0.0.1.2/README.md
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:37:23.602713 cookiestream-0.0.1.2/configs/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.2/configs/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)      234 2023-05-11 21:21:05.000000 cookiestream-0.0.1.2/configs/base_config.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:37:23.602713 cookiestream-0.0.1.2/cookiestream/
+-rw-rw-r--   0 zied      (1000) zied      (1000)       48 2023-05-11 21:26:51.000000 cookiestream-0.0.1.2/cookiestream/__init__.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:37:23.606713 cookiestream-0.0.1.2/cookiestream/src/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.2/cookiestream/src/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)      432 2023-05-11 22:08:24.000000 cookiestream-0.0.1.2/cookiestream/src/clone_template.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1978 2023-05-11 22:46:42.000000 cookiestream-0.0.1.2/cookiestream/src/make_rename.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     2906 2023-05-14 17:49:27.000000 cookiestream-0.0.1.2/cookiestream/src/modify_yaml_content.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     3781 2023-05-14 20:22:06.000000 cookiestream-0.0.1.2/cookiestream/src/stream.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:37:23.606713 cookiestream-0.0.1.2/cookiestream.egg-info/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4138 2023-05-14 21:37:23.000000 cookiestream-0.0.1.2/cookiestream.egg-info/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)      494 2023-05-14 21:37:23.000000 cookiestream-0.0.1.2/cookiestream.egg-info/SOURCES.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-14 21:37:23.000000 cookiestream-0.0.1.2/cookiestream.egg-info/dependency_links.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       29 2023-05-14 21:37:23.000000 cookiestream-0.0.1.2/cookiestream.egg-info/requires.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       70 2023-05-14 21:37:23.000000 cookiestream-0.0.1.2/cookiestream.egg-info/top_level.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       85 2023-05-14 21:35:49.000000 cookiestream-0.0.1.2/main.sh
+-rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-14 21:37:23.606713 cookiestream-0.0.1.2/setup.cfg
+-rw-rw-r--   0 zied      (1000) zied      (1000)     2018 2023-05-14 21:35:49.000000 cookiestream-0.0.1.2/setup.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-14 21:37:23.602713 cookiestream-0.0.1.2/utils/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-10 23:11:22.000000 cookiestream-0.0.1.2/utils/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-10 23:11:22.000000 cookiestream-0.0.1.2/utils/util.py
```

### Comparing `cookiestream-0.0.1.1/LICENCE` & `cookiestream-0.0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.1/PKG-INFO` & `cookiestream-0.0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiestream
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Generate template based on template_vierge project
 Home-page: https://github.com/Proxia-ai/cookiestream
 Author: BEN OTHMANE Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/Proxia-ai/cookiestream/issues
 Keywords: Python pypi template,python
```

### Comparing `cookiestream-0.0.1.1/README.md` & `cookiestream-0.0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.1/cookiestream/src/make_rename.py` & `cookiestream-0.0.1.2/cookiestream/src/make_rename.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.1/cookiestream/src/modify_yaml_content.py` & `cookiestream-0.0.1.2/cookiestream/src/modify_yaml_content.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.1/cookiestream/src/stream.py` & `cookiestream-0.0.1.2/cookiestream/src/stream.py`

 * *Files identical despite different names*

### Comparing `cookiestream-0.0.1.1/cookiestream.egg-info/PKG-INFO` & `cookiestream-0.0.1.2/cookiestream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiestream
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: Generate template based on template_vierge project
 Home-page: https://github.com/Proxia-ai/cookiestream
 Author: BEN OTHMANE Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/Proxia-ai/cookiestream/issues
 Keywords: Python pypi template,python
```

### Comparing `cookiestream-0.0.1.1/setup.py` & `cookiestream-0.0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,12 @@
               '{}'.format(asset_name)],
     package_dir={
         '{}/src'.format(asset_name): '{}/src'.format(asset_name),
         '{}/utils'.format(asset_name): './utils',
         '{}/configs'.format(asset_name): './configs',
         '{}'.format(asset_name): '{}'.format(asset_name)
     },
-    entry_points={'console_scripts': ['{} = main:main'.format(asset_name)]},
+    scripts=['main.sh'],
+    # entry_points={'console_scripts': ['{} = main:main'.format(asset_name)]},
     # include_package_data=True,
     python_requires=yaml_asset_config[0]["asset_meta_information"]["python_required"]
 )
-
-
-
```

### Comparing `cookiestream-0.0.1.1/utils/util.py` & `cookiestream-0.0.1.2/utils/util.py`

 * *Files identical despite different names*

