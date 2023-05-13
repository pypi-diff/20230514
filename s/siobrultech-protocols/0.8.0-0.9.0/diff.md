# Comparing `tmp/siobrultech-protocols-0.8.0.tar.gz` & `tmp/siobrultech-protocols-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siobrultech-protocols-0.8.0.tar", last modified: Fri Apr  7 00:15:53 2023, max compression
+gzip compressed data, was "siobrultech-protocols-0.9.0.tar", last modified: Sat Apr  8 04:51:58 2023, max compression
```

## Comparing `siobrultech-protocols-0.8.0.tar` & `siobrultech-protocols-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:15:52.999210 siobrultech-protocols-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-04-07 00:15:52.999210 siobrultech-protocols-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-07 00:15:52.999210 siobrultech-protocols-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:15:52.999210 siobrultech-protocols-0.8.0/siobrultech_protocols/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/siobrultech_protocols/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:15:52.999210 siobrultech-protocols-0.8.0/siobrultech_protocols/gem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/siobrultech_protocols/gem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/siobrultech_protocols/gem/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/siobrultech_protocols/gem/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/siobrultech_protocols/gem/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    13443 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/siobrultech_protocols/gem/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/siobrultech_protocols/gem/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/siobrultech_protocols/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:15:52.999210 siobrultech-protocols-0.8.0/siobrultech_protocols.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-04-07 00:15:52.000000 siobrultech-protocols-0.8.0/siobrultech_protocols.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-07 00:15:52.000000 siobrultech-protocols-0.8.0/siobrultech_protocols.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 00:15:52.000000 siobrultech-protocols-0.8.0/siobrultech_protocols.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-07 00:15:52.000000 siobrultech-protocols-0.8.0/siobrultech_protocols.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:15:52.999210 siobrultech-protocols-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-07 00:15:47.000000 siobrultech-protocols-0.8.0/tests/test_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:51:58.101816 siobrultech-protocols-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-04-08 04:51:58.101816 siobrultech-protocols-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-08 04:51:58.101816 siobrultech-protocols-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:51:58.097816 siobrultech-protocols-0.9.0/siobrultech_protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/siobrultech_protocols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:51:58.101816 siobrultech-protocols-0.9.0/siobrultech_protocols/gem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/siobrultech_protocols/gem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/siobrultech_protocols/gem/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/siobrultech_protocols/gem/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/siobrultech_protocols/gem/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/siobrultech_protocols/gem/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/siobrultech_protocols/gem/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/siobrultech_protocols/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:51:58.101816 siobrultech-protocols-0.9.0/siobrultech_protocols.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-04-08 04:51:58.000000 siobrultech-protocols-0.9.0/siobrultech_protocols.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-08 04:51:58.000000 siobrultech-protocols-0.9.0/siobrultech_protocols.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 04:51:58.000000 siobrultech-protocols-0.9.0/siobrultech_protocols.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-08 04:51:58.000000 siobrultech-protocols-0.9.0/siobrultech_protocols.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:51:58.101816 siobrultech-protocols-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-08 04:51:53.000000 siobrultech-protocols-0.9.0/tests/test_requirements.py
```

### Comparing `siobrultech-protocols-0.8.0/LICENSE` & `siobrultech-protocols-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siobrultech-protocols-0.8.0/PKG-INFO` & `siobrultech-protocols-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siobrultech-protocols
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Sans-I/O Python client library for Brultech Devices
 Author: Shawn Wilsher
 Author-email: me@shawnwilsher.com
 Project-URL: Bug Reports, https://github.com/sdwilsh/siobrultech-protocols/issues
 Project-URL: Release Notes, https://github.com/sdwilsh/siobrultech-protocols/releases/
 Project-URL: Source, https://github.com/sdwilsh/siobrultech-protocols
 Classifier: Development Status :: 4 - Beta
```

### Comparing `siobrultech-protocols-0.8.0/README.md` & `siobrultech-protocols-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `siobrultech-protocols-0.8.0/pyproject.toml` & `siobrultech-protocols-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `siobrultech-protocols-0.8.0/setup.cfg` & `siobrultech-protocols-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = siobrultech-protocols
-version = 0.8.0
+version = 0.9.0
 author = Shawn Wilsher
 author_email = me@shawnwilsher.com
 description = A Sans-I/O Python client library for Brultech Devices
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_file = LICENSE
 classifiers =
```

### Comparing `siobrultech-protocols-0.8.0/siobrultech_protocols/gem/api.py` & `siobrultech-protocols-0.9.0/siobrultech_protocols/gem/api.py`

 * *Files identical despite different names*

### Comparing `siobrultech-protocols-0.8.0/siobrultech_protocols/gem/const.py` & `siobrultech-protocols-0.9.0/siobrultech_protocols/gem/const.py`

 * *Files identical despite different names*

### Comparing `siobrultech-protocols-0.8.0/siobrultech_protocols/gem/fields.py` & `siobrultech-protocols-0.9.0/siobrultech_protocols/gem/fields.py`

 * *Files identical despite different names*

### Comparing `siobrultech-protocols-0.8.0/siobrultech_protocols/gem/packets.py` & `siobrultech-protocols-0.9.0/siobrultech_protocols/gem/packets.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         self.seconds: int = seconds
         self.pulse_counts: List[int] = pulse_counts or []
         self.temperatures: List[float] = temperatures or []
         if time_stamp:
             self.time_stamp: datetime = time_stamp
         else:
             self.time_stamp: datetime = datetime.now()
-        self.aux = aux
+        self.aux: List[int] = aux or []
         self.dc_voltage = dc_voltage
 
     def __str__(self) -> str:
         return json.dumps(
             {
                 "device_id": self.device_id,
                 "serial_number": self.serial_number,
@@ -96,14 +96,19 @@
         return self._delta_value(field, self.seconds, prev)
 
     def delta_pulse_count(self, index: int, prev: int) -> int:
         field = self.packet_format.fields["pulse_counts"]
         assert isinstance(field, NumericArrayField)
         return self._delta_value(field.elem_field, self.pulse_counts[index], prev)
 
+    def delta_aux_count(self, index: int, prev: int) -> int:
+        field = self.packet_format.fields["aux"]
+        assert isinstance(field, NumericArrayField)
+        return self._delta_value(field.elem_field, self.aux[index], prev)
+
     def delta_absolute_watt_seconds(self, index: int, prev: int) -> int:
         field = self.packet_format.fields["absolute_watt_seconds"]
         assert isinstance(field, NumericArrayField)
         return self._delta_value(
             field.elem_field, self.absolute_watt_seconds[index], prev
         )
 
@@ -170,24 +175,46 @@
         )
 
         delta_consumed_watt_seconds = (
             delta_absolute_watt_seconds - delta_produced_watt_seconds
         )
 
         return (
-            delta_consumed_watt_seconds - delta_produced_watt_seconds
-        ) / elapsed_seconds
+            (delta_consumed_watt_seconds - delta_produced_watt_seconds)
+            / elapsed_seconds
+            if elapsed_seconds
+            else 0
+        )
 
     def get_average_pulse_rate(self, index: int, other_packet: Packet) -> float:
         oldest_packet, newest_packet = self._packets_sorted(self, other_packet)
         elapsed_seconds = newest_packet.delta_seconds(oldest_packet.seconds)
 
         return (
-            newest_packet.delta_pulse_count(index, oldest_packet.pulse_counts[index])
-            / elapsed_seconds
+            (
+                newest_packet.delta_pulse_count(
+                    index, oldest_packet.pulse_counts[index]
+                )
+                / elapsed_seconds
+            )
+            if elapsed_seconds
+            else 0
+        )
+
+    def get_average_aux_rate_of_change(self, index: int, other_packet: Packet) -> float:
+        oldest_packet, newest_packet = self._packets_sorted(self, other_packet)
+        elapsed_seconds = newest_packet.delta_seconds(oldest_packet.seconds)
+
+        return (
+            (
+                newest_packet.delta_aux_count(index, oldest_packet.aux[index])
+                / elapsed_seconds
+            )
+            if elapsed_seconds
+            else 0
         )
 
 
 @unique
 class PacketFormatType(IntEnum):
     ECM_1220 = 1
     ECM_1240 = 3
```

### Comparing `siobrultech-protocols-0.8.0/siobrultech_protocols/gem/protocol.py` & `siobrultech-protocols-0.9.0/siobrultech_protocols/gem/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,15 @@
         """
         Ends an API request. Every begin_api_request call must have a matching end_api_request call,
         even if an error occurred in between.
         """
         self._expect_state(
             {
                 ProtocolState.RECEIVED_API_RESPONSE,
+                ProtocolState.SENT_API_REQUEST,
                 ProtocolState.SENT_PACKET_DELAY_REQUEST,
             }
         )
         self._api_buffer.clear()
         LOG.debug("%d: Ended API request", id(self))
         self._state = ProtocolState.RECEIVING_PACKETS
```

### Comparing `siobrultech-protocols-0.8.0/siobrultech_protocols.egg-info/PKG-INFO` & `siobrultech-protocols-0.9.0/siobrultech_protocols.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siobrultech-protocols
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Sans-I/O Python client library for Brultech Devices
 Author: Shawn Wilsher
 Author-email: me@shawnwilsher.com
 Project-URL: Bug Reports, https://github.com/sdwilsh/siobrultech-protocols/issues
 Project-URL: Release Notes, https://github.com/sdwilsh/siobrultech-protocols/releases/
 Project-URL: Source, https://github.com/sdwilsh/siobrultech-protocols
 Classifier: Development Status :: 4 - Beta
```

### Comparing `siobrultech-protocols-0.8.0/siobrultech_protocols.egg-info/SOURCES.txt` & `siobrultech-protocols-0.9.0/siobrultech_protocols.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siobrultech-protocols-0.8.0/tests/test_requirements.py` & `siobrultech-protocols-0.9.0/tests/test_requirements.py`

 * *Files identical despite different names*

