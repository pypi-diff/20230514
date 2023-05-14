# Comparing `tmp/AutoCarver-4.0.0.tar.gz` & `tmp/AutoCarver-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AutoCarver-4.0.0.tar", last modified: Wed Apr 12 09:41:05 2023, max compression
+gzip compressed data, was "dist\AutoCarver-4.0.1.tar", last modified: Sun May 14 14:17:14 2023, max compression
```

## Comparing `AutoCarver-4.0.0.tar` & `AutoCarver-4.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/AutoCarver/
--rw-rw-rw-   0        0        0    22755 2023-04-12 09:39:04.000000 AutoCarver-4.0.0/AutoCarver/AutoCarver.py
--rw-rw-rw-   0        0        0    50557 2023-04-11 15:29:18.000000 AutoCarver-4.0.0/AutoCarver/Discretizers.py
--rw-rw-rw-   0        0        0    14207 2023-01-28 13:57:43.000000 AutoCarver-4.0.0/AutoCarver/FeatureSelector.py
--rw-rw-rw-   0        0        0        0 2023-01-09 19:45:37.000000 AutoCarver-4.0.0/AutoCarver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/AutoCarver.egg-info/
--rw-rw-rw-   0        0        0     7905 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/AutoCarver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/AutoCarver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/AutoCarver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/AutoCarver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7905 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6003 2023-01-24 08:07:41.000000 AutoCarver-4.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 09:41:05.000000 AutoCarver-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-04-12 09:39:21.000000 AutoCarver-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/AutoCarver/
+-rw-rw-rw-   0        0        0    22800 2023-05-14 14:15:32.000000 AutoCarver-4.0.1/AutoCarver/AutoCarver.py
+-rw-rw-rw-   0        0        0    50746 2023-05-14 14:15:32.000000 AutoCarver-4.0.1/AutoCarver/Discretizers.py
+-rw-rw-rw-   0        0        0    14207 2023-01-28 13:57:43.000000 AutoCarver-4.0.1/AutoCarver/FeatureSelector.py
+-rw-rw-rw-   0        0        0        0 2023-01-09 19:45:37.000000 AutoCarver-4.0.1/AutoCarver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/AutoCarver.egg-info/
+-rw-rw-rw-   0        0        0     8312 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/AutoCarver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/AutoCarver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/AutoCarver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/AutoCarver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8312 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6346 2023-04-12 10:19:04.000000 AutoCarver-4.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-14 14:17:14.000000 AutoCarver-4.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-05-14 14:15:44.000000 AutoCarver-4.0.1/setup.py
```

### Comparing `AutoCarver-4.0.0/AutoCarver/AutoCarver.py` & `AutoCarver-4.0.1/AutoCarver/AutoCarver.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from matplotlib.ticker import PercentFormatter
 from numpy import sort, nan, inf, float32, where, isin, argsort, array, append, quantile, linspace, argmin, sqrt, random
 from pandas import DataFrame, Series, isna, qcut, notna, unique, concat, crosstab
 from pandas.api.types import is_string_dtype
 from scipy.stats import chi2_contingency
 from seaborn import color_palette, despine
 from tqdm.notebook import tqdm
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Tuple
 
 
 class AutoCarver(GroupedListDiscretizer):
     """ Automatic carving of continuous, categorical and categorical ordinal features 
     that maximizes association with a binary target.
 
     Modalities/values of features are carved/regrouped according to a computed specific
@@ -109,15 +109,15 @@
         implemented = ['tschuprowt', 'cramerv']
         assert sort_by in implemented, f"Measure {sort_by} is not yet implemented. Choose from: {', '.join(implemented)}."
         self.sort_by = sort_by
 
         self.copy = copy
         self.verbose = verbose
     
-    def prepare_data(self, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> tuple:
+    def prepare_data(self, X: DataFrame, y: Series, X_test: DataFrame=None, y_test: Series=None) -> Tuple[DataFrame, Series, DataFrame, Series]:
         """ Checks validity of provided data"""
         
         # preparing train sample
         # checking for binary target
         y_values = unique(y)
         assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
         assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
@@ -228,15 +228,15 @@
 
         # printing the new group statistics
         if self.verbose and best_groups:
             self.display_xtabs(feature, 'Fitted', xtab, xtab_test)
 
         return best_groups
 
-    def update_order(self, feature: str, best_groups: GroupedList, xtab: DataFrame, xtab_test: DataFrame=None) -> tuple[DataFrame, DataFrame]:
+    def update_order(self, feature: str, best_groups: GroupedList, xtab: DataFrame, xtab_test: DataFrame=None) -> Tuple[DataFrame, DataFrame]:
         """ Updates the values_orders and xtabs according to the best_groups"""
 
         # accessing current order for specified feature
         order = self.values_orders.get(feature)
 
         # grouping for each group of the combination
         for kept, discarded in best_groups.contained.items():
```

### Comparing `AutoCarver-4.0.0/AutoCarver/Discretizers.py` & `AutoCarver-4.0.1/AutoCarver/Discretizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,45 +500,49 @@
         self.copy = copy
         self.verbose = verbose
         self.dropna = dropna
 
     def fit(self, X: DataFrame, y: Series) -> None:
 
         # [Qualitative features] Grouping qualitative features
-        # verbose if requested
-        if self.verbose:
-            print("\n---\n[Discretizer] Fit Qualitative Features")
+        if len(self.quali_features) > 0:
 
-        # grouping qualitative features
-        discretizer = QualitativeDiscretizer(
-            self.quali_features, min_freq=self.min_freq,
-            values_orders=self.values_orders, copy=self.copy,
-            verbose=self.verbose, dropna=self.dropna
-        )
-        discretizer.fit(X, y)
-
-        # storing results
-        self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
-        self.pipe += discretizer.pipe  # adding discretizer to pipe
+            # verbose if requested
+            if self.verbose:
+                print("\n---\n[Discretizer] Fit Qualitative Features")
+
+            # grouping qualitative features
+            discretizer = QualitativeDiscretizer(
+                self.quali_features, min_freq=self.min_freq,
+                values_orders=self.values_orders, copy=self.copy,
+                verbose=self.verbose, dropna=self.dropna
+            )
+            discretizer.fit(X, y)
+
+            # storing results
+            self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
+            self.pipe += discretizer.pipe  # adding discretizer to pipe
 
         # [Quantitative features] Grouping quantitative features
-        # verbose if requested
-        if self.verbose:
-            print("\n---\n[Discretizer] Fit Quantitative Features")
+        if len(self.quanti_features) > 0:
 
-        # grouping quantitative features
-        discretizer = QuantitativeDiscretizer(
-            self.quanti_features, q=self.q, copy=self.copy,
-            verbose=self.verbose, dropna=self.dropna
-        )
-        discretizer.fit(X, y)
-
-        # storing results
-        self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
-        self.pipe += discretizer.pipe  # adding discretizer to pipe
+            # verbose if requested
+            if self.verbose:
+                print("\n---\n[Discretizer] Fit Quantitative Features")
+
+            # grouping quantitative features
+            discretizer = QuantitativeDiscretizer(
+                self.quanti_features, q=self.q, copy=self.copy,
+                verbose=self.verbose, dropna=self.dropna
+            )
+            discretizer.fit(X, y)
+
+            # storing results
+            self.values_orders.update(discretizer.values_orders)  # adding orders of grouped features
+            self.pipe += discretizer.pipe  # adding discretizer to pipe
 
         return self
 
     def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
 
         # verbose if requested
         if self.verbose:
```

### Comparing `AutoCarver-4.0.0/AutoCarver/FeatureSelector.py` & `AutoCarver-4.0.1/AutoCarver/FeatureSelector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.0.0/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-4.0.1/AutoCarver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.0.0
+Version: 4.0.1
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
-Description: # AutoCarver
+Description: </p>
+        <p align="center">
+            <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
+            <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
+            <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
+        </p>
+        
+        
+        # AutoCarver
         
         **AutoCarver** is an approach for maximising a qualitative feature's association with a binary target feature while reducing it's number of distinct modalities.
         Can also be used to discretize quantitative features, that are prealably cut in quantiles.
         
          Modalities/values of features are carved/regrouped according to a computed specific order defined based on their types:
           - *Qualitative features* grouped based on target rate per modality.
           - *Qualitative ordinal features* grouped based on specified modality order.
```

### Comparing `AutoCarver-4.0.0/PKG-INFO` & `AutoCarver-4.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.0.0
+Version: 4.0.1
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
-Description: # AutoCarver
+Description: </p>
+        <p align="center">
+            <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
+            <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
+            <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
+        </p>
+        
+        
+        # AutoCarver
         
         **AutoCarver** is an approach for maximising a qualitative feature's association with a binary target feature while reducing it's number of distinct modalities.
         Can also be used to discretize quantitative features, that are prealably cut in quantiles.
         
          Modalities/values of features are carved/regrouped according to a computed specific order defined based on their types:
           - *Qualitative features* grouped based on target rate per modality.
           - *Qualitative ordinal features* grouped based on specified modality order.
```

### Comparing `AutoCarver-4.0.0/README.md` & `AutoCarver-4.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+</p>
+<p align="center">
+    <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
+    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
+    <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
+</p>
+
+
 # AutoCarver
 
 **AutoCarver** is an approach for maximising a qualitative feature's association with a binary target feature while reducing it's number of distinct modalities.
 Can also be used to discretize quantitative features, that are prealably cut in quantiles.
 
  Modalities/values of features are carved/regrouped according to a computed specific order defined based on their types:
   - *Qualitative features* grouped based on target rate per modality.
```

### Comparing `AutoCarver-4.0.0/setup.py` & `AutoCarver-4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='AutoCarver',
-    version='4.0.0',
+    version='4.0.1',
     author='Mario DEFRANCE',
     author_email='defrancemario@gmail.com',
     description='Automatic Bucketizing of Features with Optimal Association',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mdefrance/AutoCarver',
     project_urls = {
```

