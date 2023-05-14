# Comparing `tmp/africamonitor-0.1.1.tar.gz` & `tmp/africamonitor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africamonitor-0.1.1.tar", last modified: Wed Nov 30 10:13:24 2022, max compression
+gzip compressed data, was "africamonitor-0.1.2.tar", last modified: Sun May 14 18:10:03 2023, max compression
```

## Comparing `africamonitor-0.1.1.tar` & `africamonitor-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2022-11-30 10:13:24.055462 africamonitor-0.1.1/
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)      420 2022-11-23 23:06:57.000000 africamonitor-0.1.1/LICENSE.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1461 2022-11-30 10:13:24.055536 africamonitor-0.1.1/PKG-INFO
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)      790 2022-11-24 08:37:36.000000 africamonitor-0.1.1/README.md
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)      107 2022-11-30 10:13:24.055812 africamonitor-0.1.1/setup.cfg
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1888 2022-11-30 09:52:21.000000 africamonitor-0.1.1/setup.py
-drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2022-11-30 10:13:24.054336 africamonitor-0.1.1/src/
-drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2022-11-30 10:13:24.055278 africamonitor-0.1.1/src/africamonitor.egg-info/
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1461 2022-11-30 10:13:24.000000 africamonitor-0.1.1/src/africamonitor.egg-info/PKG-INFO
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)      265 2022-11-30 10:13:24.000000 africamonitor-0.1.1/src/africamonitor.egg-info/SOURCES.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)        1 2022-11-30 10:13:24.000000 africamonitor-0.1.1/src/africamonitor.egg-info/dependency_links.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)       26 2022-11-30 10:13:24.000000 africamonitor-0.1.1/src/africamonitor.egg-info/requires.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)       14 2022-11-30 10:13:24.000000 africamonitor-0.1.1/src/africamonitor.egg-info/top_level.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)    30122 2022-11-30 10:09:50.000000 africamonitor-0.1.1/src/africamonitor.py
+drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2023-05-14 18:10:03.681753 africamonitor-0.1.2/
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)      420 2022-11-23 23:06:57.000000 africamonitor-0.1.2/LICENSE.txt
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1461 2023-05-14 18:10:03.681852 africamonitor-0.1.2/PKG-INFO
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)      790 2022-11-24 08:37:36.000000 africamonitor-0.1.2/README.md
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)      107 2023-05-14 18:10:03.682191 africamonitor-0.1.2/setup.cfg
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1888 2023-05-14 18:07:49.000000 africamonitor-0.1.2/setup.py
+drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2023-05-14 18:10:03.665398 africamonitor-0.1.2/src/
+drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2023-05-14 18:10:03.681548 africamonitor-0.1.2/src/africamonitor.egg-info/
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1461 2023-05-14 18:10:03.000000 africamonitor-0.1.2/src/africamonitor.egg-info/PKG-INFO
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)      265 2023-05-14 18:10:03.000000 africamonitor-0.1.2/src/africamonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)        1 2023-05-14 18:10:03.000000 africamonitor-0.1.2/src/africamonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)       26 2023-05-14 18:10:03.000000 africamonitor-0.1.2/src/africamonitor.egg-info/requires.txt
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)       14 2023-05-14 18:10:03.000000 africamonitor-0.1.2/src/africamonitor.egg-info/top_level.txt
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)    30186 2023-05-14 17:36:44.000000 africamonitor-0.1.2/src/africamonitor.py
```

### Comparing `africamonitor-0.1.1/PKG-INFO` & `africamonitor-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africamonitor
-Version: 0.1.1
+Version: 0.1.2
 Summary: An API providing access to a relational database with macroeconomic data for Africa.
 Home-page: https://africamonitor.ifw-kiel.de/
 Author: Sebastian Krantz
 Author-email: sebastian.krantz@graduateinstitute.ch
 License: GPL-3
 Project-URL: Bug Reports, https://github.com/IFW-Macro-Research-Group/africamonitor
 Keywords: africa,macroeconomic,data,API
```

### Comparing `africamonitor-0.1.1/README.md` & `africamonitor-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `africamonitor-0.1.1/setup.py` & `africamonitor-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name='africamonitor',
-    version='0.1.1',
+    version='0.1.2',
     description='An API providing access to a relational database with macroeconomic data for Africa.',
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",
     url='https://africamonitor.ifw-kiel.de/',
     author="Sebastian Krantz",
     author_email='sebastian.krantz@graduateinstitute.ch',
     # Classifiers help users find your project by categorizing it.
```

### Comparing `africamonitor-0.1.1/src/africamonitor.egg-info/PKG-INFO` & `africamonitor-0.1.2/src/africamonitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africamonitor
-Version: 0.1.1
+Version: 0.1.2
 Summary: An API providing access to a relational database with macroeconomic data for Africa.
 Home-page: https://africamonitor.ifw-kiel.de/
 Author: Sebastian Krantz
 Author-email: sebastian.krantz@graduateinstitute.ch
 License: GPL-3
 Project-URL: Bug Reports, https://github.com/IFW-Macro-Research-Group/africamonitor
 Keywords: africa,macroeconomic,data,API
```

### Comparing `africamonitor-0.1.1/src/africamonitor.py` & `africamonitor-0.1.2/src/africamonitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,15 +293,15 @@
 # print(result_1)
 #
 # x[5:7]
 # strptime("2011-01-01", pl.Date, "%Y-%m-%d")
 
 is_date = lambda x: (type(x) is _datetime.date or
           str(type(x)) in ["<class 'datetime.date'>", "<class 'datetime.datetime'>"] or
-          (type(x) is _pl.internals.series.series.Series and
+          (str(type(x)) == "<class 'polars.internals.series.series.Series'>" and
            x.dtype is _pl.datatypes.Date))
 
 
 def as_date(x, end = False):
   """Coerce Input to Date-String.
 
         Parameters:
@@ -486,15 +486,15 @@
          return_query = False,
          **kwargs):
     """Retrieve Data from the Africamonitor Database.
 
         This is the main function of the package and used to retrieve data from the Africamonitor Database.
 
         Parameters:
-            ctry: list of ISO3 country codes. There is a variable 'AMCOUNTRY' in the package namespace containing the codes of all 55 African countries, and this list is specified as the default argument, but the database has data for all countries where available. The codes for all countries can be found in the 'am.countries_wld()' table.
+            ctry: list of ISO3 country codes. There is a variable 'AMCOUNTRY' in the package namespace containing the codes of all 55 African countries, and this list is specified as the default argument, but the database has data for all countries where available. The codes for all countries can be found in the 'am.countries_wld()' table. Putting 'None' gets data for all countries.
             series: list of series codes matching the 'Series' column of the SERIES table (retrieved using 'am.series()').
             tfrom: set the start time of the data retrieved by either supplying a start date, a date-string of the form "YYYY-MM-DD" or "YYYY-MM", year-quarters of the form "YYYYQN" or "YYYY-QN", a numeric year YYYY (integer or string), or a fiscal year of the form "YYYY/YY". These expressions are converted to a regular date (first day of period) by the included 'as_date()' function.
             tto: same as 'from', to set the time period until which data is retrieved. For expressions that are not full "YYYY-MM-DD" dates, the last day of the period is chosen.
             labels: logical. 'True' will also return labels (series descriptions) along with the series codes. If 'wide = True', labels are returned in a separate DataFrame.
             wide: logical. 'True' calls 'am.pivot_wider()' on the result. 'False' returns the data in a long format without missing values.
             expand_date: logical. 'True' will call 'am.expand_date()' on the result.
             drop_1iso3c: logical. If only one country is selected through 'ctry', 'True' will drop the 'ISO3' column in the output.
```

