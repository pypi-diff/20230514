# Comparing `tmp/lmcloud-0.3.2.tar.gz` & `tmp/lmcloud-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcloud-0.3.2.tar", last modified: Fri May 12 19:00:14 2023, max compression
+gzip compressed data, was "lmcloud-0.3.3.tar", last modified: Sun May 14 07:24:06 2023, max compression
```

## Comparing `lmcloud-0.3.2.tar` & `lmcloud-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:00:14.940599 lmcloud-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-12 19:00:01.000000 lmcloud-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-12 19:00:14.936599 lmcloud-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-12 19:00:01.000000 lmcloud-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:00:14.936599 lmcloud-0.3.2/lmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 19:00:01.000000 lmcloud-0.3.2/lmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-12 19:00:01.000000 lmcloud-0.3.2/lmcloud/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-12 19:00:01.000000 lmcloud-0.3.2/lmcloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-12 19:00:01.000000 lmcloud-0.3.2/lmcloud/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-12 19:00:01.000000 lmcloud-0.3.2/lmcloud/lmbluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)    23575 2023-05-12 19:00:01.000000 lmcloud-0.3.2/lmcloud/lmcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-12 19:00:01.000000 lmcloud-0.3.2/lmcloud/lmlocalapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:00:14.936599 lmcloud-0.3.2/lmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-12 19:00:14.000000 lmcloud-0.3.2/lmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-12 19:00:14.000000 lmcloud-0.3.2/lmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:00:14.000000 lmcloud-0.3.2/lmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 19:00:14.000000 lmcloud-0.3.2/lmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 19:00:14.000000 lmcloud-0.3.2/lmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:00:14.940599 lmcloud-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-12 19:00:01.000000 lmcloud-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:24:06.628039 lmcloud-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-14 07:23:52.000000 lmcloud-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-14 07:24:06.624039 lmcloud-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-14 07:23:52.000000 lmcloud-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:24:06.624039 lmcloud-0.3.3/lmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 07:23:52.000000 lmcloud-0.3.3/lmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-14 07:23:52.000000 lmcloud-0.3.3/lmcloud/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-14 07:23:52.000000 lmcloud-0.3.3/lmcloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-14 07:23:52.000000 lmcloud-0.3.3/lmcloud/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-14 07:23:52.000000 lmcloud-0.3.3/lmcloud/lmbluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23575 2023-05-14 07:23:52.000000 lmcloud-0.3.3/lmcloud/lmcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-14 07:23:52.000000 lmcloud-0.3.3/lmcloud/lmlocalapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:24:06.624039 lmcloud-0.3.3/lmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-14 07:24:06.000000 lmcloud-0.3.3/lmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-14 07:24:06.000000 lmcloud-0.3.3/lmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 07:24:06.000000 lmcloud-0.3.3/lmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-14 07:24:06.000000 lmcloud-0.3.3/lmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 07:24:06.000000 lmcloud-0.3.3/lmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 07:24:06.628039 lmcloud-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-14 07:23:52.000000 lmcloud-0.3.3/setup.py
```

### Comparing `lmcloud-0.3.2/LICENSE` & `lmcloud-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.2/PKG-INFO` & `lmcloud-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.3.2/README.md` & `lmcloud-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.2/lmcloud/const.py` & `lmcloud-0.3.3/lmcloud/const.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.2/lmcloud/helpers.py` & `lmcloud-0.3.3/lmcloud/helpers.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.2/lmcloud/lmbluetooth.py` & `lmcloud-0.3.3/lmcloud/lmbluetooth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import asyncio
 import base64
 import logging
-from bleak import BleakScanner, BleakClient
+from bleak import BleakScanner, BleakClient, BLEDevice, BleakError
 from .exceptions import BluetoothDeviceNotFound
 from .const import SETTINGS_CHARACTERISTIC, AUTH_CHARACTERISTIC, MODEL_LMU
 
 _logger = logging.getLogger(__name__)
 
+
 class LMBluetooth:
     """
     class to interact with machine via Bluetooth
     """
 
     def __init__(self, username, serial_number, token):
-      self._username = username
-      self._serial_number = serial_number
-      self._token = token
-      self._address = None
-      self._name = None
-      self._client = None
-
+        self._username = username
+        self._serial_number = serial_number
+        self._token = token
+        self._address = None
+        self._name = None
+        self._client = None
 
     @classmethod
     async def create(cls, username, serial_number, token, bleak_scanner=None):
         """
         Init class by scanning for devices and selecting the first one with "MICRA" in the name
         """
         self = cls(username, serial_number, token)
@@ -50,15 +50,14 @@
         devices = await scanner.discover()
         for d in devices:
             if d.name:
                 if MODEL_LMU.upper() in d.name:
                     self._address = d.address
                     self._name = d.name
 
-    
     async def write_bluetooth_message(self, message, characteristic: str):
         """
         connect to machine and write a message
         """
         if not self._client.is_connected:
             await self._client.connect()
             await self.authenticate()
@@ -67,27 +66,38 @@
         if characteristic == SETTINGS_CHARACTERISTIC:
             message += '\x00'
         
         # check if message is already bytes string
         if not isinstance(message, bytes):
             message = bytes(message, 'utf-8')
 
+        _logger.debug(f"Sending bluetooth message: {message} to {characteristic}")
         await self._client.write_gatt_char(characteristic, message)
 
-
     async def authenticate(self):
         """
         build authentication string and send it to the machine
         """
         user = self._username + ":" + self._serial_number
         user = bytes(user, 'utf-8')
         token = bytes(self._token, 'utf-8')
         auth_string = base64.b64encode(user) + b'@' + base64.b64encode(token)
         await self.write_bluetooth_message(auth_string, AUTH_CHARACTERISTIC)
 
+    async def new_bleak_client_from_ble_device(self, ble_device: BLEDevice):
+        """
+        initalize a new bleak client from a BLEDevice (for Home Assistant)
+        """
+        self._client = BleakClient(ble_device)
+        try:
+            await self._client.connect()
+            await self.authenticate()
+        except BleakError as e:
+            _logger.error(f"Failed to connect to machine with Bluetooth: {e}")
+
     async def set_power(self, state: bool):
         """
         Power on the machine
         """
         mode = "BrewingMode" if state else "StandBy"
         msg = "{\"name\":\"MachineChangeMode\",\"parameter\":{\"mode\":\"" + mode + "\"}}"
         await self.write_bluetooth_message(msg, SETTINGS_CHARACTERISTIC)
@@ -95,24 +105,24 @@
     async def set_steam(self, state: bool):
         """
         Power on steam
         """
         msg = "{\"name\":\"SettingBoilerEnable\",\"parameter\":{\"identifier\":\"SteamBoiler\",\"state\":" + str(state).lower() + "}}"
         await self.write_bluetooth_message(msg, SETTINGS_CHARACTERISTIC)
 
-    async def set_steam_temp(self, temperature:int):
+    async def set_steam_temp(self, temperature: int):
         '''
         Set steamboiler temperature (in Celsius)
         '''
         if not temperature == 131 and not temperature == 128 and not temperature == 126:
             msg = "Steam temp must be one of 126, 128, 131 (°C)"
             raise ValueError(msg)
         else:
-            msg = "{\"name\":\"SettingBoilerTarget\",\"parameter\":{\"identifier\":\"SteamBoiler\",\"value\":" +  str(temperature) + "}}"
+            msg = "{\"name\":\"SettingBoilerTarget\",\"parameter\":{\"identifier\":\"SteamBoiler\",\"value\":" + str(temperature) + "}}"
             await self.write_bluetooth_message(msg, SETTINGS_CHARACTERISTIC)
 
     async def set_coffee_temp(self, temperature:int):
         '''
         Set Cofeeboiler temperature (in Celsius)
         '''
-        msg = "{\"name\":\"SettingBoilerTarget\",\"parameter\":{\"identifier\":\"CoffeeBoiler1\",\"value\":" +  str(temperature) + "}}"
+        msg = "{\"name\":\"SettingBoilerTarget\",\"parameter\":{\"identifier\":\"CoffeeBoiler1\",\"value\":" + str(temperature) + "}}"
         await self.write_bluetooth_message(msg, SETTINGS_CHARACTERISTIC)
```

### Comparing `lmcloud-0.3.2/lmcloud/lmcloud.py` & `lmcloud-0.3.3/lmcloud/lmcloud.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.2/lmcloud/lmlocalapi.py` & `lmcloud-0.3.3/lmcloud/lmlocalapi.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.2/lmcloud.egg-info/PKG-INFO` & `lmcloud-0.3.3/lmcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.3.2/setup.py` & `lmcloud-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="lmcloud",
-    version="0.3.2",
+    version="0.3.3",
     description="A Python implementation of the new La Marzocco API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/lmcloud",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

