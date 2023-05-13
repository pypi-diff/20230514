# Comparing `tmp/databend_py-0.4.0-py3-none-any.whl.zip` & `tmp/databend_py-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 16651 bytes, number of entries: 17
--rw-r--r--  2.0 unx      227 b- defN 23-May-10 01:50 databend_py/__init__.py
--rw-r--r--  2.0 unx    10825 b- defN 23-May-08 09:31 databend_py/client.py
--rw-r--r--  2.0 unx     6321 b- defN 23-May-08 09:31 databend_py/connection.py
+Zip file size: 17442 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      227 b- defN 23-May-13 08:52 databend_py/__init__.py
+-rw-r--r--  2.0 unx    10797 b- defN 23-May-13 23:39 databend_py/client.py
+-rw-r--r--  2.0 unx     6927 b- defN 23-May-13 23:39 databend_py/connection.py
 -rw-r--r--  2.0 unx      909 b- defN 22-Nov-07 03:45 databend_py/context.py
 -rw-r--r--  2.0 unx      931 b- defN 23-Jan-12 08:08 databend_py/datetypes.py
 -rw-r--r--  2.0 unx      184 b- defN 22-Nov-16 02:52 databend_py/defines.py
--rw-r--r--  2.0 unx      581 b- defN 22-Nov-07 03:45 databend_py/errors.py
+-rw-r--r--  2.0 unx      884 b- defN 23-May-13 23:39 databend_py/errors.py
 -rw-r--r--  2.0 unx      206 b- defN 22-Nov-07 03:45 databend_py/log.py
 -rw-r--r--  2.0 unx     2128 b- defN 23-Feb-13 02:21 databend_py/result.py
+-rw-r--r--  2.0 unx     1133 b- defN 23-May-13 23:39 databend_py/retry.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Nov-07 03:45 databend_py/util/__init__.py
 -rw-r--r--  2.0 unx     1452 b- defN 22-Nov-07 03:45 databend_py/util/escape.py
 -rw-r--r--  2.0 unx     2254 b- defN 22-Nov-12 09:37 databend_py/util/helper.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-10 01:50 databend_py-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3537 b- defN 23-May-10 01:50 databend_py-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-10 01:50 databend_py-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-10 01:50 databend_py-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1360 b- defN 23-May-10 01:50 databend_py-0.4.0.dist-info/RECORD
-17 files, 42376 bytes uncompressed, 14425 bytes compressed:  66.0%
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-13 23:39 databend_py-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3531 b- defN 23-May-13 23:39 databend_py-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-13 23:39 databend_py-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-13 23:39 databend_py-0.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1437 b- defN 23-May-13 23:39 databend_py-0.4.1.dist-info/RECORD
+18 files, 44461 bytes uncompressed, 15100 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -21,32 +21,35 @@
 
 Filename: databend_py/log.py
 Comment: 
 
 Filename: databend_py/result.py
 Comment: 
 
+Filename: databend_py/retry.py
+Comment: 
+
 Filename: databend_py/util/__init__.py
 Comment: 
 
 Filename: databend_py/util/escape.py
 Comment: 
 
 Filename: databend_py/util/helper.py
 Comment: 
 
-Filename: databend_py-0.4.0.dist-info/LICENSE
+Filename: databend_py-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: databend_py-0.4.0.dist-info/METADATA
+Filename: databend_py-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: databend_py-0.4.0.dist-info/WHEEL
+Filename: databend_py-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: databend_py-0.4.0.dist-info/top_level.txt
+Filename: databend_py-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: databend_py-0.4.0.dist-info/RECORD
+Filename: databend_py-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databend_py/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .client import Client
 from .connection import Connection
 from .datetypes import DatabendDataType
 
-VERSION = (0, 4, 0)
+VERSION = (0, 4, 1)
 __version__ = '.'.join(str(x) for x in VERSION)
 
 __all__ = ['Client', 'Connection', 'DatabendDataType']
```

## databend_py/client.py

```diff
@@ -246,15 +246,14 @@
         resp.raise_for_status()
         return stage_path
 
     def sync_csv_file_into_table(self, filename, data, table):
         start = time.time()
         stage_path = self.stage_csv_file(filename, data)
         copy_options = self.generate_copy_options()
-        print(copy_options)
         _, _ = self.execute(
             f"COPY INTO {table} FROM {stage_path} FILE_FORMAT = (type = CSV)\
              PURGE = {copy_options['PURGE']} FORCE = {copy_options['FORCE']}\
               SIZE_LIMIT={copy_options['SIZE_LIMIT']} ON_ERROR = {copy_options['ON_ERROR']}")
         print("sync %s duration:%ss" % (filename, int(time.time() - start)))
         os.remove(filename)
```

## databend_py/connection.py

```diff
@@ -6,14 +6,16 @@
 
 import environs
 import requests
 from mysql.connector.errors import Error
 from . import log
 from . import defines
 from .context import Context
+from databend_py.errors import WarehouseTimeoutException
+from databend_py.retry import retry
 
 headers = {'Content-Type': 'application/json', 'Accept': 'application/json', 'X-DATABEND-ROUTE': 'warehouse'}
 
 
 class ServerInfo(object):
     def __init__(self, name, version_major, version_minor, version_patch,
                  revision, timezone, display_name):
@@ -84,14 +86,17 @@
         if self.secure:
             self.schema = 'https'
         e = environs.Env()
         if os.getenv("ADDITIONAL_HEADERS") is not None:
             print(os.getenv("ADDITIONAL_HEADERS"))
             self.additional_headers = e.dict("ADDITIONAL_HEADERS")
 
+    def default_session(self):
+        return {"database": self.database}
+
     def make_headers(self):
         if "Authorization" not in self.additional_headers:
             return {
                 **headers, **self.additional_headers,
                 "Authorization":
                     "Basic " + base64.b64encode("{}:{}".format(
                         self.user, self.password).encode(encoding="utf-8")).decode()
@@ -101,36 +106,46 @@
 
     def get_description(self):
         return '{}:{}'.format(self.host, self.port)
 
     def disconnect(self):
         self.client_session = dict()
 
+    @retry(times=5, exceptions=WarehouseTimeoutException)
+    def do_query(self, url, query_sql):
+        response = requests.post(url,
+                                 data=json.dumps(query_sql),
+                                 headers=self.make_headers(),
+                                 auth=HTTPBasicAuth(self.user, self.password),
+                                 verify=True)
+        resp_dict = json.loads(response.content)
+        if resp_dict and resp_dict.get('error') and "no endpoint" in resp_dict.get('error'):
+            raise WarehouseTimeoutException
+
+        return resp_dict
+
     def query(self, statement):
         url = self.format_url()
         log.logger.debug(f"http sql: {statement}")
         query_sql = {'sql': statement, "string_fields": True}
         if self.client_session is not None and len(self.client_session) != 0:
+            if "database" not in self.client_session:
+                self.client_session = self.default_session()
             query_sql['session'] = self.client_session
         else:
-            self.client_session = {"db": self.database}
+            self.client_session = self.default_session()
             query_sql['session'] = self.client_session
         log.logger.debug(f"http headers {self.make_headers()}")
-        response = requests.post(url,
-                                 data=json.dumps(query_sql),
-                                 headers=self.make_headers(),
-                                 auth=HTTPBasicAuth(self.user, self.password),
-                                 verify=True)
         try:
-            resp_dict = json.loads(response.content)
-            self.client_session = resp_dict["session"]
+            resp_dict = self.do_query(url, query_sql)
+            self.client_session = resp_dict.get("session", self.default_session())
             return resp_dict
         except Exception as err:
             log.logger.error(
-                f"http error on {url}, SQL: {statement} content: {response.content} error msg:{str(err)}"
+                f"http error on {url}, SQL: {statement} error msg:{str(err)}"
             )
             raise
 
     def format_url(self):
         if self.schema == "https" and self.port is None:
             self.port = 443
         elif self.schema == "http" and self.port is None:
@@ -142,30 +157,29 @@
 
     def next_page(self, next_uri):
         url = "{}://{}:{}{}".format(self.schema, self.host, self.port, next_uri)
         return requests.get(url=url, headers=self.make_headers())
 
     # return a list of response util empty next_uri
     def query_with_session(self, statement):
-        current_session = self.client_session
         response_list = list()
         response = self.query(statement)
         log.logger.debug(f"response content: {response}")
         response_list.append(response)
         start_time = time.time()
         time_limit = 12
-        session = response['session']
+        session = response.get("session", self.default_session())
         if session:
             self.client_session = session
         while response['next_uri'] is not None:
             resp = self.next_page(response['next_uri'])
             response = json.loads(resp.content)
             log.logger.debug(f"Sql in progress, fetch next_uri content: {response}")
             self.check_error(response)
-            session = response['session']
+            session = response.get("session", self.default_session())
             if session:
                 self.client_session = session
             response_list.append(response)
             if time.time() - start_time > time_limit:
                 log.logger.warning(
                     f"after waited for {time_limit} secs, query still not finished (next uri not none)!"
                 )
```

## databend_py/errors.py

```diff
@@ -14,7 +14,17 @@
     def __init__(self, message, code=None):
         self.message = message
         self.code = code
         super(ServerException, self).__init__(message)
 
     def __str__(self):
         return 'Code: {}\n{}'.format(self.code, self.message)
+
+
+class WarehouseTimeoutException(Error):
+    def __init__(self, message, code=None):
+        self.message = message
+        self.code = code
+        super(WarehouseTimeoutException, self).__init__(message)
+
+    def __str__(self):
+        return 'Provision warehouse timeout: \n{}'.format(self.message)
```

## Comparing `databend_py-0.4.0.dist-info/LICENSE` & `databend_py-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `databend_py-0.4.0.dist-info/METADATA` & `databend_py-0.4.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python driver with native interface for Databend
 Home-page: https://github.com/databendcloud/databend-py
 Author: Databend Cloud Team
 Author-email: hantmac@outlook.com
 License: Apache License
 Keywords: databend db database cloud analytics
 Classifier: Development Status :: 4 - Beta
@@ -57,16 +57,15 @@
 > ``` python
 > >>> from databend_py import Client
 > >>> client = Client(
 >     host='tenant--warehouse.ch.datafusecloud.com',
 >     database="default",
 >     user="user",
 >     port="443",
->     password="password")
->     settings={"copy_purge":True,"force":True}
+>     password="password",settings={"copy_purge":True,"force":True})
 > >>> print(client.execute("SELECT 1"))
 > ```
 
 The [host]{.title-ref}, [user]{.title-ref}, [password]{.title-ref} info
 will be found in databend cloud warehouse connect page as flows:
 
 Pure Client example:
```

## Comparing `databend_py-0.4.0.dist-info/RECORD` & `databend_py-0.4.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-databend_py/__init__.py,sha256=bR_AXJjyGNK71Ai0KSngKhxaRj8SRFSR9C2nXnEfM4M,227
-databend_py/client.py,sha256=xPD1186k53Pz8sJ5B0P5Bjp9SylzEXxXrRVuuXQqIlw,10825
-databend_py/connection.py,sha256=9s_aY-5Ki4o1LhbTlh38ujscDDeLG8ZORyPlBr-kNgg,6321
+databend_py/__init__.py,sha256=_ZDovDFCdkUaFcLPcadXt6q2yvljnXGmNQY_XZ7G4t0,227
+databend_py/client.py,sha256=DlNZcI5jUjV5KOlx5kF9DjQ4NNT_qd40pGw8zxIYYDQ,10797
+databend_py/connection.py,sha256=90u06LUJS8216pWVqX2UcHAT24f7Dx_aOKlh_7fhPF4,6927
 databend_py/context.py,sha256=yPkJ_BN4LGODvKCOjNlDGqABwxAMQTQl7w1vIGRPBDg,909
 databend_py/datetypes.py,sha256=Yl5ZS_C5oPfyOcE2xTQNtxgPZnxnMKIc_lYSmEnFJdg,931
 databend_py/defines.py,sha256=eQOK22KSKfcBukcD4oHsmlgpXFms92ew0ORxWNnxxH0,184
-databend_py/errors.py,sha256=CJE2LDMAUqnrGT1AOd5pfLKCDgiaKKiWU7FMtN-xs88,581
+databend_py/errors.py,sha256=-4WBvTF0OvggCa9pJEWeU02BDX-IVDx6e5hGZWjH2GI,884
 databend_py/log.py,sha256=dMuMaWptI_nexWDZMtZaAnoEOluIfYWNdoR9OSAhgKM,206
 databend_py/result.py,sha256=Ru1FwwMtbbT5E2Iesv9d6fGZeL8pFJ0lG0vA3bLN3m8,2128
+databend_py/retry.py,sha256=c-kNYxqgnD30U23Xy-yHVeBp0wItsatkxql2O1rkWNE,1133
 databend_py/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databend_py/util/escape.py,sha256=DE7PaShERoOw285fkg3pu7T_oMU4_2dMkHbjXEqPcn4,1452
 databend_py/util/helper.py,sha256=0r1d3CeNtMLdTPN_v8yW-GjjpjHVneIJJKKGdTioOoE,2254
-databend_py-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-databend_py-0.4.0.dist-info/METADATA,sha256=e-qkck-eXtdTMBA9_nRcSYisbZRf4ASTH5Gzr8ne8as,3537
-databend_py-0.4.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-databend_py-0.4.0.dist-info/top_level.txt,sha256=t0rUVwHfEpXcuMreSkL69rc5DWv6FmzB4AfEGcc4_7U,12
-databend_py-0.4.0.dist-info/RECORD,,
+databend_py-0.4.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+databend_py-0.4.1.dist-info/METADATA,sha256=BuJD3cgEL7pmLwmN5N_nNdafaktJpJGsw4HHNbuDVws,3531
+databend_py-0.4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+databend_py-0.4.1.dist-info/top_level.txt,sha256=t0rUVwHfEpXcuMreSkL69rc5DWv6FmzB4AfEGcc4_7U,12
+databend_py-0.4.1.dist-info/RECORD,,
```

