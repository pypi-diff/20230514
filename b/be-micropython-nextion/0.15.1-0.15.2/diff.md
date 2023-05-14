# Comparing `tmp/be-micropython-nextion-0.15.1.tar.gz` & `tmp/be-micropython-nextion-0.15.2.tar.gz`

## Comparing `be-micropython-nextion-0.15.1.tar` & `be-micropython-nextion-0.15.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-14 18:32:49.000000 be-micropython-nextion-0.15.1/be_micropython_nextion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_dual_state_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_gauge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_rtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/ulogging.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-14 18:32:49.000000 be-micropython-nextion-0.15.1/nextion/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-14 19:46:00.000000 be-micropython-nextion-0.15.2/be_micropython_nextion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_dual_state_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_rtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/nextion_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-14 19:45:40.000000 be-micropython-nextion-0.15.2/nextion/ulogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-14 19:45:59.000000 be-micropython-nextion-0.15.2/nextion/version.py
```

### Comparing `be-micropython-nextion-0.15.1/be_micropython_nextion.egg-info/PKG-INFO` & `be-micropython-nextion-0.15.2/be_micropython_nextion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: be-micropython-nextion
-Version: 0.15.1
+Version: 0.15.2
 Summary: MicroPython Nextion serial displays library
 Home-page: https://github.com/brainelectronics/micropython-nextion
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-nextion/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-nextion
```

### Comparing `be-micropython-nextion-0.15.1/nextion/__init__.py` & `be-micropython-nextion-0.15.2/nextion/__init__.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/common.py` & `be-micropython-nextion-0.15.2/nextion/common.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/const.py` & `be-micropython-nextion-0.15.2/nextion/const.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_button.py` & `be-micropython-nextion-0.15.2/nextion/nextion_button.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_checkbox.py` & `be-micropython-nextion-0.15.2/nextion/nextion_checkbox.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_dual_state_button.py` & `be-micropython-nextion-0.15.2/nextion/nextion_dual_state_button.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_gauge.py` & `be-micropython-nextion-0.15.2/nextion/nextion_gauge.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_gpio.py` & `be-micropython-nextion-0.15.2/nextion/nextion_gpio.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_hardware.py` & `be-micropython-nextion-0.15.2/nextion/nextion_hardware.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_number.py` & `be-micropython-nextion-0.15.2/nextion/nextion_number.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_page.py` & `be-micropython-nextion-0.15.2/nextion/nextion_page.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_progressbar.py` & `be-micropython-nextion-0.15.2/nextion/nextion_progressbar.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_radio.py` & `be-micropython-nextion-0.15.2/nextion/nextion_radio.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_rtc.py` & `be-micropython-nextion-0.15.2/nextion/nextion_rtc.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,17 @@
                 minute = time[4]
                 second = time[5]
             else:
                 raise NexRtcError("Time can either be given as '{}' or '{}'".
                                   format("2016,11,25,12,34,50",
                                          [2016, 11, 25, 12, 34, 50]))
 
-            self._logger.debug("Timestamp (ISO8601): {}-{}-{}T{}:{}:{}".
-                               format(year, month, day, hour, minute, second))
+            self._nh._logger.debug(
+                "Timestamp (ISO8601): {}-{}-{}T{}:{}:{}".format(
+                    year, month, day, hour, minute, second))
 
             cmd = "rtc0={}".format(year)
             self._nh.sendCommand(cmd)
             self._nh.recvRetCommandFinished()
 
             cmd = "rtc1={}".format(month)
             self._nh.sendCommand(cmd)
@@ -117,15 +118,15 @@
             else:
                 if len(args) == 2:
                     time_type = args[0]
                     time = args[1]
                 else:
                     raise NexRtcError("Either use keyword or positional args")
 
-            self._logger.debug("Set '{}' to '{}'".format(time_type, time))
+            self._nh._logger.debug("Set '{}' to '{}'".format(time_type, time))
             rtc_index = self.time_types.index(time_type.lower())
 
             cmd = "rtc{}={}".format(rtc_index, time)
             self._nh.sendCommand(cmd)
             return self._nh.recvRetCommandFinished()
         else:
             raise NexRtcError("Only two args are allowed")
```

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_slider.py` & `be-micropython-nextion-0.15.2/nextion/nextion_slider.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_text.py` & `be-micropython-nextion-0.15.2/nextion/nextion_text.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_upload.py` & `be-micropython-nextion-0.15.2/nextion/nextion_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,56 +108,56 @@
 
         if not self._setDownloadBaudrate(self.download_baudrate):
             raise NexUploadError("Modify baudrate error")
 
         if not self._downloadTftFile():
             raise NexUploadError("Download file error")
 
-        self._logger.debug("Download ok")
+        self._nh._logger.debug("Download ok")
         return True
 
     def _checkFile(self) -> bool:
         """
         Check existance of specified TFT file
 
         :returns:   True on success, False otherwise
         :rtype:     bool
         """
         result = False
         if self._exists(self.file_name):
             # https://docs.python.org/3/library/os.html#os.stat
             info = stat(self.file_name)
             self.file_size = info[6]
-            self._logger.debug("TFT file size is '{}' bytes".
-                               format(self.file_size))
-            self._logger.debug("File check ok")
+            self._nh._logger.debug("TFT file size is '{}' bytes".
+                                   format(self.file_size))
+            self._nh._logger.debug("File check ok")
             result = True
         else:
-            self._logger.debug("File '{}' does not exist".
-                               format(self.file_name))
+            self._nh._logger.debug("File '{}' does not exist".
+                                   format(self.file_name))
         return result
 
     def _getBaudrate(self) -> int:
         """
         Get communication baudrate with Nextion display
 
         :returns:   The baudrate
         :rtype:     int
         """
         baudrate_array = [115200, 19200, 9600, 57600, 38400, 4800, 2400]
         _baudrate = 0
 
         for baudrate in baudrate_array:
-            self._logger.debug("Checking connection with '{}' baud".
-                               format(baudrate))
+            self._nh._logger.debug("Checking connection with '{}' baud".
+                                   format(baudrate))
 
             if self._searchBaudrate(baudrate):
                 _baudrate = baudrate
-                self._logger.debug("Success, baudrate set to '{}' baud".
-                                   format(_baudrate))
+                self._nh._logger.debug("Success, baudrate set to '{}' baud".
+                                       format(_baudrate))
                 return _baudrate
 
         return _baudrate
 
     def _searchBaudrate(self, baudrate: int) -> bool:
         """
         Find suitable download baudrate
@@ -170,16 +170,16 @@
         """
         self._nh._baudrate = baudrate
         self._nh._uart_init()
         self._nh.sendCommand("")
         self._nh.sendCommand("connect")
         sleep(0.1)  # necessary, data might not be available otherwise
         response = self._recvRetString()
-        self._logger.debug("_searchBaudrate response for '{}' baud: {}".
-                           format(baudrate, response))
+        self._nh._logger.debug("_searchBaudrate response for '{}' baud: {}".
+                               format(baudrate, response))
 
         if "comok" in response:
             return True
 
         return False
 
     def _setDownloadBaudrate(self, baudrate: int) -> bool:
@@ -189,24 +189,24 @@
         :param      baudrate:  The baudrate
         :type       baudrate:  int
 
         :returns:   True on success, False otherwise
         :rtype:     bool
         """
         cmd = "whmi-wri {},{},0".format(self.file_size, baudrate)
-        self._logger.debug("Set download baudrate cmd: '{}'".format(cmd))
+        self._nh._logger.debug("Set download baudrate cmd: '{}'".format(cmd))
 
         self._nh.sendCommand("")
         self._nh.sendCommand(cmd)
         sleep(0.05)
         self._nh._baudrate = baudrate
         self._nh._uart_init()
         response = self._recvRetString(500)
-        self._logger.debug("Set download baudrate response: '{}'".
-                           format(response))
+        self._nh._logger.debug(
+            "Set download baudrate response: '{}'".format(response))
         if (0x05).to_bytes(1, 'little') in response:
             return True
         return False
 
     def _downloadTftFile(self) -> bool:
         """
         Download TFT file to Nextion display
@@ -218,21 +218,21 @@
         file_content = bytearray(4096)
 
         with open(self.file_name, 'rb') as update_file:
             while True:
                 data_size = update_file.readinto(file_content)
 
                 if not data_size:
-                    self._logger.debug("Reached EOF, update finished")
+                    self._nh._logger.debug("Reached EOF, update finished")
                     break
 
                 self._nh._uart.write(file_content)
 
                 response = self._recvRetString(500)
-                # self._logger.debug("File download response: '{}'".
+                # self._nh._logger.debug("File download response: '{}'".
                 #                        format(response))
 
                 if (0x05).to_bytes(1, 'little') in response:
                     # send next chunk
                     pass
                 else:
                     return False
```

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_variable.py` & `be-micropython-nextion-0.15.2/nextion/nextion_variable.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/nextion_waveform.py` & `be-micropython-nextion-0.15.2/nextion/nextion_waveform.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         :param      number:  The value to add
         :type       number:  int
 
         :returns:   True on success, false otherwise
         :rtype:     bool
         """
         if ch > 3:
-            self._logger.debug("Only channels (0-3) supported by waveform")
+            self._nh._logger.debug("Only channels (0-3) supported by waveform")
             return False
 
         cmd = "add {},{},{}".format(self.cid, ch, number)
         self._nh.sendCommand(cmd)
         return True
 
     def clearChannel(self, ch: int) -> bool:
@@ -63,16 +63,16 @@
         :param      ch:   The channel to clear or 255 for all channels
         :type       ch:   int
 
         :returns:   True on success, false otherwise
         :rtype:     bool
         """
         if (ch > 3) and (ch != 255):
-            self._logger.debug("Only the channels (0-3) or all channels at "
-                               "once (255) can be cleared")
+            self._nh._logger.debug("Only the channels (0-3) or all channels "
+                                   "at once (255) can be cleared")
             return False
 
         cmd = "cle {},{}".format(self.cid, ch)
         self._nh.sendCommand(cmd)
         return self._nh.recvRetCommandFinished()
 
     def Get_grid_color_gdc(self) -> int:
```

### Comparing `be-micropython-nextion-0.15.1/nextion/typing.py` & `be-micropython-nextion-0.15.2/nextion/typing.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.1/nextion/ulogging.py` & `be-micropython-nextion-0.15.2/nextion/ulogging.py`

 * *Files identical despite different names*

