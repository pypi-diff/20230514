# Comparing `tmp/SimpleStereo-1.0.5.1.tar.gz` & `tmp/SimpleStereo-1.0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleStereo-1.0.5.1.tar", last modified: Sun Jan 22 15:15:38 2023, max compression
+gzip compressed data, was "SimpleStereo-1.0.6.0.tar", last modified: Sun May 14 13:52:18 2023, max compression
```

## Comparing `SimpleStereo-1.0.5.1.tar` & `SimpleStereo-1.0.6.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 decadenza  (1000) decadenza  (1000)        0 2023-01-22 15:15:38.375230 SimpleStereo-1.0.5.1/
--rw-r--r--   0 decadenza  (1000) decadenza  (1000)    35149 2022-02-09 11:03:56.000000 SimpleStereo-1.0.5.1/LICENSE
--rw-r--r--   0 decadenza  (1000) decadenza  (1000)       31 2022-03-11 19:03:13.000000 SimpleStereo-1.0.5.1/MANIFEST.in
--rw-r--r--   0 decadenza  (1000) decadenza  (1000)     3929 2023-01-22 15:15:38.375230 SimpleStereo-1.0.5.1/PKG-INFO
--rwxr-xr-x   0 decadenza  (1000) decadenza  (1000)     3648 2023-01-22 14:29:12.000000 SimpleStereo-1.0.5.1/README.md
-drwxr-xr-x   0 decadenza  (1000) decadenza  (1000)        0 2023-01-22 15:15:38.375230 SimpleStereo-1.0.5.1/SimpleStereo.egg-info/
--rw-r--r--   0 decadenza  (1000) decadenza  (1000)     3929 2023-01-22 15:15:38.000000 SimpleStereo-1.0.5.1/SimpleStereo.egg-info/PKG-INFO
--rw-r--r--   0 decadenza  (1000) decadenza  (1000)      560 2023-01-22 15:15:38.000000 SimpleStereo-1.0.5.1/SimpleStereo.egg-info/SOURCES.txt
--rw-r--r--   0 decadenza  (1000) decadenza  (1000)        1 2023-01-22 15:15:38.000000 SimpleStereo-1.0.5.1/SimpleStereo.egg-info/dependency_links.txt
--rw-r--r--   0 decadenza  (1000) decadenza  (1000)       72 2023-01-22 15:15:38.000000 SimpleStereo-1.0.5.1/SimpleStereo.egg-info/requires.txt
--rw-r--r--   0 decadenza  (1000) decadenza  (1000)       13 2023-01-22 15:15:38.000000 SimpleStereo-1.0.5.1/SimpleStereo.egg-info/top_level.txt
--rw-r--r--   0 decadenza  (1000) decadenza  (1000)      355 2023-01-22 15:15:38.375230 SimpleStereo-1.0.5.1/setup.cfg
--rwxr-xr-x   0 decadenza  (1000) decadenza  (1000)     1280 2022-03-11 19:03:13.000000 SimpleStereo-1.0.5.1/setup.py
-drwxr-xr-x   0 decadenza  (1000) decadenza  (1000)        0 2023-01-22 15:15:38.375230 SimpleStereo-1.0.5.1/simplestereo/
--rwxr-xr-x   0 decadenza  (1000) decadenza  (1000)    28032 2023-01-22 15:06:23.000000 SimpleStereo-1.0.5.1/simplestereo/__init__.py
--rwxrwxrwx   0 decadenza  (1000) decadenza  (1000)    33954 2021-09-30 10:08:54.000000 SimpleStereo-1.0.5.1/simplestereo/_passive.cpp
--rwxrwxrwx   0 decadenza  (1000) decadenza  (1000)     5071 2021-09-30 10:06:43.000000 SimpleStereo-1.0.5.1/simplestereo/_unwrapping.cpp
--rwxr-xr-x   0 decadenza  (1000) decadenza  (1000)    81796 2023-01-22 10:39:20.000000 SimpleStereo-1.0.5.1/simplestereo/active.py
--rwxr-xr-x   0 decadenza  (1000) decadenza  (1000)    43400 2022-11-07 12:14:19.000000 SimpleStereo-1.0.5.1/simplestereo/calibration.py
-drwxr-xr-x   0 decadenza  (1000) decadenza  (1000)        0 2023-01-22 15:15:38.375230 SimpleStereo-1.0.5.1/simplestereo/headers/
--rwxrwxrwx   0 decadenza  (1000) decadenza  (1000)     2851 2020-07-13 08:16:00.000000 SimpleStereo-1.0.5.1/simplestereo/headers/colorconversion.hpp
--rwxrwxrwx   0 decadenza  (1000) decadenza  (1000)     8316 2020-07-13 08:16:00.000000 SimpleStereo-1.0.5.1/simplestereo/headers/safequeue.hpp
--rwxrwxrwx   0 decadenza  (1000) decadenza  (1000)     6022 2022-02-15 11:37:36.000000 SimpleStereo-1.0.5.1/simplestereo/passive.py
--rwxrwxrwx   0 decadenza  (1000) decadenza  (1000)     7142 2022-03-05 17:00:45.000000 SimpleStereo-1.0.5.1/simplestereo/points.py
--rwxr-xr-x   0 decadenza  (1000) decadenza  (1000)    27685 2022-11-07 12:14:45.000000 SimpleStereo-1.0.5.1/simplestereo/rectification.py
--rwxrwxrwx   0 decadenza  (1000) decadenza  (1000)      980 2022-02-15 11:17:33.000000 SimpleStereo-1.0.5.1/simplestereo/unwrapping.py
--rwxr-xr-x   0 decadenza  (1000) decadenza  (1000)    10057 2023-01-22 10:13:54.000000 SimpleStereo-1.0.5.1/simplestereo/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 13:52:18.567644 SimpleStereo-1.0.6.0/
+-rw-r--r--   0 root         (0) root         (0)    35149 2022-02-09 11:03:56.000000 SimpleStereo-1.0.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       31 2022-03-11 19:03:13.000000 SimpleStereo-1.0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4947 2023-05-14 13:52:18.567644 SimpleStereo-1.0.6.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     4666 2023-05-14 10:29:33.000000 SimpleStereo-1.0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 13:52:18.563645 SimpleStereo-1.0.6.0/SimpleStereo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4947 2023-05-14 13:52:18.000000 SimpleStereo-1.0.6.0/SimpleStereo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-14 13:52:18.000000 SimpleStereo-1.0.6.0/SimpleStereo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 13:52:18.000000 SimpleStereo-1.0.6.0/SimpleStereo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-05-14 13:52:18.000000 SimpleStereo-1.0.6.0/SimpleStereo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-14 13:52:18.000000 SimpleStereo-1.0.6.0/SimpleStereo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-14 13:52:18.567644 SimpleStereo-1.0.6.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1280 2023-04-15 20:10:49.000000 SimpleStereo-1.0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 13:52:18.567644 SimpleStereo-1.0.6.0/simplestereo/
+-rwxr-xr-x   0 root         (0) root         (0)      568 2023-01-29 12:46:16.000000 SimpleStereo-1.0.6.0/simplestereo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    33997 2023-05-14 11:40:11.000000 SimpleStereo-1.0.6.0/simplestereo/_passive.cpp
+-rw-r--r--   0 root         (0) root         (0)    27660 2023-04-15 20:35:18.000000 SimpleStereo-1.0.6.0/simplestereo/_rigs.py
+-rwxrwxrwx   0 root         (0) root         (0)     5176 2023-05-14 13:47:52.000000 SimpleStereo-1.0.6.0/simplestereo/_unwrapping.cpp
+-rwxr-xr-x   0 root         (0) root         (0)    81796 2023-01-22 10:39:20.000000 SimpleStereo-1.0.6.0/simplestereo/active.py
+-rwxr-xr-x   0 root         (0) root         (0)    43127 2023-01-29 12:30:14.000000 SimpleStereo-1.0.6.0/simplestereo/calibration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 13:52:18.567644 SimpleStereo-1.0.6.0/simplestereo/headers/
+-rwxrwxrwx   0 root         (0) root         (0)     2851 2020-07-13 08:16:00.000000 SimpleStereo-1.0.6.0/simplestereo/headers/colorconversion.hpp
+-rwxrwxrwx   0 root         (0) root         (0)     8316 2020-07-13 08:16:00.000000 SimpleStereo-1.0.6.0/simplestereo/headers/safequeue.hpp
+-rwxrwxrwx   0 root         (0) root         (0)     6022 2022-02-15 11:37:36.000000 SimpleStereo-1.0.6.0/simplestereo/passive.py
+-rwxrwxrwx   0 root         (0) root         (0)     7142 2022-03-05 17:00:45.000000 SimpleStereo-1.0.6.0/simplestereo/points.py
+-rwxr-xr-x   0 root         (0) root         (0)    27685 2022-11-07 12:14:45.000000 SimpleStereo-1.0.6.0/simplestereo/rectification.py
+-rwxrwxrwx   0 root         (0) root         (0)      980 2022-02-15 11:17:33.000000 SimpleStereo-1.0.6.0/simplestereo/unwrapping.py
+-rwxr-xr-x   0 root         (0) root         (0)    10577 2023-01-29 12:30:14.000000 SimpleStereo-1.0.6.0/simplestereo/utils.py
```

### Comparing `SimpleStereo-1.0.5.1/LICENSE` & `SimpleStereo-1.0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpleStereo-1.0.5.1/PKG-INFO` & `SimpleStereo-1.0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleStereo
-Version: 1.0.5.1
+Version: 1.0.6.0
 Summary: Stereo vision made simple
 Home-page: http://github.com/decadenza/SimpleStereo
 Author: Pasquale Lafiosca
 License: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,26 +18,38 @@
 * Python 3 (tested with 3.9.2)
 * NumPy
 * SciPy
 * OpenCV
 * matplotlib (for data visualisation)
 
 ## Installation
+
+Before starting, be sure to have the latest `setuptools` package by running `pip install --upgrade setuptools`. Then proceed with one of the two options below.
+
 ### Option 1
 Install package from [PyPI](https://pypi.org/project/SimpleStereo/) with:
 ```
 pip3 install simplestereo
 ```
 
 ### Option 2
 Clone or download the latest version and unzip. Then, from the folder containing `setup.py`, run:
 ```
 pip3 install .
 ```
 
+### Windows users troubleshooting
+
+If during installation you get, together with other messages, the following error:
+```
+error: Microsoft Visual C++ 14.0 or greater is required. Get it with "Microsoft C++ Build Tools": https://visualstudio.microsoft.com/visual-cpp-build-tools/
+```
+Please install the Microsoft C++ Build Tools as indicated. These are required to build C++ extensions that are part of SimpleStereo.
+More information about compiling on Windows is available at [https://wiki.python.org/moin/WindowsCompilers](https://wiki.python.org/moin/WindowsCompilers).
+
 ## Basic example
 SimpleStereo helps you with common tasks. You can calibrate two cameras and initialise a `stereoRig` with:
 
 ```python
 import simplestereo as ss
 
 # Path to your images
@@ -56,15 +68,15 @@
 
 # Optionally print some info
 print("Reprojection error:", rig.reprojectionError)
 print("Centers:", rig.getCenters())
 print("Baseline:", rig.getBaseline())
 ```
     
-More advanced examples available in the [examples](https://github.com/decadenza/SimpleStereo/tree/master/examples) folder.
+More examples available in the [examples](https://github.com/decadenza/SimpleStereo/tree/master/examples) folder.
 
 ## Features and Future Work
 
 ### General
 * `StereoRig`, `RectifiedStereoRig` and `StructuredLightRig` classes to easily manage your stereo rigs and their calibration
 * Basic stereo capture using OpenCV `cv2.videoCapture`
 * Export and import point cloud to PLY file
@@ -90,10 +102,25 @@
 - [ ] De Brujin
 - [ ] Adapt structured light algorithms to work with two cameras
 - [x] StereoFTP (Lafiosca P. et al., [Automated Aircraft Dent Inspection via a Modified Fourier Transform Profilometry Algorithm](https://doi.org/10.3390/s22020433), Sensors, 2022)
 
 ### Unwrapping algorithms
 - [x] Infinite impulse response (Estrada et al., [Noise robust linear dynamic system for phase unwrapping and smoothing](https://doi.org/10.1364/OE.19.005126), Optics Express, 2011) 
 
+## Documentation
+Documentation follows [numpydoc style guide](https://numpydoc.readthedocs.io/en/latest/format.html).
+
+Install documentation prerequisites with:
+```
+pip install Sphinx numpydoc
+```
+
+Build documentation with:
+```
+cd sphinx-documentation-generator
+sh BUILD_SCRIPT.sh
+cd ..
+```
+
 ## Contributions
 Reporting issues and proposing integrations of other stereo vision algorithms is highly encouraged and it will be acknowledged.
 Please share your issues!
```

### Comparing `SimpleStereo-1.0.5.1/README.md` & `SimpleStereo-1.0.6.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -8,26 +8,38 @@
 * Python 3 (tested with 3.9.2)
 * NumPy
 * SciPy
 * OpenCV
 * matplotlib (for data visualisation)
 
 ## Installation
+
+Before starting, be sure to have the latest `setuptools` package by running `pip install --upgrade setuptools`. Then proceed with one of the two options below.
+
 ### Option 1
 Install package from [PyPI](https://pypi.org/project/SimpleStereo/) with:
 ```
 pip3 install simplestereo
 ```
 
 ### Option 2
 Clone or download the latest version and unzip. Then, from the folder containing `setup.py`, run:
 ```
 pip3 install .
 ```
 
+### Windows users troubleshooting
+
+If during installation you get, together with other messages, the following error:
+```
+error: Microsoft Visual C++ 14.0 or greater is required. Get it with "Microsoft C++ Build Tools": https://visualstudio.microsoft.com/visual-cpp-build-tools/
+```
+Please install the Microsoft C++ Build Tools as indicated. These are required to build C++ extensions that are part of SimpleStereo.
+More information about compiling on Windows is available at [https://wiki.python.org/moin/WindowsCompilers](https://wiki.python.org/moin/WindowsCompilers).
+
 ## Basic example
 SimpleStereo helps you with common tasks. You can calibrate two cameras and initialise a `stereoRig` with:
 
 ```python
 import simplestereo as ss
 
 # Path to your images
@@ -46,15 +58,15 @@
 
 # Optionally print some info
 print("Reprojection error:", rig.reprojectionError)
 print("Centers:", rig.getCenters())
 print("Baseline:", rig.getBaseline())
 ```
     
-More advanced examples available in the [examples](https://github.com/decadenza/SimpleStereo/tree/master/examples) folder.
+More examples available in the [examples](https://github.com/decadenza/SimpleStereo/tree/master/examples) folder.
 
 ## Features and Future Work
 
 ### General
 * `StereoRig`, `RectifiedStereoRig` and `StructuredLightRig` classes to easily manage your stereo rigs and their calibration
 * Basic stereo capture using OpenCV `cv2.videoCapture`
 * Export and import point cloud to PLY file
@@ -80,10 +92,25 @@
 - [ ] De Brujin
 - [ ] Adapt structured light algorithms to work with two cameras
 - [x] StereoFTP (Lafiosca P. et al., [Automated Aircraft Dent Inspection via a Modified Fourier Transform Profilometry Algorithm](https://doi.org/10.3390/s22020433), Sensors, 2022)
 
 ### Unwrapping algorithms
 - [x] Infinite impulse response (Estrada et al., [Noise robust linear dynamic system for phase unwrapping and smoothing](https://doi.org/10.1364/OE.19.005126), Optics Express, 2011) 
 
+## Documentation
+Documentation follows [numpydoc style guide](https://numpydoc.readthedocs.io/en/latest/format.html).
+
+Install documentation prerequisites with:
+```
+pip install Sphinx numpydoc
+```
+
+Build documentation with:
+```
+cd sphinx-documentation-generator
+sh BUILD_SCRIPT.sh
+cd ..
+```
+
 ## Contributions
 Reporting issues and proposing integrations of other stereo vision algorithms is highly encouraged and it will be acknowledged.
 Please share your issues!
```

### Comparing `SimpleStereo-1.0.5.1/SimpleStereo.egg-info/PKG-INFO` & `SimpleStereo-1.0.6.0/SimpleStereo.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleStereo
-Version: 1.0.5.1
+Version: 1.0.6.0
 Summary: Stereo vision made simple
 Home-page: http://github.com/decadenza/SimpleStereo
 Author: Pasquale Lafiosca
 License: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,26 +18,38 @@
 * Python 3 (tested with 3.9.2)
 * NumPy
 * SciPy
 * OpenCV
 * matplotlib (for data visualisation)
 
 ## Installation
+
+Before starting, be sure to have the latest `setuptools` package by running `pip install --upgrade setuptools`. Then proceed with one of the two options below.
+
 ### Option 1
 Install package from [PyPI](https://pypi.org/project/SimpleStereo/) with:
 ```
 pip3 install simplestereo
 ```
 
 ### Option 2
 Clone or download the latest version and unzip. Then, from the folder containing `setup.py`, run:
 ```
 pip3 install .
 ```
 
+### Windows users troubleshooting
+
+If during installation you get, together with other messages, the following error:
+```
+error: Microsoft Visual C++ 14.0 or greater is required. Get it with "Microsoft C++ Build Tools": https://visualstudio.microsoft.com/visual-cpp-build-tools/
+```
+Please install the Microsoft C++ Build Tools as indicated. These are required to build C++ extensions that are part of SimpleStereo.
+More information about compiling on Windows is available at [https://wiki.python.org/moin/WindowsCompilers](https://wiki.python.org/moin/WindowsCompilers).
+
 ## Basic example
 SimpleStereo helps you with common tasks. You can calibrate two cameras and initialise a `stereoRig` with:
 
 ```python
 import simplestereo as ss
 
 # Path to your images
@@ -56,15 +68,15 @@
 
 # Optionally print some info
 print("Reprojection error:", rig.reprojectionError)
 print("Centers:", rig.getCenters())
 print("Baseline:", rig.getBaseline())
 ```
     
-More advanced examples available in the [examples](https://github.com/decadenza/SimpleStereo/tree/master/examples) folder.
+More examples available in the [examples](https://github.com/decadenza/SimpleStereo/tree/master/examples) folder.
 
 ## Features and Future Work
 
 ### General
 * `StereoRig`, `RectifiedStereoRig` and `StructuredLightRig` classes to easily manage your stereo rigs and their calibration
 * Basic stereo capture using OpenCV `cv2.videoCapture`
 * Export and import point cloud to PLY file
@@ -90,10 +102,25 @@
 - [ ] De Brujin
 - [ ] Adapt structured light algorithms to work with two cameras
 - [x] StereoFTP (Lafiosca P. et al., [Automated Aircraft Dent Inspection via a Modified Fourier Transform Profilometry Algorithm](https://doi.org/10.3390/s22020433), Sensors, 2022)
 
 ### Unwrapping algorithms
 - [x] Infinite impulse response (Estrada et al., [Noise robust linear dynamic system for phase unwrapping and smoothing](https://doi.org/10.1364/OE.19.005126), Optics Express, 2011) 
 
+## Documentation
+Documentation follows [numpydoc style guide](https://numpydoc.readthedocs.io/en/latest/format.html).
+
+Install documentation prerequisites with:
+```
+pip install Sphinx numpydoc
+```
+
+Build documentation with:
+```
+cd sphinx-documentation-generator
+sh BUILD_SCRIPT.sh
+cd ..
+```
+
 ## Contributions
 Reporting issues and proposing integrations of other stereo vision algorithms is highly encouraged and it will be acknowledged.
 Please share your issues!
```

### Comparing `SimpleStereo-1.0.5.1/SimpleStereo.egg-info/SOURCES.txt` & `SimpleStereo-1.0.6.0/SimpleStereo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 SimpleStereo.egg-info/PKG-INFO
 SimpleStereo.egg-info/SOURCES.txt
 SimpleStereo.egg-info/dependency_links.txt
 SimpleStereo.egg-info/requires.txt
 SimpleStereo.egg-info/top_level.txt
 simplestereo/__init__.py
 simplestereo/_passive.cpp
+simplestereo/_rigs.py
 simplestereo/_unwrapping.cpp
 simplestereo/active.py
 simplestereo/calibration.py
 simplestereo/passive.py
 simplestereo/points.py
 simplestereo/rectification.py
 simplestereo/unwrapping.py
```

### Comparing `SimpleStereo-1.0.5.1/setup.py` & `SimpleStereo-1.0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `SimpleStereo-1.0.5.1/simplestereo/__init__.py` & `SimpleStereo-1.0.6.0/simplestereo/_rigs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 """
-simplestereo
-============
-Common classes and functions.
+_rigs
+=====
 
+Main classes loaded at package level.
+
+See :py:module:`__init__.py`.
 
-Documentation DOCSTRING follows numpy-style wherever possible.
-See https://numpydoc.readthedocs.io/en/latest/format.html
 
 .. todo::
     - Add new rig class for uncalibrated stereo.
 """
+
 import json
 import numpy as np
 import cv2
 
-from . import calibration
 from . import rectification
-from . import passive
-from . import active
-from . import unwrapping
-from . import points
 from . import utils
 
 
-### VERSION INFO
-import pkg_resources # part of setuptools
-__version__ = pkg_resources.require("SimpleStereo")[0].version
-
-
 class StereoRig:
     """ 
     Keep together and manage all parameters of a calibrated stereo rig.
     
     The essential E and fundamental F matrices are optional as they are not always available.
     They may be computed from camera parameters, if needed.
         
@@ -440,15 +431,14 @@
         distCoeffs1 = data.get('distCoeffs1')
         distCoeffs2 = data.get('distCoeffs2')
         F = data.get('F')
         E = data.get('E')
         reprojectionError = data.get('reprojectionError')
         
         return cls(Rcommon, rectHomography1, rectHomography2, res1, res2, intrinsic1, intrinsic2, distCoeffs1, distCoeffs2, R, T, F, E, reprojectionError)
-    
         
     def save(self, filepath):
         """
         Save configuration to JSON file.
         
         Save the current stereo rig configuration to a JSON file that can be loaded later.
         
@@ -474,15 +464,14 @@
                 out['F'] = self.F.tolist()
             if self.E is not None:
                 out['E'] = self.E.tolist()
             if self.reprojectionError:
                 out['reprojectionError'] = self.reprojectionError
             json.dump(out, f, indent=4)
     
-    
     def getRectifiedProjectionMatrices(self):
         """
         Calculate the projection matrices of camera 1 and camera 2 after rectification.
         
         New projection matrices, after rectification, share the same orientation `Rcommon`,
         have only one horizontal displacement (the baseline) and
         have new intrinsics that depends on all the rigid manipulation done after rectification.
@@ -495,15 +484,14 @@
             The 3x4 projection matrix of the second camera.
         """
         C1, C2 = self.getCenters()
         P1 = self.K1.dot(self.Rcommon).dot( np.hstack( (np.eye(3), -C1[:,None]) ) )
         P2 = self.K2.dot(self.Rcommon).dot( np.hstack( (np.eye(3), -C2[:,None]) ) )
         return P1, P2  
     
-    
     def computeRectificationMaps(self, destDims=None, alpha=1):
         """
         Compute the two maps to undistort and rectify the stereo pair.
         
         This method wraps ``cv2.initUndistortRectifyMap()`` plus a custom fitting algorithm to keep image within dimensions. 
         It modifies the original camera matrix applying affine transformations (x-y scale and translation, shear (x axis only)) 
         without losing rectification. The two new maps are stored internally.
@@ -548,15 +536,14 @@
         R1 = self.Rcommon
         R2 = self.Rcommon.dot(self.R.T)
         
         # Recompute final maps considering fitting transformations too
         self.mapx1, self.mapy1 = cv2.initUndistortRectifyMap(self.intrinsic1, self.distCoeffs1, R1, self.K1, destDims, cv2.CV_32FC1)
         self.mapx2, self.mapy2 = cv2.initUndistortRectifyMap(self.intrinsic2, self.distCoeffs2, R2, self.K2, destDims, cv2.CV_32FC1)
         
-        
     def rectifyImages(self, img1, img2, interpolation=cv2.INTER_LINEAR):
         """
         Undistort, rectify and apply affine transformation to a couple of images coming from the stereo rig.
         
         *img1* and *img2* must be provided as in calibration (es. img1 is the left image, img2 the right one).
         This method is wraps ``cv2.remap()`` for two images of the stereo pair. The maps used are computed by
         :meth:`computeRectificationMaps` during initialization (with default parameters). 
@@ -575,15 +562,14 @@
             The undistorted images.
         """
         img1_rect = cv2.remap(img1, self.mapx1, self.mapy1, interpolation);
         img2_rect = cv2.remap(img2, self.mapx2, self.mapy2, interpolation);
         
         return img1_rect, img2_rect
     
-    
     def get3DPoints(self, disparityMap):
         """
         Get the 3D points in the space from the disparity map.
         
         If the calibration was done with real world units (e.g. millimeters),
         the output would be in the same units. The world origin will be in the
         left camera.
@@ -608,15 +594,15 @@
         # and self.K2)
         
         # IMPLEMENTATION NOTES
         # fx and fy are assumed the same for left and right (after
         # rectification, they should)
         # Accepts different x-shear terms (generally not used)
         # cx1 is not the same of cx2
-        # cy1 is equal cy2 (as images are rectified)
+        # cy1 is equal cy2 (as images are rectified).
         
         b   = self.getBaseline()
         fx  = self.K1[0,0]
         fy  = self.K2[1,1]
         cx1 = self.K1[0,2]
         cx2 = self.K2[0,2]
         a1  = self.K1[0,1]
@@ -650,15 +636,14 @@
         if isinstance(r, StereoRig):                  # Extend unpacking a StereoRig object 
             super(StructuredLightRig, self).__init__(r.res1, r.res2, r.intrinsic1, r.intrinsic2, r.distCoeffs1, r.distCoeffs2, r.R, r.T, r.F, r.E, r.reprojectionError)
         else:
             raise ValueError("Invalid argument!")
                 
         self._computeMatrices()
     
-    
     def _computeMatrices(self):
         self.R1, self.R2, self.R = rectification._lowLevelRectify(self)    
         ### Get inverse common orientation and extend to 4x4 transform
         R_inv = np.linalg.inv(self.R)
         R_inv = np.hstack( ( np.vstack( (R_inv,np.zeros((1,3))) ), np.zeros((4,1)) ) )
         R_inv[3,3] = 1
         self.R_inv = R_inv
@@ -710,15 +695,14 @@
         # Cancel common orientation applied to first camera
         # to bring points into camera coordinate system
         # NOT NEEDED See `rectification._lowLevelRectify` 
         finalPoints = cv2.perspectiveTransform(finalPoints.reshape(-1,1,3), self.R_inv)
         
         return finalPoints
     
-    
     def undistortCameraImage(self, imgObj):
         """
         Undistort camera image.
         
         Parameters
         ----------
         imgObj : numpy.ndarray
```

### Comparing `SimpleStereo-1.0.5.1/simplestereo/_passive.cpp` & `SimpleStereo-1.0.6.0/simplestereo/_passive.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,16 @@
                     ii = y - padding + i;
                     if( ii < 0) continue;       // Image top border
                     if( ii >= height) break;    // Image bottom border
                     
                     for(j = 0; j < winSize; ++j) {
                         jj = d - padding + j;
                         kk = x - padding + j;
-                        if(jj<0 or kk<0) continue;
-                        if(jj>=width or kk>=width) break;
+                        if(jj<0 || kk<0) continue;
+                        if(jj>=width || kk>=width) break;
                         
                         // Build weight
                         w2[i*winSize+j] = proximityWeights[i*winSize + j] * 
                                    exp(-sqrt( pow(dataLab2[3*(ii*width + jj)  ] - dataLab2[3*(y*width + d)  ],2) +
                                               pow(dataLab2[3*(ii*width + jj)+1] - dataLab2[3*(y*width + d)+1],2) + 
                                               pow(dataLab2[3*(ii*width + jj)+2] - dataLab2[3*(y*width + d)+2],2) )/gammaC);
                         
@@ -150,16 +150,16 @@
                 for(i = 0; i < winSize; ++i) {
                     ii = y-padding+i;
                     if(ii<0) continue;
                     if(ii>=height) break;
                     for(j = 0; j < winSize; ++j) {
                         jj = d-padding+j;
                         kk = x-padding+j;
-                        if(jj<0 or kk<0) continue;
-                        if(jj>=width or kk>=width) break;
+                        if(jj<0 || kk<0) continue;
+                        if(jj>=width || kk>=width) break;
                         // Build weight
                         w2[i*winSize+j] = proximityWeights[i*winSize + j] * 
                                    exp(-sqrt( pow(dataLab2[3*(ii*width + jj)  ] - dataLab2[3*(y*width+d)  ],2) +
                                               pow(dataLab2[3*(ii*width + jj)+1] - dataLab2[3*(y*width+d)+1],2) + 
                                               pow(dataLab2[3*(ii*width + jj)+2] - dataLab2[3*(y*width+d)+2],2) )/gammaC);
                         
                         // Update cost
@@ -215,16 +215,16 @@
             for(i = 0; i < winSize; ++i) {
                 ii = y-padding+i;
                 if(ii<0) continue;
                 if(ii>=height) break;
                 for(j = 0; j < winSize; ++j) {
                     jj = d-padding+j;
                     kk = x-padding+j;
-                    if(jj<0 or kk<0) continue;
-                    if(jj>=width or kk>=width) break;
+                    if(jj<0 || kk<0) continue;
+                    if(jj>=width || kk>=width) break;
                     // Build weight
                     w1[i*winSize+j] = proximityWeights[i*winSize + j] * 
                                exp(-sqrt( pow(dataLab1[3*(ii*width + jj)  ] - dataLab1[3*(y*width+d)  ],2) +
                                           pow(dataLab1[3*(ii*width + jj)+1] - dataLab1[3*(y*width+d)+1],2) + 
                                           pow(dataLab1[3*(ii*width + jj)+2] - dataLab1[3*(y*width+d)+2],2) )/gammaC);
                     
                     // Update cost
@@ -256,18 +256,18 @@
     // Left-Right consistency check
     // Disparity value == -1 means invalidated (occluded) pixel
     for(j=0; j < width; ++j) {
         if(disparityMap[y*width + j] == -1){
             // Find limits
             left = j-1;
             right = j+1;
-            while(left>=0 and disparityMap[y*width + left] == -1){
+            while(left>=0 && disparityMap[y*width + left] == -1){
                 --left;
                 }
-            while(right<width and disparityMap[y*width + right] == -1){
+            while(right<width && disparityMap[y*width + right] == -1){
                 ++right;
                 }
             // Left and right contain the first non occluded pixel in that direction
             // Ensure that we are within image limits
             // and assing valid value to occluded pixels
             if(left < 0){
                 for(k=0;k<right;++k)
@@ -302,28 +302,28 @@
                           &winSize, &maxDisparity, &minDisparity, &gammaC, &gammaP,
                           &consistent)){
         PyErr_SetString(PyExc_ValueError, "Invalid input format!");
         return NULL;
         }
     
     // Check input format
-    if (!(PyArray_TYPE(img1) == NPY_UBYTE and PyArray_TYPE(img1) == NPY_UBYTE)){
+    if (!(PyArray_TYPE(img1) == NPY_UBYTE && PyArray_TYPE(img1) == NPY_UBYTE)){
         // Raising an exception in C is done by setting the exception object or string and then returning NULL from the function.
         // See https://docs.python.org/3/c-api/exceptions.html
         PyErr_SetString(PyExc_TypeError, "Wrong type input!");
         return NULL;
         }
-    if (PyArray_NDIM(img1)!=3 or PyArray_NDIM(img1)!=PyArray_NDIM(img2) or 
-        PyArray_DIM(img1,2)!=3 or PyArray_DIM(img2,2)!=3 or
-        PyArray_DIM(img1,0)!=PyArray_DIM(img2,0) or
+    if (PyArray_NDIM(img1)!=3 || PyArray_NDIM(img1)!=PyArray_NDIM(img2) || 
+        PyArray_DIM(img1,2)!=3 || PyArray_DIM(img2,2)!=3 ||
+        PyArray_DIM(img1,0)!=PyArray_DIM(img2,0) ||
         PyArray_DIM(img1,1)!=PyArray_DIM(img2,1)){
         PyErr_SetString(PyExc_ValueError, "Wrong image dimensions!");
         return NULL;
         }
-    if (!(winSize>0 and winSize%2==1)) {
+    if (!(winSize>0 && winSize%2==1)) {
         PyErr_SetString(PyExc_ValueError, "winSize must be a positive odd number!");
         return NULL;
         }
     
     
     //Retrieve input
     int height = PyArray_DIM(img1,0);
@@ -348,15 +348,15 @@
     // Working variables
     int padding = winSize / 2;
     int i,j;
     SafeQueue<int> jobs; // Jobs queue
     int num_threads = std::thread::hardware_concurrency();
     
     
-    std::thread workersArr[num_threads];
+    std::thread* workersArr = new std::thread[num_threads];
     
     // Build proximity weights matrix
     double *proximityWeights = new double[winSize*winSize];
     
     for(i = 0; i < winSize; ++i) {
         for(j = 0; j < winSize; ++j) {
             proximityWeights[i*winSize+j] = exp(-sqrt( pow(i-padding,2) + pow(j-padding,2))/gammaP);
@@ -410,15 +410,15 @@
             int minDisparity, int maxDisparity, int gamma, float fMax, int iterations, int bins)
 {
     int dBest;
     float cost, costBest, temp, wBest;
     int ii,jj,kk;
     int i,j,k,y,x,d;
     int tot = winSize*winSize;
-    float w[tot]; // Weights
+    float* w = new float[tot]; // Weights
     int center = (tot-1) / 2;
     int xx, yy;
     int left,right;
     
     while(!jobs.empty()) 
     {
         
@@ -438,24 +438,24 @@
             // Iterations
             for (d=0;d<iterations;++d){
                 
                 // Forward pass (row major order)
                 for(i=0;i<tot;++i){                 // For every window pixel
                    yy = y-padding + i/winSize; // Whole image coordinates
                    xx = x-padding + i%winSize;
-                   if(xx<0 or yy<0) continue;           //Image left border
-                   if(xx>=width or yy>=height) break;  // Image right border
+                   if(xx<0 || yy<0) continue;           //Image left border
+                   if(xx>=width || yy>=height) break;  // Image right border
                    wBest = INFINITY;  
                    
                    for(k=0;k<=center;++k) // Find minimum in upper kernel
                    {
                        jj = y-padding + k/winSize; // Whole image coordinates (kernel)
                        kk = x-padding + k%winSize;
-                       if(jj<0 or kk<0) continue;
-                       if(jj>=height or kk>=width) break;
+                       if(jj<0 || kk<0) continue;
+                       if(jj>=height || kk>=width) break;
                        
                        // OVER THE UPPER KERNEL
                        temp = w[k] + sqrt( pow(data1[3*(yy*width + xx)  ] - data1[3*(jj*width + kk)  ],2)
                                          + pow(data1[3*(yy*width + xx)+1] - data1[3*(jj*width + kk)+1],2)
                                          + pow(data1[3*(yy*width + xx)+2] - data1[3*(jj*width + kk)+2],2) ); 
                                
                        if(temp<wBest) wBest=temp;
@@ -463,24 +463,24 @@
                    w[i] = wBest;
                    }
                    
                 // Backward pass (reverse row major order)
                 for(i=tot-1;i>=0;--i){                 // For every window pixel
                    yy = y-padding + i/winSize; // Whole image coordinates
                    xx = x-padding + i%winSize;
-                   if(yy<0 or xx<0) continue;   
-                   if(yy>=height or xx>=width) break; 
+                   if(yy<0 || xx<0) continue;   
+                   if(yy>=height || xx>=width) break; 
                    wBest = INFINITY;  
                    
                    for(k=center;k<tot;++k) // Find minimum in upper kernel
                    {
                        jj = y-padding + k/winSize; // Whole image coordinates (kernel)
                        kk = x-padding + k%winSize;
-                       if(jj<0 or kk<0) continue;
-                       if(jj>=height or kk>=width) break;
+                       if(jj<0 || kk<0) continue;
+                       if(jj>=height || kk>=width) break;
                        
                        // OVER THE LOWER KERNEL
                        temp = w[k] + sqrt( pow(data1[3*(yy*width + xx)  ] - data1[3*(jj*width + kk)  ],2)
                                          + pow(data1[3*(yy*width + xx)+1] - data1[3*(jj*width + kk)+1],2)
                                          + pow(data1[3*(yy*width + xx)+2] - data1[3*(jj*width + kk)+2],2) ); 
                        
                        if(temp<wBest) wBest=temp;
@@ -515,16 +515,16 @@
                     if( ii < 0) continue;       // Image top border
                     if( ii >= height) break;    // Image bottom border
                     
                     for(j = 0; j < winSize; ++j) {
                         kk = x - padding + j;
                         jj = d - padding + j;
                         
-                        if( jj < 0 or kk < 0) continue;         // Image left border
-                        if( jj >= width or kk >= width) break;  // Image right border
+                        if( jj < 0 || kk < 0) continue;         // Image left border
+                        if( jj >= width || kk >= width) break;  // Image right border
                         
                         
                         // Update cost
                         // Color difference is capped to fMax
                         cost += w[i*winSize + j] * std::min(fMax,
                                                             (float) sqrt(pow(data1[3*(ii*width + kk)]   - data2[3*(ii*width + jj)  ], 2)
                                                                        + pow(data1[3*(ii*width + kk)+1] - data2[3*(ii*width + jj)+1], 2)
@@ -559,50 +559,50 @@
             
             // Iterations
             for (d=0;d<iterations;++d){
                 
                 // Forward pass (row major order)
                 for(i=0;i<tot;++i){                 // For every window pixel
                    yy = y-padding + i/winSize; // Whole image coordinates
-                   if(yy<0 or yy>=height) continue;   //Image y border
+                   if(yy<0 || yy>=height) continue;   //Image y border
                    xx = x-padding + i%winSize;
-                   if(xx<0 or xx>=width) continue;  // Image x border
+                   if(xx<0 || xx>=width) continue;  // Image x border
                    wBest = INFINITY;  
                    
                    for(k=0;k<=center;++k) // Find minimum in upper kernel
                    {
                        jj = y-padding + k/winSize; // Whole image coordinates (kernel)
-                       if(jj<0 or jj>=height) continue;
+                       if(jj<0 || jj>=height) continue;
                        kk = x-padding + k%winSize;
-                       if(kk<0 or kk>=width) continue;
+                       if(kk<0 || kk>=width) continue;
                        
                        // OVER THE UPPER KERNEL
                        temp = w[k] + sqrt( pow(data2[3*(yy*width + xx)  ] - data2[3*(jj*width + kk)  ],2)
                                          + pow(data2[3*(yy*width + xx)+1] - data2[3*(jj*width + kk)+1],2)
                                          + pow(data2[3*(yy*width + xx)+2] - data2[3*(jj*width + kk)+2],2) ); 
                                
                        if(temp<wBest) wBest=temp;
                        }
                    w[i] = wBest;
                    }
                    
                 // Backward pass (reverse row major order)
                 for(i=tot-1;i>=0;--i){                 // For every window pixel
                    yy = y-padding + i/winSize; // Whole image coordinates
-                   if(yy<0 or yy>=height) continue;   //Image y border
+                   if(yy<0 || yy>=height) continue;   //Image y border
                    xx = x-padding + i%winSize;
-                   if(xx<0 or xx>=width) continue;  // Image x border
+                   if(xx<0 || xx>=width) continue;  // Image x border
                    wBest = INFINITY;  
                    
                    for(k=center;k<tot;++k) // Find minimum in upper kernel
                    {
                        jj = y-padding + k/winSize; // Whole image coordinates (kernel)
-                       if(jj<0 or jj>=height) continue;
+                       if(jj<0 || jj>=height) continue;
                        kk = x-padding + k%winSize;
-                       if(kk<0 or kk>=width) continue;
+                       if(kk<0 || kk>=width) continue;
                        
                        // OVER THE LOWER KERNEL
                        temp = w[k] + sqrt( pow(data2[3*(yy*width + xx)  ] - data2[3*(jj*width + kk)  ],2)
                                          + pow(data2[3*(yy*width + xx)+1] - data2[3*(jj*width + kk)+1],2)
                                          + pow(data2[3*(yy*width + xx)+2] - data2[3*(jj*width + kk)+2],2) ); 
                        
                        if(temp<wBest) wBest=temp;
@@ -631,16 +631,16 @@
                     if( ii < 0) continue;       // Image top border
                     if( ii >= height) break;    // Image bottom border
                     
                     for(j = 0; j < winSize; ++j) {
                         kk = x - padding + j;
                         jj = d - padding + j;
                         
-                        if( jj < 0 or kk < 0) continue;         // Image left border
-                        if( jj >= width or kk >= width) break;  // Image right border
+                        if( jj < 0 || kk < 0) continue;         // Image left border
+                        if( jj >= width || kk >= width) break;  // Image right border
                         
                         
                         // Update cost
                         // Color difference is capped to fMax
                         cost += w[i*winSize + j] * std::min(fMax,
                                                             (float) sqrt(pow(data2[3*(ii*width + kk)]   - data1[3*(ii*width + jj)  ], 2)
                                                                + pow(data2[3*(ii*width + kk)+1] - data1[3*(ii*width + jj)+1], 2)
@@ -667,18 +667,18 @@
     // Left-Right consistency check
     // Disparity value == -1 means invalidated (occluded) pixel
     for(j=0; j < width; ++j) {
         if(disparityMap[y*width + j] == -1){
             // Find limits
             left = j-1;
             right = j+1;
-            while(left>=0 and disparityMap[y*width + left] == -1){
+            while(left>=0 && disparityMap[y*width + left] == -1){
                 --left;
                 }
-            while(right<width and disparityMap[y*width + right] == -1){
+            while(right<width && disparityMap[y*width + right] == -1){
                 ++right;
                 }
             // Left and right contain the first non occluded pixel in that direction
             // Ensure that we are within image limits
             // and assing valid value to occluded pixels
             if(left < 0){
                 for(k=0;k<right;++k)
@@ -710,28 +710,28 @@
                           &winSize, &maxDisparity, &minDisparity, &gamma,
                           &fMax, &iterations, &bins)){
         PyErr_SetString(PyExc_ValueError, "Invalid input format!");
         return NULL;
         }
     
     // Check input format
-    if (!(PyArray_TYPE(img1) == NPY_UBYTE and PyArray_TYPE(img1) == NPY_UBYTE)){
+    if (!(PyArray_TYPE(img1) == NPY_UBYTE && PyArray_TYPE(img1) == NPY_UBYTE)){
         // Raising an exception in C is done by setting the exception object or string and then returning NULL from the function.
         // See https://docs.python.org/3/c-api/exceptions.html
         PyErr_SetString(PyExc_TypeError, "Wrong type input!");
         return NULL;
         }
-    if (PyArray_NDIM(img1)!=3 or PyArray_NDIM(img1)!=PyArray_NDIM(img2) or 
-        PyArray_DIM(img1,2)!=3 or PyArray_DIM(img2,2)!=3 or
-        PyArray_DIM(img1,0)!=PyArray_DIM(img2,0) or
+    if (PyArray_NDIM(img1)!=3 || PyArray_NDIM(img1)!=PyArray_NDIM(img2) || 
+        PyArray_DIM(img1,2)!=3 || PyArray_DIM(img2,2)!=3 ||
+        PyArray_DIM(img1,0)!=PyArray_DIM(img2,0) ||
         PyArray_DIM(img1,1)!=PyArray_DIM(img2,1)){
         PyErr_SetString(PyExc_ValueError, "Wrong image dimensions!");
         return NULL;
         }
-    if (!(winSize>0 and winSize%2==1)) {
+    if (!(winSize>0 && winSize%2==1)) {
         PyErr_SetString(PyExc_ValueError, "winSize must be a positive odd number!");
         return NULL;
         }
     
     //Retrieve input
     int height = PyArray_DIM(img1,0);
     int width = PyArray_DIM(img1,1);
@@ -747,15 +747,15 @@
     
     // Working variables
     int padding = winSize / 2;
     int i;
     SafeQueue<int> jobs; // Jobs queue
     int num_threads = std::thread::hardware_concurrency();
     
-    std::thread workersArr[num_threads];
+    std::thread* workersArr = new std::thread[num_threads];
     
     
     // Put each image row in queue
     for(i=0; i < height; ++i) {   
         jobs.push(i);
     }
```

### Comparing `SimpleStereo-1.0.5.1/simplestereo/_unwrapping.cpp` & `SimpleStereo-1.0.6.0/simplestereo/_unwrapping.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 /* C++ extension for phase unwrapping algorithms */
+#define _USE_MATH_DEFINES
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 #include <numpy/arrayobject.h>
  
 #include <iostream>
 #include <vector>
 #include <math.h>
@@ -72,15 +73,19 @@
     int h = PyArray_DIM(phase,0);
     int w = PyArray_DIM(phase,1);
     
     //Initialisation
     npy_intp dims[2] = {h, w};
     PyArrayObject *unwrapped = (PyArrayObject *) PyArray_Zeros(2, dims, PyArray_DTYPE(phase), 0);
     
-    bool s[h][w];
+    bool** s = new bool*[h];
+    for(int i = 0; i < h; i++) {
+        s[i] = new bool[w];
+    }
+
     int y;
     int x;
     int S;
     double temp;
     double cur;
     std::vector<Coord> neigh;
```

### Comparing `SimpleStereo-1.0.5.1/simplestereo/active.py` & `SimpleStereo-1.0.6.0/simplestereo/active.py`

 * *Files identical despite different names*

### Comparing `SimpleStereo-1.0.5.1/simplestereo/calibration.py` & `SimpleStereo-1.0.6.0/simplestereo/calibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,14 @@
         proj_objps_list.append(np.float32(proj_objps))
         proj_corners_list.append(np.float32(proj_corners))
         cam_corners_list2.append(np.float32(cam_corners2))
         
     if skipped>0:
         warnings.warn(f"{skipped} over {len(proj_objps_list)*chessboardSize[0]*chessboardSize[1]} skipped corners.")
     
-    #print('Initial solution of camera\'s intrinsic parameters')
     cam_rvecs = []
     cam_tvecs = []
     
     # Calibrate camera only if intrinsic parameters are not given
     if camIntrinsic is None:
         cam_rms, cam_int, cam_dist, cam_rvecs, cam_tvecs = cv2.calibrateCamera(
             cam_objps_list, cam_corners_list, cam_shape[::-1], None, None, None, None)
@@ -591,18 +590,14 @@
     retval, intrinsic1, distCoeffs1, intrinsic2, distCoeffs2, R, T, E, F = cv2.stereoCalibrate(
         proj_objps_list, cam_corners_list2, proj_corners_list, cam_int, cam_dist, proj_int, proj_dist, None, flags=cv2.CALIB_FIX_INTRINSIC)
     
     
     # Build StereoRig object
     stereoRigObj = ss.StereoRig(cam_shape[::-1], projectorResolution, intrinsic1, intrinsic2, distCoeffs1, distCoeffs2, R, T, F = F, E = E, reprojectionError = retval)
     
-    print("cam_rms", cam_rms)
-    print("proj_rms", proj_rms)
-    print("stereo_rms", retval)
-    
     if extended:
         _, _, _, _, _, _, _, _, _, perViewErrors = cv2.stereoCalibrateExtended(
             proj_objps_list, cam_whiteCorners_list, proj_corners_list, cam_int, cam_dist, proj_int, proj_dist, None, R, T, flags=cv2.CALIB_FIX_INTRINSIC)
         
         return stereoRigObj, perViewErrors
     
     else:
@@ -958,19 +953,14 @@
     # Stereo calibrate
     retval, intrinsic1, distCoeffs1, intrinsic2, distCoeffs2, R, T, E, F = cv2.stereoCalibrate(
         proj_objps_list, cam_whiteCorners_list, proj_corners_list, cam_int, cam_dist, proj_int, proj_dist, None, flags=cv2.CALIB_FIX_INTRINSIC)
 
     # Build StereoRig object
     stereoRigObj = ss.StereoRig(cam_shape[::-1], projectorResolution, intrinsic1, intrinsic2, distCoeffs1, distCoeffs2, R, T, F = F, E = E, reprojectionError = retval)
     
-    #TEMP
-    print("cam_rms", cam_rms)
-    print("proj_rms", proj_rms)
-    print("stereo_rms", retval)
-    
     if extended:
         _, _, _, _, _, _, _, _, _, perViewErrors = cv2.stereoCalibrateExtended(
             proj_objps_list, cam_whiteCorners_list, proj_corners_list, cam_int, cam_dist, proj_int, proj_dist, None, R, T, flags=cv2.CALIB_FIX_INTRINSIC)
         
         return stereoRigObj, perViewErrors
     
     else:
```

### Comparing `SimpleStereo-1.0.5.1/simplestereo/headers/colorconversion.hpp` & `SimpleStereo-1.0.6.0/simplestereo/headers/colorconversion.hpp`

 * *Files identical despite different names*

### Comparing `SimpleStereo-1.0.5.1/simplestereo/headers/safequeue.hpp` & `SimpleStereo-1.0.6.0/simplestereo/headers/safequeue.hpp`

 * *Files identical despite different names*

### Comparing `SimpleStereo-1.0.5.1/simplestereo/passive.py` & `SimpleStereo-1.0.6.0/simplestereo/passive.py`

 * *Files identical despite different names*

### Comparing `SimpleStereo-1.0.5.1/simplestereo/points.py` & `SimpleStereo-1.0.6.0/simplestereo/points.py`

 * *Files identical despite different names*

### Comparing `SimpleStereo-1.0.5.1/simplestereo/rectification.py` & `SimpleStereo-1.0.6.0/simplestereo/rectification.py`

 * *Files identical despite different names*

### Comparing `SimpleStereo-1.0.5.1/simplestereo/unwrapping.py` & `SimpleStereo-1.0.6.0/simplestereo/unwrapping.py`

 * *Files identical despite different names*

### Comparing `SimpleStereo-1.0.5.1/simplestereo/utils.py` & `SimpleStereo-1.0.6.0/simplestereo/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,65 +35,60 @@
         and / or insert a time.sleep() after object constructor.
         
     Todo
     ----
     Add support for other options (e.g. change focal length where supported).
     """
     def __init__(self, device = 0, flipY=False):
-        # Check if we're opening a video file
+        # Check if we're opening a video file.
         self.isFile = os.path.isfile(device)
         self.video_capture = cv2.VideoCapture(device)
-        # Flip around y axis if needed
+        # Flip around y axis, if needed.
         self.flip = cv2.flip if flipY else lambda f, *a, **k: f 
         self.running = False
-        # Keep this as attribute (needed for streaming)
+        # Keep this as attribute (needed for streaming).
         self.frame = None   
         
         if self.isFile:                             # If we are opening a video file
             self.getFrame = self.video_capture.read # we use read()
             self.grab = lambda *args: None          # and cannot grab()
         else:                                       # If opening a webcam or a URL streaming
             self.grab = self.video_capture.grab     # that grabs continuously (grab() is fast)
             self.getFrame = self.video_capture.retrieve # and retrieve() (slower) the image only when needed
-            self.t=Thread(target=self.__loop)       # use a separate thread
+            self.t = Thread(target=self.__loop)       # use a separate thread
             self.t.daemon=True                          
         
-        # Check if capture is opened
+        # Check if capture is opened.
         if self.video_capture is None or not self.video_capture.isOpened():
             raise ValueError('Cannot open device!')
             
-    
     def __del__(self):
         self.stop()
         self.video_capture.release()
     
-    
     def __enter__(self):
         return self
     
-    
     def __exit__(self, type, value, traceback):
         # To allow use in with statement
         self.__del__()
     
-    
     def start(self):
         """
         Start the capture in a separate thread.
         
         No need to call this for video files.
         The thread continuously calls ``grab()`` to stay updated to the last frame,
         while ``retrieve()`` is called only when the frame is actually needed.
         """
-        if self.isFile: # Do not start if it is file
+        if self.isFile: # Do not start if it is file.
             return
         self.running = True
         self.t.start()
         
-    
     def stop(self):
         """
         Stop the capture.
         
         When finished, remember to call this method to **stop the capturing thread**.
         No need to call this for video files.
         
@@ -101,32 +96,29 @@
         if self.isFile: # N/A if is a file
             return
         if self.running:
             self.running = False
             self.t.join()
         return
     
-    
     def __loop(self):
         while(self.running):
             self.grab()
     
-    
     def get(self):
         """
         Retrieve the current frame.
         
         Returns None if there is no frame (e.g. end of video file).
         """
         ret, self.frame = self.getFrame()
         if not ret:
             return None
         return self.flip(self.frame, 1)
     
-    
     def setResolution(self, width, height):
         """
         Set resolution of the camera.
         
         Do not call this for video files or when the thread is running.
         It works only for supported cameras.
         
@@ -136,22 +128,39 @@
             Width and height to be set in pixels.
         
         Returns
         -------
         bool
             True if the resolution was set successfully, False otherwise.
         """
-        # You cannot change resolution while running or on files
+        # You cannot change resolution while running or on files.
         if self.running or self.isFile:
             return False
         
-        # Set properties. Each returns === True on success.
-        return self.video_capture.set(cv2.CAP_PROP_FRAME_WIDTH, width) and self.video_capture.set(cv2.CAP_PROP_FRAME_HEIGHT, height)
+        # Set properties. Each returns True on success.
+        retval = (
+            self.video_capture.set(cv2.CAP_PROP_FRAME_WIDTH, width) and
+            self.video_capture.set(cv2.CAP_PROP_FRAME_HEIGHT, height)
+            )
+
+        if not retval:
+            return False
+
+        # Verify that resolution was set correctly.
+        retval = (
+            self.video_capture.get(cv2.CAP_PROP_FRAME_WIDTH) == width and
+            self.video_capture.get(cv2.CAP_PROP_FRAME_HEIGHT) == height
+            )
+
+        return retval
+
+    def getResolution(self):
+        """ Return current resolution as (width, height) tuple. """
+        return self.video_capture.get(cv2.CAP_PROP_FRAME_WIDTH), self.video_capture.get(cv2.CAP_PROP_FRAME_HEIGHT)
 
-    
     def setFrameRate(self, fps):
         """
         Set framerate of the camera.
         
         Do not call this for video files or when the thread is running.
         It works only for supported cameras.
         
@@ -161,15 +170,15 @@
             Frames per second.
         
         Returns
         -------
         bool
             True if the framerate was set successfully, False otherwise.
         """
-        # You cannot change resolution while running or on files
+        # You cannot change attributes while running or on files.
         if self.running or self.isFile:
             return False
         
         return self.video_capture.set(cv2.CAP_PROP_FPS, fps)
 
 
 def moveExtrinsicOriginToFirstCamera(R1,R2,t1,t2):
```

