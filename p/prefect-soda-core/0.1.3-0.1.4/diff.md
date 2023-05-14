# Comparing `tmp/prefect-soda-core-0.1.3.tar.gz` & `tmp/prefect-soda-core-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-soda-core/prefect-soda-core/dist/.tmp-by7lh7um/prefect-soda-core-0.1.3.tar", last modified: Sat Dec 24 18:38:40 2022, max compression
+gzip compressed data, was "/home/runner/work/prefect-soda-core/prefect-soda-core/dist/.tmp-w2pkzorz/prefect-soda-core-0.1.4.tar", last modified: Sun May 14 19:14:24 2023, max compression
```

## Comparing `prefect-soda-core-0.1.3.tar` & `prefect-soda-core-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 18:38:40.000000 prefect-soda-core-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2022-12-24 18:37:07.000000 prefect-soda-core-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-24 18:37:07.000000 prefect-soda-core-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2022-12-24 18:38:40.000000 prefect-soda-core-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2022-12-24 18:37:07.000000 prefect-soda-core-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 18:38:40.000000 prefect-soda-core-0.1.3/prefect_soda_core/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-24 18:37:07.000000 prefect-soda-core-0.1.3/prefect_soda_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-24 18:38:40.000000 prefect-soda-core-0.1.3/prefect_soda_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-24 18:37:07.000000 prefect-soda-core-0.1.3/prefect_soda_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2022-12-24 18:37:07.000000 prefect-soda-core-0.1.3/prefect_soda_core/soda_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2022-12-24 18:37:07.000000 prefect-soda-core-0.1.3/prefect_soda_core/sodacl_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2022-12-24 18:37:07.000000 prefect-soda-core-0.1.3/prefect_soda_core/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-24 18:38:40.000000 prefect-soda-core-0.1.3/prefect_soda_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2022-12-24 18:38:40.000000 prefect-soda-core-0.1.3/prefect_soda_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2022-12-24 18:38:40.000000 prefect-soda-core-0.1.3/prefect_soda_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-24 18:38:40.000000 prefect-soda-core-0.1.3/prefect_soda_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      517 2022-12-24 18:38:40.000000 prefect-soda-core-0.1.3/prefect_soda_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-24 18:38:40.000000 prefect-soda-core-0.1.3/prefect_soda_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      779 2022-12-24 18:38:40.000000 prefect-soda-core-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2022-12-24 18:37:07.000000 prefect-soda-core-0.1.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2022-12-24 18:37:07.000000 prefect-soda-core-0.1.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/prefect_soda_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/prefect_soda_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/prefect_soda_core/soda_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/prefect_soda_core/sodacl_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/prefect_soda_core/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/prefect_soda_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:14:24.000000 prefect-soda-core-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/tests/test_soda_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/tests/test_sodacl_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-14 19:12:22.000000 prefect-soda-core-0.1.4/versioneer.py
```

### Comparing `prefect-soda-core-0.1.3/LICENSE` & `prefect-soda-core-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.3/PKG-INFO` & `prefect-soda-core-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-soda-core
-Version: 0.1.3
+Version: 0.1.4
 Summary: Prefect 2.0 collection for Soda Core
 Home-page: https://github.com/sodadata/prefect-soda-core
 Author: Soda Data NV.
 Author-email: vijay@soda.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -15,24 +15,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: sqlserver
-Provides-Extra: postgres
-Provides-Extra: spark-df
-Provides-Extra: athena
 Provides-Extra: redshift
-Provides-Extra: trino
-Provides-Extra: bigquery
 Provides-Extra: db2
+Provides-Extra: sqlserver
+Provides-Extra: athena
+Provides-Extra: spark-df
 Provides-Extra: snowflake
 Provides-Extra: mysql
+Provides-Extra: postgres
+Provides-Extra: trino
+Provides-Extra: bigquery
 Provides-Extra: dev
 License-File: LICENSE
 
 # prefect-soda-core
 
 ## Welcome!
```

### Comparing `prefect-soda-core-0.1.3/README.md` & `prefect-soda-core-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.3/prefect_soda_core/soda_configuration.py` & `prefect-soda-core-0.1.4/prefect_soda_core/soda_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,17 @@
         ```
     """
 
     configuration_yaml_path: str
     configuration_yaml_str: Optional[str]
 
     _block_type_name: Optional[str] = "Soda Configuration"
-    _logo_url: Optional[HttpUrl] = "https://www.TODO.todo"  # noqa
+    _logo_url: Optional[
+        HttpUrl
+    ] = "https://github.com/PrefectHQ/prefect/blob/main/docs/img/collections/soda.png"  # noqa
 
     @root_validator(pre=True)
     def check_block_configuration(cls, values):
         """
         Ensure that the configuration options are valid.
         A configuration is valid if it provides just the path to the
         YAML configuration file or if it has both the path
```

### Comparing `prefect-soda-core-0.1.3/prefect_soda_core/sodacl_check.py` & `prefect-soda-core-0.1.4/prefect_soda_core/sodacl_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,17 @@
         ```
     """
 
     sodacl_yaml_path: str
     sodacl_yaml_str: Optional[str]
 
     _block_type_name: Optional[str] = "SodaCL Check"
-    _logo_url: Optional[HttpUrl] = "https://www.to.do"  # noqa
+    _logo_url: Optional[
+        HttpUrl
+    ] = "https://github.com/PrefectHQ/prefect/blob/main/docs/img/collections/soda.png"  # noqa
 
     @root_validator(pre=True)
     def check_block_configuration(cls, values):
         """
         Ensure that the check configuration options are valid.
         A check configuration is valid if it provides just the path to the
         YAML Soda checks file or if it has both the path
```

### Comparing `prefect-soda-core-0.1.3/prefect_soda_core/tasks.py` & `prefect-soda-core-0.1.4/prefect_soda_core/tasks.py`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.3/prefect_soda_core.egg-info/PKG-INFO` & `prefect-soda-core-0.1.4/prefect_soda_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-soda-core
-Version: 0.1.3
+Version: 0.1.4
 Summary: Prefect 2.0 collection for Soda Core
 Home-page: https://github.com/sodadata/prefect-soda-core
 Author: Soda Data NV.
 Author-email: vijay@soda.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -15,24 +15,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: sqlserver
-Provides-Extra: postgres
-Provides-Extra: spark-df
-Provides-Extra: athena
 Provides-Extra: redshift
-Provides-Extra: trino
-Provides-Extra: bigquery
 Provides-Extra: db2
+Provides-Extra: sqlserver
+Provides-Extra: athena
+Provides-Extra: spark-df
 Provides-Extra: snowflake
 Provides-Extra: mysql
+Provides-Extra: postgres
+Provides-Extra: trino
+Provides-Extra: bigquery
 Provides-Extra: dev
 License-File: LICENSE
 
 # prefect-soda-core
 
 ## Welcome!
```

### Comparing `prefect-soda-core-0.1.3/prefect_soda_core.egg-info/requires.txt` & `prefect-soda-core-0.1.4/prefect_soda_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.3/setup.cfg` & `prefect-soda-core-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.3/setup.py` & `prefect-soda-core-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-soda-core-0.1.3/versioneer.py` & `prefect-soda-core-0.1.4/versioneer.py`

 * *Files identical despite different names*

