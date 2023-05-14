# Comparing `tmp/dearwatson-0.7.0.tar.gz` & `tmp/dearwatson-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dearwatson-0.7.0.tar", last modified: Fri Apr 14 18:49:27 2023, max compression
+gzip compressed data, was "dearwatson-0.7.1.tar", last modified: Sun May 14 14:29:57 2023, max compression
```

## Comparing `dearwatson-0.7.0.tar` & `dearwatson-0.7.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.644649 dearwatson-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 18:49:15.000000 dearwatson-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 18:49:15.000000 dearwatson-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-14 18:49:27.644649 dearwatson-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-14 18:49:15.000000 dearwatson-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.640649 dearwatson-0.7.0/dearwatson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-14 18:49:27.000000 dearwatson-0.7.0/dearwatson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-14 18:49:27.000000 dearwatson-0.7.0/dearwatson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:49:27.000000 dearwatson-0.7.0/dearwatson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-14 18:49:27.000000 dearwatson-0.7.0/dearwatson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 18:49:27.000000 dearwatson-0.7.0/dearwatson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:49:27.644649 dearwatson-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 18:49:16.000000 dearwatson-0.7.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 18:49:16.000000 dearwatson-0.7.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.640649 dearwatson-0.7.0/watson/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.640649 dearwatson-0.7.0/watson/data_validation_report/
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/data_validation_report/DvrPreparer.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/data_validation_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/neighbours.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.640649 dearwatson-0.7.0/watson/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.640649 dearwatson-0.7.0/watson/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/resources/images/sherlock3.png
--rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/resources/images/watson.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.644649 dearwatson-0.7.0/watson/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:17.000000 dearwatson-0.7.0/watson/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-14 18:49:17.000000 dearwatson-0.7.0/watson/tests/test_watson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.644649 dearwatson-0.7.0/watson/tpfplotterSub/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:49:18.000000 dearwatson-0.7.0/watson/tpfplotterSub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-04-14 18:49:18.000000 dearwatson-0.7.0/watson/tpfplotterSub/tpfplotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-14 18:49:18.000000 dearwatson-0.7.0/watson/tpfplotterSub/tpfplotter_py2.py
--rw-r--r--   0 runner    (1001) docker     (123)   106233 2023-04-14 18:49:17.000000 dearwatson-0.7.0/watson/watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:29:57.522244 dearwatson-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-14 14:29:42.000000 dearwatson-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 14:29:42.000000 dearwatson-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-14 14:29:57.522244 dearwatson-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-14 14:29:42.000000 dearwatson-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:29:57.514244 dearwatson-0.7.1/dearwatson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-14 14:29:57.000000 dearwatson-0.7.1/dearwatson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-14 14:29:57.000000 dearwatson-0.7.1/dearwatson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:29:57.000000 dearwatson-0.7.1/dearwatson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-14 14:29:57.000000 dearwatson-0.7.1/dearwatson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 14:29:57.000000 dearwatson-0.7.1/dearwatson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:29:57.522244 dearwatson-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-14 14:29:43.000000 dearwatson-0.7.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-14 14:29:43.000000 dearwatson-0.7.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:29:57.514244 dearwatson-0.7.1/watson/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-14 14:29:43.000000 dearwatson-0.7.1/watson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-14 14:29:43.000000 dearwatson-0.7.1/watson/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:29:57.518244 dearwatson-0.7.1/watson/data_validation_report/
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-14 14:29:43.000000 dearwatson-0.7.1/watson/data_validation_report/DvrPreparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 14:29:43.000000 dearwatson-0.7.1/watson/data_validation_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-14 14:29:43.000000 dearwatson-0.7.1/watson/neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-05-14 14:29:43.000000 dearwatson-0.7.1/watson/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:29:57.510244 dearwatson-0.7.1/watson/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:29:57.518244 dearwatson-0.7.1/watson/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-05-14 14:29:43.000000 dearwatson-0.7.1/watson/resources/images/sherlock3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-05-14 14:29:43.000000 dearwatson-0.7.1/watson/resources/images/watson.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:29:57.518244 dearwatson-0.7.1/watson/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:29:43.000000 dearwatson-0.7.1/watson/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-14 14:29:43.000000 dearwatson-0.7.1/watson/tests/test_watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:29:57.522244 dearwatson-0.7.1/watson/tpfplotterSub/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:29:44.000000 dearwatson-0.7.1/watson/tpfplotterSub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-05-14 14:29:45.000000 dearwatson-0.7.1/watson/tpfplotterSub/tpfplotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-14 14:29:45.000000 dearwatson-0.7.1/watson/tpfplotterSub/tpfplotter_py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105984 2023-05-14 14:29:43.000000 dearwatson-0.7.1/watson/watson.py
```

### Comparing `dearwatson-0.7.0/LICENSE` & `dearwatson-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.0/PKG-INFO` & `dearwatson-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.7.0
+Version: 0.7.1
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.7.0/README.md` & `dearwatson-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.0/dearwatson.egg-info/PKG-INFO` & `dearwatson-0.7.1/dearwatson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.7.0
+Version: 0.7.1
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.7.0/dearwatson.egg-info/SOURCES.txt` & `dearwatson-0.7.1/dearwatson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.0/setup.py` & `dearwatson-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-version = "0.7.0"
+version = "0.7.1"
 setuptools.setup(
     name="dearwatson", # Replace with your own username
     version=version,
     author="M. Dévora-Pajares",
     author_email="mdevorapajares@protonmail.com",
     description="Visual Vetting and Analysis of Transits from Space ObservatioNs",
     long_description=long_description,
```

### Comparing `dearwatson-0.7.0/watson/data_validation_report/DvrPreparer.py` & `dearwatson-0.7.1/watson/data_validation_report/DvrPreparer.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.0/watson/neighbours.py` & `dearwatson-0.7.1/watson/neighbours.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.0/watson/report.py` & `dearwatson-0.7.1/watson/report.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.0/watson/resources/images/sherlock3.png` & `dearwatson-0.7.1/watson/resources/images/sherlock3.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.0/watson/resources/images/watson.png` & `dearwatson-0.7.1/watson/resources/images/watson.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.0/watson/tests/test_watson.py` & `dearwatson-0.7.1/watson/tests/test_watson.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.0/watson/tpfplotterSub/tpfplotter.py` & `dearwatson-0.7.1/watson/tpfplotterSub/tpfplotter.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.0/watson/tpfplotterSub/tpfplotter_py2.py` & `dearwatson-0.7.1/watson/tpfplotterSub/tpfplotter_py2.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.0/watson/watson.py` & `dearwatson-0.7.1/watson/watson.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,18 +270,14 @@
             self.plot_folded_curve(self.data_dir, id, lc, period, t0, duration, depth / 1000, rp_rstar, a_rstar)
         metrics_df = metrics_df.append({'metric': 'snr_p_t0', 'score': snr_p_t0, 'passed': snr_p_t0 > 3}, ignore_index=True)
         metrics_df = metrics_df.append({'metric': 'snr_p_2t0', 'score': snr_p_2t0, 'passed': snr_p_2t0 < 3}, ignore_index=True)
         metrics_df = metrics_df.append({'metric': 'snr_2p_t0', 'score': snr_2p_t0, 'passed': snr_2p_t0 > 3}, ignore_index=True)
         metrics_df = metrics_df.append({'metric': 'snr_2p_2t0', 'score': snr_2p_2t0, 'passed': snr_2p_2t0 > 3}, ignore_index=True)
         metrics_df = metrics_df.append({'metric': 'snr_p2_t0', 'score': snr_p2_t0, 'passed': snr_p2_t0 < 3}, ignore_index=True)
         metrics_df = metrics_df.append({'metric': 'snr_p2_t02', 'score': snr_p2_t02, 'passed': snr_p2_t02 < 3}, ignore_index=True)
-        metrics_df = metrics_df.append({'metric': 'snr_p_score', 'score': snr_p_2t0 / snr_p_t0,
-                                        'passed': snr_p_t0 > 3 and snr_p_2t0 < 3}, ignore_index=True)
-        metrics_df = metrics_df.append({'metric': 'snr_2p_score', 'score': np.abs(snr_2p_t0 - snr_2p_2t0), 'passed': snr_2p_t0 > 3 and snr_2p_t0 > 3}, ignore_index=True)
-        metrics_df = metrics_df.append({'metric': 'snr_p2_score', 'score': np.abs(snr_p2_t0 - snr_p2_t02) / snr_p_t0, 'passed': snr_p2_t0 < 3 and snr_p2_t02 < 3}, ignore_index=True)
         if (ra_fov is not None and dec_fov is not None):
             if tpfs is not None and len(tpfs) > 0:
                 offset_ra, offset_dec, offset_err, distance_sub_arcs, core_flux_snr, halo_flux_snr, og_score, \
                 centroids_ra_snr, centroids_dec_snr =\
                     Watson.plot_folded_tpfs(self.data_dir, mission_prefix, mission, target_id, ra_fov, dec_fov, lc, lc_data,
                                         tpfs, lc_file, lc_data_file, tpfs_dir, sectors, period, t0, duration, depth / 1000,
                                         rp_rstar, a_rstar, transits_mask, transit_t0s_list, apertures, cpus)
@@ -1117,14 +1113,18 @@
         source_offset_bls_dec = np.nanmedian(np.array(source_offsets_bls)[:, 1])
         source_offset_bls_ra_err = np.nanstd(np.array(source_offsets_bls)[:, 0])
         source_offset_bls_dec_err = np.nanstd(np.array(source_offsets_bls)[:, 1])
         offset_ra = np.mean([source_offset_bls_ra, source_offset_diggimg_ra])
         offset_dec = np.mean([source_offset_bls_dec, source_offset_diggimg_dec])
         offset_ra_err = 1/2 * np.sqrt(source_offset_bls_ra_err ** 2 + source_offset_diggimg_ra_err ** 2)
         offset_dec_err = 1/2 * np.sqrt(source_offset_bls_dec_err ** 2 + source_offset_diggimg_dec_err ** 2)
+        if np.isnan(offset_ra_err) or offset_ra_err == 0.0:
+            offset_ra_err = np.nanstd([source_offset_bls_ra, source_offset_diggimg_ra])
+        if np.isnan(offset_dec_err) or offset_dec_err == 0.0:
+            offset_dec_err = np.nanstd([source_offset_bls_dec, source_offset_diggimg_dec])
         offsets_df = pd.DataFrame(columns=['name', 'ra', 'dec', 'ra_err', 'dec_err'])
         offsets_df.append({'name': 'diff_img', 'ra': source_offset_diggimg_ra, 'dec': source_offset_diggimg_dec,
                            'ra_err': source_offset_diggimg_ra_err, 'dec_err': source_offset_diggimg_dec_err}, ignore_index=True)
         offsets_df.append({'name': 'px_bls', 'ra': source_offset_bls_ra, 'dec': source_offset_bls_dec,
                            'ra_err': source_offset_bls_ra_err, 'dec_err': source_offset_bls_dec_err}, ignore_index=True)
         offsets_df.append({'name': 'mean', 'ra': offset_ra, 'dec': offset_dec,
                            'ra_err': offset_ra_err, 'dec_err': offset_dec_err}, ignore_index=True)
```

