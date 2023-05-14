# Comparing `tmp/fmpy_qi-0.1.3.tar.gz` & `tmp/fmpy_qi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmpy_qi-0.1.3.tar", last modified: Thu May  4 21:45:53 2023, max compression
+gzip compressed data, was "fmpy_qi-0.1.4.tar", last modified: Sun May 14 21:05:09 2023, max compression
```

## Comparing `fmpy_qi-0.1.3.tar` & `fmpy_qi-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-04 21:45:53.889181 fmpy_qi-0.1.3/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     1064 2023-04-22 15:25:00.000000 fmpy_qi-0.1.3/LICENSE
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2638 2023-05-04 21:45:53.888811 fmpy_qi-0.1.3/PKG-INFO
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2106 2023-05-01 20:48:32.000000 fmpy_qi-0.1.3/README.md
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      741 2023-05-04 21:45:44.000000 fmpy_qi-0.1.3/pyproject.toml
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       38 2023-05-04 21:45:53.889298 fmpy_qi-0.1.3/setup.cfg
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-04 21:45:53.882777 fmpy_qi-0.1.3/src/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-30 21:24:30.000000 fmpy_qi-0.1.3/src/__init__.py
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-04 21:45:53.885679 fmpy_qi-0.1.3/src/fmpy/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-22 15:25:28.000000 fmpy_qi-0.1.3/src/fmpy/__init__.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     8022 2023-05-04 21:40:05.000000 fmpy_qi-0.1.3/src/fmpy/client.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)    12275 2023-04-23 08:55:58.000000 fmpy_qi-0.1.3/src/fmpy/urls.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      940 2023-04-30 16:47:40.000000 fmpy_qi-0.1.3/src/fmpy/utils.py
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-04 21:45:53.888420 fmpy_qi-0.1.3/src/fmpy_qi.egg-info/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2638 2023-05-04 21:45:53.000000 fmpy_qi-0.1.3/src/fmpy_qi.egg-info/PKG-INFO
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      297 2023-05-04 21:45:53.000000 fmpy_qi-0.1.3/src/fmpy_qi.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        1 2023-05-04 21:45:53.000000 fmpy_qi-0.1.3/src/fmpy_qi.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       46 2023-05-04 21:45:53.000000 fmpy_qi-0.1.3/src/fmpy_qi.egg-info/requires.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       14 2023-05-04 21:45:53.000000 fmpy_qi-0.1.3/src/fmpy_qi.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-14 21:05:09.269323 fmpy_qi-0.1.4/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     1064 2023-04-22 15:25:00.000000 fmpy_qi-0.1.4/LICENSE
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2751 2023-05-14 21:05:09.268942 fmpy_qi-0.1.4/PKG-INFO
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2219 2023-05-14 19:24:52.000000 fmpy_qi-0.1.4/README.md
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      741 2023-05-14 21:04:22.000000 fmpy_qi-0.1.4/pyproject.toml
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       38 2023-05-14 21:05:09.269439 fmpy_qi-0.1.4/setup.cfg
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-14 21:05:09.263489 fmpy_qi-0.1.4/src/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-30 21:24:30.000000 fmpy_qi-0.1.4/src/__init__.py
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-14 21:05:09.265881 fmpy_qi-0.1.4/src/fmpy/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-22 15:25:28.000000 fmpy_qi-0.1.4/src/fmpy/__init__.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)    33698 2023-05-14 21:02:52.000000 fmpy_qi-0.1.4/src/fmpy/client.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)    12275 2023-05-14 20:08:21.000000 fmpy_qi-0.1.4/src/fmpy/urls.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      526 2023-05-14 19:02:44.000000 fmpy_qi-0.1.4/src/fmpy/utils.py
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-14 21:05:09.268513 fmpy_qi-0.1.4/src/fmpy_qi.egg-info/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2751 2023-05-14 21:05:09.000000 fmpy_qi-0.1.4/src/fmpy_qi.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      297 2023-05-14 21:05:09.000000 fmpy_qi-0.1.4/src/fmpy_qi.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        1 2023-05-14 21:05:09.000000 fmpy_qi-0.1.4/src/fmpy_qi.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       46 2023-05-14 21:05:09.000000 fmpy_qi-0.1.4/src/fmpy_qi.egg-info/requires.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       14 2023-05-14 21:05:09.000000 fmpy_qi-0.1.4/src/fmpy_qi.egg-info/top_level.txt
```

### Comparing `fmpy_qi-0.1.3/LICENSE` & `fmpy_qi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.3/PKG-INFO` & `fmpy_qi-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmpy_qi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python wrapper for the Financial Modeling Prep API
 Author-email: Nicolas THIERY <nicles.thiery@gmail.com>
 Project-URL: Homepage, https://github.com/NicolasThiery/fmpy
 Project-URL: Bug Tracker, https://github.com/NicolasThiery/fmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,16 +53,17 @@
 ```
 
 ## Historical data
 ```python
 from fmpy.client import FmpClient
 
 client = FmpClient(api_key="YOU_API_KEY")
-hist_data = client.get_historical_data('TSLA', period='1h', start='2020-01-02', end='2022-06-25')
-# Retreive historical 1h candles for Tesla stock between 2020-01-02 and 2022-06-25
+hist_data = client.get_historical_data('TSLA', period='1h', start='2020-01-02 10:00:00', end='2022-06-25 15:00:00')
+# Retreive historical 1h candles for Tesla stock between 2020-01-02 10:00:00 and 2022-06-25 15:00:00
+# start and end support both "%Y-%m-%d %H:%M:%S" and "%Y-%m-%d" time formats
 ```
 
 
 ## Licence
 ***
 © 2023 Nicolas Thiery
```

### Comparing `fmpy_qi-0.1.3/README.md` & `fmpy_qi-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -39,16 +39,17 @@
 ```
 
 ## Historical data
 ```python
 from fmpy.client import FmpClient
 
 client = FmpClient(api_key="YOU_API_KEY")
-hist_data = client.get_historical_data('TSLA', period='1h', start='2020-01-02', end='2022-06-25')
-# Retreive historical 1h candles for Tesla stock between 2020-01-02 and 2022-06-25
+hist_data = client.get_historical_data('TSLA', period='1h', start='2020-01-02 10:00:00', end='2022-06-25 15:00:00')
+# Retreive historical 1h candles for Tesla stock between 2020-01-02 10:00:00 and 2022-06-25 15:00:00
+# start and end support both "%Y-%m-%d %H:%M:%S" and "%Y-%m-%d" time formats
 ```
 
 
 ## Licence
 ***
 © 2023 Nicolas Thiery
```

### Comparing `fmpy_qi-0.1.3/pyproject.toml` & `fmpy_qi-0.1.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fmpy_qi"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Nicolas THIERY", email="nicles.thiery@gmail.com" },
 ]
 description = "A python wrapper for the Financial Modeling Prep API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `fmpy_qi-0.1.3/src/fmpy/urls.py` & `fmpy_qi-0.1.4/src/fmpy/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 KEY_METRICS_TTM = f'{API_V3_URL}/key-metrics-ttm'
 KEY_METRICS = f'{API_V3_URL}/key-metrics'
 FINANCIAL_GROWTH = f'{API_V3_URL}/financial-growth'
 RATING = f'{API_V3_URL}/rating'
 HISTORICAL_RATING = f'{API_V3_URL}/historical-rating'
 DISCOUNTED_CASH_FLOW = f'{API_V3_URL}/discounted-cash-flow'
 ADVANCED_DISCOUNTED_CASH_FLOW = f'{API_V4_URL}/advanced_discounted_cash_flow'
-ADVANCED_LEVERED_DISCOUNTED_CASH_FLOW = f'{API_V3_URL}/advanced_levered_discounted_cash_flow'
+ADVANCED_LEVERED_DISCOUNTED_CASH_FLOW = f'{API_V4_URL}/advanced_levered_discounted_cash_flow'
 HISTORICAL_DISCOUNTED_CASH_FLOW_STATEMENT = f'{API_V3_URL}/historical-discounted-cash-flow-statement'
 HISTORICAL_DAILY_DISCOUNTED_CASH_FLOW = f'{API_V3_URL}/historical-daily-discounted-cash-flow'
 
 # INSTITUTIONAL STOCK OWNERSHIP
 INSTITUTIONAL_OWNERSHIP = f'{API_V4_URL}/institutional-ownership'
 SYMBOL_OWNERSHIP = f'{INSTITUTIONAL_OWNERSHIP}/symbol-ownership'
 INSTITUTIONAL_HOLDERS = f'{INSTITUTIONAL_OWNERSHIP}/institutional-holders/symbol-ownership-percent'
```

### Comparing `fmpy_qi-0.1.3/src/fmpy/utils.py` & `fmpy_qi-0.1.4/src/fmpy/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
 
 def is_valid_time_format(time_format):
     try:
-        datetime.strptime(time_format, "%Y-%M-%d")
+        datetime.strptime(time_format, "%Y-%m-%d %H:%M:%S")
     except ValueError:
         return False
     else:
         return True
 
 
 def format_period(period):
@@ -18,19 +18,7 @@
             period = period.replace('h', 'hour')
     return period
 
 
 def get_current_minute():
     return datetime.now().replace(second=0, microsecond=0)
 
-
-def limit_data_list(data_list, date_target, end_target):
-    reversed_data = data_list[::-1]
-    start_index = 0
-    end_index = -1
-    for i, item in enumerate(reversed_data):
-        if item['date'].split(' ')[0] == date_target:
-            start_index = i+1
-        elif end_target:
-            if item['date'].split(' ')[0] == end_target:
-                end_target = i
-    return reversed_data[start_index:end_index]
```

### Comparing `fmpy_qi-0.1.3/src/fmpy_qi.egg-info/PKG-INFO` & `fmpy_qi-0.1.4/src/fmpy_qi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmpy-qi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python wrapper for the Financial Modeling Prep API
 Author-email: Nicolas THIERY <nicles.thiery@gmail.com>
 Project-URL: Homepage, https://github.com/NicolasThiery/fmpy
 Project-URL: Bug Tracker, https://github.com/NicolasThiery/fmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,16 +53,17 @@
 ```
 
 ## Historical data
 ```python
 from fmpy.client import FmpClient
 
 client = FmpClient(api_key="YOU_API_KEY")
-hist_data = client.get_historical_data('TSLA', period='1h', start='2020-01-02', end='2022-06-25')
-# Retreive historical 1h candles for Tesla stock between 2020-01-02 and 2022-06-25
+hist_data = client.get_historical_data('TSLA', period='1h', start='2020-01-02 10:00:00', end='2022-06-25 15:00:00')
+# Retreive historical 1h candles for Tesla stock between 2020-01-02 10:00:00 and 2022-06-25 15:00:00
+# start and end support both "%Y-%m-%d %H:%M:%S" and "%Y-%m-%d" time formats
 ```
 
 
 ## Licence
 ***
 © 2023 Nicolas Thiery
```

