# Comparing `tmp/litelearn-0.2.8.tar.gz` & `tmp/litelearn-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litelearn-0.2.8.tar", max compression
+gzip compressed data, was "litelearn-0.3.0.tar", max compression
```

## Comparing `litelearn-0.2.8.tar` & `litelearn-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1091 2022-11-28 18:23:59.090865 litelearn-0.2.8/LICENSE
--rw-r--r--   0        0        0      126 2022-11-28 19:43:06.686021 litelearn-0.2.8/litelearn/__init__.py
--rw-r--r--   0        0        0     3653 2023-03-03 07:54:59.350685 litelearn-0.2.8/litelearn/api.py
--rw-r--r--   0        0        0     4732 2023-03-03 08:17:52.602143 litelearn-0.2.8/litelearn/expo_ds.py
--rw-r--r--   0        0        0    17344 2023-03-03 08:17:52.603054 litelearn-0.2.8/litelearn/model_frame.py
--rw-r--r--   0        0        0     2974 2022-11-28 20:45:50.535105 litelearn-0.2.8/litelearn/residuals.py
--rw-r--r--   0        0        0     7752 2023-03-02 12:23:03.836794 litelearn-0.2.8/litelearn/train_frame.py
--rw-r--r--   0        0        0      667 2023-03-03 08:17:52.603054 litelearn-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      582 2022-11-28 20:38:15.141263 litelearn-0.2.8/README.md
--rw-r--r--   0        0        0     1394 1970-01-01 00:00:00.000000 litelearn-0.2.8/setup.py
--rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 litelearn-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1092 2022-12-19 12:19:13.133022 litelearn-0.3.0/LICENSE
+-rw-r--r--   0        0        0      177 2023-05-14 07:56:14.960576 litelearn-0.3.0/litelearn/__init__.py
+-rw-r--r--   0        0        0     3738 2023-05-14 09:47:41.895478 litelearn-0.3.0/litelearn/api.py
+-rw-r--r--   0        0        0      104 2023-05-14 07:54:49.440856 litelearn-0.3.0/litelearn/exceptions.py
+-rw-r--r--   0        0        0     5151 2023-05-14 10:23:44.478974 litelearn-0.3.0/litelearn/expo_ds.py
+-rw-r--r--   0        0        0    20411 2023-05-14 11:07:04.823111 litelearn-0.3.0/litelearn/model_frame.py
+-rw-r--r--   0        0        0     2974 2022-12-19 12:19:13.136021 litelearn-0.3.0/litelearn/residuals.py
+-rw-r--r--   0        0        0     7754 2023-05-14 07:54:49.487841 litelearn-0.3.0/litelearn/train_frame.py
+-rw-r--r--   0        0        0      692 2023-05-14 14:24:06.998863 litelearn-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2683 2023-05-14 14:05:38.363170 litelearn-0.3.0/README.md
+-rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 litelearn-0.3.0/PKG-INFO
```

### Comparing `litelearn-0.2.8/LICENSE` & `litelearn-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `litelearn-0.2.8/litelearn/api.py` & `litelearn-0.3.0/litelearn/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import catboost
 import numpy as np
 
-from litelearn import TrainFrame, ModelFrame
+from litelearn.train_frame import TrainFrame
+from litelearn.model_frame import ModelFrame
+from litelearn.exceptions import TrainingException
 
 
-def core_regress_df(
+def regress_df(
     df,
     target,
     train_index=None,
     lr=None,
     iterations=None,
     test_size=None,
     sample_weights=None,
@@ -29,15 +31,15 @@
     )
     if drop_columns:
         train_frame = train_frame.drop_columns(drop_columns)
 
     y = df[target]
 
     if not np.issubdtype(y.dtype, np.number):
-        raise Exception(
+        raise TrainingException(
             f'unable to use "{target}" as regression target since it is not numerical'
         )
 
     result = train_frame.fit(
         learning_rate=lr,
         iterations=iterations,
         fit_kwargs=fit_kwargs,
@@ -47,15 +49,15 @@
     print(f"benchmark_stdev  {y.std():.4f}")
     result.display_evaluation()
     result.display_feature_importance()
 
     return result
 
 
-def core_classify_df(
+def classify_df(
     df,
     target,
     train_index=None,
     lr=None,
     iterations=None,
     test_size=None,
     sample_weights=None,
@@ -129,8 +131,8 @@
         train_frame=train_frame,
     )
     # result.eval_pool = eval_pool  # HACK!
 
     # result.display_evaluation()
     result.display_feature_importance()
 
-    return result, eval_pool
+    return result
```

### Comparing `litelearn-0.2.8/litelearn/expo_ds.py` & `litelearn-0.3.0/litelearn/expo_ds.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 import pandas as pd
 import shap
 
 
 # For validation
 from sklearn.model_selection import train_test_split as split
 
+from litelearn.exceptions import *
+
 # logging.basicConfig(level=logging.DEBUG)
 logging.basicConfig()
 shap.initjs()
 
 UNKNOWN_CATEGORY_VALUE = "LITELEARN_UNKNOWN"
+NA_CATEGORY_VALUE = "LITELEARN_NA_VALUE"
 
 
 def print_version(lib):
     print(lib.__name__, lib.__version__)
 
 
 def default_value(value, default, marker=None):
@@ -48,15 +51,15 @@
 
 
 def xy_df(df, target, train_index=None):
     X = df.copy().drop(columns=target)
     y = df[target]
 
     if y.isna().sum():
-        raise Exception(
+        raise TrainingException(
             f'unable to use "{target}" as target column since it contains null values'
         )
 
     return X, y
 
 
 ## why is this needed?
@@ -131,22 +134,30 @@
 ):
     use_categories = default_value(use_categories, True)
     # use_nulls=True will use the native null handling of catboost
     # use_nulls=False will fillna and add _is_missing columns
     use_nulls = default_value(use_nulls, True)  # TODO: fix issues for use_nulls=False
 
     X, y = xy_df(df=df, train_index=train_index, target=target)
+    if y.dtype.name in ['string', 'object']:
+        y = y.astype('category')
 
     cat_cols = X.select_dtypes(exclude=["number", "bool", "datetime"]).columns
 
     # allow using catboost null handling capability
     if not use_nulls:
         X = fill_nulls_naively(X)
     else:
-        X[cat_cols] = X[cat_cols].fillna("LITELEARN_NA_VALUE").astype("string")
+        # add NA_CATEGORY_VALUE to categorical columns
+        for col in cat_cols:
+            if X[col].dtype.name == "category":
+                X[col].cat.add_categories(NA_CATEGORY_VALUE, inplace=True)
+
+        # fillna with NA_CATEGORY_VALUE
+        X[cat_cols] = X[cat_cols].fillna(NA_CATEGORY_VALUE).astype("string")
 
     for col in cat_cols:
         if not use_categories:
             print(f"casting {col} onto category codes")
             X[col] = X[col].astype("category").cat.codes
         else:
             print(f"casting {col} onto category")
```

### Comparing `litelearn-0.2.8/litelearn/model_frame.py` & `litelearn-0.3.0/litelearn/model_frame.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Union, Callable, Optional, List
+import pickle
 
 import catboost
 import litelearn
 import pandas as pd
 import seaborn as sns
 import shap
 
@@ -13,21 +14,22 @@
 try:
     from IPython.core.display_functions import display
 except ImportError:
     from IPython.display import display
 
 from pandas.core.dtypes.common import is_numeric_dtype
 from sklearn.inspection import permutation_importance
-from sklearn.metrics import mean_squared_error as mse
+from sklearn.metrics import mean_squared_error as mse, classification_report
 
 # from litelearn import TrainFrame
 from litelearn.expo_ds import (
     default_value,
     display_evaluation_comparison,
     UNKNOWN_CATEGORY_VALUE,
+    NA_CATEGORY_VALUE
 )
 from . import residuals
 
 
 @dataclass
 class ModelFrame:
     """
@@ -224,14 +226,45 @@
                 result.loc[y.index, "sq_error"] = (y - y_pred) ** 2
             else:
                 result.loc[y.index, "error"] = y != y_pred
 
         return result
 
     def get_evaluation(self):
+        if self.train_frame.y_train.dtype.name in ["category", 'string', 'object']:
+            return self._get_classification_evaluation()
+        else:
+            return self._get_regression_evaluation()
+
+    def _get_classification_evaluation(self):
+        evaluation = pd.DataFrame()
+        for stage in ["train", "test"]:
+            X, y = self.train_frame.get_stage_data(stage)
+            if len(X) <= 0:
+                continue
+
+            assert list(self.model.classes_) == list(self.train_frame.y_train.cat.categories)
+            y_pred = self.model.predict(X)
+            # https://stackoverflow.com/a/53780589/52917
+            report = classification_report(
+                y,
+                y_pred,
+                target_names=self.model.classes_,
+                output_dict=True
+            )
+            report.update({"accuracy": {"precision": None, "recall": None, "f1-score": report["accuracy"],
+                                        "support": report['macro avg']['support']}})
+            report = pd.DataFrame(report).transpose()
+            # https://stackoverflow.com/a/40225891/52917
+            report = pd.concat([report], axis=1, keys=[stage])
+            evaluation = pd.concat([evaluation, report], axis=1).round(3)
+
+        return evaluation
+
+    def _get_regression_evaluation(self):
         evaluation = pd.DataFrame()
         for stage in ["train", "test"]:
             X, y = self.train_frame.get_stage_data(stage)
             if len(X) <= 0:
                 continue
 
             y_pred = self.model.predict(X)
@@ -443,18 +476,23 @@
         for col in model_columns:
             src_dtype = df2[col].dtype
             dst_dtype = X_train[col].dtype
             if src_dtype != dst_dtype:
                 src_col = df2[col]
                 if dst_dtype.name == "category":
                     unknown_values = set(df[col]) - set(X_train[col].cat.categories)
-                    src_col = src_col.replace(
+                    src_col = src_col.astype('string').replace(
                         to_replace=unknown_values, value=UNKNOWN_CATEGORY_VALUE
                     )
 
+                    # fillna for categories - catboost can't handle NaNs for categorical cols
+                    if src_col.isna().any():
+                        print('fillna for', col)
+                        src_col = src_col.astype('string').fillna(NA_CATEGORY_VALUE)
+
                 print("recasting", col, "from", src_dtype, "to", dst_dtype)
                 df2[col] = src_col.astype(dst_dtype)
 
         # print(df2.columns.to_list())
         return df2
 
     def predict(self, df, drop_unused=True):
@@ -468,7 +506,43 @@
 
     def predict_proba(self, df, drop_unused=True):
         return pd.DataFrame(
             self.model.predict_proba(self.predict_prepare(df, drop_unused=drop_unused)),
             columns=list(self.model.classes_),
             index=df.index,
         )
+
+    def dump(self, filename=None):
+        """
+        Save the model to a file or to a string
+        :param filename: if specified, the model is saved to the file, otherwise it is returned as a string
+        :return: the model as a string if filename is None, otherwise None
+        """
+        if filename is None:
+            return pickle.dumps(self)
+        else:
+            with open(filename, "wb") as f:
+                pickle.dump(self, f)
+
+
+    @staticmethod
+    def load(filename=None, data=None):
+        """
+        Load the model from a file or from a string
+
+        :param filename: if specified, the model is loaded from the file, otherwise it is loaded from the string
+        :param data: if specified, the model is loaded from the string, otherwise it is loaded from the file
+        :return: the loaded model
+        """
+        if not filename and not data:
+            raise ValueError('Either filename or data must be specified')
+        if filename and data:
+            raise ValueError('Only one of filename or data must be specified')
+        result = None
+        if filename:
+            with open(filename, "rb") as f:
+                result = pickle.load(f)
+        else:
+            result = pickle.loads(data)
+        assert isinstance(result, Model)
+        return result
+
```

### Comparing `litelearn-0.2.8/litelearn/residuals.py` & `litelearn-0.3.0/litelearn/residuals.py`

 * *Files identical despite different names*

### Comparing `litelearn-0.2.8/litelearn/train_frame.py` & `litelearn-0.3.0/litelearn/train_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import catboost
 import pandas as pd
 
 from litelearn import ModelFrame
 from litelearn.expo_ds import cleanup_df, xy_split, default_value, _is_interactive
 
 
+
 @dataclass
 class TrainFrame:
     """
     holds all the information needed to train a model
     """
 
     X_train: pd.DataFrame
```

### Comparing `litelearn-0.2.8/pyproject.toml` & `litelearn-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "litelearn"
-version = "0.2.8"
+version = "0.3.0"
 description = "a python library for quickly building and evaluating models"
 authors = ["Aviad Rozenhek <aviadr1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^1.3.5"
 llvmlite = "^0.39.1" # needed because of issues in version 0.34
 numba = "^0.56" # needed because of issues in version 0.47
-catboost = "^1.1.1"
+catboost = {extras = ["widget"], version = "^1.2"}
 shap = "^0.41.0"
 seaborn = "^0.11.2"
 scikit-learn = "^1.0.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
-jupyterlab = "^3.5.0"
-ipywidgets = "^8.0.2"
+
+[tool.poetry.group.dev.dependencies]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

