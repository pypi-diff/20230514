# Comparing `tmp/datazets-0.1.3.tar.gz` & `tmp/datazets-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datazets-0.1.3.tar", last modified: Sun May 14 11:30:25 2023, max compression
+gzip compressed data, was "datazets-0.1.4.tar", last modified: Sun May 14 16:58:27 2023, max compression
```

## Comparing `datazets-0.1.3.tar` & `datazets-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 11:30:25.557941 datazets-0.1.3/
--rw-rw-rw-   0        0        0     1121 2022-03-22 18:16:18.000000 datazets-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       56 2023-05-12 07:39:26.000000 datazets-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4654 2023-05-14 11:30:25.543526 datazets-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4060 2023-05-13 19:04:51.000000 datazets-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 11:30:25.494263 datazets-0.1.3/datazets/
--rw-rw-rw-   0        0        0      700 2023-05-14 11:30:00.000000 datazets-0.1.3/datazets/__init__.py
--rw-rw-rw-   0        0        0    15441 2023-05-14 11:22:45.000000 datazets-0.1.3/datazets/datazets.py
--rw-rw-rw-   0        0        0      988 2023-05-14 11:28:51.000000 datazets-0.1.3/datazets/examples.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:30:25.542556 datazets-0.1.3/datazets/utils/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 datazets-0.1.3/datazets/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:30:25.541532 datazets-0.1.3/datazets.egg-info/
--rw-rw-rw-   0        0        0     4654 2023-05-14 11:30:25.000000 datazets-0.1.3/datazets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-14 11:30:25.000000 datazets-0.1.3/datazets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 11:30:25.000000 datazets-0.1.3/datazets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-14 11:30:25.000000 datazets-0.1.3/datazets.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 11:30:25.000000 datazets-0.1.3/datazets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 11:30:25.557941 datazets-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1382 2023-05-13 18:52:09.000000 datazets-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 16:58:27.069577 datazets-0.1.4/
+-rw-rw-rw-   0        0        0     1121 2022-03-22 18:16:18.000000 datazets-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-05-12 07:39:26.000000 datazets-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4613 2023-05-14 16:58:27.068583 datazets-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4060 2023-05-13 19:04:51.000000 datazets-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 16:58:27.026581 datazets-0.1.4/datazets/
+-rw-rw-rw-   0        0        0      755 2023-05-14 16:57:49.000000 datazets-0.1.4/datazets/__init__.py
+-rw-rw-rw-   0        0        0    15624 2023-05-14 16:52:31.000000 datazets-0.1.4/datazets/datazets.py
+-rw-rw-rw-   0        0        0      987 2023-05-14 16:33:27.000000 datazets-0.1.4/datazets/examples.py
+drwxrwxrwx   0        0        0        0 2023-05-14 16:58:27.066587 datazets-0.1.4/datazets/utils/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 datazets-0.1.4/datazets/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 16:58:27.063593 datazets-0.1.4/datazets.egg-info/
+-rw-rw-rw-   0        0        0     4613 2023-05-14 16:58:26.000000 datazets-0.1.4/datazets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-14 16:58:26.000000 datazets-0.1.4/datazets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 16:58:26.000000 datazets-0.1.4/datazets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-14 16:58:26.000000 datazets-0.1.4/datazets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 16:58:26.000000 datazets-0.1.4/datazets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 16:58:27.069577 datazets-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1382 2023-05-13 18:52:09.000000 datazets-0.1.4/setup.py
```

### Comparing `datazets-0.1.3/LICENSE` & `datazets-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datazets-0.1.3/PKG-INFO` & `datazets-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: datazets
-Version: 0.1.3
+Version: 0.1.4
 Summary: Datazets is a python package to import well known example data sets.
 Home-page: https://github.com/erdogant/datazets
+Download-URL: https://github.com/erdogant/datazets/archive/0.1.4.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/erdogant/datazets/archive/0.1.3.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -110,9 +108,7 @@
 
 ### Contribute
 * All kinds of contributions are welcome!
 * If you wish to buy me a <a href="https://www.buymeacoffee.com/erdogant">Coffee</a> for this work, it is very appreciated :)
 
 ### Licence
 See [LICENSE](LICENSE) for details.
-
-
```

### Comparing `datazets-0.1.3/README.md` & `datazets-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `datazets-0.1.3/datazets/__init__.py` & `datazets-0.1.4/datazets/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from datazets.datazets import get
+from datazets.datazets import get, get_dataproperties, download_from_url, unzip, listdir
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 # module level doc-string
 __doc__ = """
 datazets
 =====================================================================
 
 Description
```

### Comparing `datazets-0.1.3/datazets/datazets.py` & `datazets-0.1.4/datazets/datazets.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     data : str
         Multicollinear data sets:
             * 'titanic'
             * 'student'
             * 'fifa'
             * 'DS_salaries'
             * 'waterpump'
-            * 'USA_elections'
+            * 'elections'
             * 'tips'
             * 'predictive_maintenance'
         source-target
             * 'energy'
             * 'stormofswords'
         time-series
             * 'occupancy'
@@ -116,46 +116,63 @@
     """
     set_logger(verbose=verbose)
     if data is None and url is None:
         logger.error('Input parameter <data> or <url> should be used.')
         return None
 
     # Get and Set data information
-    dataproperties = adjust_to_urlname(data, sep, url)
+    dataproperties = get_dataproperties(data, sep, url)
     logger.info('Import dataset [%s]' %(dataproperties['input']))
 
     if dataproperties['url'] is None:
         logger.info('Nothing to download.')
         return None
 
     # Import dataset
     if dataproperties['type']=='files':
-        df = _import_image_data(dataproperties)
+        df = _extract_files(dataproperties)
     elif dataproperties['type']=='synthetic':
         df = _generate_data(dataproperties['filename'], **args)
+    elif dataproperties['type']=='DAG':
+        df = _extract_files(dataproperties, targetdir=os.path.join(dataproperties['curpath'], dataproperties['input']), ext='*')
+        # PATH_TO_DATA = download_from_url(dataproperties['filename'], url=dataproperties['url'], dataproperties=dataproperties)
     else:
         PATH_TO_DATA = download_from_url(dataproperties['filename'], url=dataproperties['url'])
         df = pd.read_csv(PATH_TO_DATA, sep=dataproperties['sep'])
-
+    
+    df = _set_dtypes(df, dataproperties)
     # Return
     return df
 
 
 # %%
+def _set_dtypes(df, dataproperties):
+    if dataproperties['input']=='auto_mpg':
+        df['mpg'] = df['mpg'].astype('float64')
+        df['cylinders'] = df['cylinders'].astype('int64')
+        df['displacement'] = df['displacement'].astype('float64')
+        df['horsepower'] = df['horsepower'].astype('float64')
+        df['weight'] = df['weight'].astype('float64')
+        df['acceleration'] = df['acceleration'].astype('float64')
+        df['model_year'] = df['model_year'].astype('int64')
+        df['origin'] = df['origin'].astype('int64')
+    return df
+
+# %%
 def _generate_data(urlname, **args):
     df = None
     # Generate discrete random data
     if urlname=='random_discrete':
         n = args.get('n', None) if args.get('n', None) is not None else 1000
         df = pd.DataFrame(np.random.randint(low=0, high=2, size=(n, 5)), columns=['A', 'B', 'C', 'D', 'E'])
     return df
 
 
 # %%
-def _import_image_data(dataproperties, **args):
+def _extract_files(dataproperties, **args):
     """Import example dataset from github source.
 
     Import one of the few datasets from github source or specify your own download url link.
 
     Parameters
     ----------
     data : str
@@ -168,51 +185,44 @@
 
     Returns
     -------
     pd.DataFrame()
         Dataset containing mixed features.
 
     """
-    # if dataproperties['filename']=='faces':
-    #     from sklearn.datasets import fetch_olivetti_faces
-    #     X = fetch_olivetti_faces()
-    #     return X['data']
-    #     df = pd.DataFrame(data=X['data'], index=X['target'])
-    # if dataproperties['filename']=='mnist':
-        # from sklearn.datasets import load_digits
-        # n = args.get('n', None) if args.get('n', None) is not None else 10
-        # X = load_digits(n_class=n)
-        # df = pd.DataFrame(data=X['data'], index=X['target'])
-        # return X.data
+    targetdir = args.get('targetdir', None) if args.get('targetdir', None) is not None else None
+    ext = args.get('ext', None) if args.get('ext', None) is not None else ['png', 'tiff', 'jpg']
 
     # Collect data
     PATH_TO_DATA = download_from_url(dataproperties['filename'], url=dataproperties['url'])
     # Unzip
-    dirpath = unzip(PATH_TO_DATA)
+    dirpath = unzip(PATH_TO_DATA, targetdir=targetdir)
     # Import local dataset
-    image_files = listdir(dirpath)
+    image_files = listdir(dirpath, ext=ext)
     # Return
     return image_files
 
 
 # %% Get the correct url name.
-def adjust_to_urlname(data, sep, url=None):
+def get_dataproperties(data, sep=None, url=None):
     inputname, datatype = data, None
     if data is not None:
+        data = data.lower()
         # Set datatype for imges
         if data=='flowers' or data=='scenes' or data=='southern_nebula':
             datatype='files'
             if data=='flowers': data = 'flower_images.zip'
             if data=='scenes': data = 'scenes.zip'
             # if data=='cat_and_dog': data = 'cat_and_dog.zip'
             # if data=='southern_nebula': data = 'southern_nebula.zip'
-            
-
         elif data=='alarm' or data=='andes' or data=='asia' or data=='sachs' or data=='water':
             datatype='DAG'
+            if os.path.splitext(data)[1]=='':
+                sep=','
+                data = data + '.zip'
         elif data=='random_discrete':
             datatype='synthetic'
         else:
             datatype='various'
             # Rename to correct filename
             if data=='titanic': data, sep ='titanic_train.zip', ','
             if data=='student': data, sep ='student_train.zip', ','
@@ -221,42 +231,31 @@
             if data=='ads': data, sep = 'ads_data.zip', ','
             if data=='bitcoin': data, sep = 'BTCUSDT.zip', ','
             if data=='meta': data, sep = 'facebook_stocks.zip', ','
             if data=='energy': data, sep = 'energy_source_target_value.zip', ','
             if data=='breast_cancer': data, sep = 'breast_cancer_dataset.zip', ';'
             if data=='marketing_retail': data, sep = 'marketing_data_online_retail_small.zip', ';'
             if data=='waterpump': data, sep = 'waterpump.zip', ';'
-            if data=='USA_elections': data, sep = 'USA_2016_elections.zip', ','
+            if data=='elections': data, sep = 'USA_2016_elections.zip', ','
             if data=='occupancy': data, sep = 'UCI_Occupancy_Detection.zip', ','
             if data=='predictive_maintenance': data, sep = 'predictive_maintenance_ai4i2020.zip', ','
             if data=='iris': data, sep = 'iris_dataset.zip', ';'
             if data=='gas_prices': data, sep = 'Henry_Hub_Natural_Gas_Spot_Price.zip', ','
             if data=='grocery_products': data, sep = 'grocery_products_purchase.zip', ','
-            # if data=='movingbubbles': data, sep = 'movingbubbles.zip', ','
-
             # images
             if data=='faces': data, sep = 'olivetti_faces.zip', ';'
             if data=='mnist': data, sep = 'mnist_images.zip', ';'
-            # if data=='tips': data, sep = 'tips.zip', ','
-            # if data=='sprinkler': data, sep ='sprinkler.zip', ','
-            # if data=='DS_salaries': data, sep = 'DS_salaries.zip', ','
-            # if data=='auto_mpg': data, sep = 'auto_mpg.zip', ','
-            # if data=='stormofswords': data, sep = 'stormofswords.zip', ','
-            # if data=='census_income': data, sep = 'census_income.zip', ','
-            # if data=='malicious_urls': data, sep = 'malicious_urls.zip', ','
-            # if data=='digits': data, sep = 'digits.zip', ','
 
             if os.path.splitext(data)[1]=='':
                 sep=','
                 data = data + '.zip'
 
-            # 
-
+    curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
     # Set the url
-    dataproperties = {'input': inputname, 'filename': data, 'sep': sep, 'type': datatype, 'url': url}
+    dataproperties = {'input': inputname, 'filename': data, 'sep': sep, 'type': datatype, 'url': url, 'curpath': curpath}
     # Get filename from url
     if url is not None:
         dataproperties['filename'] = wget.filename_from_url(url, ext=False)
         dataproperties['input'] = dataproperties['filename']
     else:
         dataproperties['url'] = 'https://erdogant.github.io/datasets/' + dataproperties['filename']
 
@@ -293,15 +292,15 @@
 
     getfiles = []
     for root, _, filenames in os.walk(dirpath):
         # Check if the (sub)directory is black listed
         bl_found = np.isin(os.path.split(root)[1], black_list)
         if (black_list is None) or (not bl_found):
             for iext in ext:
-                for filename in fnmatch.filter(filenames, '*.' +iext):
+                for filename in fnmatch.filter(filenames, '*.' + iext):
                     getfiles.append(os.path.join(root, filename))
         else:
             logger.info('Excluded: <%s>' %(root))
     logger.info('[%s] files are collected recursively from path: [%s]', len(getfiles), dirpath)
     return getfiles
 
 
@@ -333,15 +332,15 @@
         r = requests.get(url, stream=True)
         with open(writepath, "wb") as fd:
             for chunk in r.iter_content(chunk_size=1024):
                 fd.write(chunk)
 
 
 # %% unzip
-def unzip(path_to_zip, outputdir=None):
+def unzip(path_to_zip, targetdir=None):
     """Unzip files.
 
     Parameters
     ----------
     path_to_zip : str
         Path of the zip file.
 
@@ -357,18 +356,18 @@
 
     """
     getpath = None
     if path_to_zip[-4:]=='.zip':
         if not os.path.isdir(path_to_zip):
 
             logger.info('Extracting files..')
-            if outputdir is None:
+            if targetdir is None:
                 pathname, _ = os.path.split(path_to_zip)
             else:
-                pathname = outputdir
+                pathname = targetdir
 
             # Unzip
             zip_ref = zipfile.ZipFile(path_to_zip, 'r')
             zip_ref.extractall(pathname)
             zip_ref.close()
             getpath = path_to_zip.replace('.zip', '')
             if not os.path.isdir(getpath):
@@ -433,31 +432,21 @@
 
 # %%
 def disable_tqdm():
     """Set the logger for verbosity messages."""
     return (True if (logger.getEffectiveLevel()>=30) else False)
 
 
-# %%
-def _makedir(filename, url):
-    curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
-    # filename = os.path.basename(urlparse(url).path)
-    PATH_TO_DATA = os.path.join(curpath, filename)
-    if not os.path.isdir(curpath):
-        os.makedirs(curpath, exist_ok=True)
-    return PATH_TO_DATA
-
-
-def download_from_url(filename, url):
+def download_from_url(filename, url, **args):
     """Url import function.
 
     Parameters
     ----------
     filename : string
-        filename.
+        filename to create directory.
     url : string
         string.
 
     Returns
     -------
     PATH_TO_DATA : TYPE
         string.
@@ -466,7 +455,17 @@
     # Create directory
     PATH_TO_DATA = _makedir(filename, url)
     # Check file exists.
     if not os.path.isfile(PATH_TO_DATA):
         logger.info('Downloading [%s] dataset from github source..' %(filename))
         wget.download(url, PATH_TO_DATA)
     return PATH_TO_DATA
+
+
+# %%
+def _makedir(filename, url):
+    curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
+    # filename = os.path.basename(urlparse(url).path)
+    PATH_TO_DATA = os.path.join(curpath, filename)
+    if not os.path.isdir(curpath):
+        os.makedirs(curpath, exist_ok=True)
+    return PATH_TO_DATA
```

### Comparing `datazets-0.1.3/datazets/examples.py` & `datazets-0.1.4/datazets/examples.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # %%
-# import datazets as dz
-# url='https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data'
-# df = dz.get(url=url, sep=',')
+import datazets as dz
+url='https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data'
+df = dz.get(url=url, sep=',')
+df.shape
 
 # %%
 import datazets as dz
-df = dz.get(data='USA_elections')
-df.shape
+df = dz.get(data='auto_mpg')
+# df.shape
+
 # %% New
 
 # %% test
 datasets = ['census_income',
             'stormofswords',
             'sprinkler',
             'titanic',
@@ -28,15 +30,15 @@
             'digits',
             'energy',
             'meta',
             'gas_prices',
             'iris',
             'malicious_urls',
             'waterpump',
-            'USA_elections',
+            'elections',
             'tips',
             'predictive_maintenance',
             ]
 
 for data in datasets:
     df = dz.get(data=data)
     print(df.shape)
```

### Comparing `datazets-0.1.3/datazets.egg-info/PKG-INFO` & `datazets-0.1.4/datazets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: datazets
-Version: 0.1.3
+Version: 0.1.4
 Summary: Datazets is a python package to import well known example data sets.
 Home-page: https://github.com/erdogant/datazets
+Download-URL: https://github.com/erdogant/datazets/archive/0.1.4.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/erdogant/datazets/archive/0.1.3.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -110,9 +108,7 @@
 
 ### Contribute
 * All kinds of contributions are welcome!
 * If you wish to buy me a <a href="https://www.buymeacoffee.com/erdogant">Coffee</a> for this work, it is very appreciated :)
 
 ### Licence
 See [LICENSE](LICENSE) for details.
-
-
```

### Comparing `datazets-0.1.3/setup.py` & `datazets-0.1.4/setup.py`

 * *Files identical despite different names*

