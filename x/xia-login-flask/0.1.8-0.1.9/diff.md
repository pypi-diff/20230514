# Comparing `tmp/xia_login_flask-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_login_flask-0.1.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 197018 bytes, number of entries: 7
--rw-r--r--  2.0 unx      109 b- defN 23-Apr-02 08:05 xia_login_flask/__init__.py
--rw-r--r--  2.0 unx   520704 b- defN 23-Apr-02 08:08 xia_login_flask/account.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-02 08:08 xia_login_flask-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      739 b- defN 23-Apr-02 08:08 xia_login_flask-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-02 08:08 xia_login_flask-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-02 08:08 xia_login_flask-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      612 b- defN 23-Apr-02 08:08 xia_login_flask-0.1.8.dist-info/RECORD
-7 files, 522431 bytes uncompressed, 195920 bytes compressed:  62.5%
+Zip file size: 198021 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      109 b- defN 23-Apr-02 16:41 xia_login_flask/__init__.py
+-rw-r--r--  2.0 unx   528896 b- defN 23-Apr-02 16:45 xia_login_flask/account.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-02 16:45 xia_login_flask-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      739 b- defN 23-Apr-02 16:45 xia_login_flask-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-02 16:45 xia_login_flask-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-02 16:45 xia_login_flask-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      612 b- defN 23-Apr-02 16:45 xia_login_flask-0.1.9.dist-info/RECORD
+7 files, 530623 bytes uncompressed, 196923 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_login_flask/__init__.py
 Comment: 
 
 Filename: xia_login_flask/account.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_login_flask-0.1.8.dist-info/LICENSE.txt
+Filename: xia_login_flask-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_login_flask-0.1.8.dist-info/METADATA
+Filename: xia_login_flask-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_login_flask-0.1.8.dist-info/WHEEL
+Filename: xia_login_flask-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_login_flask-0.1.8.dist-info/top_level.txt
+Filename: xia_login_flask-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_login_flask-0.1.8.dist-info/RECORD
+Filename: xia_login_flask-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_login_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_login_flask.account import XiaLoginFlask
 
 __all__ = [
     "XiaLoginFlask",
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## Comparing `xia_login_flask-0.1.8.dist-info/METADATA` & `xia_login_flask-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-login-flask
-Version: 0.1.8
+Version: 0.1.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-login-flask/0.1.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-login-flask/0.1.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_login_flask-0.1.8.dist-info/RECORD` & `xia_login_flask-0.1.9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_login_flask/__init__.py,sha256=lq32hykFuy_JHeRW21OsdVIqXr39Tzx10YwSnYhEv8I,109
-xia_login_flask/account.cp39-win_amd64.pyd,sha256=BEVzWXdVCzVDsymQsNOoEwuVJ_aGiMtUP0cpIxp1WZ0,520704
-xia_login_flask-0.1.8.dist-info/LICENSE.txt,sha256=hxPR04Gu87DDUI5drgmeS7DmKKrZ3oegg3N-QQeTg8k,152
-xia_login_flask-0.1.8.dist-info/METADATA,sha256=IdcjVakTpKaPcpwePFgGb2izcFEJzBMi8Pn5ILPdFNM,739
-xia_login_flask-0.1.8.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_login_flask-0.1.8.dist-info/top_level.txt,sha256=WWeuEwln8f9FQAukiPEoo4waPy0-AIN8YAu-kkstnos,16
-xia_login_flask-0.1.8.dist-info/RECORD,,
+xia_login_flask/__init__.py,sha256=7h3AHr4EJzmbb2xhjj8VqCU1-q3HPyeJ74uON77ZCR4,109
+xia_login_flask/account.cp39-win_amd64.pyd,sha256=XnLABJ_10bH3b2T3vwHmOg86Qdsz4wNrV0z_d2jS7l0,528896
+xia_login_flask-0.1.9.dist-info/LICENSE.txt,sha256=hxPR04Gu87DDUI5drgmeS7DmKKrZ3oegg3N-QQeTg8k,152
+xia_login_flask-0.1.9.dist-info/METADATA,sha256=zy96PkGRuIfomARFFNYwlnCyAEq8Gm3RKw-hDB2tRMQ,739
+xia_login_flask-0.1.9.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_login_flask-0.1.9.dist-info/top_level.txt,sha256=WWeuEwln8f9FQAukiPEoo4waPy0-AIN8YAu-kkstnos,16
+xia_login_flask-0.1.9.dist-info/RECORD,,
```

