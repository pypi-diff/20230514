# Comparing `tmp/sds011lib-0.2.2.tar.gz` & `tmp/sds011lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sds011lib-0.2.2.tar", max compression
+gzip compressed data, was "sds011lib-0.3.0.tar", max compression
```

## Comparing `sds011lib-0.2.2.tar` & `sds011lib-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-12 03:40:54.500682 sds011lib-0.2.2/LICENSE
--rw-r--r--   0        0        0      945 2023-05-12 03:40:54.500682 sds011lib-0.2.2/README.md
--rw-r--r--   0        0        0      955 2023-05-12 03:40:54.500682 sds011lib-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    19852 2023-05-12 03:40:54.500682 sds011lib-0.2.2/sds011lib/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-12 03:40:54.500682 sds011lib-0.2.2/sds011lib/constants.py
--rw-r--r--   0        0        0     2332 2023-05-12 03:40:54.500682 sds011lib-0.2.2/sds011lib/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-12 03:40:54.500682 sds011lib-0.2.2/sds011lib/py.typed
--rw-r--r--   0        0        0     5797 2023-05-12 03:40:54.500682 sds011lib-0.2.2/sds011lib/responses.py
--rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 sds011lib-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-13 22:51:24.542011 sds011lib-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1163 2023-05-13 22:51:24.542011 sds011lib-0.3.0/README.md
+-rw-r--r--   0        0        0      977 2023-05-13 22:51:24.542011 sds011lib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    26710 2023-05-13 22:51:24.542011 sds011lib-0.3.0/sds011lib/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-13 22:51:24.542011 sds011lib-0.3.0/sds011lib/_constants.py
+-rw-r--r--   0        0        0     2332 2023-05-13 22:51:24.542011 sds011lib-0.3.0/sds011lib/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:51:24.542011 sds011lib-0.3.0/sds011lib/py.typed
+-rw-r--r--   0        0        0     1974 2023-05-13 22:51:24.542011 sds011lib-0.3.0/sds011lib/responses.py
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 sds011lib-0.3.0/PKG-INFO
```

### Comparing `sds011lib-0.2.2/LICENSE` & `sds011lib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sds011lib-0.2.2/README.md` & `sds011lib-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # sds011lib
 
+[![PyPI version](https://badge.fury.io/py/sds011lib.svg)](https://badge.fury.io/py/sds011lib)
 ![Main](https://github.com/TimOrme/sds011lib/actions/workflows/main.yml/badge.svg)
+[![Coverage](https://codecov.io/gh/TimOrme/sds011lib/branch/main/graph/badge.svg)](https://codecov.io/gh/TimOrme/sds011lib)
 
 `sds011lib` is a fully-typed, nearly-complete, python 3.8+ library for interacting with the SDS011 Air Quality Sensor.
 
 The SDS011 is a small, low-cost sensor created by www.inovafitness.com, used to measure particulate matter in the air.  It 
 can measure both PM 2.5 and PM10 values simultaneously, and connects to devices over a serial port, or via USB with an
 included adaptor.
```

### Comparing `sds011lib-0.2.2/pyproject.toml` & `sds011lib-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sds011lib"
-version = "0.2.2"
+version = "0.3.0"
 description = "SDS011 Library"
 authors = ["Tim Orme <TimothyOrme@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyserial = "^3.5"
@@ -17,14 +17,15 @@
 types-pyserial = "^3.5.0.8"
 myst-parser = "^1.0.0"
 mkdocs = "^1.4.2"
 mkdocs-gitbook = "^0.0.1"
 mkdocs-material = "^9.1.8"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 tox = "^4.5.1"
+pytest-cov = "^4.0.0"
 
 [tool.ruff]
 select = ["E", "F", "D"]
 ignore = ["D203", "D213"]
 line-length = 120
 
 [tool.ruff.pydocstyle]
```

### Comparing `sds011lib-0.2.2/sds011lib/__init__.py` & `sds011lib-0.3.0/sds011lib/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,98 @@
-"""Nova PM SDS011 Reader module.
+"""SDS011 Reader module.
 
-Device: https://www.amazon.com/SDS011-Quality-Detection-Conditioning-Monitor/dp/B07FSDMRR5
+Contains multiple implementations of readers, for different use cases.
 
-Spec: https://cdn.sparkfun.com/assets/parts/1/2/2/7/5/Laser_Dust_Sensor_Control_Protocol_V1.3.pdf
-Spec: https://cdn-reichelt.de/documents/datenblatt/X200/SDS011-DATASHEET.pdf
+* SDS011QueryReader - (Recommended) A reader which operates exclusively in query mode.
+* SDS011ActiveReader - A reader which operates exclusively in active mode
+* SS011Reader - A lower-level reader, which isn't opinionated about the mode.
+
+Attributes:
+    ALL_SENSORS: A special device ID which targets all sensors attached to a serial port.
 """
 
 import time
 
 import serial
 
 from .responses import (
     QueryResponse,
     ReportingModeResponse,
     SleepWakeReadResponse,
     DeviceIdResponse,
     CheckFirmwareResponse,
     WorkingPeriodReadResponse,
 )
-from . import constants as con
+from ._constants import (
+    ALL_SENSOR_ID,
+    HEAD,
+    TAIL,
+    SUBMIT_TYPE,
+    Command,
+    ResponseType,
+    OperationType,
+    SleepState,
+    ReportingMode,
+)
 from .exceptions import (
     IncompleteReadException,
     IncorrectCommandException,
     IncorrectCommandCodeException,
+    ChecksumFailedException,
+    IncorrectWrapperException,
 )
 
 from typing import Protocol, Union, Optional, runtime_checkable
+from dataclasses import dataclass
+
+# We lift this out of the private constants module, since its part of the contracts as defaults, and users might want to
+# leverage it.
+ALL_SENSORS: bytes = ALL_SENSOR_ID
 
 
 @runtime_checkable
 class SerialLike(Protocol):
     """A serial-like device."""
 
     def read(self, size: int) -> bytes:
         """Read data from the device."""
-        pass
 
     def write(self, data: bytes) -> Optional[int]:
         """Write data from the device."""
-        pass
 
     def open(self) -> None:
         """Open a connection to the device."""
-        pass
 
     def close(self) -> None:
         """Close a connection to the device."""
-        pass
+
+
+@dataclass(frozen=True)
+class _RawReadResponse:
+    """A raw read response object for responses from SDS011.
+
+    Attributes:
+        head: The header bytes from the response
+        cmd_id: The command ID from the response
+        payload: The data packet bytes from the response.
+        device_id: The device ID from the response
+        checksum: The returned checksum for the response
+        tail: The tail bytes from the response
+        expected_command_code: The expected command code
+        expected_response_type: The expected response type, either GENERAL or QUERY.
+    """
+
+    head: bytes
+    cmd_id: bytes
+    payload: bytes
+    device_id: bytes
+    checksum: int
+    tail: bytes
+    expected_command_code: Command
+    expected_response_type: ResponseType
 
 
 class SDS011Reader:
     """NOVA PM SDS011 Reader."""
 
     def __init__(self, ser_dev: Union[str, SerialLike], send_command_sleep: int = 1):
         """Create a basic device.
@@ -67,72 +109,72 @@
             self.ser: SerialLike = serial.Serial(ser_dev, timeout=2)
         elif isinstance(ser_dev, SerialLike):
             self.ser = ser_dev
         else:
             raise AttributeError("ser_dev must be a string or Serial-like object.")
         self.send_command_sleep = send_command_sleep
 
-    def request_data(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
+    def request_data(self, device_id: bytes = ALL_SENSORS) -> None:
         """Submit a request to the device to return pollutant data."""
-        cmd = con.Command.QUERY.value + (b"\x00" * 12) + device_id
+        cmd = Command.QUERY.value + (b"\x00" * 12) + device_id
         self._send_command(cmd)
 
     def query_data(self) -> QueryResponse:
         """Query the device for pollutant data.
 
         Returns:
             Pollutant data from the device.
 
         """
-        return QueryResponse(self._read_response())
+        return self._parse_query_response(self._read_response())
 
-    def request_reporting_mode(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
+    def request_reporting_mode(self, device_id: bytes = ALL_SENSORS) -> None:
         """Submit a request to the device to return the current reporting mode."""
         cmd = (
-            con.Command.SET_REPORTING_MODE.value
-            + con.OperationType.QUERY.value
-            + con.ReportingMode.ACTIVE.value
+            Command.SET_REPORTING_MODE.value
+            + OperationType.QUERY.value
+            + ReportingMode.ACTIVE.value
             + (b"\x00" * 10)
             + device_id
         )
         self._send_command(cmd)
 
     def query_reporting_mode(self) -> ReportingModeResponse:
         """Get the current reporting mode of the device.
 
         Returns:
             The current reporting mode of the device.
 
         """
-        return ReportingModeResponse(self._read_response())
+        return self._parse_reporting_mode_response(self._read_response())
 
     def set_active_mode(self) -> None:
         """Set the reporting mode to active."""
-        self._set_reporting_mode(con.ReportingMode.ACTIVE)
+        self._set_reporting_mode(ReportingMode.ACTIVE)
         try:
             self.query_reporting_mode()
         except IncorrectCommandException:
             pass
         except IncompleteReadException:
             pass
 
     def set_query_mode(self) -> None:
         """Set the reporting mode to querying."""
-        self._set_reporting_mode(con.ReportingMode.QUERYING)
+        self._set_reporting_mode(ReportingMode.QUERYING)
         try:
             self.query_reporting_mode()
         except IncorrectCommandException:
             pass
         except IncompleteReadException:
             pass
         except IncorrectCommandCodeException:
             pass
 
     def _set_reporting_mode(
-        self, reporting_mode: con.ReportingMode, device_id: bytes = con.ALL_SENSOR_ID
+        self, reporting_mode: ReportingMode, device_id: bytes = ALL_SENSORS
     ) -> None:
         """Set the reporting mode, either ACTIVE or QUERYING.
 
         ACTIVE mode means the device will always return a Query command response when data is asked for, regardless of
         what command was sent.
 
         QUERYING mode means the device will only return responses to submitted commands, even for Query commands.
@@ -140,184 +182,181 @@
         ACTIVE mode is the factory default, but generally, QUERYING mode is preferrable for the longevity of the device.
 
         Args:
             reporting_mode: The reporting mode to set.
             device_id: The device ID to set reporting mode on.
         """
         cmd = (
-            con.Command.SET_REPORTING_MODE.value
-            + con.OperationType.SET_MODE.value
+            Command.SET_REPORTING_MODE.value
+            + OperationType.SET_MODE.value
             + reporting_mode.value
             + (b"\x00" * 10)
             + device_id
         )
         self._send_command(cmd)
         # Switching between reporting modes is finicky; resetting the serial connection seems to address issues.
         self.ser.close()
         self.ser.open()
 
-    def request_sleep_state(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
+    def request_sleep_state(self, device_id: bytes = ALL_SENSORS) -> None:
         """Submit a request to get the current sleep state."""
         cmd = (
-            con.Command.SET_SLEEP.value
-            + con.OperationType.QUERY.value
+            Command.SET_SLEEP.value
+            + OperationType.QUERY.value
             + b"\x00"
             + (b"\x00" * 10)
             + device_id
         )
         self._send_command(cmd)
 
     def query_sleep_state(self) -> SleepWakeReadResponse:
         """Get the current sleep state.
 
         Returns:
             The current sleep state of the device.
         """
-        return SleepWakeReadResponse(self._read_response())
+        return self._parse_sleep_wake_response(self._read_response())
 
     def set_sleep_state(
-        self, sleep_state: con.SleepState, device_id: bytes = con.ALL_SENSOR_ID
+        self, sleep_state: SleepState, device_id: bytes = ALL_SENSORS
     ) -> None:
         """Set the sleep state, either wake or sleep.
 
         Args:
             sleep_state: The sleep state to set, either SleepState.WAKE or SleepState.SLEEP
             device_id: The device ID to sleep or wake.
         """
         cmd = (
-            con.Command.SET_SLEEP.value
-            + con.OperationType.SET_MODE.value
+            Command.SET_SLEEP.value
+            + OperationType.SET_MODE.value
             + sleep_state.value
             + (b"\x00" * 10)
             + device_id
         )
         self._send_command(cmd)
 
-    def sleep(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
+    def sleep(self, device_id: bytes = ALL_SENSORS) -> None:
         """Put the device to sleep, turning off fan and diode."""
-        self.set_sleep_state(con.SleepState.SLEEP, device_id)
+        self.set_sleep_state(SleepState.SLEEP, device_id)
 
-    def wake(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
+    def wake(self, device_id: bytes = ALL_SENSORS) -> None:
         """Wake the device up to start reading, turning on fan and diode."""
-        self.set_sleep_state(con.SleepState.WAKE, device_id)
+        self.set_sleep_state(SleepState.WAKE, device_id)
 
-    def safe_wake(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
+    def safe_wake(self, device_id: bytes = ALL_SENSORS) -> None:
         """Wake the device up, if you don't know what mode its in.
 
         This operates as a fire-and-forget, even in query mode.  You shouldn't have to (and can't) query for a response
         after this command.
         """
         self.wake(device_id=device_id)
         # If we were in query mode, this would flush out the response.  If in active mode, this would be return read
         # data, but we don't care.
         self.ser.read(10)
 
     def set_device_id(
-        self, device_id: bytes, target_device_id: bytes = con.ALL_SENSOR_ID
+        self, device_id: bytes, target_device_id: bytes = ALL_SENSORS
     ) -> None:
         """Set the device ID.
 
         Args:
             device_id: The new device ID to set.
             target_device_id: The target device ID to set the new device ID on.
 
         """
         if len(device_id) != 2 or len(target_device_id) != 2:
             raise AttributeError(
                 f"Device ID must be 4 bytes, found {len(device_id)}, and {len(target_device_id)}"
             )
         cmd = (
-            con.Command.SET_DEVICE_ID.value
-            + (b"\x00" * 10)
-            + device_id
-            + target_device_id
+            Command.SET_DEVICE_ID.value + (b"\x00" * 10) + device_id + target_device_id
         )
         self._send_command(cmd)
 
     def query_device_id(self) -> DeviceIdResponse:
         """Retrieve the current device ID.
 
         Returns:
             The current device ID.
 
         """
-        return DeviceIdResponse(self._read_response())
+        return self._parse_device_id_response(self._read_response())
 
-    def request_working_period(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
+    def request_working_period(self, device_id: bytes = ALL_SENSORS) -> None:
         """Submit a request to retrieve the current working period for the device."""
         cmd = (
-            con.Command.SET_WORKING_PERIOD.value
-            + con.OperationType.QUERY.value
+            Command.SET_WORKING_PERIOD.value
+            + OperationType.QUERY.value
             + (b"\x00" * 11)
             + device_id
         )
         self._send_command(cmd)
 
     def query_working_period(self) -> WorkingPeriodReadResponse:
         """Retrieve the current working period for the device.
 
         Returns:
             The current working period set for the device.
 
         """
-        return WorkingPeriodReadResponse(self._read_response())
+        return self._parse_working_period_reponse(self._read_response())
 
     def set_working_period(
-        self, working_period: int, device_id: bytes = con.ALL_SENSOR_ID
+        self, working_period: int, device_id: bytes = ALL_SENSORS
     ) -> None:
         """Set the working period for the device.
 
         Working period must be between 0 and 30.
 
         0 means the device will read continuously.
         Any value 1-30 means the device will wake and read for 30 seconds every n*60-30 seconds.
 
         Args:
             working_period: A value 0-30 to set as the new working period
             device_id: The device ID to set the working period for.
         """
-        if 0 >= working_period >= 30:
+        if working_period < 0 or working_period > 30:
             raise AttributeError("Working period must be between 0 and 30")
         cmd = (
-            con.Command.SET_WORKING_PERIOD.value
-            + con.OperationType.SET_MODE.value
+            Command.SET_WORKING_PERIOD.value
+            + OperationType.SET_MODE.value
             + bytes([working_period])
             + (b"\x00" * 10)
             + device_id
         )
         self._send_command(cmd)
 
-    def request_firmware_version(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
+    def request_firmware_version(self, device_id: bytes = ALL_SENSORS) -> None:
         """Submit a request to retrieve the firmware version from the device."""
-        cmd = con.Command.CHECK_FIRMWARE_VERSION.value + (b"\x00" * 12) + device_id
+        cmd = Command.CHECK_FIRMWARE_VERSION.value + (b"\x00" * 12) + device_id
         self._send_command(cmd)
 
     def query_firmware_version(self) -> CheckFirmwareResponse:
         """Retrieve the firmware version from the device.
 
         Returns:
             The firmware version from the device.
 
         """
-        return CheckFirmwareResponse(self._read_response())
+        return self._parse_firmware_response(self._read_response())
 
     def _send_command(self, cmd: bytes) -> None:
         """Send a command to the device as bytes.
 
         Manages all the wrapper needed to send data to the device, including checksum.
 
         Args:
             cmd: The data payload to send to the device.
 
         Raises:
               AttributeError: If the command length is not equal to 15.
 
         """
-        head = con.HEAD + con.SUBMIT_TYPE
-        full_command = head + cmd + bytes([self._cmd_checksum(cmd)]) + con.TAIL
+        head = HEAD + SUBMIT_TYPE
+        full_command = head + cmd + bytes([self._cmd_checksum(cmd)]) + TAIL
         if len(full_command) != 19:
             raise Exception(f"Command length must be 19, but was {len(full_command)}")
         self.ser.write(full_command)
         time.sleep(self.send_command_sleep)
 
     def _read_response(self) -> bytes:
         """Read a response from the device.
@@ -346,100 +385,235 @@
             An integer checksum of the bytes passed.
 
         """
         if len(data) != 15:
             raise AttributeError("Invalid checksum length.")
         return sum(d for d in data) % 256
 
+    def _parse_read_response(
+        self,
+        data: bytes,
+        command_code: Command,
+        response_type: ResponseType = ResponseType.GENERAL_RESPONSE,
+    ) -> _RawReadResponse:
+        """Parse bytes into a typed read response. Validates as well.
+
+        Args:
+            data: The raw data bytes to parse.  Must be of length 10.
+            command_code: The expected command code for the response.
+            response_type:  The expected response type for the response.
+
+        Returns:
+            A read response object with the parsed data.
+        """
+        if len(data) != 10:
+            raise IncompleteReadException()
+
+        head: bytes = data[0:1]
+        cmd_id: bytes = data[1:2]
+        payload: bytes = data[2:8]
+        device_id: bytes = data[6:8]
+        checksum: int = data[8]
+        tail: bytes = data[9:10]
+        expected_command_code: Command = command_code
+        expected_response_type: ResponseType = response_type
+        result = _RawReadResponse(
+            head=head,
+            cmd_id=cmd_id,
+            payload=payload,
+            device_id=device_id,
+            checksum=checksum,
+            tail=tail,
+            expected_command_code=expected_command_code,
+            expected_response_type=expected_response_type,
+        )
+        self._verify(result)
+        return result
+
+    def _parse_query_response(self, data: bytes) -> QueryResponse:
+        """Parse a query read response."""
+        raw_response = self._parse_read_response(
+            data, Command.QUERY, ResponseType.QUERY_RESPONSE
+        )
+
+        pm25: float = int.from_bytes(raw_response.payload[2:4], byteorder="little") / 10
+        pm10: float = int.from_bytes(raw_response.payload[4:6], byteorder="little") / 10
+        return QueryResponse(pm25=pm25, pm10=pm10, device_id=raw_response.device_id)
+
+    def _parse_reporting_mode_response(self, data: bytes) -> ReportingModeResponse:
+        """Parse a reporting mode response."""
+        raw_response = self._parse_read_response(
+            data, command_code=Command.SET_REPORTING_MODE
+        )
+        operation_type: OperationType = OperationType(raw_response.payload[1:2])
+        state: ReportingMode = ReportingMode(raw_response.payload[2:3])
+        return ReportingModeResponse(operation_type, state)
+
+    def _parse_device_id_response(self, data: bytes) -> DeviceIdResponse:
+        """Parse a device ID response."""
+        raw_response = self._parse_read_response(
+            data, command_code=Command.SET_DEVICE_ID
+        )
+        return DeviceIdResponse(device_id=raw_response.device_id)
+
+    def _parse_sleep_wake_response(self, data: bytes) -> SleepWakeReadResponse:
+        """Parse a sleep/wake response."""
+        raw_response = self._parse_read_response(data, command_code=Command.SET_SLEEP)
+        operation_type: OperationType = OperationType(raw_response.payload[1:2])
+        state: SleepState = SleepState(raw_response.payload[2:3])
+        return SleepWakeReadResponse(operation_type=operation_type, state=state)
+
+    def _parse_working_period_reponse(self, data: bytes) -> WorkingPeriodReadResponse:
+        """Parse a working period response."""
+        raw_response = self._parse_read_response(
+            data, command_code=Command.SET_WORKING_PERIOD
+        )
+        operation_type: OperationType = OperationType(raw_response.payload[1:2])
+        interval: int = raw_response.payload[2]
+        return WorkingPeriodReadResponse(
+            operation_type=operation_type, interval=interval
+        )
+
+    def _parse_firmware_response(self, data: bytes) -> CheckFirmwareResponse:
+        """Parse a firmware response."""
+        raw_response = self._parse_read_response(
+            data, command_code=Command.CHECK_FIRMWARE_VERSION
+        )
+        year: int = raw_response.payload[1]
+        month: int = raw_response.payload[2]
+        day: int = raw_response.payload[3]
+        return CheckFirmwareResponse(year=year, month=month, day=day)
+
+    def _verify(self, read_response: _RawReadResponse) -> None:
+        """Verify read data.
+
+        Args:
+            read_response: The raw read data to verify.
+
+        Raises:
+            IncorrectWrapperException: If the head or tail data is incorrect
+            ChecksumFailedException: If the checksum from the response is incorrect
+            IncorrectCommandException: If the command ID in the response is not the expected one.
+            IncorrectCommandCodeException: If the command code in the response is not the expected one.
+
+        """
+        if read_response.head != HEAD:
+            raise IncorrectWrapperException()
+        if read_response.tail != TAIL:
+            raise IncorrectWrapperException()
+        if read_response.checksum != self._calc_checksum(read_response.payload):
+            raise ChecksumFailedException(
+                expected=read_response.checksum,
+                actual=self._calc_checksum(read_response.payload),
+            )
+        if read_response.cmd_id != read_response.expected_response_type.value:
+            raise IncorrectCommandException(
+                expected=read_response.expected_response_type.value,
+                actual=read_response.cmd_id,
+            )
+
+        # Query responses don't validate the command code
+        if (
+            read_response.expected_response_type != ResponseType.QUERY_RESPONSE
+            and bytes([read_response.payload[0]])
+            != read_response.expected_command_code.value
+        ):
+            raise IncorrectCommandCodeException(
+                expected=read_response.expected_command_code.value,
+                actual=read_response.payload[0:1],
+            )
+
+    def _calc_checksum(self, data: bytes) -> int:
+        """Calculate the checksum for the read data."""
+        return sum(d for d in data) % 256
+
 
 class SDS011QueryReader:
     """Reader working in query mode."""
 
     def __init__(self, ser_dev: Union[str, SerialLike], send_command_sleep: int = 1):
         """Create a reader which operates exclusively in query mode.
 
         Args:
             ser_dev: A path to a serial device, or an instance of serial.Serial.
             send_command_sleep: The number of seconds to sleep after sending a command to the device.
         """
         self.base_reader = SDS011Reader(
             ser_dev=ser_dev, send_command_sleep=send_command_sleep
         )
-        self.base_reader.safe_wake(device_id=con.ALL_SENSOR_ID)
+        self.base_reader.safe_wake(device_id=ALL_SENSORS)
         self.base_reader.set_query_mode()
 
-    def query(self, device_id: bytes = con.ALL_SENSOR_ID) -> QueryResponse:
+    def query(self, device_id: bytes = ALL_SENSORS) -> QueryResponse:
         """Query the device for pollutant data.
 
         Args:
             device_id: The device ID to get pollutant data for.
 
         Returns:
             The latest pollutant data.
 
         """
         self.base_reader.request_data(device_id=device_id)
         return self.base_reader.query_data()
 
     def get_reporting_mode(
-        self, device_id: bytes = con.ALL_SENSOR_ID
+        self, device_id: bytes = ALL_SENSORS
     ) -> ReportingModeResponse:
         """Get the current reporting mode of the device.
 
         Args:
             device_id: The device ID to get the reporting mode for.
 
         Returns:
             The current reporting mode of the device.
 
         """
         self.base_reader.request_reporting_mode(device_id=device_id)
         return self.base_reader.query_reporting_mode()
 
-    def get_sleep_state(
-        self, device_id: bytes = con.ALL_SENSOR_ID
-    ) -> SleepWakeReadResponse:
+    def get_sleep_state(self, device_id: bytes = ALL_SENSORS) -> SleepWakeReadResponse:
         """Get the current sleep state.
 
         Args:
             device_id: The device ID to get the sleep state for.
 
         Returns:
             The current sleep state of the device.
         """
         self.base_reader.request_sleep_state(device_id=device_id)
         return self.base_reader.query_sleep_state()
 
-    def sleep(self, device_id: bytes = con.ALL_SENSOR_ID) -> SleepWakeReadResponse:
+    def sleep(self, device_id: bytes = ALL_SENSORS) -> SleepWakeReadResponse:
         """Put the device to sleep, turning off fan and diode.
 
         Args:
             device_id: The device ID to put to sleep.
 
         Returns:
             The new sleep state of the device.
         """
         self.base_reader.sleep(device_id=device_id)
         return self.base_reader.query_sleep_state()
 
-    def wake(self, device_id: bytes = con.ALL_SENSOR_ID) -> SleepWakeReadResponse:
+    def wake(self, device_id: bytes = ALL_SENSORS) -> SleepWakeReadResponse:
         """Wake the device up to start reading, turning on the fan and diode.
 
         Args:
             device_id: The device ID to wake up.
 
 
         Returns:
             The new sleep state of the device.
         """
         self.base_reader.wake(device_id=device_id)
         return self.base_reader.query_sleep_state()
 
     def set_device_id(
-        self, device_id: bytes, target_device_id: bytes = con.ALL_SENSOR_ID
+        self, device_id: bytes, target_device_id: bytes = ALL_SENSORS
     ) -> DeviceIdResponse:
         """Set the device ID.
 
         Args:
             device_id: The new, 4-byte device ID to set.
             target_device_id: The target device ID.
 
@@ -448,29 +622,29 @@
         """
         self.base_reader.set_device_id(
             device_id=device_id, target_device_id=target_device_id
         )
         return self.base_reader.query_device_id()
 
     def get_working_period(
-        self, device_id: bytes = con.ALL_SENSOR_ID
+        self, device_id: bytes = ALL_SENSORS
     ) -> WorkingPeriodReadResponse:
         """Retrieve the current working period for the device.
 
         Args:
             device_id: The device ID to get the working period for.
 
         Returns:
             A response with the current working period.
         """
         self.base_reader.request_working_period(device_id=device_id)
         return self.base_reader.query_working_period()
 
     def set_working_period(
-        self, working_period: int, device_id: bytes = con.ALL_SENSOR_ID
+        self, working_period: int, device_id: bytes = ALL_SENSORS
     ) -> WorkingPeriodReadResponse:
         """Set the working period for the device.
 
         Working period must be between 0 and 30.
 
         0 means the device will read continuously.
         Any value 1-30 means the device will wake and read for 30 seconds every n*60-30 seconds.
@@ -485,15 +659,15 @@
         """
         self.base_reader.set_working_period(
             working_period=working_period, device_id=device_id
         )
         return self.base_reader.query_working_period()
 
     def get_firmware_version(
-        self, device_id: bytes = con.ALL_SENSOR_ID
+        self, device_id: bytes = ALL_SENSORS
     ) -> CheckFirmwareResponse:
         """Retrieve the firmware version from the device.
 
         Args:
             device_id: The device ID to retrieve firmware version for.
 
         Returns:
@@ -529,54 +703,54 @@
 
         Returns:
             The latest pollutant data.
 
         """
         return self.base_reader.query_data()
 
-    def sleep(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
+    def sleep(self, device_id: bytes = ALL_SENSORS) -> None:
         """Put the device to sleep, turning off fan and diode.
 
         Args:
             device_id: The device ID to put to sleep.
         """
         self.base_reader.sleep(device_id)
 
         # Sleep seems to behave very strangely in active mode.  It continually outputs data for old commands for quite
         # a while before eventually having nothing to report.  This forces it to "drain" whatever it was doing before
         # returning, but also feels quite dangerous.
         while len(self.ser_dev.read(10)) == 10:
             pass
 
-    def wake(self, device_id: bytes = con.ALL_SENSOR_ID) -> None:
+    def wake(self, device_id: bytes = ALL_SENSORS) -> None:
         """Wake the device up to start reading, turning on the fan and diode.
 
         Args:
             device_id: The device ID to wake up.
         """
         self.base_reader.wake(device_id)
         self.ser_dev.read(10)
 
     def set_device_id(
-        self, device_id: bytes, target_device_id: bytes = con.ALL_SENSOR_ID
+        self, device_id: bytes, target_device_id: bytes = ALL_SENSORS
     ) -> None:
         """Set the device ID.
 
         Args:
             device_id: The new, 4-byte device ID to set.
             target_device_id: The target device ID.
 
         Returns:
             A response with the new device ID.
         """
         self.base_reader.set_device_id(device_id, target_device_id)
         self.ser_dev.read(10)
 
     def set_working_period(
-        self, working_period: int, device_id: bytes = con.ALL_SENSOR_ID
+        self, working_period: int, device_id: bytes = ALL_SENSORS
     ) -> None:
         """Set the working period for the device.
 
         Working period must be between 0 and 30.
 
         0 means the device will read continuously.
         Any value 1-30 means the device will wake and read for 30 seconds every n*60-30 seconds.
```

### Comparing `sds011lib-0.2.2/sds011lib/constants.py` & `sds011lib-0.3.0/sds011lib/_constants.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.2.2/sds011lib/exceptions.py` & `sds011lib-0.3.0/sds011lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `sds011lib-0.2.2/PKG-INFO` & `sds011lib-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: sds011lib
-Version: 0.2.2
+Version: 0.3.0
 Summary: SDS011 Library
 Author: Tim Orme
 Author-email: TimothyOrme@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyserial (>=3.5,<4.0)
 Description-Content-Type: text/markdown
 
 # sds011lib
 
+[![PyPI version](https://badge.fury.io/py/sds011lib.svg)](https://badge.fury.io/py/sds011lib)
 ![Main](https://github.com/TimOrme/sds011lib/actions/workflows/main.yml/badge.svg)
+[![Coverage](https://codecov.io/gh/TimOrme/sds011lib/branch/main/graph/badge.svg)](https://codecov.io/gh/TimOrme/sds011lib)
 
 `sds011lib` is a fully-typed, nearly-complete, python 3.8+ library for interacting with the SDS011 Air Quality Sensor.
 
 The SDS011 is a small, low-cost sensor created by www.inovafitness.com, used to measure particulate matter in the air.  It 
 can measure both PM 2.5 and PM10 values simultaneously, and connects to devices over a serial port, or via USB with an
 included adaptor.
```

