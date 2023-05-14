# Comparing `tmp/bluerpc-0.0.8.tar.gz` & `tmp/bluerpc-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluerpc-0.0.8.tar", last modified: Mon Feb 20 16:48:40 2023, max compression
+gzip compressed data, was "bluerpc-0.2.6.tar", last modified: Sun May 14 15:49:45 2023, max compression
```

## Comparing `bluerpc-0.0.8.tar` & `bluerpc-0.2.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:48:40.116718 bluerpc-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-20 16:48:40.116718 bluerpc-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 16:47:57.000000 bluerpc-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:48:40.116718 bluerpc-0.0.8/bluerpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 16:47:57.000000 bluerpc-0.0.8/bluerpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17797 2023-02-20 16:47:57.000000 bluerpc-0.0.8/bluerpc/ble_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-02-20 16:47:57.000000 bluerpc-0.0.8/bluerpc/ble_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-02-20 16:47:57.000000 bluerpc-0.0.8/bluerpc/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-02-20 16:47:57.000000 bluerpc-0.0.8/bluerpc/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:48:40.116718 bluerpc-0.0.8/bluerpc/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 16:48:33.000000 bluerpc-0.0.8/bluerpc/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-02-20 16:48:33.000000 bluerpc-0.0.8/bluerpc/rpc/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-20 16:48:33.000000 bluerpc-0.0.8/bluerpc/rpc/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-02-20 16:48:33.000000 bluerpc-0.0.8/bluerpc/rpc/gatt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-20 16:48:33.000000 bluerpc-0.0.8/bluerpc/rpc/gatt_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-02-20 16:48:33.000000 bluerpc-0.0.8/bluerpc/rpc/services_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-02-20 16:48:33.000000 bluerpc-0.0.8/bluerpc/rpc/services_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-02-20 16:47:57.000000 bluerpc-0.0.8/bluerpc/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-02-20 16:47:57.000000 bluerpc-0.0.8/bluerpc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:48:40.116718 bluerpc-0.0.8/bluerpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-20 16:48:40.000000 bluerpc-0.0.8/bluerpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-20 16:48:40.000000 bluerpc-0.0.8/bluerpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 16:48:40.000000 bluerpc-0.0.8/bluerpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-20 16:48:40.000000 bluerpc-0.0.8/bluerpc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-20 16:48:40.000000 bluerpc-0.0.8/bluerpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-20 16:48:40.000000 bluerpc-0.0.8/bluerpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 16:48:40.116718 bluerpc-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-02-20 16:47:57.000000 bluerpc-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:49:45.936654 bluerpc-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-14 15:49:45.936654 bluerpc-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:48:36.000000 bluerpc-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:49:45.932654 bluerpc-0.2.6/bluerpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:48:36.000000 bluerpc-0.2.6/bluerpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19455 2023-05-14 15:48:36.000000 bluerpc-0.2.6/bluerpc/ble_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-14 15:48:36.000000 bluerpc-0.2.6/bluerpc/ble_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-14 15:48:36.000000 bluerpc-0.2.6/bluerpc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-14 15:48:36.000000 bluerpc-0.2.6/bluerpc/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-14 15:48:36.000000 bluerpc-0.2.6/bluerpc/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:49:45.932654 bluerpc-0.2.6/bluerpc/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 15:49:39.000000 bluerpc-0.2.6/bluerpc/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-14 15:49:39.000000 bluerpc-0.2.6/bluerpc/rpc/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-14 15:49:39.000000 bluerpc-0.2.6/bluerpc/rpc/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-14 15:49:39.000000 bluerpc-0.2.6/bluerpc/rpc/gatt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-14 15:49:39.000000 bluerpc-0.2.6/bluerpc/rpc/gatt_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-14 15:49:39.000000 bluerpc-0.2.6/bluerpc/rpc/services_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-05-14 15:49:39.000000 bluerpc-0.2.6/bluerpc/rpc/services_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-14 15:48:36.000000 bluerpc-0.2.6/bluerpc/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-14 15:48:36.000000 bluerpc-0.2.6/bluerpc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:49:45.932654 bluerpc-0.2.6/bluerpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-14 15:49:45.000000 bluerpc-0.2.6/bluerpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-14 15:49:45.000000 bluerpc-0.2.6/bluerpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:49:45.000000 bluerpc-0.2.6/bluerpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-14 15:49:45.000000 bluerpc-0.2.6/bluerpc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-14 15:49:45.000000 bluerpc-0.2.6/bluerpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 15:49:45.000000 bluerpc-0.2.6/bluerpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:49:45.936654 bluerpc-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-14 15:48:36.000000 bluerpc-0.2.6/setup.py
```

### Comparing `bluerpc-0.0.8/PKG-INFO` & `bluerpc-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluerpc
-Version: 0.0.8
+Version: 0.2.6
 Summary: Python BlueRPC Worker
 Home-page: https://github.com/BlueRPC/BlueRPC
 Author: drosocode
 License: MIT
 Project-URL: Documentation, https://bluerpc.github.io/
 Project-URL: Source, https://github.com/BlueRPC/BlueRPC/python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bluerpc-0.0.8/bluerpc/ble_conn.py` & `bluerpc-0.2.6/bluerpc/ble_conn.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import json
 import platform
 from typing import Dict, List, Optional, Union
 
 from bleak import BleakClient, BleakError, BleakGATTCharacteristic
 from bleak.backends.descriptor import BleakGATTDescriptor
 from bleak.exc import BleakDeviceNotFoundError
+from bluerpc.ble_scan import BLEScanner
 from bluerpc.rpc import common_pb2, gatt_pb2
-from bluerpc.utils import get_appdata_dir, validate_mac, validate_uuid
+from bluerpc.utils import get_appdata_dir, get_kwargs, validate_mac, validate_uuid
 
 PAIRED_LIST_FILE = "paired.json"
 
 
 class BLEConn:
     """
     Class used to manipulate connections with Bluetooth Low-Energy devices
@@ -21,14 +22,35 @@
 
     devices: Dict[str, BLEConn] = {}
     paired_devices: List[gatt_pb2.BLEDevice] = []
     loaded_paired_devices = False
     disconnect_queue = asyncio.Queue()
     notif_queue = asyncio.Queue()
     macos = platform.system() == "Darwin"
+    scanner = None
+
+    @classmethod
+    def set_scanner(self, sc: BLEScanner):
+        """
+        Set scanner, used to connect when a scan is also running
+
+        Args:
+            sc: the scanner instance
+        """
+        self.scanner = sc
+
+    @classmethod
+    def set_adapter(self, adapter: str):
+        """
+        Set adapter id
+
+        Args:
+            adapter: the adapter id
+        """
+        self.adapter = adapter
 
     @staticmethod
     def get_device(dev: gatt_pb2.BLEDevice) -> BLEConn:
         """
         Static method to get a BLEConn instance from a device (mac address or uuid)
 
         Args:
@@ -167,30 +189,53 @@
             return gatt_pb2.BLEConnectResponse(
                 status=common_pb2.StatusMessage(
                     code=common_pb2.ERROR_CODE_ALREADY_CONNECTED
                 )
             )
 
         try:
+            # validate and create client (mac or uuid)
+            kwargs = get_kwargs(self._adapter)
             if self._device.mac != "":
                 c = self._check(check_connect=False, mac=self._device.mac)
                 if c is not None:
                     return c
-
                 self._client = BleakClient(
-                    self._device.mac, disconnected_callback=self.disconnect_callback
+                    self._device.mac,
+                    disconnected_callback=self.disconnect_callback,
+                    **kwargs,
                 )
             else:
                 c = self._check(check_connect=False, uuids=[self._device.uuid])
                 if c is not None:
                     return c
-
                 self._client = BleakClient(
-                    self._device.uuid, disconnected_callback=self.disconnect_callback
+                    self._device.uuid,
+                    disconnected_callback=self.disconnect_callback,
+                    **kwargs,
                 )
+
+            restart = False
+            if self.scanner is not None and self.scanner.running:
+                # check if a BLEDevice with this address was recently discovered
+                found = False
+                for i in self.scanner.scanned_devices:
+                    if i.address == self._device.mac or i.address == self._device.uuid:
+                        found = True
+                        self._client = BleakClient(
+                            i, disconnected_callback=self.disconnect_callback, **kwargs
+                        )
+                        break
+
+                if not found:
+                    # if not found, we need to stop the scanner to try to connect to the device
+                    # otherwise there is an "Operation already in progress" error
+                    await self.scanner.stop_scan()
+                    restart = True
+
             await self._client.connect()
 
             if self._client.__class__.__name__ == "BleakClientBlueZDBus":
                 await self._client._acquire_mtu()
 
             return gatt_pb2.BLEConnectResponse(
                 status=common_pb2.StatusMessage(code=common_pb2.ERROR_CODE_OK),
@@ -204,14 +249,17 @@
             )
         except BleakError as e:
             return gatt_pb2.BLEConnectResponse(
                 status=common_pb2.StatusMessage(
                     code=common_pb2.ERROR_CODE_ERROR, message=str(e)
                 )
             )
+        finally:
+            if restart:
+                await self.scanner.restart_scan()
 
     async def disconnect(self) -> common_pb2.StatusMessage:
         if self._client.is_connected:
             for i in self._notifs:
                 await self._client.stop_notify(i)
             await self._client.disconnect()
             self._notifs = []
```

### Comparing `bluerpc-0.0.8/bluerpc/ble_scan.py` & `bluerpc-0.2.6/bluerpc/ble_scan.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import asyncio
+import collections
 import platform
 import time
 from typing import Dict, List
 
 from bleak import AdvertisementData, BleakScanner, BLEDevice
 from bluerpc.rpc import common_pb2, gatt_pb2
-from bluerpc.utils import validate_mac
+from bluerpc.utils import get_kwargs, validate_mac
 
 
 class BLEScanner:
     """
     This class is used to scan for Bluetooth Low-Energy devices and store the results as ready-to-send proto objects
     """
+
     scan_queues: Dict[str, asyncio.Queue] = {}
+    scanned_devices = collections.deque(maxlen=10)
 
-    def __init__(self) -> None:
+    def __init__(self, adapter) -> None:
         self.running = False
         self._scanFilters = {}
+        self._scan_data = None
+        self._adapter = adapter
 
     def check_filters(self, device: BLEDevice) -> bool:
         """
         Check Filters
 
         Args:
             device: bleak device
@@ -55,14 +60,15 @@
 
         Args:
             device: bleak device
             advertisement_data: bleak advertisement data
         """
         if not self.check_filters(device):
             return
+        self.scanned_devices.append(device)
 
         mf_data = []
         adv_data = []
         svc = []
         for k, v in advertisement_data.manufacturer_data.items():
             mf_data.append(gatt_pb2.BLEAdvertisementData(uuid=str(k), value=v))
         for k, v in advertisement_data.service_data.items():
@@ -94,14 +100,15 @@
         """
         Start scanner method
 
         Args:
             active: if the scanner should be in active or passive mode
             filters: list of filters to apply for scanning, services uuid are processed directly by bleak, others are post-processed
         """
+        self._scan_data = (active, filters)
         self.running = True
         self._scanFilters = {}
         svc_filters = []
         for i in filters:
             if i.type == gatt_pb2.BLE_SCAN_FILTER_TYPE_UUID:
                 svc_filters.append(i.value)
             else:
@@ -111,19 +118,29 @@
 
         self._scanner = BleakScanner(
             detection_callback=self.detection_callback,
             scanning_mode=(
                 "passive" if not active or platform.system() == "Darwin" else "active"
             ),
             service_uuids=svc_filters,
+            **get_kwargs(self._adapter)
         )
         await self._scanner.start()
 
     async def stop_scan(self) -> None:
         """
         Stop scanner method
 
         Stops the scanner if not already stopped
         """
         if self.running:
             await self._scanner.stop()
             self.running = False
+
+    async def restart_scan(self) -> None:
+        """
+        Restart the scanner
+
+        Useful to restart the scanner after it was temporarily stopped to connect to a device
+        """
+        if self._scan_data and not self.running:
+            await self.scan(self._scan_data[0], self._scan_data[1])
```

### Comparing `bluerpc-0.0.8/bluerpc/rpc/common_pb2.py` & `bluerpc-0.2.6/bluerpc/rpc/common_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10rpc/common.proto\x12\x03rpc\"-\n\x0cHelloRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"\xca\x01\n\rHelloResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x0e\n\x06uptime\x18\x03 \x01(\x04\x12(\n\x0fsupported_modes\x18\x04 \x03(\x0e\x32\x0f.rpc.WorkerMode\x12$\n\x0bworker_type\x18\x05 \x01(\x0e\x32\x0f.rpc.WorkerType\x12\x18\n\x10operating_system\x18\x06 \x01(\t\x12 \n\x18operating_system_version\x18\x07 \x01(\t\">\n\rStatusMessage\x12\x1c\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0e.rpc.ErrorCode\x12\x0f\n\x07message\x18\x02 \x01(\t\"\x06\n\x04Void*V\n\nWorkerType\x12\x17\n\x13WORKER_TYPE_UNKNOWN\x10\x00\x12\x16\n\x12WORKER_TYPE_PYTHON\x10\x01\x12\x17\n\x13WORKER_TYPE_ANDROID\x10\x02*\\\n\nWorkerMode\x12\x13\n\x0fWORKER_MODE_UNK\x10\x00\x12\x1c\n\x18WORKER_MODE_GATT_PASSIVE\x10\x01\x12\x1b\n\x17WORKER_MODE_GATT_ACTIVE\x10\x02*\xa8\x04\n\tErrorCode\x12\x12\n\x0e\x45RROR_CODE_UNK\x10\x00\x12\x11\n\rERROR_CODE_OK\x10\x01\x12\x14\n\x10\x45RROR_CODE_ERROR\x10\x02\x12\x1a\n\x16\x45RROR_CODE_UNAVAILABLE\x10\x03\x12 \n\x1c\x45RROR_CODE_CONNECTION_FAILED\x10\x04\x12\x1e\n\x1a\x45RROR_CODE_UNKNOWN_SERVICE\x10\x05\x12%\n!ERROR_CODE_UNKNOWN_CHARACTERISTIC\x10\x06\x12!\n\x1d\x45RROR_CODE_UNKNOWN_DESCRIPTOR\x10\x07\x12\x1a\n\x16\x45RROR_CODE_UNSUPPORTED\x10\x08\x12*\n&ERROR_CODE_INVALID_CONNECTION_SETTINGS\x10\t\x12 \n\x1c\x45RROR_CODE_ALREADY_CONNECTED\x10\n\x12\x1a\n\x16\x45RROR_CODE_DEVICE_BUSY\x10\x0b\x12\"\n\x1e\x45RROR_CODE_CONNECTION_REQUIRED\x10\x0c\x12$\n ERROR_CODE_PAIRING_CODE_REQUIRED\x10\r\x12$\n ERROR_CODE_SCAN_FILTERS_REQUIRED\x10\x0e\x12#\n\x1f\x45RROR_CODE_SCAN_ALREADY_RUNNING\x10\x0f\x12\x1b\n\x17\x45RROR_CODE_SCAN_STOPPED\x10\x10\x42\x13\n\x0f\x63om.bluerpc.rpcP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10rpc/common.proto\x12\x03rpc\"-\n\x0cHelloRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"\x96\x02\n\rHelloResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x0e\n\x06uptime\x18\x03 \x01(\x04\x12(\n\x0fsupported_modes\x18\x04 \x03(\x0e\x32\x0f.rpc.WorkerMode\x12$\n\x0bworker_type\x18\x05 \x01(\x0e\x32\x0f.rpc.WorkerType\x12\x18\n\x10operating_system\x18\x06 \x01(\t\x12 \n\x18operating_system_version\x18\x07 \x01(\t\x12\x1c\n\x14\x62le_filters_required\x18\x08 \x01(\x08\x12\x0e\n\x06\x62t_mac\x18\t \x01(\t\x12\x0f\n\x07net_mac\x18\n \x01(\t\x12\x0b\n\x03uid\x18\x0b \x01(\t\">\n\rStatusMessage\x12\x1c\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0e.rpc.ErrorCode\x12\x0f\n\x07message\x18\x02 \x01(\t\"\x06\n\x04Void*V\n\nWorkerType\x12\x17\n\x13WORKER_TYPE_UNKNOWN\x10\x00\x12\x16\n\x12WORKER_TYPE_PYTHON\x10\x01\x12\x17\n\x13WORKER_TYPE_ANDROID\x10\x02*\\\n\nWorkerMode\x12\x13\n\x0fWORKER_MODE_UNK\x10\x00\x12\x1c\n\x18WORKER_MODE_GATT_PASSIVE\x10\x01\x12\x1b\n\x17WORKER_MODE_GATT_ACTIVE\x10\x02*\xa8\x04\n\tErrorCode\x12\x12\n\x0e\x45RROR_CODE_UNK\x10\x00\x12\x11\n\rERROR_CODE_OK\x10\x01\x12\x14\n\x10\x45RROR_CODE_ERROR\x10\x02\x12\x1a\n\x16\x45RROR_CODE_UNAVAILABLE\x10\x03\x12 \n\x1c\x45RROR_CODE_CONNECTION_FAILED\x10\x04\x12\x1e\n\x1a\x45RROR_CODE_UNKNOWN_SERVICE\x10\x05\x12%\n!ERROR_CODE_UNKNOWN_CHARACTERISTIC\x10\x06\x12!\n\x1d\x45RROR_CODE_UNKNOWN_DESCRIPTOR\x10\x07\x12\x1a\n\x16\x45RROR_CODE_UNSUPPORTED\x10\x08\x12*\n&ERROR_CODE_INVALID_CONNECTION_SETTINGS\x10\t\x12 \n\x1c\x45RROR_CODE_ALREADY_CONNECTED\x10\n\x12\x1a\n\x16\x45RROR_CODE_DEVICE_BUSY\x10\x0b\x12\"\n\x1e\x45RROR_CODE_CONNECTION_REQUIRED\x10\x0c\x12$\n ERROR_CODE_PAIRING_CODE_REQUIRED\x10\r\x12$\n ERROR_CODE_SCAN_FILTERS_REQUIRED\x10\x0e\x12#\n\x1f\x45RROR_CODE_SCAN_ALREADY_RUNNING\x10\x0f\x12\x1b\n\x17\x45RROR_CODE_SCAN_STOPPED\x10\x10\x42\x13\n\x0f\x63om.bluerpc.rpcP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'rpc.common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017com.bluerpc.rpcP\001'
-  _WORKERTYPE._serialized_start=349
-  _WORKERTYPE._serialized_end=435
-  _WORKERMODE._serialized_start=437
-  _WORKERMODE._serialized_end=529
-  _ERRORCODE._serialized_start=532
-  _ERRORCODE._serialized_end=1084
+  _WORKERTYPE._serialized_start=425
+  _WORKERTYPE._serialized_end=511
+  _WORKERMODE._serialized_start=513
+  _WORKERMODE._serialized_end=605
+  _ERRORCODE._serialized_start=608
+  _ERRORCODE._serialized_end=1160
   _HELLOREQUEST._serialized_start=25
   _HELLOREQUEST._serialized_end=70
   _HELLORESPONSE._serialized_start=73
-  _HELLORESPONSE._serialized_end=275
-  _STATUSMESSAGE._serialized_start=277
-  _STATUSMESSAGE._serialized_end=339
-  _VOID._serialized_start=341
-  _VOID._serialized_end=347
+  _HELLORESPONSE._serialized_end=351
+  _STATUSMESSAGE._serialized_start=353
+  _STATUSMESSAGE._serialized_end=415
+  _VOID._serialized_start=417
+  _VOID._serialized_end=423
 # @@protoc_insertion_point(module_scope)
```

### Comparing `bluerpc-0.0.8/bluerpc/rpc/gatt_pb2.py` & `bluerpc-0.2.6/bluerpc/rpc/gatt_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,66 +10,66 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from bluerpc.rpc import common_pb2 as rpc_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0erpc/gatt.proto\x12\x03rpc\x1a\x10rpc/common.proto\"D\n\rBLEScanFilter\x12$\n\x04type\x18\x01 \x01(\x0e\x32\x16.rpc.BLEScanFilterType\x12\r\n\x05value\x18\x02 \x01(\t\"W\n\x0e\x42LEScanRequest\x12\x10\n\x08interval\x18\x01 \x01(\x04\x12\x0e\n\x06\x61\x63tive\x18\x02 \x01(\x08\x12#\n\x07\x66ilters\x18\x03 \x03(\x0b\x32\x12.rpc.BLEScanFilter\"&\n\tBLEDevice\x12\x0b\n\x03mac\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x02 \x01(\t\"\x8c\x02\n\x0f\x42LEScanResponse\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.rpc.StatusMessage\x12\x1e\n\x06\x64\x65vice\x18\x02 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x0c\n\x04rssi\x18\x03 \x01(\x02\x12\r\n\x05txpwr\x18\x04 \x01(\x02\x12\x15\n\rservice_uuids\x18\x05 \x03(\t\x12/\n\x0cservice_data\x18\x06 \x03(\x0b\x32\x19.rpc.BLEAdvertisementData\x12\x34\n\x11manufacturer_data\x18\x07 \x03(\x0b\x32\x19.rpc.BLEAdvertisementData\x12\x0c\n\x04time\x18\x08 \x01(\x04\x12\x0c\n\x04name\x18\t \x01(\t\"3\n\x14\x42LEAdvertisementData\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\"3\n\x11\x42LEConnectRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\"E\n\x12\x42LEConnectResponse\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.rpc.StatusMessage\x12\x0b\n\x03mtu\x18\x02 \x01(\r\"3\n\x11\x42LEPairingRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\"E\n\x15\x42LEPairingCodeRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"\xc2\x01\n\x12\x42LEDevicesResponse\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.rpc.StatusMessage\x12\x17\n\x0fmax_connections\x18\x02 \x01(\r\x12)\n\x11\x63onnected_devices\x18\x03 \x03(\x0b\x32\x0e.rpc.BLEDevice\x12\x1c\n\x14reliable_paired_list\x18\x04 \x01(\x08\x12&\n\x0epaired_devices\x18\x05 \x03(\x0b\x32\x0e.rpc.BLEDevice\"S\n\x1f\x42LEConnectionPropertiesResponse\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.rpc.StatusMessage\x12\x0c\n\x04rssi\x18\x02 \x01(\x02\"\x80\x01\n\x17\x42LEListServicesResponse\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.rpc.StatusMessage\x12\x1e\n\x06\x64\x65vice\x18\x02 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12!\n\x08services\x18\x03 \x03(\x0b\x32\x0f.rpc.BLEService\"K\n\nBLEService\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12/\n\x0f\x63haracteristics\x18\x02 \x03(\x0b\x32\x16.rpc.BLECharacteristic\"s\n\x11\x42LECharacteristic\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\'\n\nproperties\x18\x02 \x03(\x0e\x32\x13.rpc.BLEChrProperty\x12\'\n\x0b\x64\x65scriptors\x18\x03 \x03(\x0b\x32\x12.rpc.BLEDescriptor\"\x1d\n\rBLEDescriptor\x12\x0c\n\x04uuid\x18\x01 \x01(\t\"C\n\x0f\x42LEReadResponse\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.rpc.StatusMessage\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"b\n\x1c\x42LEReadCharacteristicRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x14\n\x0cservice_uuid\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\"{\n\x18\x42LEReadDescriptorRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x14\n\x0cservice_uuid\x18\x02 \x01(\t\x12\x1b\n\x13\x63haracteristic_uuid\x18\x03 \x01(\t\x12\x0c\n\x04uuid\x18\x04 \x01(\t\"\x92\x01\n\x1d\x42LEWriteCharacteristicRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x14\n\x0cservice_uuid\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12\x1f\n\x04mode\x18\x05 \x01(\x0e\x32\x11.rpc.BLEWriteMode\"\x8a\x01\n\x19\x42LEWriteDescriptorRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x14\n\x0cservice_uuid\x18\x02 \x01(\t\x12\x1b\n\x13\x63haracteristic_uuid\x18\x03 \x01(\t\x12\x0c\n\x04uuid\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"o\n\x16\x42LENotificationRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x14\n\x0cservice_uuid\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x11\n\tsubscribe\x18\x04 \x01(\x08\"k\n\x17\x42LENotificationResponse\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x14\n\x0cservice_uuid\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c*\x91\x01\n\x11\x42LEScanFilterType\x12 \n\x1c\x42LE_SCAN_FILTER_TYPE_UNKNOWN\x10\x00\x12\x1c\n\x18\x42LE_SCAN_FILTER_TYPE_MAC\x10\x01\x12\x1d\n\x19\x42LE_SCAN_FILTER_TYPE_NAME\x10\x02\x12\x1d\n\x19\x42LE_SCAN_FILTER_TYPE_UUID\x10\x03*\xad\x02\n\x0e\x42LEChrProperty\x12\x18\n\x14\x42LE_CHR_PROPERTY_UNK\x10\x00\x12\x19\n\x15\x42LE_CHR_PROPERTY_READ\x10\x01\x12\x1a\n\x16\x42LE_CHR_PROPERTY_WRITE\x10\x02\x12\x1b\n\x17\x42LE_CHR_PROPERTY_NOTIFY\x10\x03\x12\x1e\n\x1a\x42LE_CHR_PROPERTY_BROADCAST\x10\x04\x12#\n\x1f\x42LE_CHR_PROPERTY_EXTENDED_PROPS\x10\x05\x12\x1d\n\x19\x42LE_CHR_PROPERTY_INDICATE\x10\x06\x12!\n\x1d\x42LE_CHR_PROPERTY_SIGNED_WRITE\x10\x07\x12&\n\"BLE_CHR_PROPERTY_WRITE_NO_RESPONSE\x10\x08*a\n\x0c\x42LEWriteMode\x12\x16\n\x12\x42LE_WRITE_MODE_UNK\x10\x00\x12\x1e\n\x1a\x42LE_WRITE_MODE_NO_RESPONSE\x10\x01\x12\x19\n\x15\x42LE_WRITE_MODE_SIGNED\x10\x02\x42\x13\n\x0f\x63om.bluerpc.rpcP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0erpc/gatt.proto\x12\x03rpc\x1a\x10rpc/common.proto\"D\n\rBLEScanFilter\x12$\n\x04type\x18\x01 \x01(\x0e\x32\x16.rpc.BLEScanFilterType\x12\r\n\x05value\x18\x02 \x01(\t\"n\n\x0e\x42LEScanRequest\x12\x10\n\x08interval\x18\x01 \x01(\x04\x12\x0e\n\x06\x61\x63tive\x18\x02 \x01(\x08\x12#\n\x07\x66ilters\x18\x03 \x03(\x0b\x32\x12.rpc.BLEScanFilter\x12\x15\n\rmerge_filters\x18\x04 \x01(\x08\"&\n\tBLEDevice\x12\x0b\n\x03mac\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x02 \x01(\t\"\x8c\x02\n\x0f\x42LEScanResponse\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.rpc.StatusMessage\x12\x1e\n\x06\x64\x65vice\x18\x02 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x0c\n\x04rssi\x18\x03 \x01(\x02\x12\r\n\x05txpwr\x18\x04 \x01(\x02\x12\x15\n\rservice_uuids\x18\x05 \x03(\t\x12/\n\x0cservice_data\x18\x06 \x03(\x0b\x32\x19.rpc.BLEAdvertisementData\x12\x34\n\x11manufacturer_data\x18\x07 \x03(\x0b\x32\x19.rpc.BLEAdvertisementData\x12\x0c\n\x04time\x18\x08 \x01(\x04\x12\x0c\n\x04name\x18\t \x01(\t\"3\n\x14\x42LEAdvertisementData\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\"3\n\x11\x42LEConnectRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\"E\n\x12\x42LEConnectResponse\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.rpc.StatusMessage\x12\x0b\n\x03mtu\x18\x02 \x01(\r\"3\n\x11\x42LEPairingRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\"E\n\x15\x42LEPairingCodeRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"\xc2\x01\n\x12\x42LEDevicesResponse\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.rpc.StatusMessage\x12\x17\n\x0fmax_connections\x18\x02 \x01(\r\x12)\n\x11\x63onnected_devices\x18\x03 \x03(\x0b\x32\x0e.rpc.BLEDevice\x12\x1c\n\x14reliable_paired_list\x18\x04 \x01(\x08\x12&\n\x0epaired_devices\x18\x05 \x03(\x0b\x32\x0e.rpc.BLEDevice\"S\n\x1f\x42LEConnectionPropertiesResponse\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.rpc.StatusMessage\x12\x0c\n\x04rssi\x18\x02 \x01(\x02\"\x80\x01\n\x17\x42LEListServicesResponse\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.rpc.StatusMessage\x12\x1e\n\x06\x64\x65vice\x18\x02 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12!\n\x08services\x18\x03 \x03(\x0b\x32\x0f.rpc.BLEService\"K\n\nBLEService\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12/\n\x0f\x63haracteristics\x18\x02 \x03(\x0b\x32\x16.rpc.BLECharacteristic\"s\n\x11\x42LECharacteristic\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\'\n\nproperties\x18\x02 \x03(\x0e\x32\x13.rpc.BLEChrProperty\x12\'\n\x0b\x64\x65scriptors\x18\x03 \x03(\x0b\x32\x12.rpc.BLEDescriptor\"\x1d\n\rBLEDescriptor\x12\x0c\n\x04uuid\x18\x01 \x01(\t\"C\n\x0f\x42LEReadResponse\x12\"\n\x06status\x18\x01 \x01(\x0b\x32\x12.rpc.StatusMessage\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"b\n\x1c\x42LEReadCharacteristicRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x14\n\x0cservice_uuid\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\"{\n\x18\x42LEReadDescriptorRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x14\n\x0cservice_uuid\x18\x02 \x01(\t\x12\x1b\n\x13\x63haracteristic_uuid\x18\x03 \x01(\t\x12\x0c\n\x04uuid\x18\x04 \x01(\t\"\x92\x01\n\x1d\x42LEWriteCharacteristicRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x14\n\x0cservice_uuid\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12\x1f\n\x04mode\x18\x05 \x01(\x0e\x32\x11.rpc.BLEWriteMode\"\x8a\x01\n\x19\x42LEWriteDescriptorRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x14\n\x0cservice_uuid\x18\x02 \x01(\t\x12\x1b\n\x13\x63haracteristic_uuid\x18\x03 \x01(\t\x12\x0c\n\x04uuid\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"o\n\x16\x42LENotificationRequest\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x14\n\x0cservice_uuid\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x11\n\tsubscribe\x18\x04 \x01(\x08\"k\n\x17\x42LENotificationResponse\x12\x1e\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x0e.rpc.BLEDevice\x12\x14\n\x0cservice_uuid\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c*\x91\x01\n\x11\x42LEScanFilterType\x12 \n\x1c\x42LE_SCAN_FILTER_TYPE_UNKNOWN\x10\x00\x12\x1c\n\x18\x42LE_SCAN_FILTER_TYPE_MAC\x10\x01\x12\x1d\n\x19\x42LE_SCAN_FILTER_TYPE_NAME\x10\x02\x12\x1d\n\x19\x42LE_SCAN_FILTER_TYPE_UUID\x10\x03*\xad\x02\n\x0e\x42LEChrProperty\x12\x18\n\x14\x42LE_CHR_PROPERTY_UNK\x10\x00\x12\x19\n\x15\x42LE_CHR_PROPERTY_READ\x10\x01\x12\x1a\n\x16\x42LE_CHR_PROPERTY_WRITE\x10\x02\x12\x1b\n\x17\x42LE_CHR_PROPERTY_NOTIFY\x10\x03\x12\x1e\n\x1a\x42LE_CHR_PROPERTY_BROADCAST\x10\x04\x12#\n\x1f\x42LE_CHR_PROPERTY_EXTENDED_PROPS\x10\x05\x12\x1d\n\x19\x42LE_CHR_PROPERTY_INDICATE\x10\x06\x12!\n\x1d\x42LE_CHR_PROPERTY_SIGNED_WRITE\x10\x07\x12&\n\"BLE_CHR_PROPERTY_WRITE_NO_RESPONSE\x10\x08*a\n\x0c\x42LEWriteMode\x12\x16\n\x12\x42LE_WRITE_MODE_UNK\x10\x00\x12\x1e\n\x1a\x42LE_WRITE_MODE_NO_RESPONSE\x10\x01\x12\x19\n\x15\x42LE_WRITE_MODE_SIGNED\x10\x02\x42\x13\n\x0f\x63om.bluerpc.rpcP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'rpc.gatt_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017com.bluerpc.rpcP\001'
-  _BLESCANFILTERTYPE._serialized_start=2257
-  _BLESCANFILTERTYPE._serialized_end=2402
-  _BLECHRPROPERTY._serialized_start=2405
-  _BLECHRPROPERTY._serialized_end=2706
-  _BLEWRITEMODE._serialized_start=2708
-  _BLEWRITEMODE._serialized_end=2805
+  _BLESCANFILTERTYPE._serialized_start=2280
+  _BLESCANFILTERTYPE._serialized_end=2425
+  _BLECHRPROPERTY._serialized_start=2428
+  _BLECHRPROPERTY._serialized_end=2729
+  _BLEWRITEMODE._serialized_start=2731
+  _BLEWRITEMODE._serialized_end=2828
   _BLESCANFILTER._serialized_start=41
   _BLESCANFILTER._serialized_end=109
   _BLESCANREQUEST._serialized_start=111
-  _BLESCANREQUEST._serialized_end=198
-  _BLEDEVICE._serialized_start=200
-  _BLEDEVICE._serialized_end=238
-  _BLESCANRESPONSE._serialized_start=241
-  _BLESCANRESPONSE._serialized_end=509
-  _BLEADVERTISEMENTDATA._serialized_start=511
-  _BLEADVERTISEMENTDATA._serialized_end=562
-  _BLECONNECTREQUEST._serialized_start=564
-  _BLECONNECTREQUEST._serialized_end=615
-  _BLECONNECTRESPONSE._serialized_start=617
-  _BLECONNECTRESPONSE._serialized_end=686
-  _BLEPAIRINGREQUEST._serialized_start=688
-  _BLEPAIRINGREQUEST._serialized_end=739
-  _BLEPAIRINGCODEREQUEST._serialized_start=741
-  _BLEPAIRINGCODEREQUEST._serialized_end=810
-  _BLEDEVICESRESPONSE._serialized_start=813
-  _BLEDEVICESRESPONSE._serialized_end=1007
-  _BLECONNECTIONPROPERTIESRESPONSE._serialized_start=1009
-  _BLECONNECTIONPROPERTIESRESPONSE._serialized_end=1092
-  _BLELISTSERVICESRESPONSE._serialized_start=1095
-  _BLELISTSERVICESRESPONSE._serialized_end=1223
-  _BLESERVICE._serialized_start=1225
-  _BLESERVICE._serialized_end=1300
-  _BLECHARACTERISTIC._serialized_start=1302
-  _BLECHARACTERISTIC._serialized_end=1417
-  _BLEDESCRIPTOR._serialized_start=1419
-  _BLEDESCRIPTOR._serialized_end=1448
-  _BLEREADRESPONSE._serialized_start=1450
-  _BLEREADRESPONSE._serialized_end=1517
-  _BLEREADCHARACTERISTICREQUEST._serialized_start=1519
-  _BLEREADCHARACTERISTICREQUEST._serialized_end=1617
-  _BLEREADDESCRIPTORREQUEST._serialized_start=1619
-  _BLEREADDESCRIPTORREQUEST._serialized_end=1742
-  _BLEWRITECHARACTERISTICREQUEST._serialized_start=1745
-  _BLEWRITECHARACTERISTICREQUEST._serialized_end=1891
-  _BLEWRITEDESCRIPTORREQUEST._serialized_start=1894
-  _BLEWRITEDESCRIPTORREQUEST._serialized_end=2032
-  _BLENOTIFICATIONREQUEST._serialized_start=2034
-  _BLENOTIFICATIONREQUEST._serialized_end=2145
-  _BLENOTIFICATIONRESPONSE._serialized_start=2147
-  _BLENOTIFICATIONRESPONSE._serialized_end=2254
+  _BLESCANREQUEST._serialized_end=221
+  _BLEDEVICE._serialized_start=223
+  _BLEDEVICE._serialized_end=261
+  _BLESCANRESPONSE._serialized_start=264
+  _BLESCANRESPONSE._serialized_end=532
+  _BLEADVERTISEMENTDATA._serialized_start=534
+  _BLEADVERTISEMENTDATA._serialized_end=585
+  _BLECONNECTREQUEST._serialized_start=587
+  _BLECONNECTREQUEST._serialized_end=638
+  _BLECONNECTRESPONSE._serialized_start=640
+  _BLECONNECTRESPONSE._serialized_end=709
+  _BLEPAIRINGREQUEST._serialized_start=711
+  _BLEPAIRINGREQUEST._serialized_end=762
+  _BLEPAIRINGCODEREQUEST._serialized_start=764
+  _BLEPAIRINGCODEREQUEST._serialized_end=833
+  _BLEDEVICESRESPONSE._serialized_start=836
+  _BLEDEVICESRESPONSE._serialized_end=1030
+  _BLECONNECTIONPROPERTIESRESPONSE._serialized_start=1032
+  _BLECONNECTIONPROPERTIESRESPONSE._serialized_end=1115
+  _BLELISTSERVICESRESPONSE._serialized_start=1118
+  _BLELISTSERVICESRESPONSE._serialized_end=1246
+  _BLESERVICE._serialized_start=1248
+  _BLESERVICE._serialized_end=1323
+  _BLECHARACTERISTIC._serialized_start=1325
+  _BLECHARACTERISTIC._serialized_end=1440
+  _BLEDESCRIPTOR._serialized_start=1442
+  _BLEDESCRIPTOR._serialized_end=1471
+  _BLEREADRESPONSE._serialized_start=1473
+  _BLEREADRESPONSE._serialized_end=1540
+  _BLEREADCHARACTERISTICREQUEST._serialized_start=1542
+  _BLEREADCHARACTERISTICREQUEST._serialized_end=1640
+  _BLEREADDESCRIPTORREQUEST._serialized_start=1642
+  _BLEREADDESCRIPTORREQUEST._serialized_end=1765
+  _BLEWRITECHARACTERISTICREQUEST._serialized_start=1768
+  _BLEWRITECHARACTERISTICREQUEST._serialized_end=1914
+  _BLEWRITEDESCRIPTORREQUEST._serialized_start=1917
+  _BLEWRITEDESCRIPTORREQUEST._serialized_end=2055
+  _BLENOTIFICATIONREQUEST._serialized_start=2057
+  _BLENOTIFICATIONREQUEST._serialized_end=2168
+  _BLENOTIFICATIONRESPONSE._serialized_start=2170
+  _BLENOTIFICATIONRESPONSE._serialized_end=2277
 # @@protoc_insertion_point(module_scope)
```

### Comparing `bluerpc-0.0.8/bluerpc/rpc/services_pb2.py` & `bluerpc-0.2.6/bluerpc/rpc/services_pb2.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.0.8/bluerpc/rpc/services_pb2_grpc.py` & `bluerpc-0.2.6/bluerpc/rpc/services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bluerpc-0.0.8/bluerpc/service.py` & `bluerpc-0.2.6/bluerpc/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,43 +2,50 @@
 import platform
 import time
 
 import grpc
 from bluerpc.ble_conn import BLEConn
 from bluerpc.ble_scan import BLEScanner
 from bluerpc.rpc import common_pb2, gatt_pb2, services_pb2_grpc
-from bluerpc.utils import get_version
+from bluerpc.utils import get_net_mac, get_version
 
 START_TIME = time.time()
 
 
 class BlueRPCService(services_pb2_grpc.BlueRPCServicer):
     """
     Implementation of the BlueRPCService
     """
 
-    def __init__(self, name) -> None:
+    def __init__(self, name, adapter_mac="00:00:00:00:00:00", adapter_id=None) -> None:
         super().__init__()
         self._name = name
-        self._ble_scanner = BLEScanner()
+        self._adapter_mac = adapter_mac
+        self._ble_scanner = BLEScanner(adapter_id)
+        BLEConn.set_scanner(self._ble_scanner)
+        BLEConn.set_adapter(adapter_id)
 
     async def Hello(
         self, request: common_pb2.HelloRequest, context: grpc.aio.ServicerContext
     ) -> common_pb2.HelloResponse:
+        net_mac = get_net_mac()
         return common_pb2.HelloResponse(
             name=self._name,
             version=get_version(),
             uptime=round(time.time() - START_TIME),
             supported_modes=[
                 common_pb2.WORKER_MODE_GATT_ACTIVE,
                 common_pb2.WORKER_MODE_GATT_PASSIVE,
             ],
             worker_type=common_pb2.WORKER_TYPE_PYTHON,
             operating_system=platform.system(),
             operating_system_version=platform.release(),
+            bt_mac=self._adapter_mac,
+            net_mac=net_mac,
+            uid=(self._adapter_mac == "00:00:00:00:00:00" or net_mac).replace(":", ""),
         )
 
     async def BLEScanStart(
         self, request: gatt_pb2.BLEScanRequest, context: grpc.aio.ServicerContext
     ) -> common_pb2.StatusMessage:
         if not self._ble_scanner.running:
             await self._ble_scanner.scan(request.active, request.filters)
```

### Comparing `bluerpc-0.0.8/bluerpc.egg-info/PKG-INFO` & `bluerpc-0.2.6/bluerpc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluerpc
-Version: 0.0.8
+Version: 0.2.6
 Summary: Python BlueRPC Worker
 Home-page: https://github.com/BlueRPC/BlueRPC
 Author: drosocode
 License: MIT
 Project-URL: Documentation, https://bluerpc.github.io/
 Project-URL: Source, https://github.com/BlueRPC/BlueRPC/python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bluerpc-0.0.8/bluerpc.egg-info/SOURCES.txt` & `bluerpc-0.2.6/bluerpc.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 setup.py
 bluerpc/__init__.py
 bluerpc/ble_conn.py
 bluerpc/ble_scan.py
 bluerpc/cli.py
 bluerpc/discovery.py
+bluerpc/log.py
 bluerpc/service.py
 bluerpc/utils.py
 bluerpc.egg-info/PKG-INFO
 bluerpc.egg-info/SOURCES.txt
 bluerpc.egg-info/dependency_links.txt
 bluerpc.egg-info/entry_points.txt
 bluerpc.egg-info/requires.txt
```

### Comparing `bluerpc-0.0.8/setup.py` & `bluerpc-0.2.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,27 +2,36 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="bluerpc",
     packages=find_packages(),
-    version="0.0.8",
+    version="0.2.6",
     author="drosocode",
     license="MIT",
     description="Python BlueRPC Worker",
     url="https://github.com/BlueRPC/BlueRPC",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["bleak", "grpcio", "protobuf", "cryptography", "zeroconf"],
+    install_requires=[
+        "bleak",
+        "bluetooth-adapters",
+        "cryptography",
+        "grpcio",
+        "grpc-interceptor",
+        "protobuf",
+        "netifaces",
+        "zeroconf",
+    ],
     python_requires=">=3.8",
     project_urls={
         "Documentation": "https://bluerpc.github.io/",
         "Source": "https://github.com/BlueRPC/BlueRPC/python",
     },
     entry_points={"console_scripts": ["bluerpc=bluerpc.cli:run"]},
 )
```

