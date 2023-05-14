# Comparing `tmp/samadb-0.2.5.tar.gz` & `tmp/samadb-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samadb-0.2.5.tar", last modified: Sun May 14 17:41:07 2023, max compression
+gzip compressed data, was "samadb-0.2.6.tar", last modified: Sun May 14 21:43:40 2023, max compression
```

## Comparing `samadb-0.2.5.tar` & `samadb-0.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2023-05-14 17:41:07.189634 samadb-0.2.5/
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1076 2023-05-14 17:41:07.189760 samadb-0.2.5/PKG-INFO
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)      461 2023-03-17 09:12:39.000000 samadb-0.2.5/README.md
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)       79 2023-05-14 17:41:07.190151 samadb-0.2.5/setup.cfg
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1758 2023-05-14 17:40:47.000000 samadb-0.2.5/setup.py
-drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2023-05-14 17:41:07.186623 samadb-0.2.5/src/
-drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2023-05-14 17:41:07.189358 samadb-0.2.5/src/samadb.egg-info/
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1076 2023-05-14 17:41:07.000000 samadb-0.2.5/src/samadb.egg-info/PKG-INFO
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)      211 2023-05-14 17:41:07.000000 samadb-0.2.5/src/samadb.egg-info/SOURCES.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)        1 2023-05-14 17:41:07.000000 samadb-0.2.5/src/samadb.egg-info/dependency_links.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)       26 2023-05-14 17:41:07.000000 samadb-0.2.5/src/samadb.egg-info/requires.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)        7 2023-05-14 17:41:07.000000 samadb-0.2.5/src/samadb.egg-info/top_level.txt
--rw-r--r--   0 sebastiankrantz   (501) staff       (20)    25882 2023-05-14 17:09:49.000000 samadb-0.2.5/src/samadb.py
+drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2023-05-14 21:43:40.222530 samadb-0.2.6/
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1075 2023-05-14 21:43:40.222595 samadb-0.2.6/PKG-INFO
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)      460 2023-05-14 18:20:14.000000 samadb-0.2.6/README.md
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)       79 2023-05-14 21:43:40.222844 samadb-0.2.6/setup.cfg
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1758 2023-05-14 21:43:06.000000 samadb-0.2.6/setup.py
+drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2023-05-14 21:43:40.221279 samadb-0.2.6/src/
+drwxr-xr-x   0 sebastiankrantz   (501) staff       (20)        0 2023-05-14 21:43:40.222400 samadb-0.2.6/src/samadb.egg-info/
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)     1075 2023-05-14 21:43:40.000000 samadb-0.2.6/src/samadb.egg-info/PKG-INFO
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)      211 2023-05-14 21:43:40.000000 samadb-0.2.6/src/samadb.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)        1 2023-05-14 21:43:40.000000 samadb-0.2.6/src/samadb.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)       26 2023-05-14 21:43:40.000000 samadb-0.2.6/src/samadb.egg-info/requires.txt
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)        7 2023-05-14 21:43:40.000000 samadb-0.2.6/src/samadb.egg-info/top_level.txt
+-rw-r--r--   0 sebastiankrantz   (501) staff       (20)    25882 2023-05-14 17:09:49.000000 samadb-0.2.6/src/samadb.py
```

### Comparing `samadb-0.2.5/PKG-INFO` & `samadb-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: samadb
-Version: 0.2.5
+Version: 0.2.6
 Summary: An python providing access to a relational database with macroeconomic data for South Africa.
 Author: Sebastian Krantz
 Author-email: sebastian.krantz@graduateinstitute.ch
 License: GPL-3
 Project-URL: Bug Reports, https://github.com/Stellenbosch-Econometrics/SAMADB-Issues/issues
 Keywords: south africa,macroeconomic,data,API
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 
 # South Africa Macroeconomic Database API
 
-A python API providing access to a relational database with macroeconomic data for South Africa, obtained from the South African Reserve Bank (SARB) and Statistics South Africa (STATSSA), and updated on a regular basis via the EconData (https://www.econdata.co.za/) platform and automated scraping of the SARB and STATSSA websites. The database is maintained at the Department of Economics at Stellenbosch University.
+A python API providing access to a relational database with macroeconomic data for South Africa, obtained from the South African Reserve Bank (SARB) and Statistics South Africa (STATSSA), and updated on a weekly basis via the EconData (https://www.econdata.co.za/) platform and automated scraping of the SARB and STATSSA websites. The database is maintained at the Department of Economics at Stellenbosch University.
```

### Comparing `samadb-0.2.5/setup.py` & `samadb-0.2.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name='samadb',
-    version='0.2.5',
+    version='0.2.6',
     description='An python providing access to a relational database with macroeconomic data for South Africa.',
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",
     # url='',
     author="Sebastian Krantz",
     author_email='sebastian.krantz@graduateinstitute.ch',
     # Classifiers help users find your project by categorizing it.
```

### Comparing `samadb-0.2.5/src/samadb.egg-info/PKG-INFO` & `samadb-0.2.6/src/samadb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: samadb
-Version: 0.2.5
+Version: 0.2.6
 Summary: An python providing access to a relational database with macroeconomic data for South Africa.
 Author: Sebastian Krantz
 Author-email: sebastian.krantz@graduateinstitute.ch
 License: GPL-3
 Project-URL: Bug Reports, https://github.com/Stellenbosch-Econometrics/SAMADB-Issues/issues
 Keywords: south africa,macroeconomic,data,API
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 
 # South Africa Macroeconomic Database API
 
-A python API providing access to a relational database with macroeconomic data for South Africa, obtained from the South African Reserve Bank (SARB) and Statistics South Africa (STATSSA), and updated on a regular basis via the EconData (https://www.econdata.co.za/) platform and automated scraping of the SARB and STATSSA websites. The database is maintained at the Department of Economics at Stellenbosch University.
+A python API providing access to a relational database with macroeconomic data for South Africa, obtained from the South African Reserve Bank (SARB) and Statistics South Africa (STATSSA), and updated on a weekly basis via the EconData (https://www.econdata.co.za/) platform and automated scraping of the SARB and STATSSA websites. The database is maintained at the Department of Economics at Stellenbosch University.
```

### Comparing `samadb-0.2.5/src/samadb.py` & `samadb-0.2.6/src/samadb.py`

 * *Files identical despite different names*

