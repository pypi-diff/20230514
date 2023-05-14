# Comparing `tmp/xia_sso_flask-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_sso_flask-0.1.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 133709 bytes, number of entries: 7
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-03 17:05 xia_sso_flask/__init__.py
--rw-r--r--  2.0 unx   327680 b- defN 23-Apr-03 17:08 xia_sso_flask/sso.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-03 17:08 xia_sso_flask-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      710 b- defN 23-Apr-03 17:08 xia_sso_flask-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-03 17:08 xia_sso_flask-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-03 17:08 xia_sso_flask-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      593 b- defN 23-Apr-03 17:08 xia_sso_flask-0.1.8.dist-info/RECORD
-7 files, 329347 bytes uncompressed, 132647 bytes compressed:  59.7%
+Zip file size: 133949 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-03 17:41 xia_sso_flask/__init__.py
+-rw-r--r--  2.0 unx   327680 b- defN 23-Apr-03 17:43 xia_sso_flask/sso.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-03 17:43 xia_sso_flask-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      710 b- defN 23-Apr-03 17:43 xia_sso_flask-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-03 17:43 xia_sso_flask-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-03 17:43 xia_sso_flask-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      593 b- defN 23-Apr-03 17:43 xia_sso_flask-0.1.9.dist-info/RECORD
+7 files, 329347 bytes uncompressed, 132887 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_sso_flask/__init__.py
 Comment: 
 
 Filename: xia_sso_flask/sso.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_sso_flask-0.1.8.dist-info/LICENSE.txt
+Filename: xia_sso_flask-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_sso_flask-0.1.8.dist-info/METADATA
+Filename: xia_sso_flask-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_sso_flask-0.1.8.dist-info/WHEEL
+Filename: xia_sso_flask-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_sso_flask-0.1.8.dist-info/top_level.txt
+Filename: xia_sso_flask-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_sso_flask-0.1.8.dist-info/RECORD
+Filename: xia_sso_flask-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_sso_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_sso_flask.sso import XiaSsoFlask
 
 __all__ = [
     "XiaSsoFlask",
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## Comparing `xia_sso_flask-0.1.8.dist-info/METADATA` & `xia_sso_flask-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-sso-flask
-Version: 0.1.8
+Version: 0.1.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-sso-flask/0.1.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-sso-flask/0.1.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

