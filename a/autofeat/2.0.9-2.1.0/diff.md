# Comparing `tmp/autofeat-2.0.9.tar.gz` & `tmp/autofeat-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autofeat-2.0.9.tar", last modified: Mon Jul 12 19:11:21 2021, max compression
+gzip compressed data, was "autofeat-2.1.0.tar", last modified: Sun May 14 13:57:49 2023, max compression
```

## Comparing `autofeat-2.0.9.tar` & `autofeat-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 franzi     (501) staff       (20)        0 2021-07-12 19:11:21.446792 autofeat-2.0.9/
--rw-r--r--   0 franzi     (501) staff       (20)     1057 2016-11-03 21:17:21.000000 autofeat-2.0.9/LICENSE
--rw-r--r--   0 franzi     (501) staff       (20)       16 2017-09-06 12:18:36.000000 autofeat-2.0.9/MANIFEST.in
--rw-r--r--   0 franzi     (501) staff       (20)     6417 2021-07-12 19:11:21.446447 autofeat-2.0.9/PKG-INFO
--rw-r--r--   0 franzi     (501) staff       (20)     5079 2021-06-03 07:52:03.000000 autofeat-2.0.9/README.md
-drwxr-xr-x   0 franzi     (501) staff       (20)        0 2021-07-12 19:11:21.443784 autofeat-2.0.9/autofeat/
--rw-r--r--   0 franzi     (501) staff       (20)      306 2021-07-12 19:10:55.000000 autofeat-2.0.9/autofeat/__init__.py
--rw-r--r--   0 franzi     (501) staff       (20)    26363 2021-06-03 07:52:03.000000 autofeat-2.0.9/autofeat/autofeat.py
--rw-r--r--   0 franzi     (501) staff       (20)    12466 2021-07-12 19:10:11.000000 autofeat-2.0.9/autofeat/autofeatlight.py
--rw-r--r--   0 franzi     (501) staff       (20)    19494 2021-06-02 11:43:19.000000 autofeat-2.0.9/autofeat/feateng.py
--rw-r--r--   0 franzi     (501) staff       (20)    17337 2021-06-02 19:38:48.000000 autofeat-2.0.9/autofeat/featsel.py
--rw-r--r--   0 franzi     (501) staff       (20)      855 2021-06-02 19:38:48.000000 autofeat-2.0.9/autofeat/nb_utils.py
-drwxr-xr-x   0 franzi     (501) staff       (20)        0 2021-07-12 19:11:21.446015 autofeat-2.0.9/autofeat.egg-info/
--rw-r--r--   0 franzi     (501) staff       (20)     6417 2021-07-12 19:11:21.000000 autofeat-2.0.9/autofeat.egg-info/PKG-INFO
--rw-r--r--   0 franzi     (501) staff       (20)      326 2021-07-12 19:11:21.000000 autofeat-2.0.9/autofeat.egg-info/SOURCES.txt
--rw-r--r--   0 franzi     (501) staff       (20)        1 2021-07-12 19:11:21.000000 autofeat-2.0.9/autofeat.egg-info/dependency_links.txt
--rw-r--r--   0 franzi     (501) staff       (20)       72 2021-07-12 19:11:21.000000 autofeat-2.0.9/autofeat.egg-info/requires.txt
--rw-r--r--   0 franzi     (501) staff       (20)        9 2021-07-12 19:11:21.000000 autofeat-2.0.9/autofeat.egg-info/top_level.txt
--rw-r--r--   0 franzi     (501) staff       (20)       38 2021-07-12 19:11:21.446943 autofeat-2.0.9/setup.cfg
--rw-r--r--   0 franzi     (501) staff       (20)     4720 2021-07-12 19:11:14.000000 autofeat-2.0.9/setup.py
+drwxr-xr-x   0 franzi     (501) staff       (20)        0 2023-05-14 13:57:49.979966 autofeat-2.1.0/
+-rw-r--r--   0 franzi     (501) staff       (20)     1057 2016-11-03 21:17:21.000000 autofeat-2.1.0/LICENSE
+-rw-r--r--   0 franzi     (501) staff       (20)       16 2017-09-06 12:18:36.000000 autofeat-2.1.0/MANIFEST.in
+-rw-r--r--   0 franzi     (501) staff       (20)     6966 2023-05-14 13:57:49.979277 autofeat-2.1.0/PKG-INFO
+-rw-r--r--   0 franzi     (501) staff       (20)     5190 2023-05-13 14:02:00.000000 autofeat-2.1.0/README.md
+drwxr-xr-x   0 franzi     (501) staff       (20)        0 2023-05-14 13:57:49.975979 autofeat-2.1.0/autofeat/
+-rw-r--r--   0 franzi     (501) staff       (20)      282 2023-05-13 16:16:16.000000 autofeat-2.1.0/autofeat/__init__.py
+-rw-r--r--   0 franzi     (501) staff       (20)    28687 2023-05-14 13:13:41.000000 autofeat-2.1.0/autofeat/autofeat.py
+-rw-r--r--   0 franzi     (501) staff       (20)    12858 2023-05-13 15:58:07.000000 autofeat-2.1.0/autofeat/autofeatlight.py
+-rw-r--r--   0 franzi     (501) staff       (20)    19859 2023-05-13 15:57:45.000000 autofeat-2.1.0/autofeat/feateng.py
+-rw-r--r--   0 franzi     (501) staff       (20)    17833 2023-05-13 16:01:10.000000 autofeat-2.1.0/autofeat/featsel.py
+-rw-r--r--   0 franzi     (501) staff       (20)      831 2023-05-13 14:15:17.000000 autofeat-2.1.0/autofeat/nb_utils.py
+drwxr-xr-x   0 franzi     (501) staff       (20)        0 2023-05-14 13:57:49.978549 autofeat-2.1.0/autofeat.egg-info/
+-rw-r--r--   0 franzi     (501) staff       (20)     6966 2023-05-14 13:57:49.000000 autofeat-2.1.0/autofeat.egg-info/PKG-INFO
+-rw-r--r--   0 franzi     (501) staff       (20)      332 2023-05-14 13:57:49.000000 autofeat-2.1.0/autofeat.egg-info/SOURCES.txt
+-rw-r--r--   0 franzi     (501) staff       (20)        1 2023-05-14 13:57:49.000000 autofeat-2.1.0/autofeat.egg-info/dependency_links.txt
+-rw-r--r--   0 franzi     (501) staff       (20)       72 2023-05-14 13:57:49.000000 autofeat-2.1.0/autofeat.egg-info/requires.txt
+-rw-r--r--   0 franzi     (501) staff       (20)        9 2023-05-14 13:57:49.000000 autofeat-2.1.0/autofeat.egg-info/top_level.txt
+-rw-r--r--   0 franzi     (501) staff       (20)      891 2023-05-14 13:54:25.000000 autofeat-2.1.0/pyproject.toml
+-rw-r--r--   0 franzi     (501) staff       (20)       38 2023-05-14 13:57:49.980135 autofeat-2.1.0/setup.cfg
```

### Comparing `autofeat-2.0.9/LICENSE` & `autofeat-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autofeat-2.0.9/PKG-INFO` & `autofeat-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,91 @@
 Metadata-Version: 2.1
 Name: autofeat
-Version: 2.0.9
+Version: 2.1.0
 Summary: Automatic Feature Engineering and Selection Linear Prediction Model
-Home-page: https://github.com/cod3licious/autofeat
-Author: Franziska Horn
-Author-email: cod3licious@gmail.com
-License: MIT
-Description: # `autofeat` library
-        ### Linear Prediction Models with Automated Feature Engineering and Selection
+Author-email: Franziska Horn <cod3licious@gmail.com>
+License: MIT License
         
-        This library contains the `AutoFeatRegressor` and `AutoFeatClassifier` models with a similar interface as `scikit-learn` models:
-        - `fit()` function to fit the model parameters
-        - `predict()` function to predict the target variable given the input
-        - `score()` function to calculate the goodness of the fit (R^2/accuracy)
-        - `fit_transform()` and `transform()` functions, which extend the given data by the additional features that were engineered and selected by the model
+        Copyright (c) 2016 
         
-        When calling the `fit()` function, internally the `fit_transform()` function will be called, so if you're planing to call `transform()` on the same data anyways, just call `fit_transform()` right away. `transform()` is mostly useful if you've split your data into training and test data and did not call `fit_transform()` on your whole dataset. The `predict()` and `score()` functions can either be given data in the format of the original dataframe that was used when calling `fit()`/`fit_transform()` or they can be given an already transformed dataframe.
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
         
-        In addition, only the feature selection part is also available in the `FeatureSelector` model.
-        
-        Furthermore (as of version 2.0.0), minimal feature selection (removing zero variance and redundant features), engineering (simple product and ratio of features), and scaling (power transform to make features more normally distributed) is also available in the `AutoFeatLight` model.
-        
-        The `AutoFeatRegressor`, `AutoFeatClassifier`, and `FeatureSelector` models need to be **fit on data without NaNs**, as they internally call the sklearn `LassoLarsCV` model, which can not handle NaNs. When calling `transform()`, NaNs (but not `np.inf`) are okay.
-        
-        The [autofeat examples notebook](https://github.com/cod3licious/autofeat/blob/master/autofeat_examples.ipynb) contains a simple usage example - try it out! :) Additional examples can be found in the autofeat benchmark notebooks for [regression](https://github.com/cod3licious/autofeat/blob/master/autofeat_benchmark_regression.ipynb) (which also contains the code to reproduce the results from the paper mentioned below) and [classification](https://github.com/cod3licious/autofeat/blob/master/autofeat_benchmark_classification.ipynb), as well as the testing scripts.
-        
-        Please keep in mind that since the `AutoFeatRegressor` and `AutoFeatClassifier` models can generate very complex features, they might **overfit on noise** in the dataset, i.e., find some new features that lead to good prediction on the training set but result in a poor performance on new test samples. While this usually only happens for datasets with very few samples, we suggest you carefully inspect the features found by `autofeat` and use those that make sense to you to train your own models.
-        
-        Depending on the number of `feateng_steps` (default 2) and the number of input features, `autofeat` can generate a very huge feature matrix (before selecting the most appropriate features from this large feature pool). By specifying in `feateng_cols` those columns that you expect to be most valuable in the feature engineering part, the number of features can be greatly reduced. Additionally, `transformations` can be limited to only those feature transformations that make sense for your data. Last but not least, you can subsample the data used for training the model to limit the memory requirements. After the model was fit, you can call `transform()` on your whole dataset to generate only those few features that were selected during `fit()`/`fit_transform()`.
-        
-        
-        ### Installation
-        You can either download the code from here and include the autofeat folder in your `$PYTHONPATH` or install (the library components only) via pip:
-        
-            $ pip install autofeat
-        
-        The library requires Python 3! Other dependencies: `numpy`, `pandas`, `scikit-learn`, `sympy`, `joblib`, `pint` and `numba`.
-        
-        
-        ### Paper
-        For further details on the model and implementation please refer to the [paper](https://arxiv.org/abs/1901.07329)  - and of course if any of this code was helpful for your research, please consider citing it:
-        ```
-        @inproceedings{horn2019autofeat,
-          title={The autofeat Python Library for Automated Feature Engineering and Selection},
-          author={Horn, Franziska and Pack, Robert and Rieger, Michael},
-          booktitle={Joint European Conference on Machine Learning and Knowledge Discovery in Databases},
-          pages={111--120},
-          year={2019},
-          organization={Springer}
-        }
-        ```
-        
-        If you don't like reading, you can also watch a video of my [talk at the PyData conference](https://www.youtube.com/watch?v=4-4pKPv9lJ4) about automated feature engineering and selection with `autofeat`.
-        
-        The code is intended for research purposes.
-        
-        If you have any questions please don't hesitate to send me an [email](mailto:cod3licious@gmail.com) and of course if you should find any bugs or want to contribute other improvements, pull requests are very welcome!
-        
-        ### Acknowledgments
-        
-        This project was made possible thanks to support by [BASF](https://www.basf.com).
-        
-Keywords: automl feature engineering feature selection linear model
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Project-URL: Homepage, https://github.com/cod3licious/autofeat
+Keywords: automl,feature engineering,feature selection,linear model
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# `autofeat` library
+### Linear Prediction Models with Automated Feature Engineering and Selection
+
+This library contains the `AutoFeatRegressor` and `AutoFeatClassifier` models with a similar interface as `scikit-learn` models:
+- `fit()` function to fit the model parameters
+- `predict()` function to predict the target variable given the input
+- `predict_proba()` function to predict probabilities of the target variable given the input (classifier only)
+- `score()` function to calculate the goodness of the fit (R^2/accuracy)
+- `fit_transform()` and `transform()` functions, which extend the given data by the additional features that were engineered and selected by the model
+
+When calling the `fit()` function, internally the `fit_transform()` function will be called, so if you're planing to call `transform()` on the same data anyways, just call `fit_transform()` right away. `transform()` is mostly useful if you've split your data into training and test data and did not call `fit_transform()` on your whole dataset. The `predict()` and `score()` functions can either be given data in the format of the original dataframe that was used when calling `fit()`/`fit_transform()` or they can be given an already transformed dataframe.
+
+In addition, only the feature selection part is also available in the `FeatureSelector` model.
+
+Furthermore (as of version 2.0.0), minimal feature selection (removing zero variance and redundant features), engineering (simple product and ratio of features), and scaling (power transform to make features more normally distributed) is also available in the `AutoFeatLight` model.
+
+The `AutoFeatRegressor`, `AutoFeatClassifier`, and `FeatureSelector` models need to be **fit on data without NaNs**, as they internally call the sklearn `LassoLarsCV` model, which can not handle NaNs. When calling `transform()`, NaNs (but not `np.inf`) are okay.
+
+The [autofeat examples notebook](https://github.com/cod3licious/autofeat/blob/master/autofeat_examples.ipynb) contains a simple usage example - try it out! :) Additional examples can be found in the autofeat benchmark notebooks for [regression](https://github.com/cod3licious/autofeat/blob/master/autofeat_benchmark_regression.ipynb) (which also contains the code to reproduce the results from the paper mentioned below) and [classification](https://github.com/cod3licious/autofeat/blob/master/autofeat_benchmark_classification.ipynb), as well as the testing scripts.
+
+Please keep in mind that since the `AutoFeatRegressor` and `AutoFeatClassifier` models can generate very complex features, they might **overfit on noise** in the dataset, i.e., find some new features that lead to good prediction on the training set but result in a poor performance on new test samples. While this usually only happens for datasets with very few samples, we suggest you carefully inspect the features found by `autofeat` and use those that make sense to you to train your own models.
+
+Depending on the number of `feateng_steps` (default 2) and the number of input features, `autofeat` can generate a very huge feature matrix (before selecting the most appropriate features from this large feature pool). By specifying in `feateng_cols` those columns that you expect to be most valuable in the feature engineering part, the number of features can be greatly reduced. Additionally, `transformations` can be limited to only those feature transformations that make sense for your data. Last but not least, you can subsample the data used for training the model to limit the memory requirements. After the model was fit, you can call `transform()` on your whole dataset to generate only those few features that were selected during `fit()`/`fit_transform()`.
+
+
+### Installation
+You can either download the code from here and include the autofeat folder in your `$PYTHONPATH` or install (the library components only) via pip:
+
+    $ pip install autofeat
+
+The library requires Python 3! Other dependencies: `numpy`, `pandas`, `scikit-learn`, `sympy`, `joblib`, `pint` and `numba`.
+
+
+### Paper
+For further details on the model and implementation please refer to the [paper](https://arxiv.org/abs/1901.07329)  - and of course if any of this code was helpful for your research, please consider citing it:
+```
+@inproceedings{horn2019autofeat,
+  title={The autofeat Python Library for Automated Feature Engineering and Selection},
+  author={Horn, Franziska and Pack, Robert and Rieger, Michael},
+  booktitle={Joint European Conference on Machine Learning and Knowledge Discovery in Databases},
+  pages={111--120},
+  year={2019},
+  organization={Springer}
+}
+```
+
+If you don't like reading, you can also watch a video of my [talk at the PyData conference](https://www.youtube.com/watch?v=4-4pKPv9lJ4) about automated feature engineering and selection with `autofeat`.
+
+The code is intended for research purposes.
+
+If you have any questions please don't hesitate to send me an [email](mailto:cod3licious@gmail.com) and of course if you should find any bugs or want to contribute other improvements, pull requests are very welcome!
+
+### Acknowledgments
+
+This project was made possible thanks to support by [BASF](https://www.basf.com).
```

### Comparing `autofeat-2.0.9/README.md` & `autofeat-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # `autofeat` library
 ### Linear Prediction Models with Automated Feature Engineering and Selection
 
 This library contains the `AutoFeatRegressor` and `AutoFeatClassifier` models with a similar interface as `scikit-learn` models:
 - `fit()` function to fit the model parameters
 - `predict()` function to predict the target variable given the input
+- `predict_proba()` function to predict probabilities of the target variable given the input (classifier only)
 - `score()` function to calculate the goodness of the fit (R^2/accuracy)
 - `fit_transform()` and `transform()` functions, which extend the given data by the additional features that were engineered and selected by the model
 
 When calling the `fit()` function, internally the `fit_transform()` function will be called, so if you're planing to call `transform()` on the same data anyways, just call `fit_transform()` right away. `transform()` is mostly useful if you've split your data into training and test data and did not call `fit_transform()` on your whole dataset. The `predict()` and `score()` functions can either be given data in the format of the original dataframe that was used when calling `fit()`/`fit_transform()` or they can be given an already transformed dataframe.
 
 In addition, only the feature selection part is also available in the `FeatureSelector` model.
```

### Comparing `autofeat-2.0.9/autofeat/autofeat.py` & `autofeat-2.1.0/autofeat/autofeat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-# -*- coding: utf-8 -*-
 # Author: Franziska Horn <cod3licious@gmail.com>
 # License: MIT
 
-from __future__ import unicode_literals, division, print_function, absolute_import
-from builtins import range
 import warnings
 import numba as nb
 import numpy as np
 import pandas as pd
 import sklearn.linear_model as lm
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.base import BaseEstimator, RegressorMixin, ClassifierMixin
@@ -15,15 +12,15 @@
 from sympy.utilities.lambdify import lambdify
 import pint
 
 from .feateng import engineer_features, n_cols_generated, colnames2symbols
 from .featsel import select_features
 
 
-def _parse_units(units, ureg=None, verbose=0):
+def _parse_units(units: dict, ureg: pint.UnitRegistry | None = None, verbose: int = 0):
     """
     Convert a dict with string units to pint quantities.
 
     Inputs:
         - units: dict with {"variable_name": "unit"}
         - ureg: optional: a pint UnitRegistry
         - verbose: verbosity level (int; default: 0)
@@ -36,36 +33,35 @@
         if ureg is None:
             ureg = pint.UnitRegistry(auto_reduce_dimensions=True, autoconvert_offset_to_baseunit=True)
         for c in units:
             try:
                 parsed_units[c] = ureg.parse_expression(units[c])
             except pint.UndefinedUnitError:
                 if verbose > 0:
-                    print("[AutoFeat] WARNING: unit %r of column %r was not recognized and will be ignored!" % (units[c], c))
+                    print(f"[AutoFeat] WARNING: unit {units[c]} of column {c} was not recognized and will be ignored!")
                 parsed_units[c] = ureg.parse_expression("")
-            parsed_units[c].__dict__["_magnitude"] = 1.
+            parsed_units[c].__dict__["_magnitude"] = 1.0
     return parsed_units
 
 
 class AutoFeatModel(BaseEstimator):
-
     def __init__(
         self,
-        problem_type="regression",
-        categorical_cols=None,
-        feateng_cols=None,
-        units=None,
-        feateng_steps=2,
-        featsel_runs=5,
-        max_gb=None,
-        transformations=("1/", "exp", "log", "abs", "sqrt", "^2", "^3"),
-        apply_pi_theorem=True,
-        always_return_numpy=False,
-        n_jobs=1,
-        verbose=0,
+        problem_type: str = "regression",
+        categorical_cols: list | None = None,
+        feateng_cols: list | None = None,
+        units: dict | None = None,
+        feateng_steps: int = 2,
+        featsel_runs: int = 5,
+        max_gb: int | None = None,
+        transformations: list | tuple = ("1/", "exp", "log", "abs", "sqrt", "^2", "^3"),
+        apply_pi_theorem: bool = True,
+        always_return_numpy: bool = False,
+        n_jobs: int = 1,
+        verbose: int = 0,
     ):
         """
         multi-step feature engineering and cross-validated feature selection to generate promising additional
         features for your dataset and train a linear prediction model with them.
 
         Inputs:
             - problem_type: str, either "regression" or "classification" (default: "regression")
@@ -123,60 +119,60 @@
 
     def __getstate__(self):
         """
         get dict for pickling without feature_functions as they are not pickleable
         """
         return {k: self.__dict__[k] if k != "feature_functions_" else {} for k in self.__dict__}
 
-    def _transform_categorical_cols(self, df):
+    def _transform_categorical_cols(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Transform categorical features into 0/1 encoding.
 
         Inputs:
             - df: pandas dataframe with original features
         Returns:
             - df: dataframe with categorical features transformed into multiple 0/1 columns
         """
         self.categorical_cols_map_ = {}
         if self.categorical_cols:
-            e = OneHotEncoder(sparse=False, categories="auto")
+            e = OneHotEncoder(sparse_output=False, categories="auto")
             for c in self.categorical_cols:
                 if c not in df.columns:
-                    raise ValueError("[AutoFeat] categorical_col %r not in df.columns" % c)
+                    raise ValueError(f"[AutoFeat] categorical_col {c} not in df.columns")
                 ohe = e.fit_transform(df[c].to_numpy()[:, None])
-                new_cat_cols = ["cat_%s_%r" % (str(c), i) for i in e.categories_[0]]
+                new_cat_cols = [f"cat_{c}_{i}" for i in e.categories_[0]]
                 self.categorical_cols_map_[c] = new_cat_cols
                 df = df.join(pd.DataFrame(ohe, columns=new_cat_cols, index=df.index))
             # remove the categorical column from our columns to consider
             df.drop(columns=self.categorical_cols, inplace=True)
         return df
 
-    def _apply_pi_theorem(self, df):
+    def _apply_pi_theorem(self, df: pd.DataFrame) -> pd.DataFrame:
         if self.apply_pi_theorem and self.units:
             ureg = pint.UnitRegistry(auto_reduce_dimensions=True, autoconvert_offset_to_baseunit=True)
             parsed_units = _parse_units(self.units, ureg, self.verbose)
             # use only original features
             parsed_units = {c: parsed_units[c] for c in self.feateng_cols_ if not parsed_units[c].dimensionless}
             if self.verbose:
                 print("[AutoFeat] Applying the Pi Theorem")
             pi_theorem_results = ureg.pi_theorem(parsed_units)
             for i, r in enumerate(pi_theorem_results, 1):
                 if self.verbose:
-                    print("[AutoFeat] Pi Theorem %i: " % i, pint.formatter(r.items()))
+                    print(f"[AutoFeat] Pi Theorem {i}: ", pint.formatter(r.items()))
                 # compute the final result by multiplying and taking the power of
                 cols = sorted(r)
                 # only use data points where non of the affected columns are NaNs
                 not_na_idx = df[cols].notna().all(axis=1)
-                ptr = df[cols[0]].to_numpy()[not_na_idx]**r[cols[0]]
+                ptr = df[cols[0]].to_numpy()[not_na_idx] ** r[cols[0]]
                 for c in cols[1:]:
-                    ptr *= df[c].to_numpy()[not_na_idx]**r[c]
-                df.loc[not_na_idx, "PT%i_%s" % (i, pint.formatter(r.items()).replace(" ", ""))] = ptr
+                    ptr *= df[c].to_numpy()[not_na_idx] ** r[c]
+                df.loc[not_na_idx, f"PT{i}_{pint.formatter(r.items()).replace(' ', '')}"] = ptr
         return df
 
-    def _generate_features(self, df, new_feat_cols):
+    def _generate_features(self, df: pd.DataFrame, new_feat_cols: list) -> pd.DataFrame:
         """
         Generate additional features based on the feature formulas for all data points in the df.
         Only works after the model was fitted.
 
         Inputs:
             - df: pandas dataframe with original features
             - new_feat_cols: names of new features that should be generated (keys of self.feature_formulas_)
@@ -185,20 +181,20 @@
         """
         check_is_fitted(self, ["feature_formulas_"])
         if not new_feat_cols:
             return df
         if not new_feat_cols[0] in self.feature_formulas_:
             raise RuntimeError("[AutoFeat] First call fit or fit_transform to generate the features!")
         if self.verbose:
-            print("[AutoFeat] Computing %i new features." % len(new_feat_cols))
+            print(f"[AutoFeat] Computing {len(new_feat_cols)} new features.")
         # generate all good feature; unscaled this time
         feat_array = np.zeros((len(df), len(new_feat_cols)))
         for i, expr in enumerate(new_feat_cols):
             if self.verbose:
-                print("[AutoFeat] %5i/%5i new features" % (i, len(new_feat_cols)), end="\r")
+                print(f"[AutoFeat] {i:5}/{len(new_feat_cols):5} new features", end="\r")
             if expr not in self.feature_functions_:
                 # generate a substitution expression based on all the original symbols of the original features
                 # for the given generated feature in good cols
                 # since sympy can handle only up to 32 original features in ufunctify, we need to check which features
                 # to consider here, therefore perform some crude check to limit the number of features used
                 cols = [c for i, c in enumerate(self.feateng_cols_) if colnames2symbols(c, i) in expr]
                 if not cols:
@@ -206,15 +202,15 @@
                     f = None
                     f_jit = None
                 else:
                     try:
                         f = lambdify([self.feature_formulas_[c] for c in cols], self.feature_formulas_[expr])
                         f_jit = nb.njit(f)
                     except Exception:
-                        print("[AutoFeat] Error while processing expression: %r" % expr)
+                        print(f"[AutoFeat] Error while processing expression: {expr}")
                         raise
                 self.feature_functions_[expr] = (cols, f, f_jit)
             else:
                 cols, f, f_jit = self.feature_functions_[expr]
             if f is not None:
                 # only generate features for completely not-nan rows
                 not_na_idx = df[cols].notna().all(axis=1)
@@ -226,23 +222,49 @@
                         # fallback on the non jitted version of the function
                         feat = f(*(df[c].to_numpy(dtype=float)[not_na_idx] for c in cols))
                         # henceforth, always use the non jitted version of the function
                         self.feature_functions_[expr] = (cols, f, f)
                     feat_array[not_na_idx, i] = feat
                     feat_array[~not_na_idx, i] = np.nan
                 except RuntimeWarning:
-                    print("[AutoFeat] WARNING: Problem while evaluating expression: %r with columns %r" % (expr, cols),
-                          " - is the data in a different range then when calling .fit()? Are maybe some values 0 that shouldn't be?")
+                    print(
+                        f"[AutoFeat] WARNING: Problem while evaluating expression: {expr} with columns {cols}",
+                        " - is the data in a different range then when calling .fit()? Are maybe some values 0 that shouldn't be?",
+                    )
                     raise
         if self.verbose:
-            print("[AutoFeat] %5i/%5i new features ...done." % (len(new_feat_cols), len(new_feat_cols)))
+            print(f"[AutoFeat] {len(new_feat_cols):5}/{len(new_feat_cols):5} new features ...done.")
         df = df.join(pd.DataFrame(feat_array, columns=new_feat_cols, index=df.index))
         return df
 
-    def fit_transform(self, X, y):
+    def _X2df(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
+        """
+        Helper function that ensures correctness of the input data for classification tasks.
+        Inputs:
+            - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
+        Returns:
+            - df: transformed dataframe
+        """
+        # store column names as they'll be lost in the other check
+        cols = [str(c) for c in X.columns] if isinstance(X, pd.DataFrame) else []
+        # check input variables
+        X = check_array(X, dtype=None)
+        if not cols:
+            cols = [f"x{i:03}" for i in range(X.shape[1])]
+        # transform X into a dataframe (again)
+        df = pd.DataFrame(X, columns=cols)
+        # do we need to call transform?
+        if not list(df.columns) == self.all_columns_:
+            temp = self.always_return_numpy
+            self.always_return_numpy = False
+            df = self.transform(df)
+            self.always_return_numpy = temp
+        return df
+
+    def fit_transform(self, X: np.ndarray | pd.DataFrame, y: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Fits the regression model and returns a new dataframe with the additional features.
 
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
             - y: pandas dataframe or numpy array with targets for all n_datapoints
         Returns:
@@ -260,26 +282,26 @@
         cols = [str(c) for c in X.columns] if isinstance(X, pd.DataFrame) else []
         # check input variables
         X, target = check_X_y(X, y, y_numeric=self.problem_type == "regression", dtype=None)
         if not cols:
             # the additional zeros in the name are because of the variable check in _generate_features,
             # where we check if the column name occurs in the the expression. this would lead to many
             # false positives if we have features x1 and x10...x19 instead of x001...x019.
-            cols = ["x%03i" % i for i in range(X.shape[1])]
+            cols = [f"x{i:03}" for i in range(X.shape[1])]
         self.original_columns_ = cols
         # transform X into a dataframe (again)
         df = pd.DataFrame(X, columns=cols)
         # possibly convert categorical columns
         df = self._transform_categorical_cols(df)
         # if we're not given specific feateng_cols, then just take all columns except categorical
         if self.feateng_cols:
             fcols = []
             for c in self.feateng_cols:
                 if c not in self.original_columns_:
-                    raise ValueError("[AutoFeat] feateng_col %r not in df.columns" % c)
+                    raise ValueError(f"[AutoFeat] feateng_col {c} not in df.columns")
                 if c in self.categorical_cols_map_:
                     fcols.extend(self.categorical_cols_map_[c])
                 else:
                     fcols.append(c)
             self.feateng_cols_ = fcols
         else:
             self.feateng_cols_ = list(df.columns)
@@ -290,70 +312,86 @@
             # apply pi-theorem -- additional columns are not used for regular feature engineering (for now)!
             df = self._apply_pi_theorem(df)
         # subsample data points and targets in case we'll generate too many features
         # (n_rows * n_cols * 32/8)/1000000000 <= max_gb
         n_cols = n_cols_generated(len(self.feateng_cols_), self.feateng_steps, len(self.transformations))
         n_gb = (len(df) * n_cols) / 250000000
         if self.verbose:
-            print("[AutoFeat] The %i step feature engineering process could generate up to %i features." % (self.feateng_steps, n_cols))
-            print("[AutoFeat] With %i data points this new feature matrix would use about %.2f gb of space." % (len(df), n_gb))
+            print(
+                f"[AutoFeat] The {self.feateng_steps} step feature engineering process could generate up to {n_cols} features."
+            )
+            print(f"[AutoFeat] With {len(df)} data points this new feature matrix would use about {n_gb:.2f} gb of space.")
         if self.max_gb and n_gb > self.max_gb:
             n_rows = int(self.max_gb * 250000000 / n_cols)
             if self.verbose:
-                print("[AutoFeat] As you specified a limit of %.1d gb, the number of data points is subsampled to %i" % (self.max_gb, n_rows))
+                print(
+                    f"[AutoFeat] As you specified a limit of {self.max_gb:.1f} gb, the number of data points is subsampled to {n_rows}"
+                )
             subsample_idx = np.random.permutation(list(df.index))[:n_rows]
             df_subs = df.iloc[subsample_idx]
             df_subs.reset_index(drop=True, inplace=True)
             target_sub = target[subsample_idx]
         else:
             df_subs = df.copy()
             target_sub = target.copy()
         # generate features
-        df_subs, self.feature_formulas_ = engineer_features(df_subs, self.feateng_cols_, _parse_units(self.units, verbose=self.verbose),
-                                                            self.feateng_steps, self.transformations, self.verbose)
+        df_subs, self.feature_formulas_ = engineer_features(
+            df_subs,
+            self.feateng_cols_,
+            _parse_units(self.units, verbose=self.verbose),
+            self.feateng_steps,
+            self.transformations,
+            self.verbose,
+        )
         # select predictive features
         if self.featsel_runs <= 0:
             if self.verbose:
                 print("[AutoFeat] WARNING: Not performing feature selection.")
             good_cols = df_subs.columns
         else:
             if self.problem_type in ("regression", "classification"):
-                good_cols = select_features(df_subs, target_sub, self.featsel_runs, None, self.problem_type, self.n_jobs, self.verbose)
+                good_cols = select_features(
+                    df_subs, target_sub, self.featsel_runs, None, self.problem_type, self.n_jobs, self.verbose
+                )
                 # if no features were selected, take the original features
                 if not good_cols:
                     good_cols = list(df.columns)
             else:
-                print("[AutoFeat] WARNING: Unknown problem_type %r - not performing feature selection." % self.problem_type)
+                print(f"[AutoFeat] WARNING: Unknown problem_type {self.problem_type} - not performing feature selection.")
                 good_cols = df_subs.columns
         # filter out those columns that were original features or generated otherwise
         self.new_feat_cols_ = [c for c in good_cols if c not in list(df.columns)]
         self.good_cols_ = good_cols
         # re-generate all good feature again; for all data points this time
         self.feature_functions_ = {}
         df = self._generate_features(df, self.new_feat_cols_)
+        # to prevent an error because sometimes the column names are numpy.str_ instead of normal str
+        df.columns = [str(c) for c in df.columns]
         # filter out unnecessary junk from self.feature_formulas_
         self.feature_formulas_ = {f: self.feature_formulas_[f] for f in self.new_feat_cols_ + self.feateng_cols_}
         self.feature_functions_ = {f: self.feature_functions_[f] for f in self.new_feat_cols_}
         self.all_columns_ = list(df.columns)
         # train final prediction model on all selected features
         if self.verbose:
             # final dataframe contains original columns and good additional columns
-            print("[AutoFeat] Final dataframe with %i feature columns (%i new)." % (len(df.columns), len(df.columns) - len(self.original_columns_)))
+            print(
+                f"[AutoFeat] Final dataframe with {len(df.columns)} feature columns ({len(df.columns) - len(self.original_columns_)} new)."
+            )
 
         # train final prediction model
         if self.problem_type == "regression":
             model = lm.LassoLarsCV(cv=5)
         elif self.problem_type == "classification":
             model = lm.LogisticRegressionCV(cv=5, class_weight="balanced")
         else:
-            print("[AutoFeat] WARNING: Unknown problem_type %r - not fitting a prediction model." % self.problem_type)
+            print(f"[AutoFeat] WARNING: Unknown problem_type {self.problem_type} - not fitting a prediction model.")
             model = None
         if model is not None:
             if self.verbose:
-                print("[AutoFeat] Training final %s model." % self.problem_type)
+                print(f"[AutoFeat] Training final {self.problem_type} model.")
             X = df[self.good_cols_].to_numpy()
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 model.fit(X, target)
             self.prediction_model_ = model
             # sklearn requires a "classes_" attribute
             if self.problem_type == "classification":
@@ -366,96 +404,85 @@
                     coefs = np.max(np.abs(model.coef_), axis=0)
                 weights = dict(zip(self.good_cols_, coefs))
                 print("[AutoFeat] Trained model: largest coefficients:")
                 print(model.intercept_)
                 for c in sorted(weights, key=lambda x: abs(weights[x]), reverse=True):
                     if abs(weights[c]) < 1e-5:
                         break
-                    print("%.6f * %s" % (weights[c], c))
-                print("[AutoFeat] Final score: %.4f" % model.score(X, target))
+                    print(f"{weights[c]:.6f} * {c}")
+                print(f"[AutoFeat] Final score: {model.score(X, target):.4f}")
         if self.always_return_numpy:
             return df.to_numpy()
         return df
 
-    def fit(self, X, y):
+    def fit(self, X: np.ndarray | pd.DataFrame, y: np.ndarray | pd.DataFrame):
         if self.verbose:
             print("[AutoFeat] Warning: This just calls fit_transform() but does not return the transformed dataframe.")
             print("[AutoFeat] It is much more efficient to call fit_transform() instead of fit() and transform()!")
         _ = self.fit_transform(X, y)  # noqa
         return self
 
-    def transform(self, X):
+    def transform(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
         Returns:
             - new_df: new pandas dataframe with all the original features (except categorical features transformed
                       into multiple 0/1 columns) and the most promising engineered features. This df can then be
                       used to train your final model.
         """
         check_is_fitted(self, ["feature_formulas_"])
         # store column names as they'll be lost in the other check
         cols = [str(c) for c in X.columns] if isinstance(X, pd.DataFrame) else []
         # check input variables
         X = check_array(X, force_all_finite="allow-nan", dtype=None)
         if not cols:
-            cols = ["x%03i" % i for i in range(X.shape[1])]
+            cols = [f"x{i:03}" for i in range(X.shape[1])]
         if not cols == self.original_columns_:
             raise ValueError("[AutoFeat] Not the same features as when calling fit.")
         # transform X into a dataframe (again)
         df = pd.DataFrame(X, columns=cols)
         # possibly convert categorical columns
         df = self._transform_categorical_cols(df)
         # possibly apply pi-theorem
         df = self._apply_pi_theorem(df)
         # generate engineered features
         df = self._generate_features(df, self.new_feat_cols_)
+        # to prevent an error because sometimes the column names are numpy.str_ instead of normal str
+        df.columns = [str(c) for c in df.columns]
         if self.always_return_numpy:
             return df.to_numpy()
         return df
 
-    def predict(self, X):
+    def predict(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
         Returns:
-            - y_pred: predicted targets return by prediction_model.predict()
+            - y_pred: predicted targets returned by prediction_model.predict()
         """
         check_is_fitted(self, ["prediction_model_"])
-        # store column names as they'll be lost in the other check
-        cols = [str(c) for c in X.columns] if isinstance(X, pd.DataFrame) else []
-        # check input variables
-        X = check_array(X, dtype=None)
-        if not cols:
-            cols = ["x%03i" % i for i in range(X.shape[1])]
-        # transform X into a dataframe (again)
-        df = pd.DataFrame(X, columns=cols)
-        # do we need to call transform?
-        if not list(df.columns) == self.all_columns_:
-            temp = self.always_return_numpy
-            self.always_return_numpy = False
-            df = self.transform(df)
-            self.always_return_numpy = temp
+        df = self._X2df(X)
         return self.prediction_model_.predict(df[self.good_cols_].to_numpy())
 
-    def score(self, X, y):
+    def score(self, X: np.ndarray | pd.DataFrame, y: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
             - y: pandas dataframe or numpy array with the targets for all n_datapoints
         Returns:
             - R^2/Accuracy returned by prediction_model.score()
         """
         check_is_fitted(self, ["prediction_model_"])
         # store column names as they'll be lost in the other check
         cols = [str(c) for c in X.columns] if isinstance(X, pd.DataFrame) else []
         # check input variables
         X, target = check_X_y(X, y, y_numeric=self.problem_type == "regression", dtype=None)
         if not cols:
-            cols = ["x%03i" % i for i in range(X.shape[1])]
+            cols = [f"x{i:03}" for i in range(X.shape[1])]
         # transform X into a dataframe (again)
         df = pd.DataFrame(X, columns=cols)
         # do we need to call transform?
         if not list(df.columns) == self.all_columns_:
             temp = self.always_return_numpy
             self.always_return_numpy = False
             df = self.transform(df)
@@ -468,42 +495,77 @@
 
 
 class AutoFeatRegressor(AutoFeatModel, BaseEstimator, RegressorMixin):
     """Short-cut initialization for AutoFeatModel with problem_type: regression"""
 
     def __init__(
         self,
-        categorical_cols=None,
-        feateng_cols=None,
-        units=None,
-        feateng_steps=2,
-        featsel_runs=5,
-        max_gb=None,
-        transformations=("1/", "exp", "log", "abs", "sqrt", "^2", "^3"),
-        apply_pi_theorem=True,
-        always_return_numpy=False,
-        n_jobs=1,
-        verbose=0,
+        categorical_cols: list | None = None,
+        feateng_cols: list | None = None,
+        units: dict | None = None,
+        feateng_steps: int = 2,
+        featsel_runs: int = 5,
+        max_gb: int | None = None,
+        transformations: list | tuple = ("1/", "exp", "log", "abs", "sqrt", "^2", "^3"),
+        apply_pi_theorem: bool = True,
+        always_return_numpy: bool = False,
+        n_jobs: int = 1,
+        verbose: int = 0,
     ):
-        super().__init__("regression", categorical_cols, feateng_cols, units, feateng_steps,
-                         featsel_runs, max_gb, transformations, apply_pi_theorem, always_return_numpy, n_jobs, verbose)
+        super().__init__(
+            "regression",
+            categorical_cols,
+            feateng_cols,
+            units,
+            feateng_steps,
+            featsel_runs,
+            max_gb,
+            transformations,
+            apply_pi_theorem,
+            always_return_numpy,
+            n_jobs,
+            verbose,
+        )
 
 
 class AutoFeatClassifier(AutoFeatModel, BaseEstimator, ClassifierMixin):
     """Short-cut initialization for AutoFeatModel with problem_type: classification"""
 
     def __init__(
         self,
-        categorical_cols=None,
-        feateng_cols=None,
-        units=None,
-        feateng_steps=2,
-        featsel_runs=5,
-        max_gb=None,
-        transformations=("1/", "exp", "log", "abs", "sqrt", "^2", "^3"),
-        apply_pi_theorem=True,
-        always_return_numpy=False,
-        n_jobs=1,
-        verbose=0,
+        categorical_cols: list | None = None,
+        feateng_cols: list | None = None,
+        units: dict | None = None,
+        feateng_steps: int = 2,
+        featsel_runs: int = 5,
+        max_gb: int | None = None,
+        transformations: list | tuple = ("1/", "exp", "log", "abs", "sqrt", "^2", "^3"),
+        apply_pi_theorem: bool = True,
+        always_return_numpy: bool = False,
+        n_jobs: int = 1,
+        verbose: int = 0,
     ):
-        super().__init__("classification", categorical_cols, feateng_cols, units, feateng_steps,
-                         featsel_runs, max_gb, transformations, apply_pi_theorem, always_return_numpy, n_jobs, verbose)
+        super().__init__(
+            "classification",
+            categorical_cols,
+            feateng_cols,
+            units,
+            feateng_steps,
+            featsel_runs,
+            max_gb,
+            transformations,
+            apply_pi_theorem,
+            always_return_numpy,
+            n_jobs,
+            verbose,
+        )
+
+    def predict_proba(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
+        """
+        Inputs:
+            - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
+        Returns:
+            - y_pred: predicted targets probabilities returned by prediction_model.predict_proba()
+        """
+        check_is_fitted(self, ["prediction_model_"])
+        df = self._X2df(X)
+        return self.prediction_model_.predict_proba(df[self.good_cols_].to_numpy())
```

### Comparing `autofeat-2.0.9/autofeat/autofeatlight.py` & `autofeat-2.1.0/autofeat/autofeatlight.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# -*- coding: utf-8 -*-
 # Author: Franziska Horn <cod3licious@gmail.com>
 # License: MIT
 
 import sys
 import numpy as np
 import pandas as pd
 from collections import defaultdict
+from typing import Tuple
 from sklearn.base import BaseEstimator
 from sklearn.utils.validation import check_array, check_is_fitted
 from sklearn.preprocessing import StandardScaler, PowerTransformer
 
 
-def _check_features(df, corrthr=0.995, verbose=0):
+def _check_features(df: pd.DataFrame, corrthr: float = 0.995, verbose: int = 0) -> list:
     """
     Identify features with zeros variance or a correlation of (almost) 1 to other features, i.e., useless features.
 
     Inputs:
         - df: pd.DataFrame with all features
         - corrthr: threshold for correlations: if a feature has a higher pearson correlation to another feature it's
                    considered as redundant and ignored (float; default: 0.995)
@@ -28,35 +28,37 @@
     useless_cols = set()
     # 1. identify features with zero variance
     for c, v in df.var().items():
         if pd.isna(v) or v <= sys.float_info.epsilon:
             useless_cols.add(c)
     # 2. identify redundant features (that have a correlation of ~1 with other features)
     correlated_cols = defaultdict(set)
-    corrmat = pd.DataFrame(np.abs(np.corrcoef(df.values, rowvar=False)), columns=df.columns)
+    corrmat = pd.DataFrame(np.abs(np.corrcoef(df.values, rowvar=False)), columns=df.columns, index=df.columns)
     np.fill_diagonal(corrmat.values, 0)
     for c, v in corrmat.unstack().sort_values(ascending=False).items():
         if v < corrthr:
             break
         if (c[0] != c[1]) and (c[0] not in useless_cols):
             correlated_cols[c[0]].add(c[1])
     # keep the columns that eliminate the most correlated columns
     for c in sorted(correlated_cols, key=lambda x: len(correlated_cols[x]), reverse=True):
         # the first variable that is correlated with others adds its correlated variables to the set of useless cols
         # since we check if a variable is in useless_cols, the correlated variables can't add the original variable
         if c not in useless_cols:
             useless_cols.update(correlated_cols[c])
     # return list of columns that should be kept
     if verbose:
-        print("[AutoFeatLight] %i columns identified as useless:" % len(useless_cols))
+        print(f"[AutoFeatLight] {len(useless_cols)} columns identified as useless:")
         print(sorted(useless_cols))
     return [c for c in df.columns if c not in useless_cols]
 
 
-def _compute_additional_features(X, feature_names=None, compute_ratio=True, compute_product=True, verbose=0):
+def _compute_additional_features(
+    X: np.ndarray, feature_names: list | None = None, compute_ratio: bool = True, compute_product: bool = True, verbose: int = 0
+) -> Tuple[np.ndarray, list]:
     """
     Compute additional non-linear features from the original features (ratio or product of two features).
 
     Inputs:
         - X: np.array with data (n_datapoints x n_features)
         - feature_names: optional list of column names to identify the features in X
         - compute_ratio: bool (default: True), whether to compute ratios of features
@@ -66,62 +68,61 @@
         - np.array (n_datapoints x n_additional_features) with newly computed features
         - list with n_additional_features names describing the newly computed features
     """
     # check how many new features we will compute
     d = X.shape[1]
     n = 0
     if compute_ratio:
-        n += d*d - d
+        n += d * d - d
     if compute_product:
-        n += (d*d - d)//2
+        n += (d * d - d) // 2
     if not n:
         print("ERROR: call _compute_additional_features with compute_ratio and/or compute_product set to True")
         return None, []
     if not feature_names:
-        feature_names = ["x%i" % i for i in range(1, d+1)]
+        feature_names = [f"x{i}" for i in range(1, d + 1)]
     # compute new features
     if verbose:
-        print("[AutoFeatLight] computing %i additional features from %i original features" % (n, d))
+        print(f"[AutoFeatLight] computing {n} additional features from {d} original features")
     new_features = []
     X_new = np.zeros((X.shape[0], n))
     new_i = 0
     if compute_ratio:
         for i in range(d):
             # compute 1/x1
-            with np.errstate(divide='ignore'):
-                x = 1/X[:, i]
+            with np.errstate(divide="ignore"):
+                x = 1 / X[:, i]
             # instead of dividing by 0 for some data points we just set the new feature to 0 there
-            x[np.invert(np.isfinite(x))] = 0.
+            x[np.invert(np.isfinite(x))] = 0.0
             for j in range(d):
                 if i != j:
                     # multiply with x2 to get x2/x1
                     X_new[:, new_i] = x * X[:, j]
-                    new_features.append("%s / %s" % (feature_names[j], feature_names[i]))
+                    new_features.append(f"{feature_names[j]} / {feature_names[i]}")
                     new_i += 1
     if compute_product:
         for i in range(d):
-            for j in range(i+1, d):
+            for j in range(i + 1, d):
                 X_new[:, new_i] = X[:, i] * X[:, j]
-                new_features.append("%s * %s" % (feature_names[i], feature_names[j]))
+                new_features.append(f"{feature_names[i]} * {feature_names[j]}")
                 new_i += 1
-    assert new_i == n, "Internal Error in _compute_additional_features: new_i: %r, n: %r" % (new_i, n)
+    assert new_i == n, f"Internal Error in _compute_additional_features: new_i: {new_i}, n: {n}"
     return X_new, new_features
 
 
 class AutoFeatLight(BaseEstimator):
-
     def __init__(
         self,
-        compute_ratio=True,
-        compute_product=True,
-        scale=False,
-        power_transform=False,
-        corrthr=0.995,
-        corrthr_init=0.99999,
-        verbose=0,
+        compute_ratio: bool = True,
+        compute_product: bool = True,
+        scale: bool = False,
+        power_transform: bool = False,
+        corrthr: float = 0.995,
+        corrthr_init: float = 0.99999,
+        verbose: int = 0,
     ):
         """
         Basic Feature Engineering:
             - remove useless features (zero variance or redundant)
             - compute additional non-linear features (ratios and product of original features, i.e. x1/x2 and x1*x2)
             - make all features more normally distributed (using the yeo-johnson power transform)
 
@@ -148,28 +149,28 @@
         self.compute_product = compute_product
         self.scale = scale
         self.power_transform = power_transform
         self.corrthr_init = corrthr_init
         self.corrthr = corrthr
         self.verbose = verbose
 
-    def fit(self, X):
+    def fit(self, X: np.ndarray | pd.DataFrame):
         """
         WARNING: call fit_transform instead!
 
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
         """
         if self.verbose:
             print("[AutoFeatLight] Warning: This just calls fit_transform() but does not return the transformed dataframe.")
             print("[AutoFeatLight] It is much more efficient to call fit_transform() instead of fit() and transform()!")
         _ = self.fit_transform(X)  # noqa
         return self
 
-    def transform(self, X):
+    def transform(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
         Returns:
             - new_X: new pandas dataframe or numpy array with additional/transformed features
         """
         check_is_fitted(self, ["good_cols_org_"])
@@ -180,77 +181,81 @@
         if isinstance(X, pd.DataFrame):
             # make sure all data is numeric or we'll get an error when checking X
             X = X.select_dtypes(include=np.number)
             df_index = X.index
         else:
             df_index = None
         # check input
-        cols = list(X.columns) if isinstance(X, pd.DataFrame) else ["x%i" % i for i in range(1, X.shape[1]+1)]
+        cols = list(X.columns) if isinstance(X, pd.DataFrame) else [f"x{i}" for i in range(1, X.shape[1] + 1)]
         X = check_array(X, force_all_finite="allow-nan")
         if not cols == self.original_columns_:
             raise ValueError("[AutoFeatLight] Not the same features as when calling fit.")
         # sort out useless original columns
         df = pd.DataFrame(X, columns=cols, index=df_index)[self.good_cols_org_]
         if self.compute_ratio or self.compute_product:
             # compute additional useful features
-            X_new, new_features = _compute_additional_features(df.to_numpy(), self.good_cols_org_, self.compute_ratio, self.compute_product, self.verbose)
+            X_new, new_features = _compute_additional_features(
+                df.to_numpy(), self.good_cols_org_, self.compute_ratio, self.compute_product, self.verbose
+            )
             df = pd.concat([df, pd.DataFrame(X_new, columns=new_features)], axis=1)
             df = df[self.features_]
         # scale/transform
         if self.scale or self.power_transform:
             X_new = self.scaler_.transform(df.to_numpy())
             if self.power_transform:
                 X_new = self.power_transformer_.transform(X_new)
             df = pd.DataFrame(X_new, columns=df.columns, index=df.index)
         # return either dataframe or array
         return df if self.return_df_ else df.to_numpy()
 
-    def fit_transform(self, X):
+    def fit_transform(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
         Returns:
             - new_X: new pandas dataframe or numpy array with additional/transformed features
         """
         self.return_df_ = isinstance(X, pd.DataFrame)
         if isinstance(X, pd.DataFrame):
             # make sure all data is numeric or we'll get an error when checking X
             X = X.select_dtypes(include=np.number)
             df_index = X.index
         else:
             df_index = None
         # store column names as they'll be lost in the other check
-        self.original_columns_ = list(X.columns) if isinstance(X, pd.DataFrame) else ["x%i" % i for i in range(1, X.shape[1]+1)]
+        self.original_columns_ = list(X.columns) if isinstance(X, pd.DataFrame) else [f"x{i}" for i in range(1, X.shape[1] + 1)]
         # check input
         X = check_array(X, force_all_finite="allow-nan")
         # transform X into a dataframe (again)
         df = pd.DataFrame(X, columns=self.original_columns_, index=df_index)
         # see which of the original features are not completely useless
         self.good_cols_org_ = _check_features(df, self.corrthr_init, self.verbose)
         if not self.good_cols_org_:
             if self.verbose > 0:
                 print("[AutoFeatLight] WARNING: No good features found; returning original features.")
             return df if self.return_df_ else X
         # compute additional features
         df = df[self.good_cols_org_]
         if self.compute_ratio or self.compute_product:
-            X_new, new_features = _compute_additional_features(df.to_numpy(), self.good_cols_org_, self.compute_ratio, self.compute_product, self.verbose)
+            X_new, new_features = _compute_additional_features(
+                df.to_numpy(), self.good_cols_org_, self.compute_ratio, self.compute_product, self.verbose
+            )
             # add new features to original dataframe
             df = pd.concat([df, pd.DataFrame(X_new, columns=new_features, index=df_index)], axis=1)
             # check again which of the features we should keep
             self.features_ = _check_features(df, self.corrthr, self.verbose)
             df = df[self.features_]
         else:
             self.features_ = self.good_cols_org_
         if self.scale or self.power_transform:
             # scale data to avoid errors due to large numbers
             self.scaler_ = StandardScaler(with_mean=False)
             X_new = self.scaler_.fit_transform(df.to_numpy())
             if self.power_transform:
-                self.power_transformer_ = PowerTransformer(method='yeo-johnson', standardize=True)
+                self.power_transformer_ = PowerTransformer(method="yeo-johnson", standardize=True)
                 X_new = self.power_transformer_.fit_transform(X_new)
             df = pd.DataFrame(X_new, columns=df.columns, index=df.index)
         if self.verbose > 0:
-            print("[AutoFeatLight] New data shape: %i x %i" % df.shape)
+            print(f"[AutoFeatLight] New data shape: {df.shape[0]} x {df.shape[1]}")
         self.n_features_in_ = len(self.original_columns_)
         # return either dataframe or array
         return df if self.return_df_ else df.to_numpy()
```

### Comparing `autofeat-2.0.9/autofeat/feateng.py` & `autofeat-2.1.0/autofeat/feateng.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-# -*- coding: utf-8 -*-
 # Author: Franziska Horn <cod3licious@gmail.com>
 # License: MIT
 
-from __future__ import unicode_literals, division, print_function, absolute_import
-from builtins import str
 import re
 import operator as op
 from functools import reduce
 from itertools import combinations, product
+from typing import Callable, Tuple
 
 import numba as nb
 import numpy as np
 import pandas as pd
 import sympy
 from sympy.utilities.lambdify import lambdify
 from sklearn.preprocessing import StandardScaler
 import pint
 
 
-def colnames2symbols(c, i=0):
+def colnames2symbols(c: str | int, i: int = 0) -> str:
     # take a messy column name and transform it to something sympy can handle
     # worst case: i is the number of the features
     # has to be a string
     c = str(c)
     # should not contain non-alphanumeric characters
     c = re.sub(r"\W+", "", c)
     if not c:
-        c = "x%03i" % i
+        c = f"x{i:03}"
     elif c[0].isdigit():
         c = "x" + c
     return c
 
 
-def ncr(n, r):
+def ncr(n: int, r: int) -> int:
     # compute number of combinations for n chose r
     r = min(r, n - r)
     numer = reduce(op.mul, range(n, n - r, -1), 1)
     denom = reduce(op.mul, range(1, r + 1), 1)
     return numer // denom
 
 
-def n_cols_generated(n_features, max_steps, n_transformations=7, n_combinations=4):
+def n_cols_generated(n_features: int, max_steps: int, n_transformations: int = 7, n_combinations: int = 4) -> int:
     """
     computes the upper bound of how many features will be generated based on n_features to start with
     and max_steps feateng steps.
     """
     # n_transformations is 1-len(func_transform) because either abs() or sqrt and log will be applied
     n_transformations -= 1
     original_cols = n_features
@@ -87,21 +85,21 @@
     if steps <= max_steps:
         # n_additions += new_cols * 2
         new_cols += new_cols * n_transformations
     return original_cols + new_cols + new_new_cols - n_additions
 
 
 def engineer_features(
-    df_org,
-    start_features=None,
-    units=None,
-    max_steps=3,
-    transformations=("1/", "exp", "log", "abs", "sqrt", "^2", "^3"),
-    verbose=0,
-):
+    df_org: pd.DataFrame,
+    start_features: list | None = None,
+    units: dict | None = None,
+    max_steps: int = 3,
+    transformations: list | tuple = ("1/", "exp", "log", "abs", "sqrt", "^2", "^3"),
+    verbose: int = 0,
+) -> Tuple[pd.DataFrame, dict]:
     """
     Given a DataFrame with original features, perform the feature engineering routine for max_steps.
     It starts with a transformation of the original features (applying log, ^2, sqrt, etc.),
     then in the next step, the features are combined (x+y, x*y, ...), and in further steps, the resulting
     features are again transformed and combinations of the resulting features are computed.
 
     Inputs:
@@ -127,73 +125,74 @@
     """
     # initialize the feature pool with columns from the dataframe
     if not start_features:
         start_features = df_org.columns
     else:
         for c in start_features:
             if c not in df_org.columns:
-                raise ValueError("[feateng] start feature %r not in df_org.columns" % c)
+                raise ValueError(f"[feateng] start feature {c} not in df_org.columns")
     feature_pool = {c: sympy.symbols(colnames2symbols(c, i), real=True) for i, c in enumerate(start_features)}
     if max_steps < 1:
         if verbose > 0:
             print("[feateng] Warning: no features generated for max_steps < 1.")
         return df_org, feature_pool
     # get a copy of the dataframe - this is where all the features will be added
     df = pd.DataFrame(df_org.copy(), dtype=np.float32)
 
     compiled_func_transformations = None
     compiled_func_transforms_cond = None
     compiled_func_combinations = None
 
-    def compile_func_transform(name, ft, plus_1=False):
+    def compile_func_transform(name: str, ft: Callable, plus_1: bool = False):
         def _abs(x):
             return np.abs(x)
+
         # create temporary variable expression and apply it to precomputed feature
         t = sympy.symbols("t")
         if plus_1:
             expr_temp = ft(t + 1)
         else:
             expr_temp = ft(t)
         if name == "abs":
             fn = _abs
         else:
             fn = lambdify(t, expr_temp)
         return nb.njit(fn)
 
-    def apply_transformations(features_list):
+    def apply_transformations(features_list: list) -> Tuple[list, set]:
         # feature transformations
         func_transform = {
             "exp": lambda x: sympy.exp(x),
             "exp-": lambda x: sympy.exp(-x),
             "log": lambda x: sympy.log(x),
             "abs": lambda x: sympy.Abs(x),
             "sqrt": lambda x: sympy.sqrt(x),
             "sin": lambda x: sympy.sin(x),
             "cos": lambda x: sympy.cos(x),
             "2^": lambda x: 2**x,
             "^2": lambda x: x**2,
             "^3": lambda x: x**3,
             "1+": lambda x: 1 + x,
             "1-": lambda x: 1 - x,
-            "1/": lambda x: 1 / x
+            "1/": lambda x: 1 / x,
         }
         func_transform_units = {
             "exp": lambda x: np.exp(x),
             "exp-": lambda x: np.exp(-x),
             "log": lambda x: np.log(x),
             "abs": lambda x: np.abs(x),
             "sqrt": lambda x: np.sqrt(x),
             "sin": lambda x: np.sin(x),
             "cos": lambda x: np.cos(x),
             "2^": lambda x: np.exp(x),
             "^2": lambda x: x**2,
             "^3": lambda x: x**3,
             "1+": lambda x: 1 + x,
             "1-": lambda x: 1 - x,
-            "1/": lambda x: 1 / x
+            "1/": lambda x: 1 / x,
         }
         # conditions on the original features that have to be met to apply the transformation
         func_transform_cond = {
             "exp": lambda x: np.all(x < 10),
             "exp-": lambda x: np.all(-x < 10),
             "log": lambda x: np.all(x >= 0),
             "abs": lambda x: np.any(x < 0),
@@ -201,39 +200,37 @@
             "sin": lambda x: True,
             "cos": lambda x: True,
             "2^": lambda x: np.all(x < 50),
             "^2": lambda x: np.all(np.abs(x) < 1000000),
             "^3": lambda x: np.all(np.abs(x) < 10000),
             "1+": lambda x: True,
             "1-": lambda x: True,
-            "1/": lambda x: np.all(x != 0)
+            "1/": lambda x: np.all(x != 0),
         }
         # apply transformations to the features in the given features list
         # modifies global variables df and feature_pool!
         nonlocal df, feature_pool, units
         nonlocal compiled_func_transformations, compiled_func_transforms_cond
 
         if compiled_func_transformations is None:
-            compiled_func_transformations = {k: compile_func_transform(k, v)
-                                             for k, v in func_transform.items()}
-            compiled_func_transformations["log_plus_1"] = compile_func_transform(
-                "log", func_transform["log"], plus_1=True)
+            compiled_func_transformations = {k: compile_func_transform(k, v) for k, v in func_transform.items()}
+            compiled_func_transformations["log_plus_1"] = compile_func_transform("log", func_transform["log"], plus_1=True)
 
             compiled_func_transforms_cond = {x[0]: nb.njit(x[1]) for x in func_transform_cond.items()}
 
         # returns a list of new features that were generated
         new_features = []
         uncorr_features = set()
         # store all new features in a preallocated numpy array before adding it to the dataframe
         feat_array = np.zeros((df.shape[0], len(features_list) * len(transformations)), dtype=np.float32)
         cat_features = {feat for feat in features_list if len(df[feat].unique()) <= 2}
-        func_transform_cond_cache = {}   # Cache for compiled_func_transforms_cond checks
+        func_transform_cond_cache = {}  # Cache for compiled_func_transforms_cond checks
         for i, feat in enumerate(features_list):
             if verbose and not i % 100:
-                print("[feateng] %15i/%15i features transformed" % (i, len(features_list)), end="\r")
+                print(f"[feateng] {i:15}/{len(features_list):15} features transformed", end="\r")
             for ft in transformations:
                 # (don't compute transformations on categorical features)
                 if feat in cat_features:
                     continue
                 # check if transformation is valid for particular feature (i.e. given actual numerical values)
                 cache_key = (ft, feat)
                 if cache_key not in func_transform_cond_cache:
@@ -244,55 +241,57 @@
                     expr_name = str(expr)
                     # we're simplifying expressions, so we might already have that one
                     if expr_name not in feature_pool:
                         # if we're given units, check if the operation is legal
                         if units:
                             try:
                                 units[expr_name] = func_transform_units[ft](units[feat])
-                                units[expr_name].__dict__["_magnitude"] = 1.
+                                units[expr_name].__dict__["_magnitude"] = 1.0
                             except (pint.DimensionalityError, pint.OffsetUnitCalculusError):
                                 continue
                         feature_pool[expr_name] = expr
                         if expr == "log" and np.any(df[feat] < 1):
                             f = compiled_func_transformations["log_plus_1"]
                         else:
                             f = compiled_func_transformations[ft]
                         new_feat = np.array(f(df[feat].to_numpy()), dtype=np.float32)
                         # near 0 variance test - sometimes all that's left is "e"
                         if np.isfinite(new_feat).all() and np.var(new_feat) > 1e-10:
                             corr = abs(np.corrcoef(new_feat, df[feat])[0, 1])
-                            if corr < 1.:
+                            if corr < 1.0:
                                 feat_array[:, len(new_features)] = new_feat
                                 new_features.append(expr_name)
                                 # correlation test: don't include features that are basically the same as the original features
                                 # but we only filter them out at the end, since they still might help in other steps!
                                 if corr < 0.95:
                                     uncorr_features.add(expr_name)
         if verbose > 0:
-            print("[feateng] Generated %i transformed features from %i original features - done." % (len(new_features), len(features_list)))
-        df = df.join(pd.DataFrame(feat_array[:, :len(new_features)], columns=new_features, index=df.index, dtype=np.float32))
+            print(
+                f"[feateng] Generated {len(new_features)} transformed features from {len(features_list)} original features - done."
+            )
+        df = df.join(pd.DataFrame(feat_array[:, : len(new_features)], columns=new_features, index=df.index, dtype=np.float32))
         return new_features, uncorr_features
 
-    def compile_func_combinations(func_combinations):
+    def compile_func_combinations(func_combinations: dict) -> dict:
         d = {}
         for fc in func_combinations:
             s, t = sympy.symbols("s t")
             expr_temp = func_combinations[fc](s, t)
             fn = lambdify((s, t), expr_temp)
             vect = nb.vectorize(["float32(float32, float32)"], nopython=True)
             d[fc] = vect(fn)
         return d
 
-    def get_feature_combinations(feature_tuples):
+    def get_feature_combinations(feature_tuples: list) -> Tuple[list, set]:
         # new features as combinations of two other features
         func_combinations = {
             "x+y": lambda x, y: x + y,
             "x*y": lambda x, y: x * y,
             "x-y": lambda x, y: x - y,
-            "y-x": lambda x, y: y - x
+            "y-x": lambda x, y: y - x,
         }
         # get all feature combinations for the given feature tuples
         # modifies global variables df and feature_pool!
         nonlocal df, feature_pool, units, compiled_func_combinations
 
         if compiled_func_combinations is None:
             compiled_func_combinations = compile_func_combinations(func_combinations)
@@ -306,42 +305,44 @@
         # returns a list of new features that were generated
         new_features = []
         uncorr_features = set()
         # store all new features in a preallocated numpy array before adding it to the dataframe
         feat_array = np.zeros((df.shape[0], len(feature_tuples) * len(combinations)), dtype=np.float32)
         for i, (feat1, feat2) in enumerate(feature_tuples):
             if verbose and not i % 100:
-                print("[feateng] %15i/%15i feature tuples combined" % (i, len(feature_tuples)), end="\r")
+                print(f"[feateng] {i:15}/{len(feature_tuples):15} feature tuples combined", end="\r")
             for fc in combinations:
                 expr = func_combinations[fc](feature_pool[feat1], feature_pool[feat2])
                 expr_name = str(expr)
                 if expr_name not in feature_pool:
                     # if we're given units, check if the operation is legal
                     if units:
                         try:
                             units[expr_name] = func_combinations[fc](units[feat1], units[feat2])
-                            units[expr_name].__dict__["_magnitude"] = 1.
+                            units[expr_name].__dict__["_magnitude"] = 1.0
                         except (pint.DimensionalityError, pint.OffsetUnitCalculusError):
                             continue
                     feature_pool[expr_name] = expr
                     f = compiled_func_combinations[fc]
                     new_feat = np.array(f(df[feat1].to_numpy(), df[feat2].to_numpy()), dtype=np.float32)
                     # near 0 variance test - sometimes all that's left is "e"
                     if np.isfinite(new_feat).all() and np.var(new_feat) > 1e-10:
                         corr = max(abs(np.corrcoef(new_feat, df[feat1])[0, 1]), abs(np.corrcoef(new_feat, df[feat2])[0, 1]))
-                        if corr < 1.:
+                        if corr < 1.0:
                             feat_array[:, len(new_features)] = new_feat
                             new_features.append(expr_name)
                             # correlation test: don't include features that are basically the same as the original features
                             # but we only filter them out at the end, since they still might help in other steps!
                             if corr < 0.95:
                                 uncorr_features.add(expr_name)
         if verbose > 0:
-            print("[feateng] Generated %i feature combinations from %i original feature tuples - done." % (len(new_features), len(feature_tuples)))
-        df = df.join(pd.DataFrame(feat_array[:, :len(new_features)], columns=new_features, index=df.index, dtype=np.float32))
+            print(
+                f"[feateng] Generated {len(new_features)} feature combinations from {len(feature_tuples)} original feature tuples - done."
+            )
+        df = df.join(pd.DataFrame(feat_array[:, : len(new_features)], columns=new_features, index=df.index, dtype=np.float32))
         return new_features, uncorr_features
 
     # get transformations of initial features
     steps = 1
     if verbose > 0:
         print("[feateng] Step 1: transformation of original features")
     original_features = list(feature_pool.keys())
@@ -356,45 +357,60 @@
             print("[feateng] Step 2: first combination of features")
         new_features, temp_uncorr = get_feature_combinations(list(combinations(original_features, 2)))
         uncorr_features.update(temp_uncorr)
         steps += 1
     while steps <= max_steps:
         # apply transformations on these new features
         if verbose > 0:
-            print("[feateng] Step %i: transformation of new features" % steps)
+            print(f"[feateng] Step {steps}: transformation of new features")
         temp_new, temp_uncorr = apply_transformations(new_features)
         new_features.extend(temp_new)
         uncorr_features.update(temp_uncorr)
         steps += 1
         # get combinations of old and new features
         if steps <= max_steps:
             if verbose > 0:
-                print("[feateng] Step %i: combining old and new features" % steps)
+                print(f"[feateng] Step {steps}: combining old and new features")
             new_new_features, temp_uncorr = get_feature_combinations(list(product(original_features, new_features)))
             uncorr_features.update(temp_uncorr)
             steps += 1
         # and combinations of new features within themselves
         if steps <= max_steps:
             if verbose > 0:
-                print("[feateng] Step %i: combining new features" % steps)
+                print(f"[feateng] Step {steps}: combining new features")
             temp_new, temp_uncorr = get_feature_combinations(list(combinations(new_features, 2)))
             new_new_features.extend(temp_new)
             uncorr_features.update(temp_uncorr)
             steps += 1
             # update old and new features and repeat
             original_features.extend(new_features)
             new_features = new_new_features
 
     # sort out all features that are just additions on the highest level or correlated with more basic features
     if verbose > 0:
-        print("[feateng] Generated altogether %i new features in %i steps" % (len(feature_pool) - len(start_features), max_steps))
+        print(f"[feateng] Generated altogether {len(feature_pool) - len(start_features)} new features in {max_steps} steps")
         print("[feateng] Removing correlated features, as well as additions at the highest level")
-    feature_pool = {c: feature_pool[c] for c in feature_pool if c in uncorr_features and not feature_pool[c].func == sympy.core.add.Add}
-    cols = [c for c in list(df.columns) if c in feature_pool and c not in df_org.columns]  # categorical cols not in feature_pool
+    feature_pool = {
+        c: feature_pool[c] for c in feature_pool if c in uncorr_features and not feature_pool[c].func == sympy.core.add.Add
+    }
+    cols = [
+        c for c in list(df.columns) if c in feature_pool and c not in df_org.columns
+    ]  # categorical cols not in feature_pool
     if cols:
         # check for correlated features again; this time with the start features
-        corrs = dict(zip(cols, np.max(np.abs(np.dot(StandardScaler().fit_transform(df[cols]).T, StandardScaler().fit_transform(df_org))/df_org.shape[0]), axis=1)))
+        corrs = dict(
+            zip(
+                cols,
+                np.max(
+                    np.abs(
+                        np.dot(StandardScaler().fit_transform(df[cols]).T, StandardScaler().fit_transform(df_org))
+                        / df_org.shape[0]
+                    ),
+                    axis=1,
+                ),
+            )
+        )
         cols = [c for c in cols if corrs[c] < 0.9]
     cols = list(df_org.columns) + cols
     if verbose > 0:
-        print("[feateng] Generated a total of %i additional features" % (len(feature_pool) - len(start_features)))
+        print(f"[feateng] Generated a total of {len(feature_pool) - len(start_features)} additional features")
     return df[cols], feature_pool
```

### Comparing `autofeat-2.0.9/autofeat/featsel.py` & `autofeat-2.1.0/autofeat/featsel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,67 @@
-# -*- coding: utf-8 -*-
 # Author: Franziska Horn <cod3licious@gmail.com>
 # License: MIT
 
-from __future__ import unicode_literals, division, print_function, absolute_import
-from builtins import zip
 import warnings
 import numpy as np
 import pandas as pd
 from collections import Counter
 from joblib import Parallel, delayed
 from sklearn.base import BaseEstimator
 from sklearn.utils.validation import check_X_y, check_array, check_is_fitted
 import sklearn.linear_model as lm
 from .nb_utils import nb_standard_scale
 
 
-def _add_noise_features(X):
+def _add_noise_features(X: np.ndarray):
     """
     Adds 3-1.5*d additional noise features to X.
 
     Inputs:
         - X: n x d numpy array with d features
     Returns:
         - X with additional noise features
     """
     n_feat = X.shape[1]
     if X.shape[0] > 50 and n_feat > 1:
         # shuffled features
         rand_noise = nb_standard_scale(np.random.permutation(X.flatten()).reshape(X.shape))
         X = np.hstack([X, rand_noise])
     # normally distributed noise
-    rand_noise = np.random.randn(X.shape[0], max(3, int(0.5*n_feat)))
+    rand_noise = np.random.randn(X.shape[0], max(3, int(0.5 * n_feat)))
     X = np.hstack([X, rand_noise])
     return X
 
 
-def _noise_filtering(X, target, good_cols=[], problem_type="regression"):
+def _noise_filtering(
+    X: np.ndarray, target: np.ndarray, good_cols: list | None = None, problem_type: str = "regression"
+) -> list:
     """
     Trains a prediction model with additional noise features and selects only those of the
     original features that have a higher coefficient than any of the noise features.
 
     Inputs:
         - X: n x d numpy array with d features
         - target: n dimensional array with targets corresponding to the data points in X
         - good_cols: list of column names for the features in X
         - problem_type: str, either "regression" or "classification" (default: "regression")
     Returns:
         - good_cols: list of noise filtered column names
     """
     n_feat = X.shape[1]
-    assert len(good_cols) == n_feat, "fewer column names provided than features in X."
-    if not good_cols:
+    if good_cols is None or not len(good_cols):
         good_cols = list(range(n_feat))
+    assert len(good_cols) == n_feat, "fewer column names provided than features in X."
     # perform noise filtering on these features
     if problem_type == "regression":
         model = lm.LassoLarsCV(cv=5, eps=1e-8)
     elif problem_type == "classification":
         model = lm.LogisticRegressionCV(cv=5, penalty="l1", solver="saga", class_weight="balanced")
     else:
-        print("[featsel] WARNING: Unknown problem_type %r - not performing noise filtering." % problem_type)
+        print(f"[featsel] WARNING: Unknown problem_type {problem_type} - not performing noise filtering.")
         model = None
     if model is not None:
         X = _add_noise_features(X)
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             # TODO: remove if sklearn least_angle issue is fixed
             try:
@@ -72,43 +71,43 @@
                 model.fit(X[rand_idx], target[rand_idx])
             # model.fit(X, target)
         if problem_type == "regression":
             coefs = np.abs(model.coef_)
         else:
             # model.coefs_ is n_classes x n_features, but we need n_features
             coefs = np.max(np.abs(model.coef_), axis=0)
-        weights = dict(zip(good_cols, coefs[:len(good_cols)]))
+        weights = dict(zip(good_cols, coefs[: len(good_cols)]))
         # only include features that are more important than our known noise features
         noise_w_thr = np.max(coefs[n_feat:])
         good_cols = [c for c in good_cols if weights[c] > noise_w_thr]
     return good_cols
 
 
-def _select_features_1run(df, target, problem_type="regression", verbose=0):
+def _select_features_1run(df: pd.DataFrame, target: np.ndarray, problem_type: str = "regression", verbose: int = 0) -> list:
     """
     One feature selection run.
 
     Inputs:
         - df: nxp pandas DataFrame with n data points and p features; to avoid overfitting, only provide data belonging
               to the n training data points. The variables have to be scaled to have 0 mean and unit variance.
         - target: n dimensional array with targets corresponding to the data points in df
         - problem_type: str, either "regression" or "classification" (default: "regression")
         - verbose: verbosity level (int; default: 0)
     Returns:
         - good_cols: list of column names for df with which a prediction model can be trained
     """
     if df.shape[0] <= 1:
-        raise ValueError("n_samples = {}".format(df.shape[0]))
+        raise ValueError(f"n_samples = {df.shape[0]}")
     # initial selection of too few but (hopefully) relevant features
     if problem_type == "regression":
         model = lm.LassoLarsCV(cv=5, eps=1e-8)
     elif problem_type == "classification":
         model = lm.LogisticRegressionCV(cv=5, penalty="l1", solver="saga", class_weight="balanced")
     else:
-        print("[featsel] WARNING: Unknown problem_type %r - not performing feature selection!" % problem_type)
+        print(f"[featsel] WARNING: Unknown problem_type {problem_type} - not performing feature selection!")
         return []
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         # TODO: remove if sklearn least_angle issue is fixed
         try:
             model.fit(df, target)
         except ValueError:
@@ -118,30 +117,30 @@
         # model.fit(df, target)
     if problem_type == "regression":
         coefs = np.abs(model.coef_)
     else:
         # model.coefs_ is n_classes x n_features, but we need n_features
         coefs = np.max(np.abs(model.coef_), axis=0)
     # weight threshold: select at most 0.2*n_train initial features
-    thr = sorted(coefs, reverse=True)[min(df.shape[1]-1, df.shape[0]//5)]
+    thr = sorted(coefs, reverse=True)[min(df.shape[1] - 1, df.shape[0] // 5)]
     initial_cols = list(df.columns[coefs > thr])
     # noise filter
     initial_cols = _noise_filtering(df[initial_cols].to_numpy(), target, initial_cols, problem_type)
-    good_cols = set(initial_cols)
+    good_cols_set = set(initial_cols)
     if verbose > 0:
-        print("[featsel]\t %i initial features." % len(initial_cols))
+        print(f"[featsel]\t {len(initial_cols)} initial features.")
     # add noise features
     X_w_noise = _add_noise_features(df[initial_cols].to_numpy())
     # go through all remaining features in splits of n_feat <= 0.5*n_train
     other_cols = list(np.random.permutation(list(set(df.columns).difference(initial_cols))))
     if other_cols:
-        n_splits = int(np.ceil(len(other_cols)/max(10, 0.5*df.shape[0]-len(initial_cols))))
-        split_size = int(np.ceil(len(other_cols)/n_splits))
+        n_splits = int(np.ceil(len(other_cols) / max(10, 0.5 * df.shape[0] - len(initial_cols))))
+        split_size = int(np.ceil(len(other_cols) / n_splits))
         for i in range(n_splits):
-            current_cols = other_cols[i*split_size:min(len(other_cols), (i+1)*split_size)]
+            current_cols = other_cols[i * split_size : min(len(other_cols), (i + 1) * split_size)]
             X = np.hstack([df[current_cols].to_numpy(), X_w_noise])
             if problem_type == "regression":
                 model = lm.LassoLarsCV(cv=5, eps=1e-8)
             else:
                 model = lm.LogisticRegressionCV(cv=5, penalty="l1", solver="saga", class_weight="balanced")
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
@@ -154,29 +153,39 @@
                 # model.fit(X, target)
             current_cols.extend(initial_cols)
             if problem_type == "regression":
                 coefs = np.abs(model.coef_)
             else:
                 # model.coefs_ is n_classes x n_features, but we need n_features
                 coefs = np.max(np.abs(model.coef_), axis=0)
-            weights = dict(zip(current_cols, coefs[:len(current_cols)]))
+            weights = dict(zip(current_cols, coefs[: len(current_cols)]))
             # only include features that are more important than our known noise features
-            noise_w_thr = np.max(coefs[len(current_cols):])
-            good_cols.update([c for c in weights if abs(weights[c]) > noise_w_thr])
+            noise_w_thr = np.max(coefs[len(current_cols) :])
+            good_cols_set.update([c for c in weights if abs(weights[c]) > noise_w_thr])
             if verbose > 0:
-                print("[featsel]\t Split %2i/%i: %3i candidate features identified." % (i+1, n_splits, len(good_cols)), end="\r")
+                print(
+                    f"[featsel]\t Split {i + 1:2}/{n_splits}: {len(good_cols_set):3} candidate features identified.", end="\r"
+                )
     # noise filtering on the combination of features
-    good_cols = list(good_cols)
+    good_cols = list(good_cols_set)
     good_cols = _noise_filtering(df[good_cols].to_numpy(), target, good_cols, problem_type)
     if verbose > 0:
-        print("\n[featsel]\t Selected %3i features after noise filtering." % len(good_cols))
+        print(f"\n[featsel]\t Selected {len(good_cols):3} features after noise filtering.")
     return good_cols
 
 
-def select_features(df, target, featsel_runs=5, keep=None, problem_type="regression", n_jobs=1, verbose=0):
+def select_features(
+    df: pd.DataFrame,
+    target: np.ndarray,
+    featsel_runs: int = 5,
+    keep: list | None = None,
+    problem_type: str = "regression",
+    n_jobs: int = 1,
+    verbose: int = 0,
+) -> list:
     """
     Selects predictive features given the data and targets.
 
     Inputs:
         - df: nxp pandas DataFrame with n data points and p features; to avoid overfitting, only provide data belonging
               to the n training data points.
         - target: n dimensional array with targets corresponding to the data points in df
@@ -209,39 +218,44 @@
     if verbose > 0:
         print("done.")
 
     good_cols = list(df.columns)
 
     # select good features in k runs in parallel
     # by doing sort of a cross-validation (i.e., randomly subsample data points)
-    def run_select_features(i):
+    def run_select_features(i: int):
         if verbose > 0:
-            print("[featsel] Feature selection run %i/%i" % (i+1, featsel_runs))
+            print(f"[featsel] Feature selection run {i + 1}/{featsel_runs}")
         np.random.seed(i)
-        rand_idx = np.random.permutation(df_scaled.index)[:max(10, int(0.85 * len(df_scaled)))]
-        return _select_features_1run(df_scaled.iloc[rand_idx], target_scaled[rand_idx], problem_type, verbose=verbose-1)
+        rand_idx = np.random.permutation(df_scaled.index)[: max(10, int(0.85 * len(df_scaled)))]
+        return _select_features_1run(df_scaled.iloc[rand_idx], target_scaled[rand_idx], problem_type, verbose=verbose - 1)
 
     if featsel_runs >= 1 and problem_type in ("regression", "classification"):
         if n_jobs == 1 or featsel_runs == 1:
             # only use parallelization code if you actually parallelize
             selected_columns = []
             for i in range(featsel_runs):
                 selected_columns.extend(run_select_features(i))
         else:
-            def flatten_lists(l):
+
+            def flatten_lists(l: list):
                 return [item for sublist in l for item in sublist]
 
-            selected_columns = flatten_lists(Parallel(n_jobs=n_jobs, verbose=100*verbose)(delayed(run_select_features)(i) for i in range(featsel_runs)))
+            selected_columns = flatten_lists(
+                Parallel(n_jobs=n_jobs, verbose=100 * verbose)(delayed(run_select_features)(i) for i in range(featsel_runs))
+            )
 
         if selected_columns:
             selected_columns = Counter(selected_columns)
             # sort by frequency, but down weight longer formulas to break ties
-            selected_columns = sorted(selected_columns, key=lambda x: selected_columns[x] - 0.000001*len(str(x)), reverse=True)
+            selected_columns = sorted(
+                selected_columns, key=lambda x: selected_columns[x] - 0.000001 * len(str(x)), reverse=True
+            )
             if verbose > 0:
-                print("[featsel] %i features after %i feature selection runs" % (len(selected_columns), featsel_runs))
+                print(f"[featsel] {len(selected_columns)} features after {featsel_runs} feature selection runs")
             # correlation filtering
             selected_columns = keep + [c for c in selected_columns if c not in keep]
             if not keep:
                 good_cols = [selected_columns[0]]
                 k = 1
             else:
                 good_cols = keep
@@ -249,39 +263,38 @@
             if len(selected_columns) > k:
                 correlations = df_scaled[selected_columns].corr()
                 for i, c in enumerate(selected_columns[k:], k):
                     # only take features that are somewhat uncorrelated with the rest
                     if np.max(np.abs(correlations[c].ravel()[:i])) < 0.9:
                         good_cols.append(c)
             if verbose > 0:
-                print("[featsel] %i features after correlation filtering" % len(good_cols))
+                print(f"[featsel] {len(good_cols)} features after correlation filtering")
 
     # perform noise filtering on these features
     good_cols = _noise_filtering(df_scaled[good_cols].to_numpy(), target_scaled, good_cols, problem_type)
     if verbose > 0:
-        print("[featsel] %i features after noise filtering" % len(good_cols))
+        print(f"[featsel] {len(good_cols)} features after noise filtering")
         if not good_cols:
             print("[featsel] WARNING: Not a single good features was found...")
 
     # add keep columns back in
     good_cols = keep + [c for c in good_cols if c not in keep]
     if verbose > 0 and keep:
-        print("[featsel] %i final features selected (including %i original keep features)." % (len(good_cols), len(keep)))
+        print(f"[featsel] {len(good_cols)} final features selected (including {len(keep)} original keep features).")
     return good_cols
 
 
 class FeatureSelector(BaseEstimator):
-
     def __init__(
         self,
-        problem_type="regression",
-        featsel_runs=5,
-        keep=None,
-        n_jobs=1,
-        verbose=0,
+        problem_type: str = "regression",
+        featsel_runs: int = 5,
+        keep: list | None = None,
+        n_jobs: int = 1,
+        verbose: int = 0,
     ):
         """
         multi-step cross-validated feature selection
 
         Inputs:
             - problem_type: str, either "regression" or "classification" (default: "regression")
             - featsel_runs: number of times to perform in the feature selection part with a random fraction of data points (int; default: 5)
@@ -297,15 +310,15 @@
         """
         self.problem_type = problem_type
         self.featsel_runs = featsel_runs
         self.keep = keep
         self.n_jobs = n_jobs
         self.verbose = verbose
 
-    def fit(self, X, y):
+    def fit(self, X: np.ndarray | pd.DataFrame, y: np.ndarray | pd.DataFrame):
         """
         Selects features.
 
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
             - y: pandas dataframe or numpy array with targets for all n_datapoints
         """
@@ -313,24 +326,26 @@
         # store column names as they'll be lost in the other check
         # first calling np.array assures that all the column names have the same dtype
         # as otherwise we get problems when calling np.random.permutation on the columns
         cols = list(np.array(list(X.columns))) if isinstance(X, pd.DataFrame) else []
         # check input variables
         X, target = check_X_y(X, y, y_numeric=self.problem_type == "regression")
         if not cols:
-            cols = ["x%i" % i for i in range(X.shape[1])]
+            cols = [f"x{i}" for i in range(X.shape[1])]
         self.original_columns_ = cols
         # transform X into a dataframe (again)
         df = pd.DataFrame(X, columns=cols)
         # do the feature selection
-        self.good_cols_ = select_features(df, target, self.featsel_runs, self.keep, self.problem_type, self.n_jobs, self.verbose)
+        self.good_cols_ = select_features(
+            df, target, self.featsel_runs, self.keep, self.problem_type, self.n_jobs, self.verbose
+        )
         self.n_features_in_ = X.shape[1]
         return self
 
-    def transform(self, X):
+    def transform(self, X: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
         Returns:
             - new_X: new pandas dataframe or numpy array with only the good features
         """
         check_is_fitted(self, ["good_cols_"])
@@ -341,25 +356,25 @@
         # store column names as they'll be lost in the other check
         # first calling np.array assures that all the column names have the same dtype
         # as otherwise we get problems when calling np.random.permutation on the columns
         cols = list(np.array(list(X.columns))) if isinstance(X, pd.DataFrame) else []
         # check input variables
         X = check_array(X, force_all_finite="allow-nan")
         if not cols:
-            cols = ["x%i" % i for i in range(X.shape[1])]
+            cols = [f"x{i}" for i in range(X.shape[1])]
         if not cols == self.original_columns_:
             raise ValueError("[FeatureSelector] Not the same features as when calling fit.")
         # transform X into a dataframe (again) and select columns
         new_X = pd.DataFrame(X, columns=cols)[self.good_cols_]
         # possibly transform into a numpy array
         if not self.return_df_:
             new_X = new_X.to_numpy()
         return new_X
 
-    def fit_transform(self, X, y):
+    def fit_transform(self, X: np.ndarray | pd.DataFrame, y: np.ndarray | pd.DataFrame) -> np.ndarray | pd.DataFrame:
         """
         Selects features and returns only those selected.
 
         Inputs:
             - X: pandas dataframe or numpy array with original features (n_datapoints x n_features)
             - y: pandas dataframe or numpy array with targets for all n_datapoints
         Returns:
```

### Comparing `autofeat-2.0.9/autofeat/nb_utils.py` & `autofeat-2.1.0/autofeat/nb_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# -*- coding: utf-8 -*-
 # Author: Jeethu Rao <jboloor@acm.org>
 # License: MIT
 
 import numba as nb
 import numpy as np
 
 
-@nb.njit(inline='always')
+@nb.njit(inline="always")
 def nb_apply_along_axis(func1d, axis, arr):
     assert arr.ndim == 2
     assert axis in [0, 1]
     if axis == 0:
         result = np.empty(arr.shape[1])
         for i in range(len(result)):
             result[i] = func1d(arr[:, i])
```

### Comparing `autofeat-2.0.9/autofeat.egg-info/PKG-INFO` & `autofeat-2.1.0/autofeat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,91 @@
 Metadata-Version: 2.1
 Name: autofeat
-Version: 2.0.9
+Version: 2.1.0
 Summary: Automatic Feature Engineering and Selection Linear Prediction Model
-Home-page: https://github.com/cod3licious/autofeat
-Author: Franziska Horn
-Author-email: cod3licious@gmail.com
-License: MIT
-Description: # `autofeat` library
-        ### Linear Prediction Models with Automated Feature Engineering and Selection
+Author-email: Franziska Horn <cod3licious@gmail.com>
+License: MIT License
         
-        This library contains the `AutoFeatRegressor` and `AutoFeatClassifier` models with a similar interface as `scikit-learn` models:
-        - `fit()` function to fit the model parameters
-        - `predict()` function to predict the target variable given the input
-        - `score()` function to calculate the goodness of the fit (R^2/accuracy)
-        - `fit_transform()` and `transform()` functions, which extend the given data by the additional features that were engineered and selected by the model
+        Copyright (c) 2016 
         
-        When calling the `fit()` function, internally the `fit_transform()` function will be called, so if you're planing to call `transform()` on the same data anyways, just call `fit_transform()` right away. `transform()` is mostly useful if you've split your data into training and test data and did not call `fit_transform()` on your whole dataset. The `predict()` and `score()` functions can either be given data in the format of the original dataframe that was used when calling `fit()`/`fit_transform()` or they can be given an already transformed dataframe.
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
         
-        In addition, only the feature selection part is also available in the `FeatureSelector` model.
-        
-        Furthermore (as of version 2.0.0), minimal feature selection (removing zero variance and redundant features), engineering (simple product and ratio of features), and scaling (power transform to make features more normally distributed) is also available in the `AutoFeatLight` model.
-        
-        The `AutoFeatRegressor`, `AutoFeatClassifier`, and `FeatureSelector` models need to be **fit on data without NaNs**, as they internally call the sklearn `LassoLarsCV` model, which can not handle NaNs. When calling `transform()`, NaNs (but not `np.inf`) are okay.
-        
-        The [autofeat examples notebook](https://github.com/cod3licious/autofeat/blob/master/autofeat_examples.ipynb) contains a simple usage example - try it out! :) Additional examples can be found in the autofeat benchmark notebooks for [regression](https://github.com/cod3licious/autofeat/blob/master/autofeat_benchmark_regression.ipynb) (which also contains the code to reproduce the results from the paper mentioned below) and [classification](https://github.com/cod3licious/autofeat/blob/master/autofeat_benchmark_classification.ipynb), as well as the testing scripts.
-        
-        Please keep in mind that since the `AutoFeatRegressor` and `AutoFeatClassifier` models can generate very complex features, they might **overfit on noise** in the dataset, i.e., find some new features that lead to good prediction on the training set but result in a poor performance on new test samples. While this usually only happens for datasets with very few samples, we suggest you carefully inspect the features found by `autofeat` and use those that make sense to you to train your own models.
-        
-        Depending on the number of `feateng_steps` (default 2) and the number of input features, `autofeat` can generate a very huge feature matrix (before selecting the most appropriate features from this large feature pool). By specifying in `feateng_cols` those columns that you expect to be most valuable in the feature engineering part, the number of features can be greatly reduced. Additionally, `transformations` can be limited to only those feature transformations that make sense for your data. Last but not least, you can subsample the data used for training the model to limit the memory requirements. After the model was fit, you can call `transform()` on your whole dataset to generate only those few features that were selected during `fit()`/`fit_transform()`.
-        
-        
-        ### Installation
-        You can either download the code from here and include the autofeat folder in your `$PYTHONPATH` or install (the library components only) via pip:
-        
-            $ pip install autofeat
-        
-        The library requires Python 3! Other dependencies: `numpy`, `pandas`, `scikit-learn`, `sympy`, `joblib`, `pint` and `numba`.
-        
-        
-        ### Paper
-        For further details on the model and implementation please refer to the [paper](https://arxiv.org/abs/1901.07329)  - and of course if any of this code was helpful for your research, please consider citing it:
-        ```
-        @inproceedings{horn2019autofeat,
-          title={The autofeat Python Library for Automated Feature Engineering and Selection},
-          author={Horn, Franziska and Pack, Robert and Rieger, Michael},
-          booktitle={Joint European Conference on Machine Learning and Knowledge Discovery in Databases},
-          pages={111--120},
-          year={2019},
-          organization={Springer}
-        }
-        ```
-        
-        If you don't like reading, you can also watch a video of my [talk at the PyData conference](https://www.youtube.com/watch?v=4-4pKPv9lJ4) about automated feature engineering and selection with `autofeat`.
-        
-        The code is intended for research purposes.
-        
-        If you have any questions please don't hesitate to send me an [email](mailto:cod3licious@gmail.com) and of course if you should find any bugs or want to contribute other improvements, pull requests are very welcome!
-        
-        ### Acknowledgments
-        
-        This project was made possible thanks to support by [BASF](https://www.basf.com).
-        
-Keywords: automl feature engineering feature selection linear model
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Project-URL: Homepage, https://github.com/cod3licious/autofeat
+Keywords: automl,feature engineering,feature selection,linear model
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# `autofeat` library
+### Linear Prediction Models with Automated Feature Engineering and Selection
+
+This library contains the `AutoFeatRegressor` and `AutoFeatClassifier` models with a similar interface as `scikit-learn` models:
+- `fit()` function to fit the model parameters
+- `predict()` function to predict the target variable given the input
+- `predict_proba()` function to predict probabilities of the target variable given the input (classifier only)
+- `score()` function to calculate the goodness of the fit (R^2/accuracy)
+- `fit_transform()` and `transform()` functions, which extend the given data by the additional features that were engineered and selected by the model
+
+When calling the `fit()` function, internally the `fit_transform()` function will be called, so if you're planing to call `transform()` on the same data anyways, just call `fit_transform()` right away. `transform()` is mostly useful if you've split your data into training and test data and did not call `fit_transform()` on your whole dataset. The `predict()` and `score()` functions can either be given data in the format of the original dataframe that was used when calling `fit()`/`fit_transform()` or they can be given an already transformed dataframe.
+
+In addition, only the feature selection part is also available in the `FeatureSelector` model.
+
+Furthermore (as of version 2.0.0), minimal feature selection (removing zero variance and redundant features), engineering (simple product and ratio of features), and scaling (power transform to make features more normally distributed) is also available in the `AutoFeatLight` model.
+
+The `AutoFeatRegressor`, `AutoFeatClassifier`, and `FeatureSelector` models need to be **fit on data without NaNs**, as they internally call the sklearn `LassoLarsCV` model, which can not handle NaNs. When calling `transform()`, NaNs (but not `np.inf`) are okay.
+
+The [autofeat examples notebook](https://github.com/cod3licious/autofeat/blob/master/autofeat_examples.ipynb) contains a simple usage example - try it out! :) Additional examples can be found in the autofeat benchmark notebooks for [regression](https://github.com/cod3licious/autofeat/blob/master/autofeat_benchmark_regression.ipynb) (which also contains the code to reproduce the results from the paper mentioned below) and [classification](https://github.com/cod3licious/autofeat/blob/master/autofeat_benchmark_classification.ipynb), as well as the testing scripts.
+
+Please keep in mind that since the `AutoFeatRegressor` and `AutoFeatClassifier` models can generate very complex features, they might **overfit on noise** in the dataset, i.e., find some new features that lead to good prediction on the training set but result in a poor performance on new test samples. While this usually only happens for datasets with very few samples, we suggest you carefully inspect the features found by `autofeat` and use those that make sense to you to train your own models.
+
+Depending on the number of `feateng_steps` (default 2) and the number of input features, `autofeat` can generate a very huge feature matrix (before selecting the most appropriate features from this large feature pool). By specifying in `feateng_cols` those columns that you expect to be most valuable in the feature engineering part, the number of features can be greatly reduced. Additionally, `transformations` can be limited to only those feature transformations that make sense for your data. Last but not least, you can subsample the data used for training the model to limit the memory requirements. After the model was fit, you can call `transform()` on your whole dataset to generate only those few features that were selected during `fit()`/`fit_transform()`.
+
+
+### Installation
+You can either download the code from here and include the autofeat folder in your `$PYTHONPATH` or install (the library components only) via pip:
+
+    $ pip install autofeat
+
+The library requires Python 3! Other dependencies: `numpy`, `pandas`, `scikit-learn`, `sympy`, `joblib`, `pint` and `numba`.
+
+
+### Paper
+For further details on the model and implementation please refer to the [paper](https://arxiv.org/abs/1901.07329)  - and of course if any of this code was helpful for your research, please consider citing it:
+```
+@inproceedings{horn2019autofeat,
+  title={The autofeat Python Library for Automated Feature Engineering and Selection},
+  author={Horn, Franziska and Pack, Robert and Rieger, Michael},
+  booktitle={Joint European Conference on Machine Learning and Knowledge Discovery in Databases},
+  pages={111--120},
+  year={2019},
+  organization={Springer}
+}
+```
+
+If you don't like reading, you can also watch a video of my [talk at the PyData conference](https://www.youtube.com/watch?v=4-4pKPv9lJ4) about automated feature engineering and selection with `autofeat`.
+
+The code is intended for research purposes.
+
+If you have any questions please don't hesitate to send me an [email](mailto:cod3licious@gmail.com) and of course if you should find any bugs or want to contribute other improvements, pull requests are very welcome!
+
+### Acknowledgments
+
+This project was made possible thanks to support by [BASF](https://www.basf.com).
```

