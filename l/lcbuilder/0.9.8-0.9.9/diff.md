# Comparing `tmp/lcbuilder-0.9.8.tar.gz` & `tmp/lcbuilder-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcbuilder-0.9.8.tar", last modified: Thu Dec  8 16:27:15 2022, max compression
+gzip compressed data, was "lcbuilder-0.9.9.tar", last modified: Thu Dec  8 16:32:09 2022, max compression
```

## Comparing `lcbuilder-0.9.8.tar` & `lcbuilder-0.9.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:15.759056 lcbuilder-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      567 2022-12-08 16:27:15.759056 lcbuilder-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:15.747056 lcbuilder-0.9.8/lcbuilder/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/HarmonicSelector.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/LcBuild.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:15.747056 lcbuilder-0.9.8/lcbuilder/curve_preparer/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/curve_preparer/CurvePreparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/curve_preparer/Flattener.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/curve_preparer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:15.751056 lcbuilder-0.9.8/lcbuilder/eleanor/
--rwxr-xr-x   0 runner    (1001) docker     (123)      262 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/crossmatch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      945 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/eleanor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20427 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/ffi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/fill_grid.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     8060 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/mast.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/maxsector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:15.751056 lcbuilder-0.9.8/lcbuilder/eleanor/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)   278730 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/metadata/ffi.guide
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10540 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/postcard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/postcard_centers.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    20387 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/source.py
--rw-r--r--   0 runner    (1001) docker     (123)    72348 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/targetdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:15.751056 lcbuilder-0.9.8/lcbuilder/eleanor/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/tests/test_ffi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/tests/test_mast.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/tests/test_postcard.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/tests/test_targetdata.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/tests/test_visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/update.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15236 2022-12-08 16:27:06.000000 lcbuilder-0.9.8/lcbuilder/eleanor/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/eleanor_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    40353 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/lcbuilder_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:15.755056 lcbuilder-0.9.8/lcbuilder/objectinfo/
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/objectinfo/InputObjectInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/objectinfo/InvalidNumberOfSectorsError.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/objectinfo/MissionInputObjectInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/objectinfo/MissionObjectInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/objectinfo/ObjectInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/objectinfo/ObjectProcessingError.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/objectinfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:15.755056 lcbuilder-0.9.8/lcbuilder/objectinfo/preparer/
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/objectinfo/preparer/LightcurveBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/objectinfo/preparer/MissionInputLightcurveBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/objectinfo/preparer/MissionLightcurveBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/objectinfo/preparer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:15.755056 lcbuilder-0.9.8/lcbuilder/photometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/photometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/photometry/aperture_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:15.755056 lcbuilder-0.9.8/lcbuilder/star/
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/star/EpicStarCatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/star/HabitabilityCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/star/KicStarCatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/star/StarCatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/star/TicStarCatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/star/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/star/starinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:15.759056 lcbuilder-0.9.8/lcbuilder/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   268237 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/tests/input.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/tests/test_apertures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/tests/test_harmonics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/lcbuilder/tests/test_lcbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:27:15.747056 lcbuilder-0.9.8/lcbuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2022-12-08 16:27:15.000000 lcbuilder-0.9.8/lcbuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2022-12-08 16:27:15.000000 lcbuilder-0.9.8/lcbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 16:27:15.000000 lcbuilder-0.9.8/lcbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2022-12-08 16:27:15.000000 lcbuilder-0.9.8/lcbuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-08 16:27:15.000000 lcbuilder-0.9.8/lcbuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 16:27:15.759056 lcbuilder-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2022-12-08 16:27:05.000000 lcbuilder-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:32:09.124437 lcbuilder-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2022-12-08 16:32:09.124437 lcbuilder-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:32:09.116437 lcbuilder-0.9.9/lcbuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/HarmonicSelector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/LcBuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:32:09.116437 lcbuilder-0.9.9/lcbuilder/curve_preparer/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/curve_preparer/CurvePreparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/curve_preparer/Flattener.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/curve_preparer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:32:09.120437 lcbuilder-0.9.9/lcbuilder/eleanor/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      262 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/crossmatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      945 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/eleanor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20427 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/ffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/fill_grid.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8060 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/mast.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/maxsector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:32:09.120437 lcbuilder-0.9.9/lcbuilder/eleanor/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)   278730 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/metadata/ffi.guide
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10540 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/postcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/postcard_centers.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20387 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72348 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/targetdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:32:09.120437 lcbuilder-0.9.9/lcbuilder/eleanor/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/tests/test_ffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/tests/test_mast.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/tests/test_postcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/tests/test_targetdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/tests/test_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/update.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15236 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/eleanor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40353 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/lcbuilder_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:32:09.120437 lcbuilder-0.9.9/lcbuilder/objectinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/objectinfo/InputObjectInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/objectinfo/InvalidNumberOfSectorsError.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/objectinfo/MissionInputObjectInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/objectinfo/MissionObjectInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/objectinfo/ObjectInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/objectinfo/ObjectProcessingError.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/objectinfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:32:09.120437 lcbuilder-0.9.9/lcbuilder/objectinfo/preparer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/objectinfo/preparer/LightcurveBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/objectinfo/preparer/MissionInputLightcurveBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/objectinfo/preparer/MissionLightcurveBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/objectinfo/preparer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:32:09.120437 lcbuilder-0.9.9/lcbuilder/photometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/photometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/photometry/aperture_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:32:09.124437 lcbuilder-0.9.9/lcbuilder/star/
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/star/EpicStarCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/star/HabitabilityCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/star/KicStarCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/star/StarCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/star/TicStarCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/star/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/star/starinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:32:09.124437 lcbuilder-0.9.9/lcbuilder/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   268237 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/tests/input.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/tests/test_apertures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/tests/test_harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/lcbuilder/tests/test_lcbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 16:32:09.116437 lcbuilder-0.9.9/lcbuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2022-12-08 16:32:09.000000 lcbuilder-0.9.9/lcbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2022-12-08 16:32:09.000000 lcbuilder-0.9.9/lcbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 16:32:09.000000 lcbuilder-0.9.9/lcbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2022-12-08 16:32:09.000000 lcbuilder-0.9.9/lcbuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-08 16:32:09.000000 lcbuilder-0.9.9/lcbuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 16:32:09.124437 lcbuilder-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2022-12-08 16:31:59.000000 lcbuilder-0.9.9/setup.py
```

### Comparing `lcbuilder-0.9.8/LICENSE` & `lcbuilder-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/PKG-INFO` & `lcbuilder-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcbuilder
-Version: 0.9.8
+Version: 0.9.9
 Summary: Easy light curve builder from multiple sources
 Home-page: https://github.com/PlanetHunders/lcbuilder
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: # lcbuilder
         Easy light curve builder from multiple sources
```

### Comparing `lcbuilder-0.9.8/lcbuilder/HarmonicSelector.py` & `lcbuilder-0.9.9/lcbuilder/HarmonicSelector.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/LcBuild.py` & `lcbuilder-0.9.9/lcbuilder/LcBuild.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/constants.py` & `lcbuilder-0.9.9/lcbuilder/constants.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/curve_preparer/Flattener.py` & `lcbuilder-0.9.9/lcbuilder/curve_preparer/Flattener.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/crossmatch.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/crossmatch.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/eleanor.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/eleanor.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/ffi.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/ffi.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/fill_grid.cpp` & `lcbuilder-0.9.9/lcbuilder/eleanor/fill_grid.cpp`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/mast.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/mast.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/metadata/ffi.guide` & `lcbuilder-0.9.9/lcbuilder/eleanor/metadata/ffi.guide`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/models.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/models.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/postcard.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/postcard.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/postcard_centers.txt` & `lcbuilder-0.9.9/lcbuilder/eleanor/postcard_centers.txt`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/source.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/source.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/targetdata.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/targetdata.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/tests/test_ffi.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/tests/test_ffi.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/tests/test_mast.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/tests/test_mast.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/tests/test_targetdata.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/tests/test_targetdata.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/update.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/update.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor/visualize.py` & `lcbuilder-0.9.9/lcbuilder/eleanor/visualize.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/eleanor_manager.py` & `lcbuilder-0.9.9/lcbuilder/eleanor_manager.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/helper.py` & `lcbuilder-0.9.9/lcbuilder/helper.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/lcbuilder_class.py` & `lcbuilder-0.9.9/lcbuilder/lcbuilder_class.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/objectinfo/InputObjectInfo.py` & `lcbuilder-0.9.9/lcbuilder/objectinfo/InputObjectInfo.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/objectinfo/MissionInputObjectInfo.py` & `lcbuilder-0.9.9/lcbuilder/objectinfo/MissionInputObjectInfo.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/objectinfo/MissionObjectInfo.py` & `lcbuilder-0.9.9/lcbuilder/objectinfo/MissionObjectInfo.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/objectinfo/ObjectInfo.py` & `lcbuilder-0.9.9/lcbuilder/objectinfo/ObjectInfo.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/objectinfo/preparer/LightcurveBuilder.py` & `lcbuilder-0.9.9/lcbuilder/objectinfo/preparer/LightcurveBuilder.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/objectinfo/preparer/MissionInputLightcurveBuilder.py` & `lcbuilder-0.9.9/lcbuilder/objectinfo/preparer/MissionInputLightcurveBuilder.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/objectinfo/preparer/MissionLightcurveBuilder.py` & `lcbuilder-0.9.9/lcbuilder/objectinfo/preparer/MissionLightcurveBuilder.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/photometry/aperture_extractor.py` & `lcbuilder-0.9.9/lcbuilder/photometry/aperture_extractor.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/star/EpicStarCatalog.py` & `lcbuilder-0.9.9/lcbuilder/star/EpicStarCatalog.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/star/HabitabilityCalculator.py` & `lcbuilder-0.9.9/lcbuilder/star/HabitabilityCalculator.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/star/KicStarCatalog.py` & `lcbuilder-0.9.9/lcbuilder/star/KicStarCatalog.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/star/TicStarCatalog.py` & `lcbuilder-0.9.9/lcbuilder/star/TicStarCatalog.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/star/starinfo.py` & `lcbuilder-0.9.9/lcbuilder/star/starinfo.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/tests/input.csv` & `lcbuilder-0.9.9/lcbuilder/tests/input.csv`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/tests/test_apertures.py` & `lcbuilder-0.9.9/lcbuilder/tests/test_apertures.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/tests/test_harmonics.py` & `lcbuilder-0.9.9/lcbuilder/tests/test_harmonics.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder/tests/test_lcbuilder.py` & `lcbuilder-0.9.9/lcbuilder/tests/test_lcbuilder.py`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/lcbuilder.egg-info/PKG-INFO` & `lcbuilder-0.9.9/lcbuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcbuilder
-Version: 0.9.8
+Version: 0.9.9
 Summary: Easy light curve builder from multiple sources
 Home-page: https://github.com/PlanetHunders/lcbuilder
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: # lcbuilder
         Easy light curve builder from multiple sources
```

### Comparing `lcbuilder-0.9.8/lcbuilder.egg-info/SOURCES.txt` & `lcbuilder-0.9.9/lcbuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lcbuilder-0.9.8/setup.py` & `lcbuilder-0.9.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = "0.9.8"
+version = "0.9.9"
 setuptools.setup(
     name="lcbuilder", # Replace with your own username
     version=version,
     author="M. Dévora-Pajares",
     author_email="mdevorapajares@protonmail.com",
     description="Easy light curve builder from multiple sources",
     long_description=long_description,
```

