# Comparing `tmp/gnssrefl-1.3.7.tar.gz` & `tmp/gnssrefl-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-1.3.7.tar", last modified: Wed Apr 26 08:55:56 2023, max compression
+gzip compressed data, was "gnssrefl-1.3.8.tar", last modified: Thu May  4 13:57:01 2023, max compression
```

## Comparing `gnssrefl-1.3.7.tar` & `gnssrefl-1.3.8.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:55:56.971593 gnssrefl-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-26 08:55:56.971593 gnssrefl-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:55:56.947593 gnssrefl-1.3.7/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:55:56.947593 gnssrefl-1.3.7/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/felipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/filesizes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gnssir.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (123)   174790 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/make_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/nmea2snr_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34303 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/quickLook_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5882 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/quickPhase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/quickPhase_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49164 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rinex3_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    58967 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/vwc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:55:56.947593 gnssrefl-1.3.7/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-26 08:55:56.000000 gnssrefl-1.3.7/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-26 08:55:56.000000 gnssrefl-1.3.7/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:55:56.000000 gnssrefl-1.3.7/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-26 08:55:56.000000 gnssrefl-1.3.7/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 08:55:56.000000 gnssrefl-1.3.7/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 08:55:56.000000 gnssrefl-1.3.7/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:55:56.971593 gnssrefl-1.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:55:56.967593 gnssrefl-1.3.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-26 08:55:42.000000 gnssrefl-1.3.7/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:01.763013 gnssrefl-1.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-04 13:57:01.763013 gnssrefl-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:01.731013 gnssrefl-1.3.8/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:01.731013 gnssrefl-1.3.8/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/felipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/filesizes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gnssir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (123)   174227 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/make_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/nmea2snr_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34303 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/quickLook_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5882 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/quickPhase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/quickPhase_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/quicklib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49164 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rinex3_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58967 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/vwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:01.731013 gnssrefl-1.3.8/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-04 13:57:01.000000 gnssrefl-1.3.8/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-04 13:57:01.000000 gnssrefl-1.3.8/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:57:01.000000 gnssrefl-1.3.8/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-04 13:57:01.000000 gnssrefl-1.3.8/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 13:57:01.000000 gnssrefl-1.3.8/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 13:57:01.000000 gnssrefl-1.3.8/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:57:01.763013 gnssrefl-1.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:01.763013 gnssrefl-1.3.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/test/test_rinex2snr.py
```

### Comparing `gnssrefl-1.3.7/LICENSE` & `gnssrefl-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/PKG-INFO` & `gnssrefl-1.3.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.7
+Version: 1.3.8
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.3.7** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.8** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.7/README.md` & `gnssrefl-1.3.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # gnssrefl
 
-**github version: 1.3.7** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.8** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.7/gnssrefl/EGM96.py` & `gnssrefl-1.3.8/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/check_rinex_file.py` & `gnssrefl-1.3.8/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/computemp1mp2.py` & `gnssrefl-1.3.8/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/daily_avg.py` & `gnssrefl-1.3.8/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/daily_avg_cl.py` & `gnssrefl-1.3.8/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-1.3.8/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/download_ioc.py` & `gnssrefl-1.3.8/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/download_noaa.py` & `gnssrefl-1.3.8/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/download_orbits.py` & `gnssrefl-1.3.8/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/download_psmsl.py` & `gnssrefl-1.3.8/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/download_rinex.py` & `gnssrefl-1.3.8/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/download_teqc.py` & `gnssrefl-1.3.8/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/download_tides.py` & `gnssrefl-1.3.8/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/download_unr.py` & `gnssrefl-1.3.8/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/download_wsv.py` & `gnssrefl-1.3.8/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/felipe.py` & `gnssrefl-1.3.8/gnssrefl/felipe.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/filesizes.py` & `gnssrefl-1.3.8/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/gnssir.py` & `gnssrefl-1.3.8/gnssrefl/gnssir.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/gnssir_cl.py` & `gnssrefl-1.3.8/gnssrefl/gnssir_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/gnsssnr.f` & `gnssrefl-1.3.8/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/gnsssnrbigger.f` & `gnssrefl-1.3.8/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/gps.py` & `gnssrefl-1.3.8/gnssrefl/gps.py`

 * *Files 0% similar despite different names*

```diff
@@ -767,40 +767,30 @@
     if (mgex == 1):
         name = file1[:-2]
 
     if not foundit:
         print('Type 1 filename',file1)
         print('Type 2 filename',file2)
         if (mgex == 0):
-            if (igps_week > 2137):
-            # filename without the compression ending
+            if not foundit:
                 name = file2[:-3] 
                 secure_file = file2
-                print('check the correct GPS week ')
                 secure_dir = '/gps/products/mgex/' + str(igps_week) + '/'
                 foundit = orbfile_cddis(name, year, secure_file, secure_dir, file2)
-
-                if not foundit:
-                    #print('use the wrong GPS week at CDDIS')
-                    # test newest nonsense
-                    print('check a different directory week because CDDIS has changed their file structure')
-                    # kluge for a CDDIS screwup when they put the orbits in the wrong
-                    # GPS week directory
-                    #secure_dir = '/gps/products/mgex/' + str(igps_week_at_cddis) + '/'
-                    secure_dir = '/gps/products/' + str(igps_week) + '/'
-                    foundit = orbfile_cddis(name, year, secure_file, secure_dir, file2)
-            else:
+            if not foundit:
+                secure_dir = '/gps/products/' + str(igps_week) + '/'
+                foundit = orbfile_cddis(name, year, secure_file, secure_dir, file2)
+            if not foundit:
                 secure_dir = '/gps/products/mgex/' + str(igps_week) + '/'
                 secure_file = file1 # Z compressed
                 name = file1[:-2]
                 foundit = orbfile_cddis(name, year, secure_file, secure_dir, file1)
-                if (not foundit):
-                    name = file2[:-3]
-                    secure_file = file2
-                    foundit = orbfile_cddis(name, year, secure_file, secure_dir, file2)
+            if (not foundit):
+                secure_dir = '/gps/products/' + str(igps_week) + '/'
+                foundit = orbfile_cddis(name, year, secure_file, secure_dir, file2)
 
     return name, fdir, foundit
 
 def orbfile_cddis(name, year, secure_file, secure_dir, file2):
     """
     tries to download a file from a directory at CDDIS
     file2 is like this: GFZ0MGXRAP_' + cyyyy + cdoy + '0000_01D_05M_ORB.SP3.gz
```

### Comparing `gnssrefl-1.3.7/gnssrefl/gpssnr.f` & `gnssrefl-1.3.8/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/gpsweek.py` & `gnssrefl-1.3.8/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/gpt_1wA.pickle` & `gnssrefl-1.3.8/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/highrate.py` & `gnssrefl-1.3.8/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/installexe_cl.py` & `gnssrefl-1.3.8/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/invsnr_cl.py` & `gnssrefl-1.3.8/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/invsnr_input.py` & `gnssrefl-1.3.8/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/karnak_libraries.py` & `gnssrefl-1.3.8/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/kelly.py` & `gnssrefl-1.3.8/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/llh2xyz.py` & `gnssrefl-1.3.8/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/make_json_input.py` & `gnssrefl-1.3.8/gnssrefl/make_json_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
         default is True.
     extension : str, optional
         provide extension name so you can try different strategies. 
         Results will then go into $REFL_CODE/YYYY/results/ssss/extension
         Default is '' 
     ediff : float
         quality control parameter (Degrees)
+        Allowed min/max elevation angle diff from requested min/max elev angle
         default is 2
     delTmax : float
         maximum allowed arc length (minutes)
         default is 75, which is a bit long for tides
     azlist : list of floats
         lets the user set the azimuth regions, in degrees
         each region must be < 100 degrees! e.g. 0 90 90 180 would be all the east
```

### Comparing `gnssrefl-1.3.7/gnssrefl/nmea2snr.py` & `gnssrefl-1.3.8/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/nmea2snr_cl.py` & `gnssrefl-1.3.8/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/phase_functions.py` & `gnssrefl-1.3.8/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/prn2gps.py` & `gnssrefl-1.3.8/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/query_unr.py` & `gnssrefl-1.3.8/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/quickLook_cl.py` & `gnssrefl-1.3.8/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/quickLook_function.py` & `gnssrefl-1.3.8/gnssrefl/quickLook_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/quickPhase.py` & `gnssrefl-1.3.8/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/quickPhase_function.py` & `gnssrefl-1.3.8/gnssrefl/quickPhase_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/quickplt.py` & `gnssrefl-1.3.8/gnssrefl/quickplt.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import datetime
 import numpy as np
 import matplotlib.pyplot as plt
 import os
 import sys
 
 
+import gnssrefl.quicklib as q
+
+
 def main():
     """
     quick file plotting using matplotlib
 
     Examples
     --------
 
@@ -68,14 +71,15 @@
     parser.add_argument("-xlabel", type=str, help="optional x-axis label", default=None)
     parser.add_argument("-ylabel", type=str, help="optional y-axis label", default=None)
     parser.add_argument("-symbol", help="plot symbol ", type=str,default=None)
     parser.add_argument("-title", help="optional title", type=str,default=None)
     parser.add_argument("-outfile", help="optional filename for plot", type=str,default=None)
     parser.add_argument("-ylimits", nargs="*",type=float, help="optional ylimits", default=None)
     parser.add_argument("-ydoy", help="if True/T, columns 1-2 are year and doy", type=str,default=None)
+    parser.add_argument("-filename2", help="second filename", type=str, default=None)
 
     args = parser.parse_args()
 
     filename = args.filename
     # change column numbers to pythonese
     xcol = int(args.xcol) - 1
     ycol = int(args.ycol) - 1
@@ -114,51 +118,34 @@
             return
         tval = []
         yval = []
     else:
         print('input file does not exist')
         sys.exit()
 
+    tvd2=[]
+    secondFile = False
+    if args.filename2 is not None:
+        filename2 = args.filename2
+        if os.path.isfile(filename2):
+            tvd2 = np.loadtxt(filename2,comments=commentsign)
+            if len(tvd2) == 0:
+                print('empty input for filenumber 2')
+                return
+            else:
+                secondFile = True
+        else:
+            print('second filename does not exist')
+
+
+    tval,yval = q.trans_time(tvd, ymd, convert_mjd, ydoy,xcol,ycol)
     if secondFile:
-        tvd2 = np.loadtxt(filename2,comments=commentsign)
-        if len(tvd2) == 0:
-            print('empty input file number 2')
-            return
+        tval2,yval2 = q.trans_time(tvd2, ymd, convert_mjd, ydoy,xcol,ycol)
 
 
-    if ymd == True:
-        year = tvd[:,0]; month = tvd[:,1]; day = tvd[:,2];
-        hour = tvd[:,3] ; minute = tvd[:,4]
-        for i in range(0,len(tvd)):
-            if (tvd[i, 4]) > 0:
-                y = int(year[i]); m = int(month[i]); d = int(day[i])
-                # i am sure there is a better way to do this
-                today=datetime.datetime(y,m,d)
-                doy = (today - datetime.datetime(today.year, 1, 1)).days + 1
-                h = int(hour[i])
-                mi = int(minute[i])
-                tval.append(y + (doy +  h/24 + mi/24/60)/365.25);
-                yval.append( tvd[i,ycol]/1000)
-    else:
-        if convert_mjd:
-            t1 = Time(tvd[:,xcol],format='mjd')
-            t1_utc = t1.utc # change to UTC
-            # probably can be done in one step!
-            tval =  t1_utc.datetime # change to datetime
-            yval = tvd[:,ycol] # save the y values
-        elif ydoy:
-            tval = tvd[:,0]  + tvd[:,1]/365.25
-            yval = tvd[:,ycol]
-            ii = np.argsort( tval)
-            tval = tval[ii]; yval=yval[ii]
-        else:
-            tval = tvd[:,xcol] ; yval = tvd[:,ycol]
-            x1 = min(tval) ; x2 = max(tval)
-            if secondFile:
-                tval2 = tvd2[:,xcol] ; yval2 = tvd2[:,ycol]
 
     fig,ax=plt.subplots()
     if args.symbol is None:
         ax.plot(tval, yval, 'b.')
     else:
         ax.plot(tval, yval, args.symbol)
```

### Comparing `gnssrefl-1.3.7/gnssrefl/read_snr_files.py` & `gnssrefl-1.3.8/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/refl_zones.py` & `gnssrefl-1.3.8/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/refl_zones_cl.py` & `gnssrefl-1.3.8/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/refraction.py` & `gnssrefl-1.3.8/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/rh_plot.py` & `gnssrefl-1.3.8/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/rinex2snr.py` & `gnssrefl-1.3.8/gnssrefl/rinex2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/rinex2snr_cl.py` & `gnssrefl-1.3.8/gnssrefl/rinex2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/rinex3_rinex2.py` & `gnssrefl-1.3.8/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/rinex3_snr.py` & `gnssrefl-1.3.8/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/rinpy.py` & `gnssrefl-1.3.8/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-1.3.8/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/smoosh.py` & `gnssrefl-1.3.8/gnssrefl/smoosh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/snow_functions.py` & `gnssrefl-1.3.8/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/snowdepth_cl.py` & `gnssrefl-1.3.8/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/spline_functions.py` & `gnssrefl-1.3.8/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/subdaily.py` & `gnssrefl-1.3.8/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/subdaily_cl.py` & `gnssrefl-1.3.8/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/utils.py` & `gnssrefl-1.3.8/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/veg_multiyr.py` & `gnssrefl-1.3.8/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/vwc.py` & `gnssrefl-1.3.8/gnssrefl/vwc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/vwc_input.py` & `gnssrefl-1.3.8/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/xyz2llh.py` & `gnssrefl-1.3.8/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/ydoy.py` & `gnssrefl-1.3.8/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl/ymd.py` & `gnssrefl-1.3.8/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-1.3.8/gnssrefl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.7
+Version: 1.3.8
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.3.7** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.8** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.7/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-1.3.8/gnssrefl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 gnssrefl/pickle_dilemma.py
 gnssrefl/prn2gps.py
 gnssrefl/query_unr.py
 gnssrefl/quickLook_cl.py
 gnssrefl/quickLook_function.py
 gnssrefl/quickPhase.py
 gnssrefl/quickPhase_function.py
+gnssrefl/quicklib.py
 gnssrefl/quickplt.py
 gnssrefl/read_snr_files.py
 gnssrefl/refl_zones.py
 gnssrefl/refl_zones_cl.py
 gnssrefl/refraction.py
 gnssrefl/rh_plot.py
 gnssrefl/rinex2snr.py
```

### Comparing `gnssrefl-1.3.7/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-1.3.8/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/pyproject.toml` & `gnssrefl-1.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.7/setup.py` & `gnssrefl-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["numpy","wget","scipy","matplotlib","requests","progress","astropy","simplekml","earthscope-sdk"]
 setup(
     name="gnssrefl",
-    version="1.3.7",
+    version="1.3.8",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-1.3.7/test/test_gps.py` & `gnssrefl-1.3.8/test/test_gps.py`

 * *Files identical despite different names*

