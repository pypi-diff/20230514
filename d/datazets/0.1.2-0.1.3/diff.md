# Comparing `tmp/datazets-0.1.2.tar.gz` & `tmp/datazets-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datazets-0.1.2.tar", last modified: Sat May 13 19:15:35 2023, max compression
+gzip compressed data, was "datazets-0.1.3.tar", last modified: Sun May 14 11:30:25 2023, max compression
```

## Comparing `datazets-0.1.2.tar` & `datazets-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 19:15:35.940380 datazets-0.1.2/
--rw-rw-rw-   0        0        0     1121 2022-03-22 18:16:18.000000 datazets-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       56 2023-05-12 07:39:26.000000 datazets-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4654 2023-05-13 19:15:35.938967 datazets-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4060 2023-05-13 19:04:51.000000 datazets-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 19:15:35.921440 datazets-0.1.2/datazets/
--rw-rw-rw-   0        0        0      700 2023-05-13 19:13:14.000000 datazets-0.1.2/datazets/__init__.py
--rw-rw-rw-   0        0        0    12367 2023-05-13 19:10:27.000000 datazets-0.1.2/datazets/datazets.py
--rw-rw-rw-   0        0        0      749 2023-05-13 19:11:03.000000 datazets-0.1.2/datazets/examples.py
-drwxrwxrwx   0        0        0        0 2023-05-13 19:15:35.937387 datazets-0.1.2/datazets/utils/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 datazets-0.1.2/datazets/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 19:15:35.936416 datazets-0.1.2/datazets.egg-info/
--rw-rw-rw-   0        0        0     4654 2023-05-13 19:15:35.000000 datazets-0.1.2/datazets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-13 19:15:35.000000 datazets-0.1.2/datazets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 19:15:35.000000 datazets-0.1.2/datazets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-13 19:15:35.000000 datazets-0.1.2/datazets.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-13 19:15:35.000000 datazets-0.1.2/datazets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 19:15:35.940380 datazets-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1382 2023-05-13 18:52:09.000000 datazets-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:30:25.557941 datazets-0.1.3/
+-rw-rw-rw-   0        0        0     1121 2022-03-22 18:16:18.000000 datazets-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-05-12 07:39:26.000000 datazets-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4654 2023-05-14 11:30:25.543526 datazets-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4060 2023-05-13 19:04:51.000000 datazets-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 11:30:25.494263 datazets-0.1.3/datazets/
+-rw-rw-rw-   0        0        0      700 2023-05-14 11:30:00.000000 datazets-0.1.3/datazets/__init__.py
+-rw-rw-rw-   0        0        0    15441 2023-05-14 11:22:45.000000 datazets-0.1.3/datazets/datazets.py
+-rw-rw-rw-   0        0        0      988 2023-05-14 11:28:51.000000 datazets-0.1.3/datazets/examples.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:30:25.542556 datazets-0.1.3/datazets/utils/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 datazets-0.1.3/datazets/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:30:25.541532 datazets-0.1.3/datazets.egg-info/
+-rw-rw-rw-   0        0        0     4654 2023-05-14 11:30:25.000000 datazets-0.1.3/datazets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-14 11:30:25.000000 datazets-0.1.3/datazets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 11:30:25.000000 datazets-0.1.3/datazets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-14 11:30:25.000000 datazets-0.1.3/datazets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 11:30:25.000000 datazets-0.1.3/datazets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 11:30:25.557941 datazets-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1382 2023-05-13 18:52:09.000000 datazets-0.1.3/setup.py
```

### Comparing `datazets-0.1.2/LICENSE` & `datazets-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datazets-0.1.2/PKG-INFO` & `datazets-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datazets
-Version: 0.1.2
+Version: 0.1.3
 Summary: Datazets is a python package to import well known example data sets.
 Home-page: https://github.com/erdogant/datazets
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/erdogant/datazets/archive/0.1.2.tar.gz
+Download-URL: https://github.com/erdogant/datazets/archive/0.1.3.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `datazets-0.1.2/README.md` & `datazets-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `datazets-0.1.2/datazets/__init__.py` & `datazets-0.1.3/datazets/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datazets.datazets import get
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 # module level doc-string
 __doc__ = """
 datazets
 =====================================================================
 
 Description
```

### Comparing `datazets-0.1.2/datazets/datazets.py` & `datazets-0.1.3/datazets/datazets.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,35 +35,49 @@
     Parameters
     ----------
     data : str
         Multicollinear data sets:
             * 'titanic'
             * 'student'
             * 'fifa'
-            * 'waterpump'
             * 'DS_salaries'
+            * 'waterpump'
+            * 'USA_elections'
+            * 'tips'
+            * 'predictive_maintenance'
+        source-target
             * 'energy'
+            * 'stormofswords'
+        time-series
+            * 'occupancy'
+            * 'ps_data'
+            * 'gas_prices'
         synthetic discrete
             * 'random_discrete'
         Discrete data sets:
             * 'sprinkler'
-            * 'stormofswords'
             * 'census_income'
             * 'ads'
         Continous data sets:
             * 'breast_cancer'
             * 'cancer'
             * 'auto_mpg'
-        Image data sets:
-            * 'flowers'
+            * 'iris'
+        Images
             * 'faces'
             * 'mnist'
-            * 'scenes'
+        files:
+            * 'southern_nebula' (images)
+            * 'flowers' (images)
+            * 'scenes' (images)
+            * 'cat_and_dog' (images)
         Text data sets:
-            * 'retail'
+            * 'marketing_retail'
+            * 'malicious_urls'
+            * 'grocery_products'
         Time series:
             * 'bitcoin'
             * 'meta'
     url : str
         url link to to dataset.
     n : int
         Number of samples to generate in case of 'random_discrete'.
@@ -84,14 +98,17 @@
     --------
     >>> # Import library
     >>> import datazets as dz
     >>> #
     >>> # Import data set
     >>> df = dz.get('titanic')
     >>> #
+    >>> # Import data set
+    >>> img = dz.get('faces')
+    >>> #
     >>> # Import from url
     >>> url='https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data'
     >>> df = dz.get(url=url, sep=',')
 
     References
     ----------
     * Census Income. (1996). UCI Machine Learning Repository. https://doi.org/10.24432/C5S595.
@@ -99,46 +116,46 @@
     """
     set_logger(verbose=verbose)
     if data is None and url is None:
         logger.error('Input parameter <data> or <url> should be used.')
         return None
 
     # Get and Set data information
-    file_data, url, datatype, sep = _set_names_and_url(data, url, sep)
-    logger.info('Import dataset [%s]' %(file_data))
+    dataproperties = adjust_to_urlname(data, sep, url)
+    logger.info('Import dataset [%s]' %(dataproperties['input']))
 
-    if url is None:
+    if dataproperties['url'] is None:
         logger.info('Nothing to download.')
         return None
 
     # Import dataset
-    if datatype=='image':
-        df = _import_image_data(file_data, url)
-    elif datatype=='synthetic':
-        df = _generate_data(file_data, **args)
+    if dataproperties['type']=='files':
+        df = _import_image_data(dataproperties)
+    elif dataproperties['type']=='synthetic':
+        df = _generate_data(dataproperties['filename'], **args)
     else:
-        PATH_TO_DATA = import_url(file_data, url)
-        df = pd.read_csv(PATH_TO_DATA, sep=sep)
+        PATH_TO_DATA = download_from_url(dataproperties['filename'], url=dataproperties['url'])
+        df = pd.read_csv(PATH_TO_DATA, sep=dataproperties['sep'])
 
     # Return
     return df
 
 
 # %%
-def _generate_data(file_data, **args):
+def _generate_data(urlname, **args):
     df = None
     # Generate discrete random data
-    if file_data=='random_discrete.zip':
+    if urlname=='random_discrete':
         n = args.get('n', None) if args.get('n', None) is not None else 1000
         df = pd.DataFrame(np.random.randint(low=0, high=2, size=(n, 5)), columns=['A', 'B', 'C', 'D', 'E'])
     return df
 
 
 # %%
-def _import_image_data(data, url=None, curpath=None, **args):
+def _import_image_data(dataproperties, **args):
     """Import example dataset from github source.
 
     Import one of the few datasets from github source or specify your own download url link.
 
     Parameters
     ----------
     data : str
@@ -151,73 +168,103 @@
 
     Returns
     -------
     pd.DataFrame()
         Dataset containing mixed features.
 
     """
-    if data=='faces.zip':
-        from sklearn.datasets import fetch_olivetti_faces
-        X = fetch_olivetti_faces()
-        return X['data']
-    elif data=='mnist.zip':
-        from sklearn.datasets import load_digits
-        n = args.get('n', None) if args.get('n', None) is not None else 10
-        digits = load_digits(n_class=n)
-        return digits.data
+    # if dataproperties['filename']=='faces':
+    #     from sklearn.datasets import fetch_olivetti_faces
+    #     X = fetch_olivetti_faces()
+    #     return X['data']
+    #     df = pd.DataFrame(data=X['data'], index=X['target'])
+    # if dataproperties['filename']=='mnist':
+        # from sklearn.datasets import load_digits
+        # n = args.get('n', None) if args.get('n', None) is not None else 10
+        # X = load_digits(n_class=n)
+        # df = pd.DataFrame(data=X['data'], index=X['target'])
+        # return X.data
 
     # Collect data
-    PATH_TO_DATA = import_url(data, url)
+    PATH_TO_DATA = download_from_url(dataproperties['filename'], url=dataproperties['url'])
     # Unzip
     dirpath = unzip(PATH_TO_DATA)
     # Import local dataset
     image_files = listdir(dirpath)
     # Return
     return image_files
 
 
-# %%
-def _set_names_and_url(data, url, sep):
-    datatype=None
-
-    # Set names
+# %% Get the correct url name.
+def adjust_to_urlname(data, sep, url=None):
+    inputname, datatype = data, None
     if data is not None:
-        sep=';'
         # Set datatype for imges
-        if data=='flowers' or data=='faces' or data=='mnist' or data=='scenes':
-            datatype='image'
+        if data=='flowers' or data=='scenes' or data=='southern_nebula':
+            datatype='files'
+            if data=='flowers': data = 'flower_images.zip'
+            if data=='scenes': data = 'scenes.zip'
+            # if data=='cat_and_dog': data = 'cat_and_dog.zip'
+            # if data=='southern_nebula': data = 'southern_nebula.zip'
+            
+
+        elif data=='alarm' or data=='andes' or data=='asia' or data=='sachs' or data=='water':
+            datatype='DAG'
         elif data=='random_discrete':
             datatype='synthetic'
         else:
             datatype='various'
+            # Rename to correct filename
+            if data=='titanic': data, sep ='titanic_train.zip', ','
+            if data=='student': data, sep ='student_train.zip', ','
+            if data=='cancer': data, sep = 'cancer_dataset.zip', ','
+            if data=='fifa': data, sep = 'FIFA_2018.zip', ','
+            if data=='ads': data, sep = 'ads_data.zip', ','
+            if data=='bitcoin': data, sep = 'BTCUSDT.zip', ','
+            if data=='meta': data, sep = 'facebook_stocks.zip', ','
+            if data=='energy': data, sep = 'energy_source_target_value.zip', ','
+            if data=='breast_cancer': data, sep = 'breast_cancer_dataset.zip', ';'
+            if data=='marketing_retail': data, sep = 'marketing_data_online_retail_small.zip', ';'
+            if data=='waterpump': data, sep = 'waterpump.zip', ';'
+            if data=='USA_elections': data, sep = 'USA_2016_elections.zip', ','
+            if data=='occupancy': data, sep = 'UCI_Occupancy_Detection.zip', ','
+            if data=='predictive_maintenance': data, sep = 'predictive_maintenance_ai4i2020.zip', ','
+            if data=='iris': data, sep = 'iris_dataset.zip', ';'
+            if data=='gas_prices': data, sep = 'Henry_Hub_Natural_Gas_Spot_Price.zip', ','
+            if data=='grocery_products': data, sep = 'grocery_products_purchase.zip', ','
+            # if data=='movingbubbles': data, sep = 'movingbubbles.zip', ','
+
+            # images
+            if data=='faces': data, sep = 'olivetti_faces.zip', ';'
+            if data=='mnist': data, sep = 'mnist_images.zip', ';'
+            # if data=='tips': data, sep = 'tips.zip', ','
+            # if data=='sprinkler': data, sep ='sprinkler.zip', ','
+            # if data=='DS_salaries': data, sep = 'DS_salaries.zip', ','
+            # if data=='auto_mpg': data, sep = 'auto_mpg.zip', ','
+            # if data=='stormofswords': data, sep = 'stormofswords.zip', ','
+            # if data=='census_income': data, sep = 'census_income.zip', ','
+            # if data=='malicious_urls': data, sep = 'malicious_urls.zip', ','
+            # if data=='digits': data, sep = 'digits.zip', ','
+
+            if os.path.splitext(data)[1]=='':
+                sep=','
+                data = data + '.zip'
 
-        # Rename to correct filename
-        if data=='flowers': data = 'flower_images'
-        if data=='titanic': data, sep ='titanic_train', ','
-        if data=='student': data, sep ='student_train', ','
-        if data=='cancer': data, sep = 'cancer_dataset', ','
-        if data=='fifa': data, sep = 'FIFA_2018', ','
-        if data=='ads': data, sep = 'ads_data', ','
-        if data=='bitcoin': data, sep = 'BTCUSDT', ','
-        if data=='meta': data, sep = 'facebook_stocks', ','
-        if data=='DS_salaries': sep = ','
-        if data=='energy': data, sep = 'energy_source_target_value', ','
-        if data=='breast_cancer': data = 'breast_cancer_dataset'
-        if data=='retail': data = 'marketing_data_online_retail_small'
-        if data=='auto_mpg': sep = ','
-        if data=='stormofswords': sep = ','
-        if data=='census_income': sep = ','
-
-        # Set the url
-        url = 'https://erdogant.github.io/datasets/' + data + '.zip'
+            # 
 
+    # Set the url
+    dataproperties = {'input': inputname, 'filename': data, 'sep': sep, 'type': datatype, 'url': url}
     # Get filename from url
-    file_data = wget.filename_from_url(url)
+    if url is not None:
+        dataproperties['filename'] = wget.filename_from_url(url, ext=False)
+        dataproperties['input'] = dataproperties['filename']
+    else:
+        dataproperties['url'] = 'https://erdogant.github.io/datasets/' + dataproperties['filename']
 
-    return file_data, url, datatype, sep
+    return dataproperties
 
 
 # %% Recursively list files from directory
 def listdir(dirpath, ext=['png', 'tiff', 'jpg'], black_list=None):
     """Collect recursive images from path.
 
     Parameters
@@ -258,17 +305,19 @@
     return getfiles
 
 
 # %% Retrieve files files.
 class wget:
     """Retrieve file from url."""
 
-    def filename_from_url(url):
+    def filename_from_url(url, ext=True):
         """Return filename."""
-        return os.path.basename(url)
+        urlname = os.path.basename(url)
+        if not ext: _, ext = os.path.splitext(urlname)
+        return urlname
 
     def download(url, writepath):
         """Download.
 
         Parameters
         ----------
         url : str.
@@ -284,15 +333,15 @@
         r = requests.get(url, stream=True)
         with open(writepath, "wb") as fd:
             for chunk in r.iter_content(chunk_size=1024):
                 fd.write(chunk)
 
 
 # %% unzip
-def unzip(path_to_zip):
+def unzip(path_to_zip, outputdir=None):
     """Unzip files.
 
     Parameters
     ----------
     path_to_zip : str
         Path of the zip file.
 
@@ -306,16 +355,21 @@
     >>> import clustimage as cl
     >>> dirpath = cl.unzip('c://temp//flower_images.zip')
 
     """
     getpath = None
     if path_to_zip[-4:]=='.zip':
         if not os.path.isdir(path_to_zip):
+
             logger.info('Extracting files..')
-            pathname, _ = os.path.split(path_to_zip)
+            if outputdir is None:
+                pathname, _ = os.path.split(path_to_zip)
+            else:
+                pathname = outputdir
+
             # Unzip
             zip_ref = zipfile.ZipFile(path_to_zip, 'r')
             zip_ref.extractall(pathname)
             zip_ref.close()
             getpath = path_to_zip.replace('.zip', '')
             if not os.path.isdir(getpath):
                 logger.error('Extraction failed.')
@@ -389,15 +443,15 @@
     # filename = os.path.basename(urlparse(url).path)
     PATH_TO_DATA = os.path.join(curpath, filename)
     if not os.path.isdir(curpath):
         os.makedirs(curpath, exist_ok=True)
     return PATH_TO_DATA
 
 
-def import_url(filename, url):
+def download_from_url(filename, url):
     """Url import function.
 
     Parameters
     ----------
     filename : string
         filename.
     url : string
```

### Comparing `datazets-0.1.2/datazets/examples.py` & `datazets-0.1.3/datazets/examples.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 # %%
-import datazets as dz
-url='https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data'
-df = dz.get(url=url, sep=',')
+# import datazets as dz
+# url='https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data'
+# df = dz.get(url=url, sep=',')
 
 # %%
 import datazets as dz
-df = dz.get(data='mnist')
+df = dz.get(data='USA_elections')
+df.shape
+# %% New
 
 # %% test
 datasets = ['census_income',
             'stormofswords',
             'sprinkler',
             'titanic',
             'student',
             'fifa',
             'cancer',
             'auto_mpg',
             'cancer',
-            'retail',
+            'marketing_retail',
             'auto_mpg',
             'random_discrete',
             'ads',
             'breast_cancer',
             'bitcoin',
             'digits',
             'energy',
             'meta',
+            'gas_prices',
+            'iris',
+            'malicious_urls',
+            'waterpump',
+            'USA_elections',
+            'tips',
+            'predictive_maintenance',
             ]
 
 for data in datasets:
     df = dz.get(data=data)
     print(df.shape)
```

### Comparing `datazets-0.1.2/datazets.egg-info/PKG-INFO` & `datazets-0.1.3/datazets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datazets
-Version: 0.1.2
+Version: 0.1.3
 Summary: Datazets is a python package to import well known example data sets.
 Home-page: https://github.com/erdogant/datazets
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/erdogant/datazets/archive/0.1.2.tar.gz
+Download-URL: https://github.com/erdogant/datazets/archive/0.1.3.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `datazets-0.1.2/setup.py` & `datazets-0.1.3/setup.py`

 * *Files identical despite different names*

