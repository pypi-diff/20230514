# Comparing `tmp/json-fingerprint-0.9.1.tar.gz` & `tmp/json-fingerprint-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-fingerprint-0.9.1.tar", last modified: Tue Jan  5 00:30:02 2021, max compression
+gzip compressed data, was "json-fingerprint-0.9.2.tar", last modified: Tue Jan  5 10:52:55 2021, max compression
```

## Comparing `json-fingerprint-0.9.1.tar` & `json-fingerprint-0.9.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 00:30:02.643586 json-fingerprint-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (116)       57 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7725 2021-01-05 00:30:02.643586 json-fingerprint-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6006 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 00:30:02.639586 json-fingerprint-0.9.1/json_fingerprint/
--rw-r--r--   0 runner    (1001) docker     (116)      147 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      280 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3280 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/_jfpv1.py
--rw-r--r--   0 runner    (1001) docker     (116)      245 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1811 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/_validators.py
--rw-r--r--   0 runner    (1001) docker     (116)      442 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/decode_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (116)      598 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/fingerprint_match.py
--rw-r--r--   0 runner    (1001) docker     (116)      628 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/json_fingerprint.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 00:30:02.643586 json-fingerprint-0.9.1/json_fingerprint/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      424 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/tests/run.py
--rw-r--r--   0 runner    (1001) docker     (116)     1616 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/tests/test_decode_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (116)     1673 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/tests/test_fingerprint_match.py
--rw-r--r--   0 runner    (1001) docker     (116)     9914 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/tests/test_jfpv1.py
--rw-r--r--   0 runner    (1001) docker     (116)     3970 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/tests/test_json_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (116)     4128 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/tests/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 00:30:02.643586 json-fingerprint-0.9.1/json_fingerprint/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (116)     5319 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/tests/testdata/jfpv1_test_obj_1.json
--rw-r--r--   0 runner    (1001) docker     (116)     5319 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/json_fingerprint/tests/testdata/jfpv1_test_obj_2.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 00:30:02.643586 json-fingerprint-0.9.1/json_fingerprint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7725 2021-01-05 00:30:02.000000 json-fingerprint-0.9.1/json_fingerprint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      850 2021-01-05 00:30:02.000000 json-fingerprint-0.9.1/json_fingerprint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-05 00:30:02.000000 json-fingerprint-0.9.1/json_fingerprint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-01-05 00:30:02.000000 json-fingerprint-0.9.1/json_fingerprint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-05 00:30:02.643586 json-fingerprint-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1132 2021-01-05 00:29:50.000000 json-fingerprint-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 10:52:55.653082 json-fingerprint-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (116)       52 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     7725 2021-01-05 10:52:55.649082 json-fingerprint-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     6006 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 10:52:55.649082 json-fingerprint-0.9.2/json_fingerprint/
+-rw-r--r--   0 runner    (1001) docker     (116)      147 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      280 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3280 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/_jfpv1.py
+-rw-r--r--   0 runner    (1001) docker     (116)      245 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1811 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/_validators.py
+-rw-r--r--   0 runner    (1001) docker     (116)      442 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/decode_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (116)      598 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/fingerprint_match.py
+-rw-r--r--   0 runner    (1001) docker     (116)      628 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/json_fingerprint.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 10:52:55.649082 json-fingerprint-0.9.2/json_fingerprint/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      424 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/tests/run.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1616 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/tests/test_decode_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1673 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/tests/test_fingerprint_match.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9914 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/tests/test_jfpv1.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3970 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/tests/test_json_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4128 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 10:52:55.649082 json-fingerprint-0.9.2/json_fingerprint/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (116)     5319 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/tests/testdata/jfpv1_test_obj_1.json
+-rw-r--r--   0 runner    (1001) docker     (116)     5319 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/json_fingerprint/tests/testdata/jfpv1_test_obj_2.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 10:52:55.649082 json-fingerprint-0.9.2/json_fingerprint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     7725 2021-01-05 10:52:55.000000 json-fingerprint-0.9.2/json_fingerprint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      850 2021-01-05 10:52:55.000000 json-fingerprint-0.9.2/json_fingerprint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-05 10:52:55.000000 json-fingerprint-0.9.2/json_fingerprint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       17 2021-01-05 10:52:55.000000 json-fingerprint-0.9.2/json_fingerprint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-05 10:52:55.653082 json-fingerprint-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1163 2021-01-05 10:52:42.000000 json-fingerprint-0.9.2/setup.py
```

### Comparing `json-fingerprint-0.9.1/PKG-INFO` & `json-fingerprint-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-fingerprint
-Version: 0.9.1
+Version: 0.9.2
 Summary: Create consistent and comparable fingerprints with secure hashes from unordered JSON data
 Home-page: https://github.com/cobaltine/json-fingerprint
 Author: Ville Lehtinen
 Author-email: ville.lehtinen@cobaltine.fi
 License: MIT
 Description: # json-fingerprint
```

### Comparing `json-fingerprint-0.9.1/README.md` & `json-fingerprint-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/json_fingerprint/_jfpv1.py` & `json-fingerprint-0.9.2/json_fingerprint/_jfpv1.py`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/json_fingerprint/_validators.py` & `json-fingerprint-0.9.2/json_fingerprint/_validators.py`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/json_fingerprint/fingerprint_match.py` & `json-fingerprint-0.9.2/json_fingerprint/fingerprint_match.py`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/json_fingerprint/json_fingerprint.py` & `json-fingerprint-0.9.2/json_fingerprint/json_fingerprint.py`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/json_fingerprint/tests/test_decode_fingerprint.py` & `json-fingerprint-0.9.2/json_fingerprint/tests/test_decode_fingerprint.py`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/json_fingerprint/tests/test_fingerprint_match.py` & `json-fingerprint-0.9.2/json_fingerprint/tests/test_fingerprint_match.py`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/json_fingerprint/tests/test_jfpv1.py` & `json-fingerprint-0.9.2/json_fingerprint/tests/test_jfpv1.py`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/json_fingerprint/tests/test_json_fingerprint.py` & `json-fingerprint-0.9.2/json_fingerprint/tests/test_json_fingerprint.py`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/json_fingerprint/tests/test_validators.py` & `json-fingerprint-0.9.2/json_fingerprint/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/json_fingerprint/tests/testdata/jfpv1_test_obj_1.json` & `json-fingerprint-0.9.2/json_fingerprint/tests/testdata/jfpv1_test_obj_1.json`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/json_fingerprint/tests/testdata/jfpv1_test_obj_2.json` & `json-fingerprint-0.9.2/json_fingerprint/tests/testdata/jfpv1_test_obj_2.json`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/json_fingerprint.egg-info/PKG-INFO` & `json-fingerprint-0.9.2/json_fingerprint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-fingerprint
-Version: 0.9.1
+Version: 0.9.2
 Summary: Create consistent and comparable fingerprints with secure hashes from unordered JSON data
 Home-page: https://github.com/cobaltine/json-fingerprint
 Author: Ville Lehtinen
 Author-email: ville.lehtinen@cobaltine.fi
 License: MIT
 Description: # json-fingerprint
```

### Comparing `json-fingerprint-0.9.1/json_fingerprint.egg-info/SOURCES.txt` & `json-fingerprint-0.9.2/json_fingerprint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json-fingerprint-0.9.1/setup.py` & `json-fingerprint-0.9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     author_email='ville.lehtinen@cobaltine.fi',
     license='MIT',
     description='Create consistent and comparable fingerprints with secure hashes from unordered JSON data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cobaltine/json-fingerprint',
     packages=setuptools.find_packages(),
+    include_package_data=True,
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

