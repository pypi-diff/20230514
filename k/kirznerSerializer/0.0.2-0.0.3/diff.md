# Comparing `tmp/kirznerSerializer-0.0.2.tar.gz` & `tmp/kirznerSerializer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirznerSerializer-0.0.2.tar", last modified: Sun May 14 20:51:34 2023, max compression
+gzip compressed data, was "kirznerSerializer-0.0.3.tar", last modified: Sun May 14 20:57:09 2023, max compression
```

## Comparing `kirznerSerializer-0.0.2.tar` & `kirznerSerializer-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 20:51:34.369397 kirznerSerializer-0.0.2/
--rw-rw-rw-   0        0        0      806 2023-05-14 20:51:34.369397 kirznerSerializer-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-05-14 20:16:00.000000 kirznerSerializer-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 20:51:34.353767 kirznerSerializer-0.0.2/kirznerSerializer/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:58:02.000000 kirznerSerializer-0.0.2/kirznerSerializer/__init__.py
--rw-rw-rw-   0        0        0     5802 2023-05-14 20:04:46.000000 kirznerSerializer-0.0.2/kirznerSerializer/base_serializer.py
--rw-rw-rw-   0        0        0     3939 2023-05-14 19:51:30.000000 kirznerSerializer-0.0.2/kirznerSerializer/constants.py
--rw-rw-rw-   0        0        0    10645 2023-05-14 20:04:46.000000 kirznerSerializer-0.0.2/kirznerSerializer/json_serializer.py
--rw-rw-rw-   0        0        0     7825 2023-05-14 20:51:08.000000 kirznerSerializer-0.0.2/kirznerSerializer/xml_serializer.py
-drwxrwxrwx   0        0        0        0 2023-05-14 20:51:34.369397 kirznerSerializer-0.0.2/kirznerSerializer.egg-info/
--rw-rw-rw-   0        0        0      806 2023-05-14 20:51:34.000000 kirznerSerializer-0.0.2/kirznerSerializer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-05-14 20:51:34.000000 kirznerSerializer-0.0.2/kirznerSerializer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 20:51:34.000000 kirznerSerializer-0.0.2/kirznerSerializer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-14 20:51:34.000000 kirznerSerializer-0.0.2/kirznerSerializer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-05-14 20:25:16.000000 kirznerSerializer-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      473 2023-05-14 20:51:34.385015 kirznerSerializer-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 20:51:34.369397 kirznerSerializer-0.0.2/tests/
--rw-rw-rw-   0        0        0     5850 2023-05-14 14:50:03.000000 kirznerSerializer-0.0.2/tests/test_constants.py
--rw-rw-rw-   0        0        0    13015 2023-05-14 20:04:46.000000 kirznerSerializer-0.0.2/tests/test_json.py
--rw-rw-rw-   0        0        0    12822 2023-05-14 20:04:46.000000 kirznerSerializer-0.0.2/tests/test_xml.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:57:09.473236 kirznerSerializer-0.0.3/
+-rw-rw-rw-   0        0        0      806 2023-05-14 20:57:09.473236 kirznerSerializer-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-05-14 20:16:00.000000 kirznerSerializer-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 20:57:09.457612 kirznerSerializer-0.0.3/kirznerSerializer/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:58:02.000000 kirznerSerializer-0.0.3/kirznerSerializer/__init__.py
+-rw-rw-rw-   0        0        0     5802 2023-05-14 20:04:46.000000 kirznerSerializer-0.0.3/kirznerSerializer/base_serializer.py
+-rw-rw-rw-   0        0        0     3939 2023-05-14 19:51:30.000000 kirznerSerializer-0.0.3/kirznerSerializer/constants.py
+-rw-rw-rw-   0        0        0    10663 2023-05-14 20:55:06.000000 kirznerSerializer-0.0.3/kirznerSerializer/json_serializer.py
+-rw-rw-rw-   0        0        0     7825 2023-05-14 20:51:08.000000 kirznerSerializer-0.0.3/kirznerSerializer/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:57:09.473236 kirznerSerializer-0.0.3/kirznerSerializer.egg-info/
+-rw-rw-rw-   0        0        0      806 2023-05-14 20:57:09.000000 kirznerSerializer-0.0.3/kirznerSerializer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-05-14 20:57:09.000000 kirznerSerializer-0.0.3/kirznerSerializer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 20:57:09.000000 kirznerSerializer-0.0.3/kirznerSerializer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-14 20:57:09.000000 kirznerSerializer-0.0.3/kirznerSerializer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-05-14 20:25:16.000000 kirznerSerializer-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      473 2023-05-14 20:57:09.473236 kirznerSerializer-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 20:57:09.473236 kirznerSerializer-0.0.3/tests/
+-rw-rw-rw-   0        0        0     5850 2023-05-14 14:50:03.000000 kirznerSerializer-0.0.3/tests/test_constants.py
+-rw-rw-rw-   0        0        0    13015 2023-05-14 20:04:46.000000 kirznerSerializer-0.0.3/tests/test_json.py
+-rw-rw-rw-   0        0        0    12822 2023-05-14 20:04:46.000000 kirznerSerializer-0.0.3/tests/test_xml.py
```

### Comparing `kirznerSerializer-0.0.2/PKG-INFO` & `kirznerSerializer-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirznerSerializer
-Version: 0.0.2
+Version: 0.0.3
 Summary: This project is my laboratory work
 Author: Kirzner Nastya
 Author-email: kirznernasta@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `kirznerSerializer-0.0.2/kirznerSerializer/base_serializer.py` & `kirznerSerializer-0.0.3/kirznerSerializer/base_serializer.py`

 * *Files identical despite different names*

### Comparing `kirznerSerializer-0.0.2/kirznerSerializer/constants.py` & `kirznerSerializer-0.0.3/kirznerSerializer/constants.py`

 * *Files identical despite different names*

### Comparing `kirznerSerializer-0.0.2/kirznerSerializer/json_serializer.py` & `kirznerSerializer-0.0.3/kirznerSerializer/json_serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 import re
 
-from base_serializer import BaseSerializer
+from kirznerSerializer.base_serializer import BaseSerializer
 from kirznerSerializer.constants import (CLASS_OR_STATIC_METHOD_TYPE,
                                          InvalidJsonException,
                                          UnknownTypeException,
                                          CLOSE_SQUARE_BRACKET,
                                          OPEN_SQUARE_BRACKET,
                                          FUNCTION_TYPE_NAME,
                                          STATIC_METHOD_TYPE,
```

### Comparing `kirznerSerializer-0.0.2/kirznerSerializer/xml_serializer.py` & `kirznerSerializer-0.0.3/kirznerSerializer/xml_serializer.py`

 * *Files identical despite different names*

### Comparing `kirznerSerializer-0.0.2/kirznerSerializer.egg-info/PKG-INFO` & `kirznerSerializer-0.0.3/kirznerSerializer.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirznerSerializer
-Version: 0.0.2
+Version: 0.0.3
 Summary: This project is my laboratory work
 Author: Kirzner Nastya
 Author-email: kirznernasta@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `kirznerSerializer-0.0.2/tests/test_constants.py` & `kirznerSerializer-0.0.3/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `kirznerSerializer-0.0.2/tests/test_json.py` & `kirznerSerializer-0.0.3/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `kirznerSerializer-0.0.2/tests/test_xml.py` & `kirznerSerializer-0.0.3/tests/test_xml.py`

 * *Files identical despite different names*

