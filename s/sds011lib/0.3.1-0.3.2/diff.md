# Comparing `tmp/sds011lib-0.3.1.tar.gz` & `tmp/sds011lib-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sds011lib-0.3.1.tar", max compression
+gzip compressed data, was "sds011lib-0.3.2.tar", max compression
```

## Comparing `sds011lib-0.3.1.tar` & `sds011lib-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-13 22:54:59.328288 sds011lib-0.3.1/LICENSE
--rw-r--r--   0        0        0     1163 2023-05-13 22:54:59.328288 sds011lib-0.3.1/README.md
--rw-r--r--   0        0        0      977 2023-05-13 22:54:59.328288 sds011lib-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    26710 2023-05-13 22:54:59.328288 sds011lib-0.3.1/sds011lib/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-13 22:54:59.328288 sds011lib-0.3.1/sds011lib/_constants.py
--rw-r--r--   0        0        0     2332 2023-05-13 22:54:59.328288 sds011lib-0.3.1/sds011lib/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-13 22:54:59.328288 sds011lib-0.3.1/sds011lib/py.typed
--rw-r--r--   0        0        0     1974 2023-05-13 22:54:59.328288 sds011lib-0.3.1/sds011lib/responses.py
--rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 sds011lib-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-14 18:45:11.075500 sds011lib-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1163 2023-05-14 18:45:11.075500 sds011lib-0.3.2/README.md
+-rw-r--r--   0        0        0      977 2023-05-14 18:45:11.075500 sds011lib-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    26710 2023-05-14 18:45:11.075500 sds011lib-0.3.2/sds011lib/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-14 18:45:11.075500 sds011lib-0.3.2/sds011lib/_constants.py
+-rw-r--r--   0        0        0     2332 2023-05-14 18:45:11.075500 sds011lib-0.3.2/sds011lib/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-14 18:45:11.075500 sds011lib-0.3.2/sds011lib/py.typed
+-rw-r--r--   0        0        0     1974 2023-05-14 18:45:11.075500 sds011lib-0.3.2/sds011lib/responses.py
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 sds011lib-0.3.2/PKG-INFO
```

### Comparing `sds011lib-0.3.1/LICENSE` & `sds011lib-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.1/README.md` & `sds011lib-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.1/pyproject.toml` & `sds011lib-0.3.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sds011lib"
-version = "0.3.1"
+version = "0.3.2"
 description = "SDS011 Library"
 authors = ["Tim Orme <TimothyOrme@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyserial = "^3.5"
```

### Comparing `sds011lib-0.3.1/sds011lib/__init__.py` & `sds011lib-0.3.2/sds011lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         Args:
             device_id: The new device ID to set.
             target_device_id: The target device ID to set the new device ID on.
 
         """
         if len(device_id) != 2 or len(target_device_id) != 2:
             raise AttributeError(
-                f"Device ID must be 4 bytes, found {len(device_id)}, and {len(target_device_id)}"
+                f"Device ID must be 2 bytes, found {len(device_id)}, and {len(target_device_id)}"
             )
         cmd = (
             Command.SET_DEVICE_ID.value + (b"\x00" * 10) + device_id + target_device_id
         )
         self._send_command(cmd)
 
     def query_device_id(self) -> DeviceIdResponse:
@@ -431,16 +431,16 @@
 
     def _parse_query_response(self, data: bytes) -> QueryResponse:
         """Parse a query read response."""
         raw_response = self._parse_read_response(
             data, Command.QUERY, ResponseType.QUERY_RESPONSE
         )
 
-        pm25: float = int.from_bytes(raw_response.payload[2:4], byteorder="little") / 10
-        pm10: float = int.from_bytes(raw_response.payload[4:6], byteorder="little") / 10
+        pm25: float = int.from_bytes(raw_response.payload[0:2], byteorder="little") / 10
+        pm10: float = int.from_bytes(raw_response.payload[2:4], byteorder="little") / 10
         return QueryResponse(pm25=pm25, pm10=pm10, device_id=raw_response.device_id)
 
     def _parse_reporting_mode_response(self, data: bytes) -> ReportingModeResponse:
         """Parse a reporting mode response."""
         raw_response = self._parse_read_response(
             data, command_code=Command.SET_REPORTING_MODE
         )
```

### Comparing `sds011lib-0.3.1/sds011lib/_constants.py` & `sds011lib-0.3.2/sds011lib/_constants.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.1/sds011lib/exceptions.py` & `sds011lib-0.3.2/sds011lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.1/sds011lib/responses.py` & `sds011lib-0.3.2/sds011lib/responses.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.3.1/PKG-INFO` & `sds011lib-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sds011lib
-Version: 0.3.1
+Version: 0.3.2
 Summary: SDS011 Library
 Author: Tim Orme
 Author-email: TimothyOrme@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

