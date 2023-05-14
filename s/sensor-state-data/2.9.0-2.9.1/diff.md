# Comparing `tmp/sensor-state-data-2.9.0.tar.gz` & `tmp/sensor-state-data-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensor-state-data-2.9.0.tar", max compression
+gzip compressed data, was "sensor-state-data-2.9.1.tar", max compression
```

## Comparing `sensor-state-data-2.9.0.tar` & `sensor-state-data-2.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11345 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/LICENSE
--rw-r--r--   0        0        0     3610 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/README.md
--rw-r--r--   0        0        0     2367 2022-09-30 06:15:15.798010 sensor-state-data-2.9.0/pyproject.toml
--rw-r--r--   0        0        0      853 2022-09-30 06:15:15.754010 sensor-state-data-2.9.0/src/sensor_state_data/__init__.py
--rw-r--r--   0        0        0      136 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/base/__init__.py
--rw-r--r--   0        0        0        0 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/binary_sensor/__init__.py
--rw-r--r--   0        0        0     2311 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/binary_sensor/device_class.py
--rw-r--r--   0        0        0    10581 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/data.py
--rw-r--r--   0        0        0     1243 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/description.py
--rw-r--r--   0        0        0      257 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/device.py
--rw-r--r--   0        0        0      220 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/device_class.py
--rw-r--r--   0        0        0      689 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/enum.py
--rw-r--r--   0        0        0     4820 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/library.py
--rw-r--r--   0        0        0        0 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/py.typed
--rw-r--r--   0        0        0        0 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/sensor/__init__.py
--rw-r--r--   0        0        0     2749 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/sensor/device_class.py
--rw-r--r--   0        0        0     5702 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/units.py
--rw-r--r--   0        0        0      715 2022-09-30 06:15:14.766001 sensor-state-data-2.9.0/src/sensor_state_data/value.py
--rw-r--r--   0        0        0     4605 1970-01-01 00:00:00.000000 sensor-state-data-2.9.0/setup.py
--rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 sensor-state-data-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11345 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/LICENSE
+-rw-r--r--   0        0        0     3610 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/README.md
+-rw-r--r--   0        0        0     2367 2022-10-03 08:48:09.265419 sensor-state-data-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0      853 2022-10-03 08:48:09.217419 sensor-state-data-2.9.1/src/sensor_state_data/__init__.py
+-rw-r--r--   0        0        0      136 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/base/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/binary_sensor/__init__.py
+-rw-r--r--   0        0        0     2311 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/binary_sensor/device_class.py
+-rw-r--r--   0        0        0    10622 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/data.py
+-rw-r--r--   0        0        0     1243 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/description.py
+-rw-r--r--   0        0        0      257 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/device.py
+-rw-r--r--   0        0        0      220 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/device_class.py
+-rw-r--r--   0        0        0      689 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/enum.py
+-rw-r--r--   0        0        0     4820 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/library.py
+-rw-r--r--   0        0        0        0 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/py.typed
+-rw-r--r--   0        0        0        0 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/sensor/__init__.py
+-rw-r--r--   0        0        0     2749 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/sensor/device_class.py
+-rw-r--r--   0        0        0     5702 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/units.py
+-rw-r--r--   0        0        0      750 2022-10-03 08:48:08.185409 sensor-state-data-2.9.1/src/sensor_state_data/value.py
+-rw-r--r--   0        0        0     4605 1970-01-01 00:00:00.000000 sensor-state-data-2.9.1/setup.py
+-rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 sensor-state-data-2.9.1/PKG-INFO
```

### Comparing `sensor-state-data-2.9.0/LICENSE` & `sensor-state-data-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sensor-state-data-2.9.0/README.md` & `sensor-state-data-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sensor-state-data-2.9.0/pyproject.toml` & `sensor-state-data-2.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sensor-state-data"
-version = "2.9.0"
+version = "2.9.1"
 description = "Models for storing and converting Sensor Data state"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/sensor-state-data"
 documentation = "https://sensor-state-data.readthedocs.io"
 classifiers = [
```

### Comparing `sensor-state-data-2.9.0/src/sensor_state_data/__init__.py` & `sensor-state-data-2.9.1/src/sensor_state_data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.9.0"
+__version__ = "2.9.1"
 
 from .base import BaseDeviceClass
 from .binary_sensor.device_class import BinarySensorDeviceClass
 from .data import SensorData, SensorDeviceInfo, SensorUpdate
 from .description import BinarySensorDescription, SensorDescription
 from .device import DeviceKey
 from .device_class import DeviceClass
```

### Comparing `sensor-state-data-2.9.0/src/sensor_state_data/binary_sensor/device_class.py` & `sensor-state-data-2.9.1/src/sensor_state_data/binary_sensor/device_class.py`

 * *Files identical despite different names*

### Comparing `sensor-state-data-2.9.0/src/sensor_state_data/data.py` & `sensor-state-data-2.9.1/src/sensor_state_data/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,19 +286,19 @@
             device_class=device_class,
         )
 
     def fire_event(
         self,
         key: str,
         event_type: str,
-        event_subtype: str | None = None,
+        event_properties: dict[str, str | int | float | None] | None = None,
         name: str | None = None,
         device_id: str | None = None,
     ) -> None:
         """Fire an event."""
         device_key = DeviceKey(key, device_id)
         self._events_updates[device_key] = Event(
             name=name or self._get_key_name(key, device_id),
             device_key=device_key,
             event_type=event_type,
-            event_subtype=event_subtype,
+            event_properties=event_properties,
         )
```

### Comparing `sensor-state-data-2.9.0/src/sensor_state_data/description.py` & `sensor-state-data-2.9.1/src/sensor_state_data/description.py`

 * *Files identical despite different names*

### Comparing `sensor-state-data-2.9.0/src/sensor_state_data/enum.py` & `sensor-state-data-2.9.1/src/sensor_state_data/enum.py`

 * *Files identical despite different names*

### Comparing `sensor-state-data-2.9.0/src/sensor_state_data/library.py` & `sensor-state-data-2.9.1/src/sensor_state_data/library.py`

 * *Files identical despite different names*

### Comparing `sensor-state-data-2.9.0/src/sensor_state_data/sensor/device_class.py` & `sensor-state-data-2.9.1/src/sensor_state_data/sensor/device_class.py`

 * *Files identical despite different names*

### Comparing `sensor-state-data-2.9.0/src/sensor_state_data/units.py` & `sensor-state-data-2.9.1/src/sensor_state_data/units.py`

 * *Files identical despite different names*

### Comparing `sensor-state-data-2.9.0/src/sensor_state_data/value.py` & `sensor-state-data-2.9.1/src/sensor_state_data/value.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 
 
 @dataclass(frozen=True)
 class Event(BaseValue):
     """A class that describes device events."""
 
     event_type: str
-    event_subtype: str | None
+    event_properties: dict[str, str | int | float | None] | None
```

### Comparing `sensor-state-data-2.9.0/setup.py` & `sensor-state-data-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 extras_require = \
 {'docs': ['Sphinx>=5.0,<6.0',
           'sphinx-rtd-theme>=1.0,<2.0',
           'myst-parser>=0.18,<0.19']}
 
 setup_kwargs = {
     'name': 'sensor-state-data',
-    'version': '2.9.0',
+    'version': '2.9.1',
     'description': 'Models for storing and converting Sensor Data state',
     'long_description': '# Sensor State Data\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/sensor-state-data/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bluetooth-devices/sensor-state-data/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://sensor-state-data.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/sensor-state-data.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/sensor-state-data">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/sensor-state-data.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/sensor-state-data/">\n    <img src="https://img.shields.io/pypi/v/sensor-state-data.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/sensor-state-data.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/sensor-state-data.svg?style=flat-square" alt="License">\n</p>\n\nModels for storing and converting Sensor Data state\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install sensor-state-data`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bluetooth-devices/sensor-state-data',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['sensor_state_data', 'sensor_state_data.base',
 'sensor_state_data.binary_sensor', 'sensor_state_data.sensor'] package_data = \
 {'': ['*']} extras_require = \ {'docs': ['Sphinx>=5.0,<6.0', 'sphinx-rtd-
 theme>=1.0,<2.0', 'myst-parser>=0.18,<0.19']} setup_kwargs = { 'name': 'sensor-
-state-data', 'version': '2.9.0', 'description': 'Models for storing and
+state-data', 'version': '2.9.1', 'description': 'Models for storing and
 converting Sensor Data state', 'long_description': '# Sensor State Data\n\n
      \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
                                 percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
```

### Comparing `sensor-state-data-2.9.0/PKG-INFO` & `sensor-state-data-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensor-state-data
-Version: 2.9.0
+Version: 2.9.1
 Summary: Models for storing and converting Sensor Data state
 Home-page: https://github.com/bluetooth-devices/sensor-state-data
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sensor-state-data Version: 2.9.0 Summary: Models
+Metadata-Version: 2.1 Name: sensor-state-data Version: 2.9.1 Summary: Models
 for storing and converting Sensor Data state Home-page: https://github.com/
 bluetooth-devices/sensor-state-data License: Apache Software License 2.0
 Author: J. Nick Koston Author-email: nick@koston.org Requires-Python:
 >=3.9,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

