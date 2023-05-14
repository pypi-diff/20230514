# Comparing `tmp/saic_ismart_client-1.2.4.tar.gz` & `tmp/saic_ismart_client-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.2.4.tar", last modified: Sat May 13 21:43:18 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.2.5.tar", last modified: Sun May 14 10:12:11 2023, max compression
```

## Comparing `saic_ismart_client-1.2.4.tar` & `saic_ismart_client-1.2.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:18.646944 saic_ismart_client-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-13 21:43:18.646944 saic_ismart_client-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 21:43:18.646944 saic_ismart_client-1.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:18.642944 saic_ismart_client-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:18.642944 saic_ismart_client-1.2.4/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:18.642944 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:18.642944 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:18.642944 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:18.646944 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/common_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:18.646944 saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:18.646944 saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:18.646944 saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    29630 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:18.642944 saic_ismart_client-1.2.4/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-13 21:43:18.000000 saic_ismart_client-1.2.4/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-13 21:43:18.000000 saic_ismart_client-1.2.4/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 21:43:18.000000 saic_ismart_client-1.2.4/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-13 21:43:18.000000 saic_ismart_client-1.2.4/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-13 21:43:18.000000 saic_ismart_client-1.2.4/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:43:18.646944 saic_ismart_client-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/tests/test_abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-05-13 21:43:04.000000 saic_ismart_client-1.2.4/tests/test_saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.647162 saic_ismart_client-1.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.651162 saic_ismart_client-1.2.5/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.651162 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.651162 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.651162 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21607 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/common_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29707 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.651162 saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-14 10:12:11.000000 saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-14 10:12:11.000000 saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 10:12:11.000000 saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 10:12:11.000000 saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 10:12:11.000000 saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/tests/test_saic_api.py
```

### Comparing `saic_ismart_client-1.2.4/LICENSE` & `saic_ismart_client-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/PKG-INFO` & `saic_ismart_client-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.2.4
+Version: 1.2.5
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.2.4/README.md` & `saic_ismart_client-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/pyproject.toml` & `saic_ismart_client-1.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.165.0",
     "requests >= 2.28.2",
     "urllib3 >= 1.26.14",
```

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.2.5/src/saic_ismart_client/abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.2.5/src/saic_ismart_client/common_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,18 +419,25 @@
         header_bytes = buffered_message_bytes.read(self.header_length)
         header.protocol_version = int(header_bytes[0])
         header.dispatcher_message_length = int(header_bytes[1])
         header.dispatcher_body_encoding = int(header_bytes[2])
 
         decoded_message.reserved = buffered_message_bytes.read(self.reserved_size)
 
-        dispatcher_message_bytes = buffered_message_bytes.read(header.dispatcher_message_length - self.header_length)
-        message_body_dict = self.asn1_tool_uper.decode('MPDispatcherBody', dispatcher_message_bytes)
-        message_body = decoded_message.body
-        message_body.init_from_dict(message_body_dict)
+        if header.protocol_version == 32:
+            message_body = decoded_message.body
+            message_body.application_data_length = 0
+            message_body.result = -1
+            message_body.error_message = 'Skipping unknown protocol version 32'.encode()
+        else:
+            dispatcher_message_bytes = buffered_message_bytes.read(
+                header.dispatcher_message_length - self.header_length)
+            message_body_dict = self.asn1_tool_uper.decode('MPDispatcherBody', dispatcher_message_bytes)
+            message_body = decoded_message.body
+            message_body.init_from_dict(message_body_dict)
 
         if message_body.application_data_length > 0:
             application_data_bytes = buffered_message_bytes.read(message_body.application_data_length)
             application_data_dict = self.asn1_tool_uper.decode(decoded_message.application_data.asn_type,
                                                                application_data_bytes)
             decoded_message.application_data.init_from_dict(application_data_dict)
         else:
```

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.2.5/src/saic_ismart_client/saic_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,14 +613,16 @@
                                 + f'Waiting {self.relogin_delay} seconds before attempting another login')
                 time.sleep(float(self.relogin_delay))
             self.login()
         elif message_body.result == 4:
             # please try again later
             logging.debug(message)
             time.sleep(float(AVG_SMS_DELIVERY_TIME))
+        elif message_body.result == -1:
+            logging.warning(message)
         else:
             logging.error(message)
 
 
 def hash_md5(password: str) -> str:
     return hashlib.md5(password.encode('utf-8')).hexdigest()
```

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.2.4
+Version: 1.2.5
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.2.4/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/tests/test_Message_v1_1.py` & `saic_ismart_client-1.2.5/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/tests/test_Message_v2_1.py` & `saic_ismart_client-1.2.5/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/tests/test_Message_v3_0.py` & `saic_ismart_client-1.2.5/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/tests/test_abrp_api.py` & `saic_ismart_client-1.2.5/tests/test_abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.4/tests/test_saic_api.py` & `saic_ismart_client-1.2.5/tests/test_saic_api.py`

 * *Files identical despite different names*

