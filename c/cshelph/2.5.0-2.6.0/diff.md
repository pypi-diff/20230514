# Comparing `tmp/cshelph-2.5.0.tar.gz` & `tmp/cshelph-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshelph-2.5.0.tar", last modified: Sun May  7 17:48:35 2023, max compression
+gzip compressed data, was "cshelph-2.6.0.tar", last modified: Sat May 13 21:34:50 2023, max compression
```

## Comparing `cshelph-2.5.0.tar` & `cshelph-2.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-07 17:48:35.380735 cshelph-2.5.0/
--rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.5.0/LICENSE.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)     3072 2023-05-07 17:48:35.380607 cshelph-2.5.0/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)     2564 2023-05-07 17:17:40.000000 cshelph-2.5.0/README.md
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-07 17:48:35.380441 cshelph-2.5.0/cshelph.egg-info/
--rw-r--r--   0 nmthoma1   (503) staff       (20)     3072 2023-05-07 17:48:35.000000 cshelph-2.5.0/cshelph.egg-info/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)      165 2023-05-07 17:48:35.000000 cshelph-2.5.0/cshelph.egg-info/SOURCES.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-07 17:48:35.000000 cshelph-2.5.0/cshelph.egg-info/dependency_links.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-05-07 17:48:35.000000 cshelph-2.5.0/cshelph.egg-info/top_level.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)    18644 2023-05-07 17:32:46.000000 cshelph-2.5.0/cshelph.py
--rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-07 17:48:35.380779 cshelph-2.5.0/setup.cfg
--rw-r--r--   0 nmthoma1   (503) staff       (20)     1669 2023-05-07 17:48:28.000000 cshelph-2.5.0/setup.py
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-13 21:34:50.490641 cshelph-2.6.0/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.6.0/LICENSE.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     3072 2023-05-13 21:34:50.490520 cshelph-2.6.0/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     2564 2023-05-07 17:17:40.000000 cshelph-2.6.0/README.md
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-13 21:34:50.490362 cshelph-2.6.0/cshelph.egg-info/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     3072 2023-05-13 21:34:50.000000 cshelph-2.6.0/cshelph.egg-info/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      165 2023-05-13 21:34:50.000000 cshelph-2.6.0/cshelph.egg-info/SOURCES.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-13 21:34:50.000000 cshelph-2.6.0/cshelph.egg-info/dependency_links.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-05-13 21:34:50.000000 cshelph-2.6.0/cshelph.egg-info/top_level.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    19415 2023-05-13 21:25:55.000000 cshelph-2.6.0/cshelph.py
+-rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-13 21:34:50.490682 cshelph-2.6.0/setup.cfg
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     1669 2023-05-13 21:34:41.000000 cshelph-2.6.0/setup.py
```

### Comparing `cshelph-2.5.0/LICENSE.txt` & `cshelph-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cshelph-2.5.0/PKG-INFO` & `cshelph-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cshelph
-Version: 2.5.0
+Version: 2.6.0
 Summary: Classification of Sub-aquatic Height Extracted Photons
 Home-page: https://github.com/nmt28/C-SHELPh
 Author: Nathan Thomas and Brian Lee
 Author-email: nmthomas28@gmail.com
 License: LICENSE.txt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cshelph-2.5.0/README.md` & `cshelph-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cshelph-2.5.0/cshelph.egg-info/PKG-INFO` & `cshelph-2.6.0/cshelph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cshelph
-Version: 2.5.0
+Version: 2.6.0
 Summary: Classification of Sub-aquatic Height Extracted Photons
 Home-page: https://github.com/nmt28/C-SHELPh
 Author: Nathan Thomas and Brian Lee
 Author-email: nmthomas28@gmail.com
 License: LICENSE.txt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cshelph-2.5.0/cshelph.py` & `cshelph-2.6.0/cshelph.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 import fiona
 import geopandas
 #import netCDF4
 from datetime import datetime
 import utm
 import xarray as xr
 import fsspec
+import earthaccess
+import geopandas
+
 # need s3fs installed
 
 def read_atl03(h5_file, laser_num):
     # Read File
     f = h5.File(h5_file,'r')
     
     # Select a laser
@@ -243,35 +246,61 @@
     dataset = netCDF4.Dataset(url)
     
     # Access the data and convert the temperature from K to C
     sea_temp = dataset['analysed_sst'][0,new_lat_ratio, new_lon_ratio] - 273.15
     return sea_temp
 
 def get_water_temp(data_path, latitude, longitude):
-    '''
-    pull down surface water temperature along the track from the MUR SST:
-    https://aws.amazon.com/marketplace/pp/prodview-kvgy4vkuhavsc?sr=0-3&ref_=beagle&applicationId=AWSMpContessa#overview.
-    '''
+
+    try:
+        auth = earthaccess.login(strategy="netrc")
+    except:
+        print("Login credentials not found. Sign in manually, your netrc file will be created for next time")
+        auth = earthaccess.login(strategy="interactive", persist=True)
+    
     # Get date from data filename
     file_date = data_path[-33:-25]
     
-    start_date = str(datetime.strptime(file_date + ' 00:00:00', '%Y%m%d %H:%M:%S'))
-    end_date = str(datetime.strptime(file_date + ' 23:59:59', '%Y%m%d %H:%M:%S'))
+    start_date = str(datetime.strptime(file_date, '%Y%m%d'))
+    end_date = str(datetime.strptime(file_date, '%Y%m%d'))
 
-    # Calculate ratio of latitude from mid-point of IS2 track
-    lat_med = np.median(latitude)
+    location_df = pd.DataFrame({'longitude':longitude,'latitude':latitude})
+    
+    location_df = location_df.dropna(axis=0)
+    
+    med_lon = np.nanmedian(location_df['longitude'])
+    med_lat = np.nanmedian(location_df['latitude'])
+    
+    minx, miny, maxx, maxy = list(location_df.total_bounds)
+    
+    # The first step is to create a DataCollections query
 
-    # Calculate ratio of longitude from mid-point of IS2 track
-    lon_med = np.median(longitude)
+    Query = earthaccess.collection_query()
+
+    # Use chain methods to customize our query
+    Query.keyword('GHRSST Level 4 CMC0.1deg Global Foundation Sea Surface Temperature Analysis').bounding_box(minx,miny,maxx,maxy).temporal(start_date,end_date)
 
-    sea_temp_xr = xr.open_zarr(fsspec.get_mapper('s3://mur-sst/zarr', anon=True),consolidated=True)
+    collections = Query.fields(['ShortName','Version']).get(10)
+
+    short_name = collections[0]["umm"]["ShortName"]
+    
+    Query = earthaccess.granule_query().short_name(short_name).version("3.0").bounding_box(minx,miny,maxx,maxy).temporal("2020-01-01","2020-01-01")
+    
+    granules = Query.get(10)
+    
+    ds_L3 = xr.open_mfdataset(
+    earthaccess.open(granules),
+    combine='nested',
+    concat_dim='time',
+    coords='minimal',
+    )
     
-    sea_temp = sea_temp_xr['analysed_sst'].sel(time=slice(start_date,end_date))
+    sea_temp = ds_L3['analysed_sst'].sel(lat=lat_med,lon=lon_med,method='nearest').load()
     
-    sst = round(sea_temp.sel(lat=lat_med,lon=lon_med,method='nearest').load().values[0] - 273,2)
+    sst = round(np.nanmedian(sea_temp.values)-273,2)
     
     return sst
 
 def refraction_correction(water_temp, water_surface, wavelength, photon_ref_elev, ph_ref_azimuth, photon_z, photon_x, photon_y, ph_conf, satellite_altitude):
     
     '''
     WTemp; there is python library that pulls water temp data
```

### Comparing `cshelph-2.5.0/setup.py` & `cshelph-2.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 #
 #
 # Purpose:  Installation of the C-SHELPh software
 #
 # Author: Nathan Thomas
 # Email: nmthomas28@gmail.com
 # Date: 05/05/2023
-# Version: 2.5.0
+# Version: 2.6.0
 #
 # History:
 # Version 2.5.0
 
 from distutils.core import setup
 import os
 
 setup(name='cshelph',
-    version='2.5.0',
+    version='2.6.0',
     description='Classification of Sub-aquatic Height Extracted Photons',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Nathan Thomas and Brian Lee',
     author_email='nmthomas28@gmail.com',
     scripts=['cshelph.py'],
     package_dir={},
```

