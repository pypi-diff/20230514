# Comparing `tmp/xtrack-0.9.4.tar.gz` & `tmp/xtrack-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xtrack-0.9.4.tar", last modified: Tue Mar  8 21:42:00 2022, max compression
+gzip compressed data, was "dist/xtrack-0.9.5.tar", last modified: Thu Mar 10 15:00:54 2022, max compression
```

## Comparing `xtrack-0.9.4.tar` & `xtrack-0.9.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-08 21:42:00.109121 xtrack-0.9.4/
--rw-r--r--   0 giadarol (37539) hpc       (2035)      136 2021-10-31 12:34:24.000000 xtrack-0.9.4/MANIFEST.in
--rw-r--r--   0 giadarol (37539) hpc       (2035)      268 2022-03-08 21:42:00.108310 xtrack-0.9.4/PKG-INFO
--rw-r--r--   0 giadarol (37539) hpc       (2035)       91 2021-07-21 13:52:16.000000 xtrack-0.9.4/README.md
-drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-08 21:41:59.843952 xtrack-0.9.4/ducktrack/
--rw-r--r--   0 giadarol (37539) hpc       (2035)      124 2021-11-18 17:49:27.000000 xtrack-0.9.4/ducktrack/__init__.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     2651 2021-11-18 17:49:27.000000 xtrack-0.9.4/ducktrack/base_classes.py
-drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-08 21:41:59.902384 xtrack-0.9.4/ducktrack/be_beamfields/
--rw-r--r--   0 giadarol (37539) hpc       (2035)     5307 2021-11-18 17:49:27.000000 xtrack-0.9.4/ducktrack/be_beamfields/BB6D.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     8076 2021-11-18 17:49:27.000000 xtrack-0.9.4/ducktrack/be_beamfields/BB6Ddata.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)       86 2021-11-18 17:49:27.000000 xtrack-0.9.4/ducktrack/be_beamfields/__init__.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     8018 2021-11-18 17:49:27.000000 xtrack-0.9.4/ducktrack/be_beamfields/beambeam.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     3162 2021-11-18 17:49:27.000000 xtrack-0.9.4/ducktrack/be_beamfields/boost.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     5571 2021-11-18 17:49:27.000000 xtrack-0.9.4/ducktrack/be_beamfields/gaussian_fields.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     8350 2021-11-18 17:49:27.000000 xtrack-0.9.4/ducktrack/be_beamfields/propagate_sigma_matrix.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     2143 2021-11-18 17:49:27.000000 xtrack-0.9.4/ducktrack/be_beamfields/qgauss.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     1748 2021-11-18 17:49:27.000000 xtrack-0.9.4/ducktrack/be_beamfields/slicing.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     6078 2021-11-18 17:49:27.000000 xtrack-0.9.4/ducktrack/be_beamfields/spacecharge.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)    21714 2022-03-06 14:43:54.000000 xtrack-0.9.4/ducktrack/elements.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     1198 2021-11-18 17:49:28.000000 xtrack-0.9.4/ducktrack/line.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)      416 2021-11-18 17:49:28.000000 xtrack-0.9.4/ducktrack/mathlibs.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)      142 2021-11-18 17:49:28.000000 xtrack-0.9.4/ducktrack/particles.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)      115 2021-07-21 13:52:16.000000 xtrack-0.9.4/pyproject.toml
--rw-r--r--   0 giadarol (37539) hpc       (2035)       38 2022-03-08 21:42:00.109417 xtrack-0.9.4/setup.cfg
--rw-r--r--   0 giadarol (37539) hpc       (2035)      651 2022-03-08 21:41:04.000000 xtrack-0.9.4/setup.py
-drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-08 21:41:59.993217 xtrack-0.9.4/xtrack/
--rw-r--r--   0 giadarol (37539) hpc       (2035)      750 2022-02-27 21:46:29.000000 xtrack-0.9.4/xtrack/__init__.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     5658 2021-11-18 17:49:28.000000 xtrack-0.9.4/xtrack/base_element.py
-drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-08 21:42:00.005252 xtrack-0.9.4/xtrack/beam_elements/
--rw-r--r--   0 giadarol (37539) hpc       (2035)      243 2021-11-18 17:49:28.000000 xtrack-0.9.4/xtrack/beam_elements/__init__.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     9527 2022-02-27 21:46:29.000000 xtrack-0.9.4/xtrack/beam_elements/apertures.py
-drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-08 21:42:00.028124 xtrack-0.9.4/xtrack/beam_elements/apertures_src/
--rw-r--r--   0 giadarol (37539) hpc       (2035)      748 2022-01-26 10:23:52.000000 xtrack-0.9.4/xtrack/beam_elements/apertures_src/limitellipse.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)     4330 2021-10-31 12:34:24.000000 xtrack-0.9.4/xtrack/beam_elements/apertures_src/limitpolygon.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)     1957 2022-01-26 10:23:52.000000 xtrack-0.9.4/xtrack/beam_elements/apertures_src/limitracetrack.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)      823 2021-10-31 12:34:24.000000 xtrack-0.9.4/xtrack/beam_elements/apertures_src/limitrect.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)     1015 2021-10-31 12:34:24.000000 xtrack-0.9.4/xtrack/beam_elements/apertures_src/limitrectellipse.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)     1781 2021-11-18 17:49:28.000000 xtrack-0.9.4/xtrack/beam_elements/beam_interaction.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)    27637 2022-03-06 14:43:54.000000 xtrack-0.9.4/xtrack/beam_elements/elements.py
-drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-08 21:42:00.071303 xtrack-0.9.4/xtrack/beam_elements/elements_src/
--rw-r--r--   0 giadarol (37539) hpc       (2035)      932 2022-02-27 21:46:29.000000 xtrack-0.9.4/xtrack/beam_elements/elements_src/cavity.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)      515 2021-10-31 12:34:24.000000 xtrack-0.9.4/xtrack/beam_elements/elements_src/dipoleedge.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)      791 2021-10-31 12:34:24.000000 xtrack-0.9.4/xtrack/beam_elements/elements_src/drift.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)     4449 2021-12-10 12:41:15.000000 xtrack-0.9.4/xtrack/beam_elements/elements_src/elens.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)     7081 2022-01-26 10:23:52.000000 xtrack-0.9.4/xtrack/beam_elements/elements_src/lineartransfermatrix.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)     2904 2022-02-27 21:46:29.000000 xtrack-0.9.4/xtrack/beam_elements/elements_src/multipole.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)      474 2021-10-31 12:34:24.000000 xtrack-0.9.4/xtrack/beam_elements/elements_src/referenceenergyincrease.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)     2630 2021-12-10 12:41:15.000000 xtrack-0.9.4/xtrack/beam_elements/elements_src/rfmultipole.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)      917 2021-10-31 12:34:24.000000 xtrack-0.9.4/xtrack/beam_elements/elements_src/srotation.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)     1674 2022-03-06 14:43:54.000000 xtrack-0.9.4/xtrack/beam_elements/elements_src/wire.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)      423 2021-10-31 12:34:24.000000 xtrack-0.9.4/xtrack/beam_elements/elements_src/xyshift.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)       71 2021-07-21 13:52:16.000000 xtrack-0.9.4/xtrack/general.py
-drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-08 21:42:00.074998 xtrack-0.9.4/xtrack/headers/
--rw-r--r--   0 giadarol (37539) hpc       (2035)      975 2022-03-06 14:43:54.000000 xtrack-0.9.4/xtrack/headers/constants.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)     7536 2022-02-27 21:46:29.000000 xtrack-0.9.4/xtrack/headers/synrad_spectrum.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)    28132 2022-03-08 21:40:44.000000 xtrack-0.9.4/xtrack/line.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     2777 2022-03-06 14:43:54.000000 xtrack-0.9.4/xtrack/line_frozen.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     5455 2022-02-27 21:46:29.000000 xtrack-0.9.4/xtrack/linear_normal_form.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)    18052 2022-03-08 20:50:25.000000 xtrack-0.9.4/xtrack/loader_mad.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     5808 2021-11-18 17:49:28.000000 xtrack-0.9.4/xtrack/loader_sixtrack.py
-drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-08 21:42:00.083686 xtrack-0.9.4/xtrack/loss_location_refinement/
--rw-r--r--   0 giadarol (37539) hpc       (2035)       61 2021-10-31 12:34:24.000000 xtrack-0.9.4/xtrack/loss_location_refinement/__init__.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)    16489 2022-02-27 21:46:29.000000 xtrack-0.9.4/xtrack/loss_location_refinement/loss_location_refinement.py
--rw-r--r--   0 giadarol (37539) hpc       (2035)     3181 2022-02-04 16:25:51.000000 xtrack-0.9.4/xtrack/monitors.py
-drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-08 21:42:00.104901 xtrack-0.9.4/xtrack/monitors_src/
--rw-r--r--   0 giadarol (37539) hpc       (2035)     1262 2022-02-04 16:25:51.000000 xtrack-0.9.4/xtrack/monitors_src/monitors.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)    28145 2022-03-06 14:43:54.000000 xtrack-0.9.4/xtrack/tracker.py
-drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-08 21:42:00.107180 xtrack-0.9.4/xtrack/tracker_src/
--rw-r--r--   0 giadarol (37539) hpc       (2035)     2045 2022-03-06 14:43:54.000000 xtrack-0.9.4/xtrack/tracker_src/tracker.h
--rw-r--r--   0 giadarol (37539) hpc       (2035)    17241 2022-03-06 14:43:54.000000 xtrack-0.9.4/xtrack/twiss_from_tracker.py
-drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-08 21:42:00.000920 xtrack-0.9.4/xtrack.egg-info/
--rw-r--r--   0 giadarol (37539) hpc       (2035)      268 2022-03-08 21:41:58.000000 xtrack-0.9.4/xtrack.egg-info/PKG-INFO
--rw-r--r--   0 giadarol (37539) hpc       (2035)     2074 2022-03-08 21:41:58.000000 xtrack-0.9.4/xtrack.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol (37539) hpc       (2035)        1 2022-03-08 21:41:58.000000 xtrack-0.9.4/xtrack.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol (37539) hpc       (2035)       38 2022-03-08 21:41:58.000000 xtrack-0.9.4/xtrack.egg-info/requires.txt
--rw-r--r--   0 giadarol (37539) hpc       (2035)       17 2022-03-08 21:41:58.000000 xtrack-0.9.4/xtrack.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-10 15:00:54.754422 xtrack-0.9.5/
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      136 2021-10-31 12:34:24.000000 xtrack-0.9.5/MANIFEST.in
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      268 2022-03-10 15:00:54.753772 xtrack-0.9.5/PKG-INFO
+-rw-r--r--   0 giadarol (37539) hpc       (2035)       91 2021-07-21 13:52:16.000000 xtrack-0.9.5/README.md
+drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-10 15:00:54.447386 xtrack-0.9.5/ducktrack/
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      124 2021-11-18 17:49:27.000000 xtrack-0.9.5/ducktrack/__init__.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     2651 2021-11-18 17:49:27.000000 xtrack-0.9.5/ducktrack/base_classes.py
+drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-10 15:00:54.516187 xtrack-0.9.5/ducktrack/be_beamfields/
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     5307 2021-11-18 17:49:27.000000 xtrack-0.9.5/ducktrack/be_beamfields/BB6D.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     8076 2021-11-18 17:49:27.000000 xtrack-0.9.5/ducktrack/be_beamfields/BB6Ddata.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)       86 2021-11-18 17:49:27.000000 xtrack-0.9.5/ducktrack/be_beamfields/__init__.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     8018 2021-11-18 17:49:27.000000 xtrack-0.9.5/ducktrack/be_beamfields/beambeam.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     3162 2021-11-18 17:49:27.000000 xtrack-0.9.5/ducktrack/be_beamfields/boost.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     5571 2021-11-18 17:49:27.000000 xtrack-0.9.5/ducktrack/be_beamfields/gaussian_fields.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     8350 2021-11-18 17:49:27.000000 xtrack-0.9.5/ducktrack/be_beamfields/propagate_sigma_matrix.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     2143 2021-11-18 17:49:27.000000 xtrack-0.9.5/ducktrack/be_beamfields/qgauss.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     1748 2021-11-18 17:49:27.000000 xtrack-0.9.5/ducktrack/be_beamfields/slicing.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     6078 2021-11-18 17:49:27.000000 xtrack-0.9.5/ducktrack/be_beamfields/spacecharge.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)    21714 2022-03-06 14:43:54.000000 xtrack-0.9.5/ducktrack/elements.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     1198 2021-11-18 17:49:28.000000 xtrack-0.9.5/ducktrack/line.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      416 2021-11-18 17:49:28.000000 xtrack-0.9.5/ducktrack/mathlibs.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      142 2021-11-18 17:49:28.000000 xtrack-0.9.5/ducktrack/particles.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      115 2021-07-21 13:52:16.000000 xtrack-0.9.5/pyproject.toml
+-rw-r--r--   0 giadarol (37539) hpc       (2035)       38 2022-03-10 15:00:54.754710 xtrack-0.9.5/setup.cfg
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      651 2022-03-10 15:00:02.000000 xtrack-0.9.5/setup.py
+drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-10 15:00:54.578735 xtrack-0.9.5/xtrack/
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      750 2022-02-27 21:46:29.000000 xtrack-0.9.5/xtrack/__init__.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     5658 2021-11-18 17:49:28.000000 xtrack-0.9.5/xtrack/base_element.py
+drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-10 15:00:54.614945 xtrack-0.9.5/xtrack/beam_elements/
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      243 2021-11-18 17:49:28.000000 xtrack-0.9.5/xtrack/beam_elements/__init__.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     9527 2022-02-27 21:46:29.000000 xtrack-0.9.5/xtrack/beam_elements/apertures.py
+drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-10 15:00:54.662552 xtrack-0.9.5/xtrack/beam_elements/apertures_src/
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      748 2022-01-26 10:23:52.000000 xtrack-0.9.5/xtrack/beam_elements/apertures_src/limitellipse.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     4330 2021-10-31 12:34:24.000000 xtrack-0.9.5/xtrack/beam_elements/apertures_src/limitpolygon.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     1957 2022-01-26 10:23:52.000000 xtrack-0.9.5/xtrack/beam_elements/apertures_src/limitracetrack.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      823 2021-10-31 12:34:24.000000 xtrack-0.9.5/xtrack/beam_elements/apertures_src/limitrect.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     1015 2021-10-31 12:34:24.000000 xtrack-0.9.5/xtrack/beam_elements/apertures_src/limitrectellipse.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     1781 2021-11-18 17:49:28.000000 xtrack-0.9.5/xtrack/beam_elements/beam_interaction.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)    27637 2022-03-06 14:43:54.000000 xtrack-0.9.5/xtrack/beam_elements/elements.py
+drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-10 15:00:54.718394 xtrack-0.9.5/xtrack/beam_elements/elements_src/
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      932 2022-02-27 21:46:29.000000 xtrack-0.9.5/xtrack/beam_elements/elements_src/cavity.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      515 2021-10-31 12:34:24.000000 xtrack-0.9.5/xtrack/beam_elements/elements_src/dipoleedge.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      791 2021-10-31 12:34:24.000000 xtrack-0.9.5/xtrack/beam_elements/elements_src/drift.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     4449 2021-12-10 12:41:15.000000 xtrack-0.9.5/xtrack/beam_elements/elements_src/elens.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     7081 2022-01-26 10:23:52.000000 xtrack-0.9.5/xtrack/beam_elements/elements_src/lineartransfermatrix.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     2904 2022-02-27 21:46:29.000000 xtrack-0.9.5/xtrack/beam_elements/elements_src/multipole.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      474 2021-10-31 12:34:24.000000 xtrack-0.9.5/xtrack/beam_elements/elements_src/referenceenergyincrease.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     2630 2021-12-10 12:41:15.000000 xtrack-0.9.5/xtrack/beam_elements/elements_src/rfmultipole.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      917 2021-10-31 12:34:24.000000 xtrack-0.9.5/xtrack/beam_elements/elements_src/srotation.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     1674 2022-03-06 14:43:54.000000 xtrack-0.9.5/xtrack/beam_elements/elements_src/wire.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      423 2021-10-31 12:34:24.000000 xtrack-0.9.5/xtrack/beam_elements/elements_src/xyshift.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)       71 2021-07-21 13:52:16.000000 xtrack-0.9.5/xtrack/general.py
+drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-10 15:00:54.720277 xtrack-0.9.5/xtrack/headers/
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      975 2022-03-06 14:43:54.000000 xtrack-0.9.5/xtrack/headers/constants.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     7536 2022-02-27 21:46:29.000000 xtrack-0.9.5/xtrack/headers/synrad_spectrum.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)    29039 2022-03-10 14:59:46.000000 xtrack-0.9.5/xtrack/line.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     2777 2022-03-06 14:43:54.000000 xtrack-0.9.5/xtrack/line_frozen.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     5810 2022-03-10 14:59:46.000000 xtrack-0.9.5/xtrack/linear_normal_form.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)    18305 2022-03-10 14:59:46.000000 xtrack-0.9.5/xtrack/loader_mad.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     5808 2021-11-18 17:49:28.000000 xtrack-0.9.5/xtrack/loader_sixtrack.py
+drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-10 15:00:54.724987 xtrack-0.9.5/xtrack/loss_location_refinement/
+-rw-r--r--   0 giadarol (37539) hpc       (2035)       61 2021-10-31 12:34:24.000000 xtrack-0.9.5/xtrack/loss_location_refinement/__init__.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)    16489 2022-02-27 21:46:29.000000 xtrack-0.9.5/xtrack/loss_location_refinement/loss_location_refinement.py
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     3181 2022-02-04 16:25:51.000000 xtrack-0.9.5/xtrack/monitors.py
+drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-10 15:00:54.751747 xtrack-0.9.5/xtrack/monitors_src/
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     1262 2022-02-04 16:25:51.000000 xtrack-0.9.5/xtrack/monitors_src/monitors.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)    28750 2022-03-10 14:59:46.000000 xtrack-0.9.5/xtrack/tracker.py
+drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-10 15:00:54.752639 xtrack-0.9.5/xtrack/tracker_src/
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     2045 2022-03-06 14:43:54.000000 xtrack-0.9.5/xtrack/tracker_src/tracker.h
+-rw-r--r--   0 giadarol (37539) hpc       (2035)    20550 2022-03-10 14:59:46.000000 xtrack-0.9.5/xtrack/twiss_from_tracker.py
+drwxr-xr-x   0 giadarol (37539) hpc       (2035)        0 2022-03-10 15:00:54.591093 xtrack-0.9.5/xtrack.egg-info/
+-rw-r--r--   0 giadarol (37539) hpc       (2035)      268 2022-03-10 15:00:52.000000 xtrack-0.9.5/xtrack.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol (37539) hpc       (2035)     2074 2022-03-10 15:00:52.000000 xtrack-0.9.5/xtrack.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol (37539) hpc       (2035)        1 2022-03-10 15:00:52.000000 xtrack-0.9.5/xtrack.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol (37539) hpc       (2035)       38 2022-03-10 15:00:52.000000 xtrack-0.9.5/xtrack.egg-info/requires.txt
+-rw-r--r--   0 giadarol (37539) hpc       (2035)       17 2022-03-10 15:00:52.000000 xtrack-0.9.5/xtrack.egg-info/top_level.txt
```

### Comparing `xtrack-0.9.4/ducktrack/base_classes.py` & `xtrack-0.9.5/ducktrack/base_classes.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/ducktrack/be_beamfields/BB6D.py` & `xtrack-0.9.5/ducktrack/be_beamfields/BB6D.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/ducktrack/be_beamfields/BB6Ddata.py` & `xtrack-0.9.5/ducktrack/be_beamfields/BB6Ddata.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/ducktrack/be_beamfields/beambeam.py` & `xtrack-0.9.5/ducktrack/be_beamfields/beambeam.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/ducktrack/be_beamfields/boost.py` & `xtrack-0.9.5/ducktrack/be_beamfields/boost.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/ducktrack/be_beamfields/gaussian_fields.py` & `xtrack-0.9.5/ducktrack/be_beamfields/gaussian_fields.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/ducktrack/be_beamfields/propagate_sigma_matrix.py` & `xtrack-0.9.5/ducktrack/be_beamfields/propagate_sigma_matrix.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/ducktrack/be_beamfields/qgauss.py` & `xtrack-0.9.5/ducktrack/be_beamfields/qgauss.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/ducktrack/be_beamfields/slicing.py` & `xtrack-0.9.5/ducktrack/be_beamfields/slicing.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/ducktrack/be_beamfields/spacecharge.py` & `xtrack-0.9.5/ducktrack/be_beamfields/spacecharge.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/ducktrack/elements.py` & `xtrack-0.9.5/ducktrack/elements.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/ducktrack/line.py` & `xtrack-0.9.5/ducktrack/line.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/setup.py` & `xtrack-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 #########
 # Setup #
 #########
 
 setup(
     name='xtrack',
-    version='0.9.4',
+    version='0.9.5',
     description='Tracking library for particle accelerators',
     url='https://github.com/xsuite/xtrack',
     author='Riccard De Maria, Giovanni Iadarola',
     packages=find_packages(),
     ext_modules = extensions,
     include_package_data=True,
     install_requires=[
```

### Comparing `xtrack-0.9.4/xtrack/__init__.py` & `xtrack-0.9.5/xtrack/__init__.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/base_element.py` & `xtrack-0.9.5/xtrack/base_element.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/apertures.py` & `xtrack-0.9.5/xtrack/beam_elements/apertures.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/apertures_src/limitellipse.h` & `xtrack-0.9.5/xtrack/beam_elements/apertures_src/limitellipse.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/apertures_src/limitpolygon.h` & `xtrack-0.9.5/xtrack/beam_elements/apertures_src/limitpolygon.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/apertures_src/limitracetrack.h` & `xtrack-0.9.5/xtrack/beam_elements/apertures_src/limitracetrack.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/apertures_src/limitrect.h` & `xtrack-0.9.5/xtrack/beam_elements/apertures_src/limitrect.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/apertures_src/limitrectellipse.h` & `xtrack-0.9.5/xtrack/beam_elements/apertures_src/limitrectellipse.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/beam_interaction.py` & `xtrack-0.9.5/xtrack/beam_elements/beam_interaction.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/elements.py` & `xtrack-0.9.5/xtrack/beam_elements/elements.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/elements_src/cavity.h` & `xtrack-0.9.5/xtrack/beam_elements/elements_src/cavity.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/elements_src/dipoleedge.h` & `xtrack-0.9.5/xtrack/beam_elements/elements_src/dipoleedge.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/elements_src/drift.h` & `xtrack-0.9.5/xtrack/beam_elements/elements_src/drift.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/elements_src/elens.h` & `xtrack-0.9.5/xtrack/beam_elements/elements_src/elens.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/elements_src/lineartransfermatrix.h` & `xtrack-0.9.5/xtrack/beam_elements/elements_src/lineartransfermatrix.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/elements_src/multipole.h` & `xtrack-0.9.5/xtrack/beam_elements/elements_src/multipole.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/elements_src/rfmultipole.h` & `xtrack-0.9.5/xtrack/beam_elements/elements_src/rfmultipole.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/elements_src/srotation.h` & `xtrack-0.9.5/xtrack/beam_elements/elements_src/srotation.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/beam_elements/elements_src/wire.h` & `xtrack-0.9.5/xtrack/beam_elements/elements_src/wire.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/headers/constants.h` & `xtrack-0.9.5/xtrack/headers/constants.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/headers/synrad_spectrum.h` & `xtrack-0.9.5/xtrack/headers/synrad_spectrum.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/line.py` & `xtrack-0.9.5/xtrack/line.py`

 * *Files 5% similar despite different names*

```diff
@@ -201,14 +201,24 @@
         self._var_management = None
         self._needs_rng = False
 
     @property
     def elements(self):
         return tuple([self.element_dict[nn] for nn in self.element_names])
 
+    def __getitem__(self, ii):
+        if isinstance(ii, str):
+            return self.element_dict.__getitem__(ii)
+        else:
+            names = self.element_names.__getitem__(ii)
+            if isinstance(names, str):
+                return self.element_dict.__getitem__(names)
+            else:
+                return [self.element_dict[nn] for nn in names]
+
     def filter_elements(self, mask=None, exclude_types_starting_with=None):
 
         if mask is None:
             assert exclude_types_starting_with is not None
 
         if exclude_types_starting_with is not None:
             assert mask is None
@@ -305,42 +315,52 @@
         assert ((index is not None and at_s is None) or
                 (index is None and at_s is not None)), (
                     "Either `index` or `at_s` must be provided"
                 )
 
         if at_s is not None:
             s_vect_upstream = np.array(self.get_s_position(mode='upstream'))
+
+            if not _is_thick(element) or np.abs(element.length)==0:
+                i_closest = np.argmin(np.abs(s_vect_upstream - at_s))
+                if np.abs(s_vect_upstream[i_closest] - at_s) < 1e-6:
+                    return self.insert_element(index=i_closest,
+                                            element=element, name=name)
+
             s_vect_downstream = np.array(self.get_s_position(mode='downstream'))
 
             s_start_ele = at_s
             i_first_drift_to_cut = np.where(s_vect_downstream > s_start_ele)[0][0]
 
             # Shortcut for thin element without drift splitting
             if (not _is_thick(element)
                 and np.abs(s_vect_upstream[i_first_drift_to_cut]-at_s)<1e-10):
                     return self.insert_element(index=i_first_drift_to_cut,
                                               element=element, name=name)
 
-            if _is_thick(element):
+            if _is_thick(element) and np.abs(element.length)>0:
                 s_end_ele = at_s + element.length
             else:
                 s_end_ele = s_start_ele
 
             i_last_drift_to_cut = np.where(s_vect_upstream < s_end_ele)[0][-1]
-            assert i_first_drift_to_cut <= i_last_drift_to_cut
+            if _is_thick(element) and element.length > 0:
+                assert i_first_drift_to_cut <= i_last_drift_to_cut
             name_first_drift_to_cut = self.element_names[i_first_drift_to_cut]
             name_last_drift_to_cut = self.element_names[i_last_drift_to_cut]
             first_drift_to_cut = self.element_dict[name_first_drift_to_cut]
             last_drift_to_cut = self.element_dict[name_last_drift_to_cut]
 
             assert _is_drift(first_drift_to_cut)
             assert _is_drift(last_drift_to_cut)
 
             for ii in range(i_first_drift_to_cut, i_last_drift_to_cut+1):
-                if not _is_drift(self.element_dict[self.element_names[ii]]):
+                e_to_replace = self.element_dict[self.element_names[ii]]
+                if (not _is_drift(e_to_replace) and
+                    not e_to_replace.__class__.__name__.startswith('Limit')):
                     raise ValueError('Cannot replace active element '
                                         f'{self.element_names[ii]}')
 
             l_left_part = s_start_ele - s_vect_upstream[i_first_drift_to_cut]
             l_right_part = s_vect_downstream[i_last_drift_to_cut] - s_end_ele
             assert l_left_part >= 0
             assert l_right_part >= 0
@@ -373,15 +393,15 @@
 
             self.element_names[i_insert] = names_to_insert[-1]
             if len(names_to_insert) > 1:
                 for nn in names_to_insert[:-1][::-1]:
                     self.element_names.insert(i_insert, nn)
 
         else:
-            if _is_thick(element):
+            if _is_thick(element) and np.abs(element.length)>0:
                 raise NotImplementedError('use `at_s` to insert thick elements')
             assert name not in self.element_dict.keys()
             self.element_dict[name] = element
             self.element_names.insert(index, name)
 
         return self
 
@@ -649,35 +669,33 @@
 
         # Original strengths
         for ii, vv in enumerate(element.knl):
             new_knl[ii] += element.knl[ii]
         for ii, vv in enumerate(element.ksl):
             new_ksl[ii] += element.ksl[ii]
 
-        # Errors
-        for ii, vv in enumerate(knl):
-            new_knl[ii] += knl[ii]
-        for ii, vv in enumerate(ksl):
-            new_ksl[ii] += ksl[ii]
-
         new_element = Multipole(knl=new_knl, ksl=new_ksl,
                 length=element.length, hxl=element.hxl,
                 hyl=element.hyl, radiation_flag=element.radiation_flag)
 
         self.element_dict[element_name] = new_element
 
-        # Handle deferred expressions
+        # Errors
         if self._var_management is not None:
+            # Handle deferred expressions
             lref = self._var_management['lref']
-            manager = self._var_management['manager']
-            for ii in range(min([len(knl), len(element.knl)])):
+            for ii, vv in enumerate(knl):
                 lref[element_name].knl[ii] += knl[ii]
-
-            for ii in range(min([len(ksl), len(element.ksl)])):
+            for ii, vv in enumerate(ksl):
                 lref[element_name].ksl[ii] += ksl[ii]
+        else:
+            for ii, vv in enumerate(knl):
+                new_element.knl[ii] += knl[ii]
+            for ii, vv in enumerate(ksl):
+                new_element.ksl[ii] += ksl[ii]
 
     def _apply_madx_errors(self, madx_sequence):
         """Applies errors from MAD-X sequence to existing
         elements in this Line instance.
 
         Return names of MAD-X elements with existing align_errors
         or field_errors which were not found in the elements of
```

### Comparing `xtrack-0.9.4/xtrack/line_frozen.py` & `xtrack-0.9.5/xtrack/line_frozen.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/linear_normal_form.py` & `xtrack-0.9.5/xtrack/linear_normal_form.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import numpy as np
 
+DEFAULT_MATRIX_RESPONSIVENESS_TOL = 1e-15
+DEFAULT_MATRIX_STABILITY_TOL = 1e-3
+
 def healy_symplectify(M):
     # https://accelconf.web.cern.ch/e06/PAPERS/WEPCH152.PDF
     #print("Symplectifying linear One-Turn-Map...")
 
     #print("Before symplectifying: det(M) = {}".format(np.linalg.det(M)))
     I = np.identity(6)
 
@@ -45,33 +48,37 @@
 ### Implement Normalization of fully coupled motion ##
 ######################################################
 
 def Rot2D(mu):
     return np.array([[ np.cos(mu), np.sin(mu)],
                      [-np.sin(mu), np.cos(mu)]])
 
-def compute_linear_normal_form(M, symplectify=True, tol_det_M=0.05):
-
-    if np.abs(np.linalg.det(M)-1) > tol_det_M:
-        raise ValueError('The determinant of M is out tolerance.')
+def compute_linear_normal_form(M, symplectify=True,
+                        responsiveness_tol=DEFAULT_MATRIX_RESPONSIVENESS_TOL,
+                        stability_tol=DEFAULT_MATRIX_STABILITY_TOL):
+
+    if np.abs(np.linalg.det(M)-1) > stability_tol:
+        raise ValueError(
+            f'The determinant of M is out tolerance. det={np.linalg.det(M)}')
 
     for ii in range(6):
-        mask_non_zero = np.abs(M[ii, :])>1e-15
+        mask_non_zero = np.abs(M[ii, :]) > responsiveness_tol
         mask_non_zero[ii] = False
         if np.sum(mask_non_zero)<1:
             raise ValueError(
                 'Invalid one-turn map: No coordinates respond to variations of '
                 + 'x px y py zeta delta'.split()[ii])
 
     if symplectify:
         M = healy_symplectify(M)
 
     w0, v0 = np.linalg.eig(M)
-    if np.any(np.abs(w0) > 1. + 1e-4):
-        raise ValueError('One-turn matrix is unstable')
+    if np.any(np.abs(w0) > 1. + stability_tol):
+        raise ValueError('One-turn matrix is unstable. '
+                         f'Magnitudes of eigenvalues are:\n{repr(np.abs(w0))}')
 
     a0 = np.real(v0)
     b0 = np.imag(v0)
 
     index_list = [0,5,1,2,3,4] # we mix them up to check the algorithm
 
     ##### Sort modes in pairs of conjugate modes #####
```

### Comparing `xtrack-0.9.4/xtrack/loader_mad.py` & `xtrack-0.9.5/xtrack/loader_mad.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,25 +47,33 @@
                 _vref[name]=madeval(par.expr)
 
     elements = seq.elements
     ele_pos = seq.element_positions()
 
     old_pp = 0.0
     i_drift = 0
+    counters = {}
     for pp, ee in sorted(zip(ele_pos,elements),key=lambda x:x[0]):
         skiptilt=False
 
         if pp > old_pp + drift_threshold:
             line.append_element(myDrift(length=(pp - old_pp)), f"drift_{i_drift}")
             old_pp = pp
             i_drift += 1
 
-        eename = ee.name
+        eename_mad = ee.name
         mad_etype = ee.base_type.name
 
+        if eename_mad not in counters.keys():
+            eename = eename_mad
+            counters[eename_mad] = 0
+        else:
+            counters[eename_mad] += 1
+            eename = eename_mad + f'_{counters[eename_mad]}'
+
         if mad_etype in [
             "marker",
             "monitor",
             "hmonitor",
             "vmonitor",
             "collimator",
             "rcollimator",
@@ -186,18 +194,18 @@
                     if eepar.knl.expr[ii] is not None:
                         _lref[eename].knl[ii] = madeval(eepar.knl.expr[ii])
                 for ii, _ in enumerate(ksl):
                     if eepar.ksl.expr[ii] is not None:
                         _lref[eename].ksl[ii] = madeval(eepar.ksl.expr[ii])
                 for ii, _ in enumerate(ee.pnl):
                     if eepar.pn.expr[ii] is not None:
-                        _lref[eename].pn[ii] = madeval(eepar.pn.expr[ii]) * 360
+                        _lref[eename].pn[ii] = madeval(eepar.pnl.expr[ii]) * 360
                 for ii, _ in enumerate(ee.psl):
                     if eepar.ps.expr[ii] is not None:
-                        _lref[eename].ps[ii] = madeval(eepar.ps.expr[ii]) * 360
+                        _lref[eename].ps[ii] = madeval(eepar.psl.expr[ii]) * 360
 
 
         elif mad_etype == "wire":
             if len(ee.L_phy) == 1:
                 newele = classes.Wire(
                     wire_L_phy   = ee.L_phy[0],
                     wire_L_int   = ee.L_int[0],
```

### Comparing `xtrack-0.9.4/xtrack/loader_sixtrack.py` & `xtrack-0.9.5/xtrack/loader_sixtrack.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/loss_location_refinement/loss_location_refinement.py` & `xtrack-0.9.5/xtrack/loss_location_refinement/loss_location_refinement.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/monitors.py` & `xtrack-0.9.5/xtrack/monitors.py`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/monitors_src/monitors.h` & `xtrack-0.9.5/xtrack/monitors_src/monitors.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack/tracker.py` & `xtrack-0.9.5/xtrack/tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 import xobjects as xo
 import xpart as xp
 
 from .beam_elements import Drift
 from .line import Line
 
+from . import linear_normal_form as lnf
+
 logger = logging.getLogger(__name__)
 
 def _check_is_collective(ele):
     iscoll = not hasattr(ele, 'iscollective') or ele.iscollective
     return iscoll
 
 class Tracker:
@@ -80,14 +82,17 @@
                 skip_end_turn_actions=skip_end_turn_actions,
                 reset_s_at_end_turn=reset_s_at_end_turn,
                 particles_monitor_class=particles_monitor_class,
                 global_xy_limit=global_xy_limit,
                 local_particle_src=local_particle_src,
                 save_source_as=save_source_as)
 
+        self.matrix_responsiveness_tol = lnf.DEFAULT_MATRIX_RESPONSIVENESS_TOL
+        self.matrix_stability_tol = lnf.DEFAULT_MATRIX_STABILITY_TOL
+
     def _init_track_with_collective(
         self,
         _context=None,
         _buffer=None,
         _offset=None,
         line=None,
         track_kernel=None,
@@ -304,17 +309,24 @@
 
     def twiss(self, particle_ref=None, r_sigma=0.01,
         nemitt_x=1e-6, nemitt_y=1e-6,
         n_theta=1000, delta_disp=1e-5, delta_chrom=1e-4,
         particle_co_guess=None, steps_r_matrix=None,
         co_search_settings=None, at_elements=None, at_s=None,
         eneloss_and_damping=False,
+        matrix_responsiveness_tol=None,
+        matrix_stability_tol=None,
         symplectify=False
         ):
 
+        if matrix_responsiveness_tol is None:
+            matrix_responsiveness_tol = self.matrix_responsiveness_tol
+        if matrix_stability_tol is None:
+            matrix_stability_tol = self.matrix_stability_tol
+
         if self.iscollective:
             logger.warning(
                 'The tracker has collective elements.\n'
                 'In the twiss computation collective elements are'
                 ' replaced by drifts')
             tracker = self._supertracker
         else:
@@ -332,14 +344,16 @@
             nemitt_x=nemitt_x, nemitt_y=nemitt_y,
             n_theta=n_theta, delta_disp=delta_disp, delta_chrom=delta_chrom,
             particle_co_guess=particle_co_guess,
             steps_r_matrix=steps_r_matrix,
             co_search_settings=co_search_settings,
             at_elements=at_elements, at_s=at_s,
             eneloss_and_damping=eneloss_and_damping,
+            matrix_responsiveness_tol=matrix_responsiveness_tol,
+            matrix_stability_tol=matrix_stability_tol,
             symplectify=symplectify)
 
 
     def filter_elements(self, mask=None, exclude_types_starting_with=None):
         return self.__class__(
                  _buffer=self._buffer,
                  line=self.line.filter_elements(mask=mask,
```

### Comparing `xtrack-0.9.4/xtrack/tracker_src/tracker.h` & `xtrack-0.9.5/xtrack/tracker_src/tracker.h`

 * *Files identical despite different names*

### Comparing `xtrack-0.9.4/xtrack.egg-info/SOURCES.txt` & `xtrack-0.9.5/xtrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

