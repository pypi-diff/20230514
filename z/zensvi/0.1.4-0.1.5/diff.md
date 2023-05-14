# Comparing `tmp/zensvi-0.1.4.tar.gz` & `tmp/zensvi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.1.4.tar", max compression
+gzip compressed data, was "zensvi-0.1.5.tar", max compression
```

## Comparing `zensvi-0.1.4.tar` & `zensvi-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.1.4/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.1.4/README.md
--rwxr-xr-x   0        0        0      694 2023-05-14 13:07:47.290546 zensvi-0.1.4/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.1.4/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.1.4/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.1.4/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    38123 2023-05-14 01:59:06.770688 zensvi-0.1.4/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       55 2023-05-14 01:59:06.771355 zensvi-0.1.4/src/zensvi/download/__init__.py
--rwxr-xr-x   0        0        0    14464 2023-05-14 13:02:40.359162 zensvi-0.1.4/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.1.4/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.1.4/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8453 2023-05-14 12:56:31.947059 zensvi-0.1.4/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.1.4/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.1.4/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     8149 2023-05-14 12:56:31.947970 zensvi-0.1.4/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.1.4/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.1.4/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0     6500 2023-05-14 01:59:06.778828 zensvi-0.1.4/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.1.4/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 zensvi-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.1.5/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.1.5/README.md
+-rwxr-xr-x   0        0        0      694 2023-05-14 13:26:50.320956 zensvi-0.1.5/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.1.5/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.1.5/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.1.5/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    38123 2023-05-14 01:59:06.770688 zensvi-0.1.5/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       55 2023-05-14 01:59:06.771355 zensvi-0.1.5/src/zensvi/download/__init__.py
+-rwxr-xr-x   0        0        0    14464 2023-05-14 13:02:40.359162 zensvi-0.1.5/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.1.5/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.1.5/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8291 2023-05-14 13:25:54.052907 zensvi-0.1.5/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.1.5/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.1.5/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     8149 2023-05-14 12:56:31.947970 zensvi-0.1.5/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.1.5/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.1.5/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0     6500 2023-05-14 01:59:06.778828 zensvi-0.1.5/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.1.5/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 zensvi-0.1.5/PKG-INFO
```

### Comparing `zensvi-0.1.4/LICENSE` & `zensvi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.4/README.md` & `zensvi-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.4/pyproject.toml` & `zensvi-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.1.4"
+version = "0.1.5"
 description = "This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `zensvi-0.1.4/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.1.5/src/zensvi/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.4/src/zensvi/download/streetview_downloader.py` & `zensvi-0.1.5/src/zensvi/download/streetview_downloader.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.4/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.1.5/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.4/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.1.5/src/zensvi/download/utils/geoprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -142,19 +142,18 @@
                 
                 for future in tqdm(as_completed(batch_futures.keys()), total=len(batch_futures), desc=f"Processing polygon for batch #{i+1}"):
                     geom = batch_futures[future]
                     try:
                         result = future.result()
                         results.append(result)
                     except (ValueError, networkx.exception.NetworkXPointlessConcept):
-                        tqdm.write("Found no graph nodes within the polygon or connectivity is undefined for the null graph. Store the polygon as a failed geom and retry later")
                         failed_geoms.append(geom)
 
         if len(failed_geoms) > 0:
-            print("Retrying failed geoms")
+            print("Retrying failed geoms by making grids")
             with ProcessPoolExecutor() as executor:
                 retry_futures = {}
                 for geom in tqdm(failed_geoms, desc="Preparing Failed Geoms"):
                     future = executor.submit(self.create_point_grid, geom, self.grid_size)
                     retry_futures[future] = geom
                 
                 for future in tqdm(as_completed(retry_futures.keys()), total=len(retry_futures), desc="Processing Failed Geoms"):
```

### Comparing `zensvi-0.1.4/src/zensvi/download/utils/get_pids.py` & `zensvi-0.1.5/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.4/src/zensvi/download/utils/helpers.py` & `zensvi-0.1.5/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.4/src/zensvi/download/utils/imtool.py` & `zensvi-0.1.5/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.4/src/zensvi/download/utils/proxies.csv` & `zensvi-0.1.5/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.4/src/zensvi/transform/transform_image.py` & `zensvi-0.1.5/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.4/PKG-INFO` & `zensvi-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.1.4
+Version: 0.1.5
 Summary: This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

