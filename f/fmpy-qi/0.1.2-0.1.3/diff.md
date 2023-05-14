# Comparing `tmp/fmpy_qi-0.1.2.tar.gz` & `tmp/fmpy_qi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmpy_qi-0.1.2.tar", last modified: Mon May  1 20:51:00 2023, max compression
+gzip compressed data, was "fmpy_qi-0.1.3.tar", last modified: Thu May  4 21:45:53 2023, max compression
```

## Comparing `fmpy_qi-0.1.2.tar` & `fmpy_qi-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-01 20:51:00.384616 fmpy_qi-0.1.2/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     1064 2023-04-22 15:25:00.000000 fmpy_qi-0.1.2/LICENSE
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2638 2023-05-01 20:51:00.384246 fmpy_qi-0.1.2/PKG-INFO
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2106 2023-05-01 20:48:32.000000 fmpy_qi-0.1.2/README.md
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      741 2023-05-01 20:49:38.000000 fmpy_qi-0.1.2/pyproject.toml
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       38 2023-05-01 20:51:00.384724 fmpy_qi-0.1.2/setup.cfg
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-01 20:51:00.379011 fmpy_qi-0.1.2/src/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-30 21:24:30.000000 fmpy_qi-0.1.2/src/__init__.py
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-01 20:51:00.381182 fmpy_qi-0.1.2/src/fmpy/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-22 15:25:28.000000 fmpy_qi-0.1.2/src/fmpy/__init__.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     7942 2023-05-01 20:45:18.000000 fmpy_qi-0.1.2/src/fmpy/client.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)    12275 2023-04-23 08:55:58.000000 fmpy_qi-0.1.2/src/fmpy/urls.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      940 2023-04-30 16:47:40.000000 fmpy_qi-0.1.2/src/fmpy/utils.py
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-01 20:51:00.383827 fmpy_qi-0.1.2/src/fmpy_qi.egg-info/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2638 2023-05-01 20:51:00.000000 fmpy_qi-0.1.2/src/fmpy_qi.egg-info/PKG-INFO
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      297 2023-05-01 20:51:00.000000 fmpy_qi-0.1.2/src/fmpy_qi.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        1 2023-05-01 20:51:00.000000 fmpy_qi-0.1.2/src/fmpy_qi.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       46 2023-05-01 20:51:00.000000 fmpy_qi-0.1.2/src/fmpy_qi.egg-info/requires.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       14 2023-05-01 20:51:00.000000 fmpy_qi-0.1.2/src/fmpy_qi.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-04 21:45:53.889181 fmpy_qi-0.1.3/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     1064 2023-04-22 15:25:00.000000 fmpy_qi-0.1.3/LICENSE
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2638 2023-05-04 21:45:53.888811 fmpy_qi-0.1.3/PKG-INFO
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2106 2023-05-01 20:48:32.000000 fmpy_qi-0.1.3/README.md
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      741 2023-05-04 21:45:44.000000 fmpy_qi-0.1.3/pyproject.toml
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       38 2023-05-04 21:45:53.889298 fmpy_qi-0.1.3/setup.cfg
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-04 21:45:53.882777 fmpy_qi-0.1.3/src/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-30 21:24:30.000000 fmpy_qi-0.1.3/src/__init__.py
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-04 21:45:53.885679 fmpy_qi-0.1.3/src/fmpy/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-22 15:25:28.000000 fmpy_qi-0.1.3/src/fmpy/__init__.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     8022 2023-05-04 21:40:05.000000 fmpy_qi-0.1.3/src/fmpy/client.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)    12275 2023-04-23 08:55:58.000000 fmpy_qi-0.1.3/src/fmpy/urls.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      940 2023-04-30 16:47:40.000000 fmpy_qi-0.1.3/src/fmpy/utils.py
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-04 21:45:53.888420 fmpy_qi-0.1.3/src/fmpy_qi.egg-info/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2638 2023-05-04 21:45:53.000000 fmpy_qi-0.1.3/src/fmpy_qi.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      297 2023-05-04 21:45:53.000000 fmpy_qi-0.1.3/src/fmpy_qi.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        1 2023-05-04 21:45:53.000000 fmpy_qi-0.1.3/src/fmpy_qi.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       46 2023-05-04 21:45:53.000000 fmpy_qi-0.1.3/src/fmpy_qi.egg-info/requires.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       14 2023-05-04 21:45:53.000000 fmpy_qi-0.1.3/src/fmpy_qi.egg-info/top_level.txt
```

### Comparing `fmpy_qi-0.1.2/LICENSE` & `fmpy_qi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.2/PKG-INFO` & `fmpy_qi-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmpy_qi
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python wrapper for the Financial Modeling Prep API
 Author-email: Nicolas THIERY <nicles.thiery@gmail.com>
 Project-URL: Homepage, https://github.com/NicolasThiery/fmpy
 Project-URL: Bug Tracker, https://github.com/NicolasThiery/fmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fmpy_qi-0.1.2/README.md` & `fmpy_qi-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.2/pyproject.toml` & `fmpy_qi-0.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fmpy_qi"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Nicolas THIERY", email="nicles.thiery@gmail.com" },
 ]
 description = "A python wrapper for the Financial Modeling Prep API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `fmpy_qi-0.1.2/src/fmpy/client.py` & `fmpy_qi-0.1.3/src/fmpy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,16 @@
         _end = end
         batch_data = []
         end_date = None
         prev_start = None
         while True:
             url = self._get_historical_url(symbol, period, start, _end)
             data = self._request(url)
+            if not data:
+                return None
             data_list = data if isinstance(data, list) else data['historical']
             new_start = datetime.strftime(datetime.strptime(data_list[-1]['date'].split(' ')[0], '%Y-%m-%d') - timedelta(days=3), '%Y-%m-%d')
             sanitize_data = utils.limit_data_list(data_list, date_target=new_start, end_target=end_date)
             batch_data = sanitize_data + batch_data
             end_date = new_start
             new_start_datetime = datetime.strptime(new_start, '%Y-%m-%d')
             if new_start_datetime <= target_start_datetime or prev_start == new_start:
@@ -185,14 +187,15 @@
 
     def _convert_raw_data_to_df(self, raw_data):
         data_dict = {item: [] for item in raw_data[0].keys()}
         for data in raw_data[::-1]:
             for key, value in data.items():
                 data_dict[key].append(value)
         df = pd.DataFrame.from_dict(data_dict)
+        df = df.iloc[::-1]
         return df.set_index('date')
 
     def download_historical_data_to_excel(self, symbol, file, period='1d', start=None, end=None, sheet_name=None):
         """
         Description
         ----
         Gives current information for the provided list of assets (can be stocks,ETF,Funds,Index,Crypto and Commodities).
```

### Comparing `fmpy_qi-0.1.2/src/fmpy/urls.py` & `fmpy_qi-0.1.3/src/fmpy/urls.py`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.2/src/fmpy/utils.py` & `fmpy_qi-0.1.3/src/fmpy/utils.py`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.2/src/fmpy_qi.egg-info/PKG-INFO` & `fmpy_qi-0.1.3/src/fmpy_qi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmpy-qi
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python wrapper for the Financial Modeling Prep API
 Author-email: Nicolas THIERY <nicles.thiery@gmail.com>
 Project-URL: Homepage, https://github.com/NicolasThiery/fmpy
 Project-URL: Bug Tracker, https://github.com/NicolasThiery/fmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

