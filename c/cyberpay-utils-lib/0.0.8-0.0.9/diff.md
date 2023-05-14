# Comparing `tmp/cyberpay-utils-lib-0.0.8.tar.gz` & `tmp/cyberpay-utils-lib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberpay-utils-lib-0.0.8.tar", last modified: Thu Feb 16 17:02:22 2023, max compression
+gzip compressed data, was "cyberpay-utils-lib-0.0.9.tar", last modified: Tue Feb 21 09:03:08 2023, max compression
```

## Comparing `cyberpay-utils-lib-0.0.8.tar` & `cyberpay-utils-lib-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 17:02:22.484552 cyberpay-utils-lib-0.0.8/
--rw-rw-rw-   0        0        0      132 2023-02-16 17:02:22.477554 cyberpay-utils-lib-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-16 17:02:22.419553 cyberpay-utils-lib-0.0.8/cyberpay_utils/
--rw-rw-rw-   0        0        0       48 2023-02-14 10:31:32.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-16 17:02:22.420554 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/
--rw-rw-rw-   0        0        0       62 2023-02-14 10:31:29.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-16 17:02:22.421554 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/client/
--rw-rw-rw-   0        0        0        0 2023-02-14 10:23:14.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-16 17:02:22.433553 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/
--rw-rw-rw-   0        0        0      160 2023-02-16 15:44:32.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/__init__.py
--rw-rw-rw-   0        0        0      547 2023-02-16 16:59:14.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/billing.proto
--rw-rw-rw-   0        0        0     2035 2023-02-16 17:02:11.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/billing_pb2.py
--rw-rw-rw-   0        0        0     1230 2023-02-16 17:02:11.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/billing_pb2.pyi
--rw-rw-rw-   0        0        0     4598 2023-02-16 17:02:11.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/billing_pb2_grpc.py
--rw-rw-rw-   0        0        0      196 2023-02-16 13:08:25.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/receipt.proto
--rw-rw-rw-   0        0        0     1199 2023-02-16 17:02:11.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/receipt_pb2.py
--rw-rw-rw-   0        0        0      845 2023-02-16 17:02:11.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/receipt_pb2.pyi
--rw-rw-rw-   0        0        0      159 2023-02-16 17:02:11.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/receipt_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-02-16 17:02:22.475553 cyberpay-utils-lib-0.0.8/cyberpay_utils_lib.egg-info/
--rw-rw-rw-   0        0        0      132 2023-02-16 17:02:22.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1270 2023-02-16 17:02:22.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 17:02:22.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-16 13:16:39.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils_lib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-02-16 17:02:22.000000 cyberpay-utils-lib-0.0.8/cyberpay_utils_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      222 2023-02-14 11:34:58.000000 cyberpay-utils-lib-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-16 17:02:22.484552 cyberpay-utils-lib-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      381 2023-02-16 17:00:48.000000 cyberpay-utils-lib-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-21 09:03:08.770794 cyberpay-utils-lib-0.0.9/
+-rw-rw-rw-   0        0        0      132 2023-02-21 09:03:08.770794 cyberpay-utils-lib-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-02-21 09:03:08.709797 cyberpay-utils-lib-0.0.9/cyberpay_utils/
+-rw-rw-rw-   0        0        0       48 2023-02-14 10:31:32.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-21 09:03:08.710794 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/
+-rw-rw-rw-   0        0        0       62 2023-02-14 10:31:29.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-21 09:03:08.711794 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/client/
+-rw-rw-rw-   0        0        0        0 2023-02-14 10:23:14.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-21 09:03:08.725794 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/
+-rw-rw-rw-   0        0        0      160 2023-02-16 15:44:32.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/__init__.py
+-rw-rw-rw-   0        0        0     1023 2023-02-21 09:00:12.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/billing.proto
+-rw-rw-rw-   0        0        0     3062 2023-02-21 09:02:23.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/billing_pb2.py
+-rw-rw-rw-   0        0        0     2304 2023-02-21 09:02:23.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/billing_pb2.pyi
+-rw-rw-rw-   0        0        0     8382 2023-02-21 09:02:23.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/billing_pb2_grpc.py
+-rw-rw-rw-   0        0        0      196 2023-02-16 13:08:25.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/receipt.proto
+-rw-rw-rw-   0        0        0     1199 2023-02-21 09:02:23.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/receipt_pb2.py
+-rw-rw-rw-   0        0        0      845 2023-02-21 09:02:23.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/receipt_pb2.pyi
+-rw-rw-rw-   0        0        0      159 2023-02-21 09:02:23.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/receipt_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-02-21 09:03:08.768792 cyberpay-utils-lib-0.0.9/cyberpay_utils_lib.egg-info/
+-rw-rw-rw-   0        0        0      132 2023-02-21 09:03:08.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1270 2023-02-21 09:03:08.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-21 09:03:08.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-16 13:16:39.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils_lib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-02-21 09:03:08.000000 cyberpay-utils-lib-0.0.9/cyberpay_utils_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      222 2023-02-14 11:34:58.000000 cyberpay-utils-lib-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-02-21 09:03:08.771794 cyberpay-utils-lib-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      381 2023-02-21 09:02:59.000000 cyberpay-utils-lib-0.0.9/setup.py
```

### Comparing `cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/billing_pb2.py` & `cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/billing_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,23 +11,31 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from cyberpay_utils.billing.proto import receipt_pb2 as cyberpay__utils_dot_billing_dot_proto_dot_receipt__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*cyberpay_utils/billing/proto/billing.proto\x12\rbilling.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a*cyberpay_utils/billing/proto/receipt.proto\"*\n\x14\x43reateReceiptRequest\x12\x12\n\ncompany_id\x18\x01 \x01(\x04\"@\n\x15\x43reateReceiptResponse\x12\'\n\x07receipt\x18\x01 \x01(\x0b\x32\x16.billing.proto.Receipt\"B\n\x16GetAllReceiptsResponse\x12(\n\x08receipts\x18\x01 \x03(\x0b\x32\x16.billing.proto.Receipt2\xba\x01\n\x07\x42illing\x12\\\n\rCreateReceipt\x12#.billing.proto.CreateReceiptRequest\x1a$.billing.proto.CreateReceiptResponse\"\x00\x12Q\n\x0eGetAllReceipts\x12\x16.google.protobuf.Empty\x1a%.billing.proto.GetAllReceiptsResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*cyberpay_utils/billing/proto/billing.proto\x12\rbilling.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a*cyberpay_utils/billing/proto/receipt.proto\"*\n\x14\x43reateReceiptRequest\x12\x12\n\ncompany_id\x18\x01 \x01(\x04\".\n\x18GetCurrentReceiptRequest\x12\x12\n\ncompany_id\x18\x01 \x01(\x04\"2\n\x1cIncreaseActiveWorkersRequest\x12\x12\n\ncompany_id\x18\x01 \x01(\x04\"@\n\x15\x43reateReceiptResponse\x12\'\n\x07receipt\x18\x01 \x01(\x0b\x32\x16.billing.proto.Receipt\"B\n\x16GetAllReceiptsResponse\x12(\n\x08receipts\x18\x01 \x03(\x0b\x32\x16.billing.proto.Receipt\"E\n\x19GetCurrentReceiptResponse\x12(\n\x08receipts\x18\x01 \x03(\x0b\x32\x16.billing.proto.Receipt\"I\n\x1dIncreaseActiveWorkersResponse\x12(\n\x08receipts\x18\x01 \x03(\x0b\x32\x16.billing.proto.Receipt2\x9a\x03\n\x07\x42illing\x12\\\n\rCreateReceipt\x12#.billing.proto.CreateReceiptRequest\x1a$.billing.proto.CreateReceiptResponse\"\x00\x12Q\n\x0eGetAllReceipts\x12\x16.google.protobuf.Empty\x1a%.billing.proto.GetAllReceiptsResponse\"\x00\x12h\n\x11GetCurrentReceipt\x12\'.billing.proto.GetCurrentReceiptRequest\x1a(.billing.proto.GetCurrentReceiptResponse\"\x00\x12t\n\x15IncreaseActiveWorkers\x12+.billing.proto.IncreaseActiveWorkersRequest\x1a,.billing.proto.IncreaseActiveWorkersResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'cyberpay_utils.billing.proto.billing_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _CREATERECEIPTREQUEST._serialized_start=134
   _CREATERECEIPTREQUEST._serialized_end=176
-  _CREATERECEIPTRESPONSE._serialized_start=178
-  _CREATERECEIPTRESPONSE._serialized_end=242
-  _GETALLRECEIPTSRESPONSE._serialized_start=244
-  _GETALLRECEIPTSRESPONSE._serialized_end=310
-  _BILLING._serialized_start=313
-  _BILLING._serialized_end=499
+  _GETCURRENTRECEIPTREQUEST._serialized_start=178
+  _GETCURRENTRECEIPTREQUEST._serialized_end=224
+  _INCREASEACTIVEWORKERSREQUEST._serialized_start=226
+  _INCREASEACTIVEWORKERSREQUEST._serialized_end=276
+  _CREATERECEIPTRESPONSE._serialized_start=278
+  _CREATERECEIPTRESPONSE._serialized_end=342
+  _GETALLRECEIPTSRESPONSE._serialized_start=344
+  _GETALLRECEIPTSRESPONSE._serialized_end=410
+  _GETCURRENTRECEIPTRESPONSE._serialized_start=412
+  _GETCURRENTRECEIPTRESPONSE._serialized_end=481
+  _INCREASEACTIVEWORKERSRESPONSE._serialized_start=483
+  _INCREASEACTIVEWORKERSRESPONSE._serialized_end=556
+  _BILLING._serialized_start=559
+  _BILLING._serialized_end=969
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/receipt_pb2.py` & `cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/receipt_pb2.py`

 * *Files identical despite different names*

### Comparing `cyberpay-utils-lib-0.0.8/cyberpay_utils/billing/proto/receipt_pb2.pyi` & `cyberpay-utils-lib-0.0.9/cyberpay_utils/billing/proto/receipt_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cyberpay-utils-lib-0.0.8/cyberpay_utils_lib.egg-info/SOURCES.txt` & `cyberpay-utils-lib-0.0.9/cyberpay_utils_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

