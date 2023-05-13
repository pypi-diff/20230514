# Comparing `tmp/kiwis-pie-0.8.0.tar.gz` & `tmp/kiwis-pie-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kiwis-pie-0.8.0.tar", last modified: Wed Feb  7 01:11:21 2018, max compression
+gzip compressed data, was "dist/kiwis-pie-0.9.0.tar", last modified: Mon Apr 30 22:58:53 2018, max compression
```

## Comparing `kiwis-pie-0.8.0.tar` & `kiwis-pie-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/
--rw-r--r--   0 amacdon    (501) staff       (20)       35 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/.gitattributes
--rw-r--r--   0 amacdon    (501) staff       (20)      164 2017-05-09 07:58:41.000000 kiwis-pie-0.8.0/.gitignore
-drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/conda.recipe/
--rw-r--r--   0 amacdon    (501) staff       (20)       24 2017-05-09 07:58:47.000000 kiwis-pie-0.8.0/conda.recipe/build.sh
--rw-r--r--   0 amacdon    (501) staff       (20)      422 2017-05-09 22:08:21.000000 kiwis-pie-0.8.0/conda.recipe/meta.yaml
-drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/docs/
--rw-r--r--   0 amacdon    (501) staff       (20)    11565 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/docs/conf.py
--rw-r--r--   0 amacdon    (501) staff       (20)      450 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/docs/index.rst
--rw-r--r--   0 amacdon    (501) staff       (20)     7248 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/docs/make.bat
--rw-r--r--   0 amacdon    (501) staff       (20)     7417 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/docs/Makefile
--rw-r--r--   0 amacdon    (501) staff       (20)    72191 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/kiwis_and_pie.jpg
-drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/kiwis_pie/
--rw-r--r--   0 amacdon    (501) staff       (20)      152 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/kiwis_pie/__init__.py
--rw-r--r--   0 amacdon    (501) staff       (20)      471 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/kiwis_pie/_version.py
--rw-r--r--   0 amacdon    (501) staff       (20)    11266 2017-05-09 07:58:41.000000 kiwis-pie-0.8.0/kiwis_pie/kiwis.py
-drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/kiwis_pie/testing/
--rw-r--r--   0 amacdon    (501) staff       (20)        0 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/kiwis_pie/testing/__init__.py
-drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/kiwis_pie/testing/test_data/
--rw-r--r--   0 amacdon    (501) staff       (20)      610 2017-05-09 07:58:41.000000 kiwis-pie-0.8.0/kiwis_pie/testing/test_data/bom_parameter_list.csv
--rw-r--r--   0 amacdon    (501) staff       (20)      709 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/kiwis_pie/testing/test_data/bom_parameter_list.request
--rw-r--r--   0 amacdon    (501) staff       (20)      670 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/kiwis_pie/testing/test_data/LICENSE
--rw-r--r--   0 amacdon    (501) staff       (20)      963 2017-05-09 07:58:41.000000 kiwis-pie-0.8.0/kiwis_pie/testing/test_kiwis_pie.py
-drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/kiwis_pie.egg-info/
--rw-r--r--   0 amacdon    (501) staff       (20)        1 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/kiwis_pie.egg-info/dependency_links.txt
--rw-r--r--   0 amacdon    (501) staff       (20)     3604 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/kiwis_pie.egg-info/PKG-INFO
--rw-r--r--   0 amacdon    (501) staff       (20)       25 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/kiwis_pie.egg-info/requires.txt
--rw-r--r--   0 amacdon    (501) staff       (20)      643 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/kiwis_pie.egg-info/SOURCES.txt
--rw-r--r--   0 amacdon    (501) staff       (20)       10 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/kiwis_pie.egg-info/top_level.txt
--rw-r--r--   0 amacdon    (501) staff       (20)     1420 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/LICENSE
--rw-r--r--   0 amacdon    (501) staff       (20)       52 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/MANIFEST.in
--rw-r--r--   0 amacdon    (501) staff       (20)     3604 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/PKG-INFO
--rw-r--r--   0 amacdon    (501) staff       (20)     2292 2017-05-09 07:58:41.000000 kiwis-pie-0.8.0/README.rst
--rw-r--r--   0 amacdon    (501) staff       (20)      207 2018-02-07 01:11:21.000000 kiwis-pie-0.8.0/setup.cfg
--rw-r--r--   0 amacdon    (501) staff       (20)     1492 2017-05-09 21:39:45.000000 kiwis-pie-0.8.0/setup.py
--rw-r--r--   0 amacdon    (501) staff       (20)    65747 2017-01-11 10:20:00.000000 kiwis-pie-0.8.0/versioneer.py
+drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/
+-rw-r--r--   0 amacdon    (501) staff       (20)       35 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/.gitattributes
+-rw-r--r--   0 amacdon    (501) staff       (20)      164 2017-05-09 07:58:41.000000 kiwis-pie-0.9.0/.gitignore
+drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/conda.recipe/
+-rw-r--r--   0 amacdon    (501) staff       (20)       24 2017-05-09 07:58:47.000000 kiwis-pie-0.9.0/conda.recipe/build.sh
+-rw-r--r--   0 amacdon    (501) staff       (20)      422 2017-05-09 22:08:21.000000 kiwis-pie-0.9.0/conda.recipe/meta.yaml
+drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/docs/
+-rw-r--r--   0 amacdon    (501) staff       (20)    11565 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/docs/conf.py
+-rw-r--r--   0 amacdon    (501) staff       (20)      450 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/docs/index.rst
+-rw-r--r--   0 amacdon    (501) staff       (20)     7248 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/docs/make.bat
+-rw-r--r--   0 amacdon    (501) staff       (20)     7417 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/docs/Makefile
+-rw-r--r--   0 amacdon    (501) staff       (20)    72191 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/kiwis_and_pie.jpg
+drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/kiwis_pie/
+-rw-r--r--   0 amacdon    (501) staff       (20)      152 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/kiwis_pie/__init__.py
+-rw-r--r--   0 amacdon    (501) staff       (20)      471 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/kiwis_pie/_version.py
+-rw-r--r--   0 amacdon    (501) staff       (20)    12006 2018-04-30 22:56:30.000000 kiwis-pie-0.9.0/kiwis_pie/kiwis.py
+drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/kiwis_pie/testing/
+-rw-r--r--   0 amacdon    (501) staff       (20)        0 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/kiwis_pie/testing/__init__.py
+drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/kiwis_pie/testing/test_data/
+-rw-r--r--   0 amacdon    (501) staff       (20)      610 2017-05-09 07:58:41.000000 kiwis-pie-0.9.0/kiwis_pie/testing/test_data/bom_parameter_list.csv
+-rw-r--r--   0 amacdon    (501) staff       (20)      709 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/kiwis_pie/testing/test_data/bom_parameter_list.request
+-rw-r--r--   0 amacdon    (501) staff       (20)      670 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/kiwis_pie/testing/test_data/LICENSE
+-rw-r--r--   0 amacdon    (501) staff       (20)      963 2017-05-09 07:58:41.000000 kiwis-pie-0.9.0/kiwis_pie/testing/test_kiwis_pie.py
+drwxr-xr-x   0 amacdon    (501) staff       (20)        0 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/kiwis_pie.egg-info/
+-rw-r--r--   0 amacdon    (501) staff       (20)        1 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/kiwis_pie.egg-info/dependency_links.txt
+-rw-r--r--   0 amacdon    (501) staff       (20)     3815 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/kiwis_pie.egg-info/PKG-INFO
+-rw-r--r--   0 amacdon    (501) staff       (20)       25 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/kiwis_pie.egg-info/requires.txt
+-rw-r--r--   0 amacdon    (501) staff       (20)      643 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/kiwis_pie.egg-info/SOURCES.txt
+-rw-r--r--   0 amacdon    (501) staff       (20)       10 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/kiwis_pie.egg-info/top_level.txt
+-rw-r--r--   0 amacdon    (501) staff       (20)     1420 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/LICENSE
+-rw-r--r--   0 amacdon    (501) staff       (20)       52 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/MANIFEST.in
+-rw-r--r--   0 amacdon    (501) staff       (20)     3815 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/PKG-INFO
+-rw-r--r--   0 amacdon    (501) staff       (20)     2479 2018-04-30 22:57:47.000000 kiwis-pie-0.9.0/README.rst
+-rw-r--r--   0 amacdon    (501) staff       (20)      228 2018-04-30 22:58:53.000000 kiwis-pie-0.9.0/setup.cfg
+-rw-r--r--   0 amacdon    (501) staff       (20)     1492 2017-05-09 21:39:45.000000 kiwis-pie-0.9.0/setup.py
+-rw-r--r--   0 amacdon    (501) staff       (20)    65747 2017-01-11 10:20:00.000000 kiwis-pie-0.9.0/versioneer.py
```

### Comparing `kiwis-pie-0.8.0/docs/conf.py` & `kiwis-pie-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kiwis-pie-0.8.0/docs/make.bat` & `kiwis-pie-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kiwis-pie-0.8.0/docs/Makefile` & `kiwis-pie-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kiwis-pie-0.8.0/kiwis_and_pie.jpg` & `kiwis-pie-0.9.0/kiwis_and_pie.jpg`

 * *Files identical despite different names*

### Comparing `kiwis-pie-0.8.0/kiwis_pie/kiwis.py` & `kiwis-pie-0.9.0/kiwis_pie/kiwis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import collections
 QueryOption = collections.namedtuple('QueryOption', ['wildcard', 'list', 'parser'])
 
 import pandas as pd
+import pytz
 import re
 import requests
 from tabulate import tabulate
 
 import logging
 logger = logging.getLogger(__name__)
 
@@ -46,15 +47,15 @@
     return pd.to_datetime(input_dt).strftime('%Y-%m-%d')
 
 def __gen_kiwis_method(cls, method_name, available_query_options, available_return_fields):
 
     start_snake = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', method_name)
     snake_name = re.sub('([a-z0-9])([A-Z])', r'\1_\2', start_snake).lower()
 
-    def kiwis_method(self, return_fields = None, **kwargs):
+    def kiwis_method(self, return_fields = None, keep_tz=False, **kwargs):
 
         for query_key in kwargs.keys():
             if query_key not in available_query_options.keys():
                 raise ValueError(query_key)
 
             if (available_query_options[query_key].list and
                     isinstance(kwargs[query_key], collections.Iterable) and
@@ -70,21 +71,21 @@
                     raise ValueError(return_key)
 
         params = self._KIWIS__default_args.copy()
         params.update(kwargs)
         params['request'] = method_name
         if return_fields is not None:
             params['returnfields'] = ','.join(return_fields)
-        
-        
+
+
         r = requests.get(self.server_url, params = params)
         logger.debug(r.url)
         logger.debug(r.status_code)
         r.raise_for_status() #raise error if service returns an error, i.e. 404, 500 etc.
-        
+
         json_data = r.json()
         if type(json_data) is dict and 'type' in json_data.keys() and json_data['type'] == 'error':
             raise KIWISError(
                 'KIWIS returned an error:\n\tCode: {0}\n\tMessage: "{1}"'.format(
                     json_data['code'],
                     json_data['message']
                 )
@@ -101,25 +102,35 @@
                 'getTimeseriesList'
             ]:
             return pd.DataFrame(json_data[1:], columns = json_data[0])
         elif method_name in ['getTimeseriesValues']:
             df = pd.DataFrame(json_data[0]['data'], columns = json_data[0]['columns'].split(','))
             if 'Timestamp' in df.columns:
                 df.set_index('Timestamp', inplace = True)
-                df.index = pd.to_datetime(df.index)
+                if keep_tz:
+                    hour_offset, minute_offset = map(int, df.index[0].split('+')[1].split(':'))
+                    logger.debug('Using timezone offset %d hour(s) and %d minute(s)', hour_offset, minute_offset)
+                    df.index = pd.to_datetime(df.index).tz_localize('UTC').tz_convert(pytz.FixedOffset(hour_offset*60+minute_offset))
+                else:
+                    df.index = pd.to_datetime(df.index)
             return df
         else:
             raise NotImplementedError("Method '{0}' has no return implemented.".format(method_name))
 
     docstring = {}
     docstring['doc_intro'] = "Python method to query the '{0}' KiWIS method.".format(method_name)
 
     docstring['doc_intro'] += "\n\nKeyword arguments are those available in the 'Query field' name list below. "
     docstring['doc_intro'] += "That is the keywords match the Queryfield names used by KiWIS."
 
+    docstring['doc_intro'] += "\n\n:param keep_tz: "
+    docstring['doc_intro'] += "Set to true to prevent the series datetimes from being converted to UTC."
+    docstring['doc_intro'] += " This optional argument only applies when the returned data includes data with timestamps."
+    docstring['doc_intro'] += "\n:type keep_tz: boolean"
+
     docstring['return_fields'] = ":type return_fields: list(string)\n:param return_fields: Optional keyword argument, which is a list made up from the following available fields:\n\n * {0}.".format(',\n * '.join(available_return_fields))
 
     doc_map = {
         True: 'yes',
         False: 'no',
         None: 'n/a',
     }
```

### Comparing `kiwis-pie-0.8.0/kiwis_pie/testing/test_data/bom_parameter_list.csv` & `kiwis-pie-0.9.0/kiwis_pie/testing/test_data/bom_parameter_list.csv`

 * *Files identical despite different names*

### Comparing `kiwis-pie-0.8.0/kiwis_pie/testing/test_data/bom_parameter_list.request` & `kiwis-pie-0.9.0/kiwis_pie/testing/test_data/bom_parameter_list.request`

 * *Files identical despite different names*

### Comparing `kiwis-pie-0.8.0/kiwis_pie/testing/test_data/LICENSE` & `kiwis-pie-0.9.0/kiwis_pie/testing/test_data/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwis-pie-0.8.0/kiwis_pie/testing/test_kiwis_pie.py` & `kiwis-pie-0.9.0/kiwis_pie/testing/test_kiwis_pie.py`

 * *Files identical despite different names*

### Comparing `kiwis-pie-0.8.0/kiwis_pie.egg-info/PKG-INFO` & `kiwis-pie-0.9.0/kiwis_pie.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kiwis-pie
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python library for accessing a Kisters WISKI system via the KiWIS API.
 Home-page: https://github.com/amacd31/kiwis_pie
 Author: Andrew MacDonald
 Author-email: andrew@maccas.net
 License: BSD
 Description: Kiwis Pie
         ===============
@@ -56,14 +56,17 @@
         
          # Get timeseries ID for daily mean streamflow (Q) at Cotter River at Gingera
          ts_id = k.get_timeseries_list(station_id = station_id, ts_name = 'DMQaQc.Merged.DailyMean.24HR', parametertype_name = 'Water Course Discharge').ts_id.values[0]
         
          # Read 31 days of daily water course discharge data for Cotter River at Gingera
          k.get_timeseries_values(ts_id = ts_id, to = date(2016,1,31), **{'from': date(2016,1,1)})
         
+         # Optionally use the `keep_tz` option to return in local timezone instead of UTC
+         k.get_timeseries_values(ts_id = ts_id, to = date(2016,1,31), **{'from': date(2016,1,1)}, keep_tz=True)
+        
         Documentation
         -------------
         The methods on the KIWIS class all have docstrings detailing the keyword arguments they take.
         Rendered documentation is available on Read the Docs: http://kiwis-pie.readthedocs.io/en/latest/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kiwis-pie-0.8.0/kiwis_pie.egg-info/SOURCES.txt` & `kiwis-pie-0.9.0/kiwis_pie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiwis-pie-0.8.0/LICENSE` & `kiwis-pie-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwis-pie-0.8.0/PKG-INFO` & `kiwis-pie-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kiwis-pie
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python library for accessing a Kisters WISKI system via the KiWIS API.
 Home-page: https://github.com/amacd31/kiwis_pie
 Author: Andrew MacDonald
 Author-email: andrew@maccas.net
 License: BSD
 Description: Kiwis Pie
         ===============
@@ -56,14 +56,17 @@
         
          # Get timeseries ID for daily mean streamflow (Q) at Cotter River at Gingera
          ts_id = k.get_timeseries_list(station_id = station_id, ts_name = 'DMQaQc.Merged.DailyMean.24HR', parametertype_name = 'Water Course Discharge').ts_id.values[0]
         
          # Read 31 days of daily water course discharge data for Cotter River at Gingera
          k.get_timeseries_values(ts_id = ts_id, to = date(2016,1,31), **{'from': date(2016,1,1)})
         
+         # Optionally use the `keep_tz` option to return in local timezone instead of UTC
+         k.get_timeseries_values(ts_id = ts_id, to = date(2016,1,31), **{'from': date(2016,1,1)}, keep_tz=True)
+        
         Documentation
         -------------
         The methods on the KIWIS class all have docstrings detailing the keyword arguments they take.
         Rendered documentation is available on Read the Docs: http://kiwis-pie.readthedocs.io/en/latest/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kiwis-pie-0.8.0/README.rst` & `kiwis-pie-0.9.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -48,11 +48,14 @@
 
  # Get timeseries ID for daily mean streamflow (Q) at Cotter River at Gingera
  ts_id = k.get_timeseries_list(station_id = station_id, ts_name = 'DMQaQc.Merged.DailyMean.24HR', parametertype_name = 'Water Course Discharge').ts_id.values[0]
 
  # Read 31 days of daily water course discharge data for Cotter River at Gingera
  k.get_timeseries_values(ts_id = ts_id, to = date(2016,1,31), **{'from': date(2016,1,1)})
 
+ # Optionally use the `keep_tz` option to return in local timezone instead of UTC
+ k.get_timeseries_values(ts_id = ts_id, to = date(2016,1,31), **{'from': date(2016,1,1)}, keep_tz=True)
+
 Documentation
 -------------
 The methods on the KIWIS class all have docstrings detailing the keyword arguments they take.
 Rendered documentation is available on Read the Docs: http://kiwis-pie.readthedocs.io/en/latest/
```

### Comparing `kiwis-pie-0.8.0/setup.py` & `kiwis-pie-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `kiwis-pie-0.8.0/versioneer.py` & `kiwis-pie-0.9.0/versioneer.py`

 * *Files identical despite different names*

