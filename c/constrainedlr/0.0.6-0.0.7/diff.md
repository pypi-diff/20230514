# Comparing `tmp/constrainedlr-0.0.6.tar.gz` & `tmp/constrainedlr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constrainedlr-0.0.6.tar", last modified: Sun May 14 19:45:50 2023, max compression
+gzip compressed data, was "constrainedlr-0.0.7.tar", last modified: Sun May 14 20:45:44 2023, max compression
```

## Comparing `constrainedlr-0.0.6.tar` & `constrainedlr-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 19:45:50.966699 constrainedlr-0.0.6/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 constrainedlr-0.0.6/LICENCE
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2009 2023-05-14 19:45:50.958703 constrainedlr-0.0.6/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1020 2023-05-14 13:41:44.000000 constrainedlr-0.0.6/README.md
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1304 2023-05-14 19:45:36.000000 constrainedlr-0.0.6/pyproject.toml
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-14 19:45:50.968699 constrainedlr-0.0.6/setup.cfg
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 19:45:50.358522 constrainedlr-0.0.6/src/
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 19:45:50.602700 constrainedlr-0.0.6/src/constrainedlr/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       61 2023-05-14 19:35:04.000000 constrainedlr-0.0.6/src/constrainedlr/__init__.py
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3485 2023-05-13 17:36:33.000000 constrainedlr-0.0.6/src/constrainedlr/model.py
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 19:45:50.856700 constrainedlr-0.0.6/src/constrainedlr.egg-info/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2009 2023-05-14 19:45:50.000000 constrainedlr-0.0.6/src/constrainedlr.egg-info/PKG-INFO
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      311 2023-05-14 19:45:50.000000 constrainedlr-0.0.6/src/constrainedlr.egg-info/SOURCES.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-14 19:45:50.000000 constrainedlr-0.0.6/src/constrainedlr.egg-info/dependency_links.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       48 2023-05-14 19:45:50.000000 constrainedlr-0.0.6/src/constrainedlr.egg-info/requires.txt
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       14 2023-05-14 19:45:50.000000 constrainedlr-0.0.6/src/constrainedlr.egg-info/top_level.txt
-drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 19:45:50.909699 constrainedlr-0.0.6/tests/
--rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2761 2023-05-14 19:35:02.000000 constrainedlr-0.0.6/tests/test_fit.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 20:45:44.530480 constrainedlr-0.0.7/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1089 2023-04-29 16:41:09.000000 constrainedlr-0.0.7/LICENCE
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2156 2023-05-14 20:45:44.524474 constrainedlr-0.0.7/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1167 2023-05-14 20:43:16.000000 constrainedlr-0.0.7/README.md
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     1304 2023-05-14 20:44:03.000000 constrainedlr-0.0.7/pyproject.toml
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       38 2023-05-14 20:45:44.533475 constrainedlr-0.0.7/setup.cfg
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 20:45:43.912477 constrainedlr-0.0.7/src/
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 20:45:44.131481 constrainedlr-0.0.7/src/constrainedlr/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       61 2023-05-14 19:35:04.000000 constrainedlr-0.0.7/src/constrainedlr/__init__.py
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3560 2023-05-14 20:17:25.000000 constrainedlr-0.0.7/src/constrainedlr/model.py
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 20:45:44.408478 constrainedlr-0.0.7/src/constrainedlr.egg-info/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     2156 2023-05-14 20:45:43.000000 constrainedlr-0.0.7/src/constrainedlr.egg-info/PKG-INFO
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)      311 2023-05-14 20:45:43.000000 constrainedlr-0.0.7/src/constrainedlr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        1 2023-05-14 20:45:43.000000 constrainedlr-0.0.7/src/constrainedlr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       48 2023-05-14 20:45:43.000000 constrainedlr-0.0.7/src/constrainedlr.egg-info/requires.txt
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)       14 2023-05-14 20:45:43.000000 constrainedlr-0.0.7/src/constrainedlr.egg-info/top_level.txt
+drwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)        0 2023-05-14 20:45:44.461486 constrainedlr-0.0.7/tests/
+-rwxrwxrwx   0 tsitsimis  (1000) tsitsimis  (1000)     3083 2023-05-14 20:41:10.000000 constrainedlr-0.0.7/tests/test_fit.py
```

### Comparing `constrainedlr-0.0.6/LICENCE` & `constrainedlr-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `constrainedlr-0.0.6/PKG-INFO` & `constrainedlr-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -38,17 +38,19 @@
 
 ### Example Usage
 ```python
 from constrained_lr import ConstrainedLinearRegression
 from sklearn.metrics import mean_squared_error
 
 model = ConstrainedLinearRegression()
-model.fit(X_train, y_train)
+model.fit(X_train, y_train, features_sign_constraints={"s3": 1, "s4": -1})
 
 y_pred = model.predict(X_test)
 print(mean_squared_error(y_test, y_pred))
-
+print(dict(zip(X.columns, model.coef_)))
 ```
 
+See full example in the [notebook](./notebooks/demo.ipynb)
+
 
 ### Licence
 MIT
```

### Comparing `constrainedlr-0.0.6/README.md` & `constrainedlr-0.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 
 ### Example Usage
 ```python
 from constrained_lr import ConstrainedLinearRegression
 from sklearn.metrics import mean_squared_error
 
 model = ConstrainedLinearRegression()
-model.fit(X_train, y_train)
+model.fit(X_train, y_train, features_sign_constraints={"s3": 1, "s4": -1})
 
 y_pred = model.predict(X_test)
 print(mean_squared_error(y_test, y_pred))
-
+print(dict(zip(X.columns, model.coef_)))
 ```
 
+See full example in the [notebook](./notebooks/demo.ipynb)
+
 
 ### Licence
 MIT
```

### Comparing `constrainedlr-0.0.6/pyproject.toml` & `constrainedlr-0.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'constrainedlr'
-version = '0.0.6'
+version = '0.0.7'
 description = 'Constrained Linear Regression with sklearn-compatible API'
 readme = 'README.md'
 authors = [
   { name = 'Theodore Tsitsimis', email='th.tsitsimis@gmail.com' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.8'
```

### Comparing `constrainedlr-0.0.6/src/constrainedlr/model.py` & `constrainedlr-0.0.7/src/constrainedlr/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import numpy as np
 import pandas as pd
 from cvxopt import matrix, solvers
 from sklearn.base import BaseEstimator, RegressorMixin
 
 
 class ConstrainedLinearRegression(BaseEstimator, RegressorMixin):
-    def __init__(self, fit_intercept: bool = True):
+    def __init__(self, fit_intercept: bool = True, alpha: float = 0.0):
         self.fit_intercept = fit_intercept
         self.coef_ = None
         self.intercept_ = None
+        self.alpha = alpha
 
     def fit(
         self,
         X: pd.DataFrame,
         y: np.ndarray,
         features_sign_constraints: dict = {},
         intercept_sign_constraint: int = 0,
@@ -48,15 +49,15 @@
 
         # Augment features to fit intercept
         if self.fit_intercept:
             X_ = np.hstack([X_, np.ones(n_samples).reshape(-1, 1)])
 
         dim = X_.shape[1]
 
-        P = X_.T.dot(X_)
+        P = X_.T.dot(X_) + self.alpha * np.eye(dim)
         P = matrix(P)
         q = (-y_.T.dot(X_)).T
         q = matrix(q)
 
         features_sign_constraints_full = {feature: 0 for feature in X.columns}
         features_sign_constraints_full.update(features_sign_constraints)
         diag_values = list(features_sign_constraints_full.values())
```

### Comparing `constrainedlr-0.0.6/src/constrainedlr.egg-info/PKG-INFO` & `constrainedlr-0.0.7/src/constrainedlr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constrainedlr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Constrained Linear Regression with sklearn-compatible API
 Author-email: Theodore Tsitsimis <th.tsitsimis@gmail.com>
 Project-URL: Homepage, https://github.com/tsitsimis/constrainedlr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -38,17 +38,19 @@
 
 ### Example Usage
 ```python
 from constrained_lr import ConstrainedLinearRegression
 from sklearn.metrics import mean_squared_error
 
 model = ConstrainedLinearRegression()
-model.fit(X_train, y_train)
+model.fit(X_train, y_train, features_sign_constraints={"s3": 1, "s4": -1})
 
 y_pred = model.predict(X_test)
 print(mean_squared_error(y_test, y_pred))
-
+print(dict(zip(X.columns, model.coef_)))
 ```
 
+See full example in the [notebook](./notebooks/demo.ipynb)
+
 
 ### Licence
 MIT
```

### Comparing `constrainedlr-0.0.6/tests/test_fit.py` & `constrainedlr-0.0.7/tests/test_fit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 
 import numpy as np
 import pandas as pd
 from sklearn.datasets import load_diabetes
-from sklearn.linear_model import LinearRegression
+from sklearn.linear_model import LinearRegression, Ridge
 
 from constrainedlr.model import ConstrainedLinearRegression
 
 atol = 1e-5
 
 dataset = load_diabetes()
 X = pd.DataFrame(dataset["data"], columns=dataset["feature_names"])
@@ -80,7 +80,18 @@
     assert np.allclose(sum_of_weights, features_sum_constraint_equal, atol=atol)
 
     clr = ConstrainedLinearRegression(fit_intercept=False)
     features_sum_constraint_equal = 15
     clr.fit(X, y, features_sum_constraint_equal=features_sum_constraint_equal)
     sum_of_weights = clr.coef_.sum()
     assert np.allclose(sum_of_weights, features_sum_constraint_equal, atol=atol)
+
+
+def test_alpha():
+    clr = ConstrainedLinearRegression(fit_intercept=True, alpha=1.0)
+    clr.fit(X, y)
+
+    ridge = Ridge(fit_intercept=True, alpha=1.0)
+    ridge.fit(X, y)
+
+    assert np.allclose(ridge.intercept_, clr.intercept_, rtol=0.01)
+    assert np.allclose(ridge.coef_, clr.coef_, rtol=0.01)
```

