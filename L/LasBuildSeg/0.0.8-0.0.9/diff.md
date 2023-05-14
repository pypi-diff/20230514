# Comparing `tmp/LasBuildSeg-0.0.8.tar.gz` & `tmp/LasBuildSeg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.0.8.tar", last modified: Wed May 10 09:17:32 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.0.9.tar", last modified: Wed May 10 09:50:16 2023, max compression
```

## Comparing `LasBuildSeg-0.0.8.tar` & `LasBuildSeg-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 09:17:32.678023 LasBuildSeg-0.0.8/
--rw-rw-rw-   0        0        0       90 2023-05-10 09:15:44.000000 LasBuildSeg-0.0.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.0.8/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 09:17:32.602270 LasBuildSeg-0.0.8/LasBuildSeg/
--rw-rw-rw-   0        0        0    11870 2023-05-10 09:15:32.000000 LasBuildSeg-0.0.8/LasBuildSeg/LasBuildSeg.py
--rw-rw-rw-   0        0        0      375 2023-05-10 08:51:25.000000 LasBuildSeg-0.0.8/LasBuildSeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 09:17:32.672041 LasBuildSeg-0.0.8/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0     2043 2023-05-10 09:17:31.000000 LasBuildSeg-0.0.8/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-10 09:17:31.000000 LasBuildSeg-0.0.8/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 09:17:31.000000 LasBuildSeg-0.0.8/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-05-10 09:17:31.000000 LasBuildSeg-0.0.8/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 09:17:31.000000 LasBuildSeg-0.0.8/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       25 2022-09-19 08:00:05.000000 LasBuildSeg-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2043 2023-05-10 09:17:32.676025 LasBuildSeg-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1112 2023-05-10 09:16:07.000000 LasBuildSeg-0.0.8/README.md
--rw-rw-rw-   0        0        0     1495 2023-05-10 09:15:48.000000 LasBuildSeg-0.0.8/Setup.py
--rw-rw-rw-   0        0        0      106 2023-05-10 07:11:46.000000 LasBuildSeg-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 09:17:32.679013 LasBuildSeg-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 09:50:16.559576 LasBuildSeg-0.0.9/
+-rw-rw-rw-   0        0        0      107 2023-05-10 09:49:42.000000 LasBuildSeg-0.0.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.0.9/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 09:50:16.495789 LasBuildSeg-0.0.9/LasBuildSeg/
+-rw-rw-rw-   0        0        0    11872 2023-05-10 09:29:06.000000 LasBuildSeg-0.0.9/LasBuildSeg/LasBuildSeg.py
+-rw-rw-rw-   0        0        0      375 2023-05-10 08:51:25.000000 LasBuildSeg-0.0.9/LasBuildSeg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:50:16.552600 LasBuildSeg-0.0.9/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0     2057 2023-05-10 09:50:14.000000 LasBuildSeg-0.0.9/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-10 09:50:15.000000 LasBuildSeg-0.0.9/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 09:50:14.000000 LasBuildSeg-0.0.9/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-05-10 09:50:14.000000 LasBuildSeg-0.0.9/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 09:50:14.000000 LasBuildSeg-0.0.9/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-05-10 09:31:40.000000 LasBuildSeg-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2057 2023-05-10 09:50:16.556602 LasBuildSeg-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1126 2023-05-10 09:49:28.000000 LasBuildSeg-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1495 2023-05-10 09:49:45.000000 LasBuildSeg-0.0.9/Setup.py
+-rw-rw-rw-   0        0        0      106 2023-05-10 07:11:46.000000 LasBuildSeg-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 09:50:16.560580 LasBuildSeg-0.0.9/setup.cfg
```

### Comparing `LasBuildSeg-0.0.8/LICENSE.txt` & `LasBuildSeg-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.0.8/LasBuildSeg/LasBuildSeg.py` & `LasBuildSeg-0.0.9/LasBuildSeg/LasBuildSeg.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,7 +298,8 @@
     # Open a new GeoTIFF file in write mode using the profile information
     with rasterio.open(filename, 'w', **profile) as dst:
         # Set the CRS information for the output file
         dst.crs = profile['crs']  # Add CRS information
         dst.write(data.astype(rasterio.uint8), 1)
 #input_crs = pyproj.CRS.from_epsg(input_epsg)        
 #crs=pyproj.CRS.from_epsg(3857)
+
```

### Comparing `LasBuildSeg-0.0.8/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.0.9/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.0.8
+Version: 0.0.9
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,17 +19,19 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 This Python package is BUilding Footprint Extractor Test
 
 This of example of an how you can run your code
+
+```python
 import LasBuildSeg as Lasb
 import numpy as np
-
+ 
 Lasb.generate_dsm('USGS_LPC_IL_HicksDome_FluorsparDistrict_2019_D19_2339_5650.laz', 8734, 1)
 Lasb.generate_dtm('USGS_LPC_IL_HicksDome_FluorsparDistrict_2019_D19_2339_5650.laz', 8734, 1)
 Lasb.generate_ndhm('dtm.tif', 'dsm.tif')
 img, profile = Lasb.read_geotiff('ndhm.tif')
 img_8bit = Lasb.to_8bit(img)
 constant = 4.6
 block_size = 51
```

### Comparing `LasBuildSeg-0.0.8/PKG-INFO` & `LasBuildSeg-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.0.8
+Version: 0.0.9
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,17 +19,19 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 This Python package is BUilding Footprint Extractor Test
 
 This of example of an how you can run your code
+
+```python
 import LasBuildSeg as Lasb
 import numpy as np
-
+ 
 Lasb.generate_dsm('USGS_LPC_IL_HicksDome_FluorsparDistrict_2019_D19_2339_5650.laz', 8734, 1)
 Lasb.generate_dtm('USGS_LPC_IL_HicksDome_FluorsparDistrict_2019_D19_2339_5650.laz', 8734, 1)
 Lasb.generate_ndhm('dtm.tif', 'dsm.tif')
 img, profile = Lasb.read_geotiff('ndhm.tif')
 img_8bit = Lasb.to_8bit(img)
 constant = 4.6
 block_size = 51
```

### Comparing `LasBuildSeg-0.0.8/README.md` & `LasBuildSeg-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 This Python package is BUilding Footprint Extractor Test
 
 This of example of an how you can run your code
+
+```python
 import LasBuildSeg as Lasb
 import numpy as np
-
+ 
 Lasb.generate_dsm('USGS_LPC_IL_HicksDome_FluorsparDistrict_2019_D19_2339_5650.laz', 8734, 1)
 Lasb.generate_dtm('USGS_LPC_IL_HicksDome_FluorsparDistrict_2019_D19_2339_5650.laz', 8734, 1)
 Lasb.generate_ndhm('dtm.tif', 'dsm.tif')
 img, profile = Lasb.read_geotiff('ndhm.tif')
 img_8bit = Lasb.to_8bit(img)
 constant = 4.6
 block_size = 51
```

### Comparing `LasBuildSeg-0.0.8/Setup.py` & `LasBuildSeg-0.0.9/Setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.0.8',
+  version='0.0.9',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

