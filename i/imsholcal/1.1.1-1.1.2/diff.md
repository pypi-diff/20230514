# Comparing `tmp/imsholcal-1.1.1.tar.gz` & `tmp/imsholcal-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsholcal-1.1.1.tar", last modified: Sat May 13 11:36:33 2023, max compression
+gzip compressed data, was "imsholcal-1.1.2.tar", last modified: Sat May 13 22:54:31 2023, max compression
```

## Comparing `imsholcal-1.1.1.tar` & `imsholcal-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:36:33.592734 imsholcal-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:36:33.592734 imsholcal-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:36:33.592734 imsholcal-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-13 11:36:21.000000 imsholcal-1.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-13 11:36:21.000000 imsholcal-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-13 11:36:33.592734 imsholcal-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-13 11:36:21.000000 imsholcal-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 11:36:21.000000 imsholcal-1.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 11:36:21.000000 imsholcal-1.1.1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-13 11:36:21.000000 imsholcal-1.1.1/exchange_holidays.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:36:33.592734 imsholcal-1.1.1/imsholcal/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 11:36:21.000000 imsholcal-1.1.1/imsholcal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-13 11:36:21.000000 imsholcal-1.1.1/imsholcal/business_day.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:36:33.592734 imsholcal-1.1.1/imsholcal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-13 11:36:33.000000 imsholcal-1.1.1/imsholcal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-13 11:36:33.000000 imsholcal-1.1.1/imsholcal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 11:36:33.000000 imsholcal-1.1.1/imsholcal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-13 11:36:33.000000 imsholcal-1.1.1/imsholcal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-13 11:36:33.000000 imsholcal-1.1.1/imsholcal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 11:36:33.592734 imsholcal-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-13 11:36:21.000000 imsholcal-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:54:31.368419 imsholcal-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:54:31.364419 imsholcal-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:54:31.364419 imsholcal-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-13 22:54:19.000000 imsholcal-1.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-13 22:54:19.000000 imsholcal-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-13 22:54:31.368419 imsholcal-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-13 22:54:19.000000 imsholcal-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 22:54:19.000000 imsholcal-1.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 22:54:19.000000 imsholcal-1.1.2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-13 22:54:19.000000 imsholcal-1.1.2/exchange_holidays.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:54:31.368419 imsholcal-1.1.2/imsholcal/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 22:54:19.000000 imsholcal-1.1.2/imsholcal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-13 22:54:19.000000 imsholcal-1.1.2/imsholcal/business_day.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 22:54:31.368419 imsholcal-1.1.2/imsholcal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-13 22:54:31.000000 imsholcal-1.1.2/imsholcal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-13 22:54:31.000000 imsholcal-1.1.2/imsholcal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 22:54:31.000000 imsholcal-1.1.2/imsholcal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-13 22:54:31.000000 imsholcal-1.1.2/imsholcal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-13 22:54:31.000000 imsholcal-1.1.2/imsholcal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 22:54:31.368419 imsholcal-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-13 22:54:19.000000 imsholcal-1.1.2/setup.py
```

### Comparing `imsholcal-1.1.1/.github/workflows/python-publish.yml` & `imsholcal-1.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `imsholcal-1.1.1/imsholcal/business_day.py` & `imsholcal-1.1.2/imsholcal/business_day.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from pandas.tseries.offsets import CustomBusinessDay
 import pandas as pd
 import requests
 import io
 
 
 def exch_hols(n, country):
-
+    # Clear cache
+    requests_cache.clear()
     url = 'https://raw.githubusercontent.com/mcunningto/imsholcal/main/exchange_holidays.csv'
     response = requests.get(url)
     holidays_df = pd.read_csv(io.StringIO(response.text))
 	
     # Filter the DataFrame to include only holidays for the specified country
     filtered_df = holidays_df[holidays_df['country'] == country]
     # Convert the date column to datetime format with specified date format
```

### Comparing `imsholcal-1.1.1/setup.py` & `imsholcal-1.1.2/setup.py`

 * *Files identical despite different names*

