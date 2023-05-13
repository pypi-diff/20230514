# Comparing `tmp/aqimon-0.4.0.tar.gz` & `tmp/aqimon-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqimon-0.4.0.tar", max compression
+gzip compressed data, was "aqimon-0.5.0.tar", max compression
```

## Comparing `aqimon-0.4.0.tar` & `aqimon-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-04-26 04:51:03.327597 aqimon-0.4.0/LICENSE
--rw-r--r--   0        0        0     5828 2023-04-26 04:51:03.327597 aqimon-0.4.0/README.md
--rw-r--r--   0        0        0       45 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/__init__.py
--rw-r--r--   0        0        0     2633 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/aqi_common.py
--rw-r--r--   0        0        0     2372 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/config.py
--rw-r--r--   0        0        0     7030 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/database.py
--rw-r--r--   0        0        0      881 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/__init__.py
--rw-r--r--   0        0        0     1712 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/mock.py
--rw-r--r--   0        0        0     2133 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/novapm.py
--rw-r--r--   0        0        0    12441 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/sds011/__init__.py
--rw-r--r--   0        0        0     1511 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/sds011/constants.py
--rw-r--r--   0        0        0     1524 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/sds011/exceptions.py
--rw-r--r--   0        0        0     4082 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/sds011/responses.py
--rw-r--r--   0        0        0     8437 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/server.py
--rw-r--r--   0        0        0     6835 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/android-chrome-192x192.png
--rw-r--r--   0        0        0    20365 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/android-chrome-512x512.png
--rw-r--r--   0        0        0     6288 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/apple-touch-icon.png
--rw-r--r--   0        0        0   452012 2023-04-26 04:51:29.004291 aqimon-0.4.0/aqimon/static/elm.js
--rw-r--r--   0        0        0      351 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/favicon-16x16.png
--rw-r--r--   0        0        0      754 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/favicon.ico
--rw-r--r--   0        0        0     1799 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/images/failing.png
--rw-r--r--   0        0        0     2418 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/images/idle.png
--rw-r--r--   0        0        0     6349 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/images/loading.gif
--rw-r--r--   0        0        0    44088 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/images/warmingup.gif
--rw-r--r--   0        0        0      696 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/index.html
--rw-r--r--   0        0        0     5587 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/templates/index.html
--rw-r--r--   0        0        0      968 2023-04-26 04:51:03.327597 aqimon-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6420 1970-01-01 00:00:00.000000 aqimon-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-13 23:19:48.848806 aqimon-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5905 2023-05-13 23:19:48.848806 aqimon-0.5.0/README.md
+-rw-r--r--   0        0        0       45 2023-05-13 23:19:48.848806 aqimon-0.5.0/aqimon/__init__.py
+-rw-r--r--   0        0        0     2633 2023-05-13 23:19:48.848806 aqimon-0.5.0/aqimon/aqi_common.py
+-rw-r--r--   0        0        0     2372 2023-05-13 23:19:48.848806 aqimon-0.5.0/aqimon/config.py
+-rw-r--r--   0        0        0     7030 2023-05-13 23:19:48.848806 aqimon-0.5.0/aqimon/database.py
+-rw-r--r--   0        0        0      881 2023-05-13 23:19:48.848806 aqimon-0.5.0/aqimon/read/__init__.py
+-rw-r--r--   0        0        0     1712 2023-05-13 23:19:48.848806 aqimon-0.5.0/aqimon/read/mock.py
+-rw-r--r--   0        0        0     2139 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/read/novapm.py
+-rw-r--r--   0        0        0     8437 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/server.py
+-rw-r--r--   0        0        0     6835 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/static/android-chrome-192x192.png
+-rw-r--r--   0        0        0    20365 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/static/android-chrome-512x512.png
+-rw-r--r--   0        0        0     6288 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/static/apple-touch-icon.png
+-rw-r--r--   0        0        0   452012 2023-05-13 23:20:19.745451 aqimon-0.5.0/aqimon/static/elm.js
+-rw-r--r--   0        0        0      351 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/static/favicon-16x16.png
+-rw-r--r--   0        0        0      754 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/static/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/static/favicon.ico
+-rw-r--r--   0        0        0     1799 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/static/images/failing.png
+-rw-r--r--   0        0        0     2418 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/static/images/idle.png
+-rw-r--r--   0        0        0     6349 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/static/images/loading.gif
+-rw-r--r--   0        0        0    44088 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/static/images/warmingup.gif
+-rw-r--r--   0        0        0      696 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/static/index.html
+-rw-r--r--   0        0        0     5587 2023-05-13 23:19:48.852806 aqimon-0.5.0/aqimon/templates/index.html
+-rw-r--r--   0        0        0      989 2023-05-13 23:19:48.852806 aqimon-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6539 1970-01-01 00:00:00.000000 aqimon-0.5.0/PKG-INFO
```

### Comparing `aqimon-0.4.0/LICENSE` & `aqimon-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/README.md` & `aqimon-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # AQIMON
 
 A simple Air Quality Index monitor, designed to work on the Raspberry Pi with the SDS011 Nova PM Sensor.
 
 - [AQIMON](#aqimon)
+  - [Screenshot](#screenshot) 
   - [Installation](#installation)
     - [Pre-Requisites](#pre-requisites)
     - [Install](#install)
   - [Running Aqimon](#running-aqimon)
     - [Configure With Systemd](#configure-with-systemd)
   - [Configuration](#configuration)
   - [Contributing](#contributing)
     - [Toolset](#toolset)
     - [Quickstart](#quickstart)
     - [Using the Mock Reader](#using-the-mock-reader)
     - [Submitting a PR](#submitting-a-pr)
 
+## Screenshot
+
+![Screenshot](screenshot.png)
+
 ## Installation
 
 ### Pre-Requisites
 
 - Python 3.9+
 
 ### Install
```

### Comparing `aqimon-0.4.0/aqimon/aqi_common.py` & `aqimon-0.5.0/aqimon/aqi_common.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/config.py` & `aqimon-0.5.0/aqimon/config.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/database.py` & `aqimon-0.5.0/aqimon/database.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/read/__init__.py` & `aqimon-0.5.0/aqimon/read/__init__.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/read/mock.py` & `aqimon-0.5.0/aqimon/read/mock.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/read/novapm.py` & `aqimon-0.5.0/aqimon/read/novapm.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 https://www.amazon.com/SDS011-Quality-Detection-Conditioning-Monitor/dp/B07FSDMRR5
 """
 import asyncio
 
 from . import AqiRead, ReaderState, ReaderStatus
 import serial
 from typing import Union
-from .sds011 import QueryModeReader
+from sds011lib import SDS011QueryReader
 from statistics import mean
 
 
 class OpinionatedReader:
     """NOVA PM SDS011 Reader."""
 
     def __init__(
@@ -22,15 +22,15 @@
         sleep_time: int = 3,
         command_wait_time: int = 15,
     ):
         """Create the device."""
         if isinstance(ser_dev, str):
             ser_dev = serial.Serial(ser_dev, timeout=2)
 
-        self.reader = QueryModeReader(ser_dev=ser_dev, send_command_sleep=command_wait_time)
+        self.reader = SDS011QueryReader(ser_dev=ser_dev, send_command_sleep=command_wait_time)
 
         # Initial the reader to be in the mode we want.
         self.reader.wake()
         self.reader.set_working_period(0)
 
         self.warm_up_secs = warm_up_secs
         self.iterations = iterations
```

### Comparing `aqimon-0.4.0/aqimon/server.py` & `aqimon-0.5.0/aqimon/server.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/static/android-chrome-192x192.png` & `aqimon-0.5.0/aqimon/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/static/android-chrome-512x512.png` & `aqimon-0.5.0/aqimon/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/static/apple-touch-icon.png` & `aqimon-0.5.0/aqimon/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/static/elm.js` & `aqimon-0.5.0/aqimon/static/elm.js`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/static/favicon-32x32.png` & `aqimon-0.5.0/aqimon/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/static/favicon.ico` & `aqimon-0.5.0/aqimon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/static/images/failing.png` & `aqimon-0.5.0/aqimon/static/images/failing.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/static/images/idle.png` & `aqimon-0.5.0/aqimon/static/images/idle.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/static/images/loading.gif` & `aqimon-0.5.0/aqimon/static/images/loading.gif`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/static/images/warmingup.gif` & `aqimon-0.5.0/aqimon/static/images/warmingup.gif`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/static/index.html` & `aqimon-0.5.0/aqimon/static/index.html`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/aqimon/templates/index.html` & `aqimon-0.5.0/aqimon/templates/index.html`

 * *Files identical despite different names*

### Comparing `aqimon-0.4.0/pyproject.toml` & `aqimon-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "aqimon"
-version = "0.4.0"
+version = "0.5.0"
 description = "Air Quality Index Monitor"
 authors = ["Tim Orme"]
 readme = "README.md"
 include = ["aqimon/static/elm.js"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fastapi = "^0.92.0"
 pyserial = "^3.5"
 uvicorn = "^0.21.0"
 databases = {extras = ["aiosqlite"], version = "^0.7.0"}
 fastapi-utils = "^0.2.1"
+sds011lib = "^0.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.256"
 black = "^23.1.0"
 mypy = "^1.1.1"
 pytest = "^7.3.1"
```

### Comparing `aqimon-0.4.0/PKG-INFO` & `aqimon-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 Metadata-Version: 2.1
 Name: aqimon
-Version: 0.4.0
+Version: 0.5.0
 Summary: Air Quality Index Monitor
 Author: Tim Orme
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: databases[aiosqlite] (>=0.7.0,<0.8.0)
 Requires-Dist: fastapi (>=0.92.0,<0.93.0)
 Requires-Dist: fastapi-utils (>=0.2.1,<0.3.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
+Requires-Dist: sds011lib (>=0.3.0,<0.4.0)
 Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 # AQIMON
 
 A simple Air Quality Index monitor, designed to work on the Raspberry Pi with the SDS011 Nova PM Sensor.
 
 - [AQIMON](#aqimon)
+  - [Screenshot](#screenshot) 
   - [Installation](#installation)
     - [Pre-Requisites](#pre-requisites)
     - [Install](#install)
   - [Running Aqimon](#running-aqimon)
     - [Configure With Systemd](#configure-with-systemd)
   - [Configuration](#configuration)
   - [Contributing](#contributing)
     - [Toolset](#toolset)
     - [Quickstart](#quickstart)
     - [Using the Mock Reader](#using-the-mock-reader)
     - [Submitting a PR](#submitting-a-pr)
 
+## Screenshot
+
+![Screenshot](screenshot.png)
+
 ## Installation
 
 ### Pre-Requisites
 
 - Python 3.9+
 
 ### Install
```

