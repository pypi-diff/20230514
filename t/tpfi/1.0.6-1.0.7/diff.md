# Comparing `tmp/tpfi-1.0.6.tar.gz` & `tmp/tpfi-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpfi-1.0.6.tar", max compression
+gzip compressed data, was "tpfi-1.0.7.tar", max compression
```

## Comparing `tpfi-1.0.6.tar` & `tpfi-1.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-05-12 04:17:51.238296 tpfi-1.0.6/LICENSE
--rw-r--r--   0        0        0     2271 2023-05-12 04:17:51.594298 tpfi-1.0.6/README.md
--rw-r--r--   0        0        0      563 2023-05-12 04:17:51.246296 tpfi-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      154 2023-05-12 04:17:51.246296 tpfi-1.0.6/src/tpfi/__init__.py
--rw-r--r--   0        0        0    15241 2023-05-12 04:17:51.246296 tpfi-1.0.6/src/tpfi/tpfi.py
--rw-r--r--   0        0        0     5333 2023-05-12 04:17:51.246296 tpfi-1.0.6/src/tpfi/utils.py
--rw-r--r--   0        0        0       22 2023-05-12 04:17:51.246296 tpfi-1.0.6/src/tpfi/version.py
--rw-r--r--   0        0        0     2950 1970-01-01 00:00:00.000000 tpfi-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-13 12:14:06.001297 tpfi-1.0.7/LICENSE
+-rw-r--r--   0        0        0     2367 2023-05-13 12:14:06.301303 tpfi-1.0.7/README.md
+-rw-r--r--   0        0        0      563 2023-05-13 12:14:06.009297 tpfi-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-05-13 12:14:06.009297 tpfi-1.0.7/src/tpfi/__init__.py
+-rw-r--r--   0        0        0    15241 2023-05-13 12:14:06.009297 tpfi-1.0.7/src/tpfi/tpfi.py
+-rw-r--r--   0        0        0     5333 2023-05-13 12:14:06.009297 tpfi-1.0.7/src/tpfi/utils.py
+-rw-r--r--   0        0        0       22 2023-05-13 12:14:06.009297 tpfi-1.0.7/src/tpfi/version.py
+-rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 tpfi-1.0.7/PKG-INFO
```

### Comparing `tpfi-1.0.6/LICENSE` & `tpfi-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tpfi-1.0.6/README.md` & `tpfi-1.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 
 ![alt text](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/k2.png)
 
 ![alt text](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/tess.png)
 
 The `plot_identification` function creates identification charts, which are useful 
 for determining if a target is contaminated by nearby stars. In each chart, the 
-right panel displays the target (marked by a cross symbol) and nearby stars. The 
-circle size indicates their relative brightness. The left panel displays the same 
-sky coverage but from the [DSS2 Red survey](https://skyview.gsfc.nasa.gov/current/cgi/moreinfo.pl?survey=DSS2%20Red).
+right panel overlays the Gaia DR3 catalog onto the TESS Target Pixel Files (TPF) 
+with the target marked by a cross symbol. The circle size represents the relative 
+brightness of the stars according to Gaia G magnitude. The left panel displays the 
+same sky coverage but taken from the 
+[DSS2 Red survey](https://skyview.gsfc.nasa.gov/current/cgi/moreinfo.pl?survey=DSS2%20Red).
 
 This function is revised based on 
 [_tpfplotter_](https://github.com/jlillo/tpfplotter). 
 
 ---
 
 **Plot season charts for Kepler targets.**
```

### Comparing `tpfi-1.0.6/pyproject.toml` & `tpfi-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tpfi"
-version = "1.0.6"
+version = "1.0.7"
 description = "Plot identification charts for Kepler, K2 and TESS."
 authors = ["Keyu Xing <kyxing@mail.bnu.edu.cn>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/keyuxing/tpfi"
 repository = "https://github.com/keyuxing/tpfi"
```

### Comparing `tpfi-1.0.6/src/tpfi/tpfi.py` & `tpfi-1.0.7/src/tpfi/tpfi.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             coords = coords_j2000.apply_space_motion(new_obstime=REF_EPOCH)
     else:
         coords = SkyCoord(ra, dec, frame="icrs")
 
     j = Gaia.cone_search_async(coords, radius, columns=["source_id", "phot_g_mean_mag", "ra", "dec", "pmra", "pmdec"])
     r = j.get_results()
 
-    if not (r["dist"] < 3 / 3600).any():
+    if not (r["dist"] < 4 / 3600).any():
         if verbose:
             print("Target not found in Gaia DR3")
         return None
     else:
         if verbose:
             print(f"Target Gaia Source DR3 ID: {r[0]['source_id']}")
         return r
```

### Comparing `tpfi-1.0.6/src/tpfi/utils.py` & `tpfi-1.0.7/src/tpfi/utils.py`

 * *Files identical despite different names*

### Comparing `tpfi-1.0.6/PKG-INFO` & `tpfi-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpfi
-Version: 1.0.6
+Version: 1.0.7
 Summary: Plot identification charts for Kepler, K2 and TESS.
 Home-page: https://github.com/keyuxing/tpfi
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -34,17 +34,19 @@
 
 ![alt text](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/k2.png)
 
 ![alt text](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/tess.png)
 
 The `plot_identification` function creates identification charts, which are useful 
 for determining if a target is contaminated by nearby stars. In each chart, the 
-right panel displays the target (marked by a cross symbol) and nearby stars. The 
-circle size indicates their relative brightness. The left panel displays the same 
-sky coverage but from the [DSS2 Red survey](https://skyview.gsfc.nasa.gov/current/cgi/moreinfo.pl?survey=DSS2%20Red).
+right panel overlays the Gaia DR3 catalog onto the TESS Target Pixel Files (TPF) 
+with the target marked by a cross symbol. The circle size represents the relative 
+brightness of the stars according to Gaia G magnitude. The left panel displays the 
+same sky coverage but taken from the 
+[DSS2 Red survey](https://skyview.gsfc.nasa.gov/current/cgi/moreinfo.pl?survey=DSS2%20Red).
 
 This function is revised based on 
 [_tpfplotter_](https://github.com/jlillo/tpfplotter). 
 
 ---
 
 **Plot season charts for Kepler targets.**
```

