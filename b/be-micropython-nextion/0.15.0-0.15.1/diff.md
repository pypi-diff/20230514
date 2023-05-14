# Comparing `tmp/be-micropython-nextion-0.15.0.tar.gz` & `tmp/be-micropython-nextion-0.15.1.tar.gz`

## Comparing `be-micropython-nextion-0.15.0.tar` & `be-micropython-nextion-0.15.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-13 11:59:56.000000 be-micropython-nextion-0.15.0/be_micropython_nextion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-13 11:59:56.000000 be-micropython-nextion-0.15.0/be_micropython_nextion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_dual_state_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_gauge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_rtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/nextion_waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-13 11:59:42.000000 be-micropython-nextion-0.15.0/nextion/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-13 11:59:55.000000 be-micropython-nextion-0.15.0/nextion/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-05-14 18:32:49.000000 be-micropython-nextion-0.15.1/be_micropython_nextion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_dual_state_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_rtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/nextion_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-14 18:32:39.000000 be-micropython-nextion-0.15.1/nextion/ulogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-14 18:32:49.000000 be-micropython-nextion-0.15.1/nextion/version.py
```

### Comparing `be-micropython-nextion-0.15.0/be_micropython_nextion.egg-info/PKG-INFO` & `be-micropython-nextion-0.15.1/be_micropython_nextion.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: be-micropython-nextion
-Version: 0.15.0
+Version: 0.15.1
 Summary: MicroPython Nextion serial displays library
 Home-page: https://github.com/brainelectronics/micropython-nextion
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-nextion/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-nextion
@@ -151,38 +151,14 @@
 
 cp nextion/* /pyboard/lib/nextion
 
 cp examples/basic/main.py /pyboard
 cp examples/boot.py /pyboard
 ```
 
-### Install additional MicroPython packages
-
-To use this package with the provided [`boot.py`](examples/boot.py) and one of
-the `main.py` files of an [example subfolder](examples/), the additional
-module `ulogging` is required.
-
-Either install the required package(s) using `upip` as follows after
-connecting to a WiFi network:
-
-```python
-# network connection already established
-
-import upip
-upip.install('micropython-ulogging')
-```
-
-or copy it manually to the MicroPython board using e.g. `rshell`:
-
-```bash
-mkdir /pyboard/lib
-
-cp -r libs_external/* /pyboard/lib
-```
-
 ## Usage
 
 Use one of the [examples](examples/) to get started. Read also the
 [examples README](examples/README.md) to find all supported elements
 
 ## Credits
```

### Comparing `be-micropython-nextion-0.15.0/nextion/__init__.py` & `be-micropython-nextion-0.15.1/nextion/__init__.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/common.py` & `be-micropython-nextion-0.15.1/nextion/common.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/const.py` & `be-micropython-nextion-0.15.1/nextion/const.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_button.py` & `be-micropython-nextion-0.15.1/nextion/nextion_button.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_checkbox.py` & `be-micropython-nextion-0.15.1/nextion/nextion_checkbox.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_dual_state_button.py` & `be-micropython-nextion-0.15.1/nextion/nextion_dual_state_button.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_gauge.py` & `be-micropython-nextion-0.15.1/nextion/nextion_gauge.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_gpio.py` & `be-micropython-nextion-0.15.1/nextion/nextion_gpio.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_hardware.py` & `be-micropython-nextion-0.15.1/nextion/nextion_hardware.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     - sendCommand uses the default timeout, but should use timeout = 0
       https://github.com/micropython/micropython/issues/3434
 """
 
 # system packages
 from machine import UART
 from time import ticks_diff, ticks_ms
-import ulogging as logging
 
 # custom packages
 from .typing import Optional
 from . import const as Const
+from . import ulogging as logging
 
 
 class NexHardwareError(Exception):
     """Base class for exceptions in this module."""
     pass
```

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_number.py` & `be-micropython-nextion-0.15.1/nextion/nextion_number.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_page.py` & `be-micropython-nextion-0.15.1/nextion/nextion_page.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_progressbar.py` & `be-micropython-nextion-0.15.1/nextion/nextion_progressbar.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_radio.py` & `be-micropython-nextion-0.15.1/nextion/nextion_radio.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_rtc.py` & `be-micropython-nextion-0.15.1/nextion/nextion_rtc.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_slider.py` & `be-micropython-nextion-0.15.1/nextion/nextion_slider.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_text.py` & `be-micropython-nextion-0.15.1/nextion/nextion_text.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_upload.py` & `be-micropython-nextion-0.15.1/nextion/nextion_upload.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_variable.py` & `be-micropython-nextion-0.15.1/nextion/nextion_variable.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/nextion_waveform.py` & `be-micropython-nextion-0.15.1/nextion/nextion_waveform.py`

 * *Files identical despite different names*

### Comparing `be-micropython-nextion-0.15.0/nextion/typing.py` & `be-micropython-nextion-0.15.1/nextion/typing.py`

 * *Files identical despite different names*

