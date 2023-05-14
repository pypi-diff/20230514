# Comparing `tmp/polar_api-1.0.2.tar.gz` & `tmp/polar_api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polar_api-1.0.2.tar", last modified: Mon May  1 08:39:48 2023, max compression
+gzip compressed data, was "polar_api-2.0.0.tar", last modified: Sun May 14 09:04:43 2023, max compression
```

## Comparing `polar_api-1.0.2.tar` & `polar_api-2.0.0.tar`

### file list

```diff
@@ -1,28 +1,14 @@
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:39:48.986368 polar_api-1.0.2/
--rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-01 08:39:48.986256 polar_api-1.0.2/PKG-INFO
--rw-r--r--   0 cronsholt   (501) staff       (20)      896 2023-04-14 08:55:43.000000 polar_api-1.0.2/README.md
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:39:48.983302 polar_api-1.0.2/polar_api/
--rw-r--r--   0 cronsholt   (501) staff       (20)     7286 2023-05-01 08:38:20.000000 polar_api-1.0.2/polar_api/PolarAPI.py
--rw-r--r--   0 cronsholt   (501) staff       (20)       94 2023-04-22 06:14:40.000000 polar_api-1.0.2/polar_api/__init__.py
--rw-r--r--   0 cronsholt   (501) staff       (20)    30259 2023-04-14 08:55:43.000000 polar_api-1.0.2/polar_api/cleaning.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     6417 2023-04-14 10:45:49.000000 polar_api-1.0.2/polar_api/polar_api.py
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:39:48.984175 polar_api-1.0.2/polar_api.egg-info/
--rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-01 08:39:48.000000 polar_api-1.0.2/polar_api.egg-info/PKG-INFO
--rw-r--r--   0 cronsholt   (501) staff       (20)      533 2023-05-01 08:39:48.000000 polar_api-1.0.2/polar_api.egg-info/SOURCES.txt
--rw-r--r--   0 cronsholt   (501) staff       (20)        1 2023-05-01 08:39:48.000000 polar_api-1.0.2/polar_api.egg-info/dependency_links.txt
--rw-r--r--   0 cronsholt   (501) staff       (20)       69 2023-05-01 08:39:48.000000 polar_api-1.0.2/polar_api.egg-info/requires.txt
--rw-r--r--   0 cronsholt   (501) staff       (20)       28 2023-05-01 08:39:48.000000 polar_api-1.0.2/polar_api.egg-info/top_level.txt
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:39:48.985255 polar_api-1.0.2/scripts/
--rw-r--r--   0 cronsholt   (501) staff       (20)        0 2023-04-14 08:55:43.000000 polar_api-1.0.2/scripts/__init__.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     3063 2023-04-14 08:55:43.000000 polar_api-1.0.2/scripts/download_raw_data.py
--rw-r--r--   0 cronsholt   (501) staff       (20)      999 2023-04-14 08:55:43.000000 polar_api-1.0.2/scripts/get_player_session_trimmed.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     3929 2023-04-14 08:55:43.000000 polar_api-1.0.2/scripts/get_session_raw_gps.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     1828 2023-04-14 08:55:43.000000 polar_api-1.0.2/scripts/gps_data_project.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     7680 2023-04-14 08:55:43.000000 polar_api-1.0.2/scripts/session_viz.py
--rw-r--r--   0 cronsholt   (501) staff       (20)       38 2023-05-01 08:39:48.986413 polar_api-1.0.2/setup.cfg
--rw-r--r--   0 cronsholt   (501) staff       (20)      364 2023-05-01 08:39:33.000000 polar_api-1.0.2/setup.py
-drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-01 08:39:48.985771 polar_api-1.0.2/utilities/
--rw-r--r--   0 cronsholt   (501) staff       (20)        0 2023-04-14 08:55:43.000000 polar_api-1.0.2/utilities/__init__.py
--rw-r--r--   0 cronsholt   (501) staff       (20)     1595 2023-04-14 08:55:43.000000 polar_api-1.0.2/utilities/metadata.py
--rw-r--r--   0 cronsholt   (501) staff       (20)      548 2023-04-14 08:55:43.000000 polar_api-1.0.2/utilities/polar_IO.py
--rw-r--r--   0 cronsholt   (501) staff       (20)    27284 2023-04-26 06:29:30.000000 polar_api-1.0.2/utilities/polar_api_old.py
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-14 09:04:43.918477 polar_api-2.0.0/
+-rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-14 09:04:43.918332 polar_api-2.0.0/PKG-INFO
+-rw-r--r--   0 cronsholt   (501) staff       (20)      896 2023-04-14 08:55:43.000000 polar_api-2.0.0/README.md
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-14 09:04:43.917064 polar_api-2.0.0/polar_api/
+-rw-r--r--   0 cronsholt   (501) staff       (20)     5129 2023-05-14 09:01:55.000000 polar_api-2.0.0/polar_api/PolarAPI.py
+-rw-r--r--   0 cronsholt   (501) staff       (20)       38 2023-05-14 09:02:39.000000 polar_api-2.0.0/polar_api/__init__.py
+drwxr-xr-x   0 cronsholt   (501) staff       (20)        0 2023-05-14 09:04:43.918082 polar_api-2.0.0/polar_api.egg-info/
+-rw-r--r--   0 cronsholt   (501) staff       (20)      156 2023-05-14 09:04:43.000000 polar_api-2.0.0/polar_api.egg-info/PKG-INFO
+-rw-r--r--   0 cronsholt   (501) staff       (20)      226 2023-05-14 09:04:43.000000 polar_api-2.0.0/polar_api.egg-info/SOURCES.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)        1 2023-05-14 09:04:43.000000 polar_api-2.0.0/polar_api.egg-info/dependency_links.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)       71 2023-05-14 09:04:43.000000 polar_api-2.0.0/polar_api.egg-info/requires.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)       10 2023-05-14 09:04:43.000000 polar_api-2.0.0/polar_api.egg-info/top_level.txt
+-rw-r--r--   0 cronsholt   (501) staff       (20)       38 2023-05-14 09:04:43.918561 polar_api-2.0.0/setup.cfg
+-rw-r--r--   0 cronsholt   (501) staff       (20)      366 2023-05-14 09:04:06.000000 polar_api-2.0.0/setup.py
```

### Comparing `polar_api-1.0.2/README.md` & `polar_api-2.0.0/README.md`

 * *Files identical despite different names*

