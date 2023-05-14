# Comparing `tmp/PyNAU7802-0.2.1.tar.gz` & `tmp/pynau7802-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNAU7802-0.2.1.tar", last modified: Sat Jul 10 01:09:47 2021, max compression
+gzip compressed data, was "pynau7802-0.2.2.tar", max compression
```

## Comparing `PyNAU7802-0.2.1.tar` & `pynau7802-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,7 @@
-drwxrwxr-x   0 busb2601  (1000) busb2601  (1000)        0 2021-07-10 01:09:47.207363 PyNAU7802-0.2.1/
--rw-rw-r--   0 busb2601  (1000) busb2601  (1000)     1067 2021-07-10 00:37:06.000000 PyNAU7802-0.2.1/LICENSE
--rw-rw-r--   0 busb2601  (1000) busb2601  (1000)     1791 2021-07-10 01:09:47.207363 PyNAU7802-0.2.1/PKG-INFO
-drwxrwxr-x   0 busb2601  (1000) busb2601  (1000)        0 2021-07-10 01:09:47.207363 PyNAU7802-0.2.1/PyNAU7802/
--rw-rw-r--   0 busb2601  (1000) busb2601  (1000)    14007 2021-07-10 00:46:43.000000 PyNAU7802-0.2.1/PyNAU7802/NAU7802.py
--rw-rw-r--   0 busb2601  (1000) busb2601  (1000)       29 2021-07-10 00:37:06.000000 PyNAU7802-0.2.1/PyNAU7802/__init__.py
-drwxrwxr-x   0 busb2601  (1000) busb2601  (1000)        0 2021-07-10 01:09:47.207363 PyNAU7802-0.2.1/PyNAU7802.egg-info/
--rw-rw-r--   0 busb2601  (1000) busb2601  (1000)     1791 2021-07-10 01:09:47.000000 PyNAU7802-0.2.1/PyNAU7802.egg-info/PKG-INFO
--rw-rw-r--   0 busb2601  (1000) busb2601  (1000)      233 2021-07-10 01:09:47.000000 PyNAU7802-0.2.1/PyNAU7802.egg-info/SOURCES.txt
--rw-rw-r--   0 busb2601  (1000) busb2601  (1000)        1 2021-07-10 01:09:47.000000 PyNAU7802-0.2.1/PyNAU7802.egg-info/dependency_links.txt
--rw-rw-r--   0 busb2601  (1000) busb2601  (1000)       12 2021-07-10 01:09:47.000000 PyNAU7802-0.2.1/PyNAU7802.egg-info/requires.txt
--rw-rw-r--   0 busb2601  (1000) busb2601  (1000)       10 2021-07-10 01:09:47.000000 PyNAU7802-0.2.1/PyNAU7802.egg-info/top_level.txt
--rw-rw-r--   0 busb2601  (1000) busb2601  (1000)     1338 2021-07-10 00:37:06.000000 PyNAU7802-0.2.1/README.md
--rw-rw-r--   0 busb2601  (1000) busb2601  (1000)       38 2021-07-10 01:09:47.207363 PyNAU7802-0.2.1/setup.cfg
--rw-rw-r--   0 busb2601  (1000) busb2601  (1000)      664 2021-07-10 01:09:35.000000 PyNAU7802-0.2.1/setup.py
+-rw-r--r--   0        0        0     1088 2023-05-13 21:54:55.925358 pynau7802-0.2.2/LICENSE
+-rw-r--r--   0        0        0       56 2023-05-13 22:39:35.319192 pynau7802-0.2.2/PyNAU7802/__init__.py
+-rw-r--r--   0        0        0     2624 2023-05-13 22:37:16.467008 pynau7802-0.2.2/PyNAU7802/constants.py
+-rw-r--r--   0        0        0    11799 2023-05-13 22:39:35.303234 pynau7802-0.2.2/PyNAU7802/nau7802.py
+-rw-r--r--   0        0        0      500 2023-05-13 22:52:14.497864 pynau7802-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1464 2023-05-13 22:37:01.867173 pynau7802-0.2.2/README.md
+-rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 pynau7802-0.2.2/PKG-INFO
```

### Comparing `PyNAU7802-0.2.1/PKG-INFO` & `pynau7802-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
-Name: PyNAU7802
-Version: 0.2.1
+Name: pynau7802
+Version: 0.2.2
 Summary: Python port of the SparkFun Qwiic Scale NAU7802 Arduino Library
-Home-page: https://github.com/BrunoB81HK/PyNAU7802.git
+License: MIT
 Author: Bruno-Pier Busque
-Author-email: bruno-pier.busque@usherbrooke.ca
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Author-email: bruno.hockey.13@hotmail.com
+Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: smbus2 (>=0.4.2,<0.5.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # PyNAU7802
 Python port of the [SparkFun Qwiic Scale NAU7802 Arduino Library](https://github.com/sparkfun/SparkFun_Qwiic_Scale_NAU7802_Arduino_Library)
 
 ## Install
 
 To install, simply use : `pip install PyNAU7802` in a terminal window
 
 ## How to use
 
 The function name and arguments are the exact same as the original library, use it's 
 [documentation](https://github.com/sparkfun/SparkFun_Qwiic_Scale_NAU7802_Arduino_Library)
 to get started.
 
-## Example
+## Examples
+
+Multiple examples are available in the [`examples/`](/examples) directory.
 
 This package use smbus2 as the I2C bus. Here is a small working example :
 
 ```python
 import PyNAU7802
 import smbus2
 
@@ -56,8 +62,7 @@
 print("Calculating the calibration factor...")
 scale.calculateCalibrationFactor(cal)
 print("The calibration factor is : {0:0.3f}\n".format(scale.getCalibrationFactor()))
 
 input("Press [Enter] to measure a mass. ")
 print("Mass is {0:0.3f} kg".format(scale.getWeight()))
 ```
-
```

### Comparing `PyNAU7802-0.2.1/README.md` & `pynau7802-0.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-# PyNAU7802
-Python port of the [SparkFun Qwiic Scale NAU7802 Arduino Library](https://github.com/sparkfun/SparkFun_Qwiic_Scale_NAU7802_Arduino_Library)
-
-## Install
-
-To install, simply use : `pip install PyNAU7802` in a terminal window
-
-## How to use
-
-The function name and arguments are the exact same as the original library, use it's 
-[documentation](https://github.com/sparkfun/SparkFun_Qwiic_Scale_NAU7802_Arduino_Library)
-to get started.
-
-## Example
-
-This package use smbus2 as the I2C bus. Here is a small working example :
-
-```python
-import PyNAU7802
-import smbus2
-
-# Create the bus
-bus = smbus2.SMBus(1)
-
-# Create the scale and initialize it
-scale = PyNAU7802.NAU7802()
-if scale.begin(bus):
-    print("Connected!\n")
-else:
-    print("Can't find the scale, exiting ...\n")
-    exit()
-
-# Calculate the zero offset
-print("Calculating the zero offset...")
-scale.calculateZeroOffset()
-print("The zero offset is : {0}\n".format(scale.getZeroOffset()))
-
-print("Put a known mass on the scale.")
-cal = float(input("Mass in kg? "))
-
-# Calculate the calibration factor
-print("Calculating the calibration factor...")
-scale.calculateCalibrationFactor(cal)
-print("The calibration factor is : {0:0.3f}\n".format(scale.getCalibrationFactor()))
-
-input("Press [Enter] to measure a mass. ")
-print("Mass is {0:0.3f} kg".format(scale.getWeight()))
+# PyNAU7802
+Python port of the [SparkFun Qwiic Scale NAU7802 Arduino Library](https://github.com/sparkfun/SparkFun_Qwiic_Scale_NAU7802_Arduino_Library)
+
+## Install
+
+To install, simply use : `pip install PyNAU7802` in a terminal window
+
+## How to use
+
+The function name and arguments are the exact same as the original library, use it's 
+[documentation](https://github.com/sparkfun/SparkFun_Qwiic_Scale_NAU7802_Arduino_Library)
+to get started.
+
+## Examples
+
+Multiple examples are available in the [`examples/`](/examples) directory.
+
+This package use smbus2 as the I2C bus. Here is a small working example :
+
+```python
+import PyNAU7802
+import smbus2
+
+# Create the bus
+bus = smbus2.SMBus(1)
+
+# Create the scale and initialize it
+scale = PyNAU7802.NAU7802()
+if scale.begin(bus):
+    print("Connected!\n")
+else:
+    print("Can't find the scale, exiting ...\n")
+    exit()
+
+# Calculate the zero offset
+print("Calculating the zero offset...")
+scale.calculateZeroOffset()
+print("The zero offset is : {0}\n".format(scale.getZeroOffset()))
+
+print("Put a known mass on the scale.")
+cal = float(input("Mass in kg? "))
+
+# Calculate the calibration factor
+print("Calculating the calibration factor...")
+scale.calculateCalibrationFactor(cal)
+print("The calibration factor is : {0:0.3f}\n".format(scale.getCalibrationFactor()))
+
+input("Press [Enter] to measure a mass. ")
+print("Mass is {0:0.3f} kg".format(scale.getWeight()))
 ```
```

