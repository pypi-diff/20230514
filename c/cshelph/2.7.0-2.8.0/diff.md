# Comparing `tmp/cshelph-2.7.0.tar.gz` & `tmp/cshelph-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshelph-2.7.0.tar", last modified: Sat May 13 22:44:05 2023, max compression
+gzip compressed data, was "cshelph-2.8.0.tar", last modified: Sun May 14 00:02:48 2023, max compression
```

## Comparing `cshelph-2.7.0.tar` & `cshelph-2.8.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-13 22:44:05.738008 cshelph-2.7.0/
--rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.7.0/LICENSE.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)     3072 2023-05-13 22:44:05.737885 cshelph-2.7.0/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)     2564 2023-05-07 17:17:40.000000 cshelph-2.7.0/README.md
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-13 22:44:05.737707 cshelph-2.7.0/cshelph.egg-info/
--rw-r--r--   0 nmthoma1   (503) staff       (20)     3072 2023-05-13 22:44:05.000000 cshelph-2.7.0/cshelph.egg-info/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)      165 2023-05-13 22:44:05.000000 cshelph-2.7.0/cshelph.egg-info/SOURCES.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-13 22:44:05.000000 cshelph-2.7.0/cshelph.egg-info/dependency_links.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-05-13 22:44:05.000000 cshelph-2.7.0/cshelph.egg-info/top_level.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)    16694 2023-05-13 22:41:28.000000 cshelph-2.7.0/cshelph.py
--rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-13 22:44:05.738049 cshelph-2.7.0/setup.cfg
--rw-r--r--   0 nmthoma1   (503) staff       (20)     1669 2023-05-13 22:42:50.000000 cshelph-2.7.0/setup.py
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-14 00:02:48.693502 cshelph-2.8.0/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.8.0/LICENSE.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     3098 2023-05-14 00:02:48.693375 cshelph-2.8.0/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     2590 2023-05-13 23:59:02.000000 cshelph-2.8.0/README.md
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-14 00:02:48.693188 cshelph-2.8.0/cshelph.egg-info/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     3098 2023-05-14 00:02:48.000000 cshelph-2.8.0/cshelph.egg-info/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      165 2023-05-14 00:02:48.000000 cshelph-2.8.0/cshelph.egg-info/SOURCES.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-14 00:02:48.000000 cshelph-2.8.0/cshelph.egg-info/dependency_links.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-05-14 00:02:48.000000 cshelph-2.8.0/cshelph.egg-info/top_level.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    16694 2023-05-13 22:41:28.000000 cshelph-2.8.0/cshelph.py
+-rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-14 00:02:48.693543 cshelph-2.8.0/setup.cfg
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     1669 2023-05-14 00:00:44.000000 cshelph-2.8.0/setup.py
```

### Comparing `cshelph-2.7.0/LICENSE.txt` & `cshelph-2.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cshelph-2.7.0/PKG-INFO` & `cshelph-2.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cshelph
-Version: 2.7.0
+Version: 2.8.0
 Summary: Classification of Sub-aquatic Height Extracted Photons
 Home-page: https://github.com/nmt28/C-SHELPh
 Author: Nathan Thomas and Brian Lee
 Author-email: nmthomas28@gmail.com
 License: LICENSE.txt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -19,15 +19,15 @@
 
 ### C-SHELPh is the Classification of Sub-aquatic Height Extracted Photons. It is designed to isolate bathymetric photons in ICESat2 ATL03 files.
 
 ## Installation
 
 ### It is recommended that the dependancies are installed via:
 ```
-conda install -c conda-forge geopandas utm numpy matplotlib s3fs xarray zarr pyproj proj-data h5py
+conda install -c conda-forge geopandas utm numpy matplotlib s3fs xarray zarr pyproj proj-data h5py earthaccess h5netcdf dask
 
 pip install cshelph
 
 ```
 
 ## Using C-SHELPh
```

### Comparing `cshelph-2.7.0/README.md` & `cshelph-2.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ### C-SHELPh is the Classification of Sub-aquatic Height Extracted Photons. It is designed to isolate bathymetric photons in ICESat2 ATL03 files.
 
 ## Installation
 
 ### It is recommended that the dependancies are installed via:
 ```
-conda install -c conda-forge geopandas utm numpy matplotlib s3fs xarray zarr pyproj proj-data h5py
+conda install -c conda-forge geopandas utm numpy matplotlib s3fs xarray zarr pyproj proj-data h5py earthaccess h5netcdf dask
 
 pip install cshelph
 
 ```
 
 ## Using C-SHELPh
```

### Comparing `cshelph-2.7.0/cshelph.egg-info/PKG-INFO` & `cshelph-2.8.0/cshelph.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cshelph
-Version: 2.7.0
+Version: 2.8.0
 Summary: Classification of Sub-aquatic Height Extracted Photons
 Home-page: https://github.com/nmt28/C-SHELPh
 Author: Nathan Thomas and Brian Lee
 Author-email: nmthomas28@gmail.com
 License: LICENSE.txt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -19,15 +19,15 @@
 
 ### C-SHELPh is the Classification of Sub-aquatic Height Extracted Photons. It is designed to isolate bathymetric photons in ICESat2 ATL03 files.
 
 ## Installation
 
 ### It is recommended that the dependancies are installed via:
 ```
-conda install -c conda-forge geopandas utm numpy matplotlib s3fs xarray zarr pyproj proj-data h5py
+conda install -c conda-forge geopandas utm numpy matplotlib s3fs xarray zarr pyproj proj-data h5py earthaccess h5netcdf dask
 
 pip install cshelph
 
 ```
 
 ## Using C-SHELPh
```

### Comparing `cshelph-2.7.0/cshelph.py` & `cshelph-2.8.0/cshelph.py`

 * *Files identical despite different names*

### Comparing `cshelph-2.7.0/setup.py` & `cshelph-2.8.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 #
 #
 # Purpose:  Installation of the C-SHELPh software
 #
 # Author: Nathan Thomas
 # Email: nmthomas28@gmail.com
 # Date: 05/05/2023
-# Version: 2.7.0
+# Version: 2.8.0
 #
 # History:
 # Version 2.7.0
 
 from distutils.core import setup
 import os
 
 setup(name='cshelph',
-    version='2.7.0',
+    version='2.8.0',
     description='Classification of Sub-aquatic Height Extracted Photons',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Nathan Thomas and Brian Lee',
     author_email='nmthomas28@gmail.com',
     scripts=['cshelph.py'],
     package_dir={},
```

