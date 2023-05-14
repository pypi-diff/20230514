# Comparing `tmp/gmltools-0.0.63.tar.gz` & `tmp/gmltools-0.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.63.tar", last modified: Sat May 13 10:13:14 2023, max compression
+gzip compressed data, was "gmltools-0.0.64.tar", last modified: Sun May 14 14:09:48 2023, max compression
```

## Comparing `gmltools-0.0.63.tar` & `gmltools-0.0.64.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 10:13:14.403435 gmltools-0.0.63/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.63/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.63/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-05-13 10:13:14.401296 gmltools-0.0.63/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.63/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 10:13:14.055795 gmltools-0.0.63/dist/
--rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.63/dist/gmltools-0.0.59.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.63/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.63/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-05-13 10:12:29.000000 gmltools-0.0.63/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 10:13:14.403435 gmltools-0.0.63/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-05-13 10:12:19.000000 gmltools-0.0.63/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 10:13:13.943063 gmltools-0.0.63/src/
-drwxrwxrwx   0        0        0        0 2023-05-13 10:13:14.089362 gmltools-0.0.63/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.63/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.63/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 10:13:14.181881 gmltools-0.0.63/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.63/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    40126 2023-04-17 07:50:02.000000 gmltools-0.0.63/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-05-13 10:13:14.288147 gmltools-0.0.63/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.63/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.63/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.63/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5143 2023-04-14 11:04:34.000000 gmltools-0.0.63/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   119146 2023-05-13 10:11:58.000000 gmltools-0.0.63/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.63/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.63/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-05-13 10:13:14.333257 gmltools-0.0.63/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.63/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.63/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.63/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-05-13 10:13:14.396121 gmltools-0.0.63/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.63/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.63/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.63/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.63/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-05-13 10:13:14.153269 gmltools-0.0.63/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-05-13 10:13:13.000000 gmltools-0.0.63/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-05-13 10:13:13.000000 gmltools-0.0.63/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 10:13:13.000000 gmltools-0.0.63/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-05-13 10:13:13.000000 gmltools-0.0.63/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-13 10:13:13.000000 gmltools-0.0.63/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.905955 gmltools-0.0.64/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.64/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.64/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-05-14 14:09:48.904946 gmltools-0.0.64/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.64/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.604745 gmltools-0.0.64/dist/
+-rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.64/dist/gmltools-0.0.59.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.64/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.64/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-05-14 14:09:21.000000 gmltools-0.0.64/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 14:09:48.905955 gmltools-0.0.64/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-05-14 14:09:10.000000 gmltools-0.0.64/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.544846 gmltools-0.0.64/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.616658 gmltools-0.0.64/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.64/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.64/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.661170 gmltools-0.0.64/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.64/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    40126 2023-04-17 07:50:02.000000 gmltools-0.0.64/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.788846 gmltools-0.0.64/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.64/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.64/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.64/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5143 2023-04-14 11:04:34.000000 gmltools-0.0.64/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   119407 2023-05-14 14:08:53.000000 gmltools-0.0.64/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.64/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.64/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.839899 gmltools-0.0.64/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.64/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.64/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.64/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.901894 gmltools-0.0.64/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.64/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.64/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.64/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.64/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:09:48.643169 gmltools-0.0.64/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-05-14 14:09:48.000000 gmltools-0.0.64/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-05-14 14:09:48.000000 gmltools-0.0.64/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:09:48.000000 gmltools-0.0.64/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-05-14 14:09:48.000000 gmltools-0.0.64/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 14:09:48.000000 gmltools-0.0.64/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.63/LICENSE` & `gmltools-0.0.64/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/Models.ipynb` & `gmltools-0.0.64/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/PKG-INFO` & `gmltools-0.0.64/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.63
+Version: 0.0.64
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.63/README.md` & `gmltools-0.0.64/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/dist/gmltools-0.0.59.tar.gz` & `gmltools-0.0.64/dist/gmltools-0.0.59.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/gmltools.yml` & `gmltools-0.0.64/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/mltools.yml` & `gmltools-0.0.64/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/pyproject.toml` & `gmltools-0.0.64/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.63"
+version = "0.0.64"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.63/setup.py` & `gmltools-0.0.64/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.63',
+    'version': '0.0.64',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.63/src/gmltools/To_Do.txt` & `gmltools-0.0.64/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/src/gmltools/eda/eda.py` & `gmltools-0.0.64/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/src/gmltools/models/bayes.py` & `gmltools-0.0.64/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.64/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/src/gmltools/models/dummy_model.py` & `gmltools-0.0.64/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/src/gmltools/models/model.py` & `gmltools-0.0.64/src/gmltools/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1800,16 +1800,18 @@
         joblib.dump(self.model, os.path.join(path, self.model_name+'.joblib'))
         #save cv results if exists grid search or random search
         if hasattr(self.model, 'cv_results_'):
             df = pd.DataFrame(self.model.cv_results_)
             df.sort_values('rank_test_score', inplace=True)
             if hasattr(self.cv, 'is_timeseriesinitialsplit'):
                 #rename the split columns
-                new_column_names = self.cv.get_test_days(self.X_train)
-                df.rename(columns=dict(zip(df.filter(regex='split').filter(regex='_test_score').columns, new_column_names)), inplace=True)
+                new_column_names_score = self.cv.get_test_days(self.X_train)
+                new_column_names_pred = ["y_pred_" + date for date in self.cv.get_test_days(self.X_train)]
+                df.rename(columns=dict(zip(df.filter(regex='split').filter(regex='_test_score').columns, new_column_names_score)), inplace=True)
+                df.rename(columns=dict(zip(df.filter(regex='split').filter(regex='_y_pred').columns, new_column_names_pred)), inplace=True)
             df.to_excel(os.path.join(path, self.model_name+'_cv_results.xlsx'), index=False)
 
             #save the best register of the cv_results in a second sheet of excel file called summary_models.xlsx
             df_best = pd.DataFrame(df.iloc[0]).T
             df_best["Search conditions"]=str(self._overall_dict_params)
             df_best['model_name'] = self.model_name
             #set model_name the firts column and Search conditions the second column
```

### Comparing `gmltools-0.0.63/src/gmltools/models/models_info.py` & `gmltools-0.0.64/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.64/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.64/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.64/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.64/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.64/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.64/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.63/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.64/src/gmltools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.63
+Version: 0.0.64
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.63/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.64/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

