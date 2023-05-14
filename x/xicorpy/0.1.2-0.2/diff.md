# Comparing `tmp/xicorpy-0.1.2.tar.gz` & `tmp/xicorpy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xicorpy-0.1.2.tar", max compression
+gzip compressed data, was "xicorpy-0.2.tar", max compression
```

## Comparing `xicorpy-0.1.2.tar` & `xicorpy-0.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1076 2022-01-18 02:45:06.355715 xicorpy-0.1.2/LICENSE
--rw-r--r--   0        0        0     1479 2022-01-18 02:45:06.359715 xicorpy-0.1.2/README.md
--rw-r--r--   0        0        0     1538 2022-01-18 02:45:06.359715 xicorpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      256 2022-01-18 02:45:06.359715 xicorpy-0.1.2/xicorpy/__init__.py
--rw-r--r--   0        0        0     1175 2022-01-18 02:45:06.359715 xicorpy-0.1.2/xicorpy/_utils.py
--rw-r--r--   0        0        0     8901 2022-01-18 02:45:06.359715 xicorpy-0.1.2/xicorpy/conditional_dependence.py
--rw-r--r--   0        0        0    11369 2022-01-18 02:45:06.359715 xicorpy-0.1.2/xicorpy/correlation.py
--rw-r--r--   0        0        0     5505 2022-01-18 02:45:06.359715 xicorpy-0.1.2/xicorpy/foci.py
--rw-r--r--   0        0        0     2524 2022-01-18 02:45:28.233826 xicorpy-0.1.2/setup.py
--rw-r--r--   0        0        0     2961 2022-01-18 02:45:28.234190 xicorpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-14 02:14:45.142979 xicorpy-0.2/LICENSE
+-rw-r--r--   0        0        0     1479 2023-05-14 02:14:45.142979 xicorpy-0.2/README.md
+-rw-r--r--   0        0        0     1562 2023-05-14 02:14:45.142979 xicorpy-0.2/pyproject.toml
+-rw-r--r--   0        0        0      256 2023-05-14 02:14:45.142979 xicorpy-0.2/xicorpy/__init__.py
+-rw-r--r--   0        0        0     1175 2023-05-14 02:14:45.142979 xicorpy-0.2/xicorpy/_utils.py
+-rw-r--r--   0        0        0     8832 2023-05-14 02:14:45.142979 xicorpy-0.2/xicorpy/conditional_dependence.py
+-rw-r--r--   0        0        0    12440 2023-05-14 02:14:45.142979 xicorpy-0.2/xicorpy/correlation.py
+-rw-r--r--   0        0        0     4324 2023-05-14 02:14:45.142979 xicorpy-0.2/xicorpy/foci.py
+-rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 xicorpy-0.2/PKG-INFO
```

### Comparing `xicorpy-0.1.2/LICENSE` & `xicorpy-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xicorpy-0.1.2/README.md` & `xicorpy-0.2/README.md`

 * *Files identical despite different names*

### Comparing `xicorpy-0.1.2/pyproject.toml` & `xicorpy-0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xicorpy"
-version = "0.1.2"
+version = "0.2"
 description = "Python implementation of Chatterjee's Rank Correlation, its modifications, and other offshoots"
 authors = ["Swarna Vallabhaneni <swarnakumar@gmail.com>"]
 maintainers = ["Swarna Vallabhaneni <swarnakumar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/swarnakumar/xicorpy"
 homepage = "https://swarnakumar.github.io/xicorpy"
@@ -41,15 +41,15 @@
 typings = ["mypy"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
-addopts = "--cov=xicorpy"
+addopts = "--cov=xicorpy --cov-report term-missing"
 
 [tool.coverage.run]
 omit = [".*", "*/site-packages/*"]
 source = ["xicorpy"]
 
 [tool.coverage.report]
 fail_under = 100
```

### Comparing `xicorpy-0.1.2/xicorpy/_utils.py` & `xicorpy-0.2/xicorpy/_utils.py`

 * *Files identical despite different names*

### Comparing `xicorpy-0.1.2/xicorpy/conditional_dependence.py` & `xicorpy-0.2/xicorpy/conditional_dependence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Dict, Union
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
-import scipy.stats as ss
 
 from sklearn.neighbors import NearestNeighbors
 
 from ._utils import convert_to_numeric, validate_and_prepare_for_conditional_dependence
 
 
 class ConditionalDependence:
@@ -209,15 +208,15 @@
 
     x_z_neighbors = NearestNeighbors(n_neighbors=2).fit(x_z.values)
     m = x_z_neighbors.kneighbors(n_neighbors=1, return_distance=False).ravel()
     r_m = r_y[m]
 
     x_neighbors = NearestNeighbors(n_neighbors=2).fit(x.values)
     n_i = x_neighbors.kneighbors(n_neighbors=1, return_distance=False).ravel()
-    r_n = ss.rankdata(n_i, method="max")
+    r_n = r_y[n_i]
 
     num = (np.minimum(r_y, r_m) - np.minimum(r_y, r_n)).sum()
     den = (r_y - np.minimum(r_y, r_n)).sum()
     return num / den
 
 
 def _conditional_dependence_with_each_z(
@@ -227,15 +226,15 @@
     if y.min() == y.max():
         return ret
 
     r_y = y.rank(method="max", ascending=True).values
 
     x_neighbors = NearestNeighbors(n_neighbors=2).fit(x.values)
     n_i = x_neighbors.kneighbors(n_neighbors=1, return_distance=False).ravel()
-    r_n = ss.rankdata(n_i, method="max")
+    r_n = r_y[n_i]
 
     for c in z.columns:
         x_z = pd.concat([x, z[[c]]], axis=1)
 
         x_z_neighbors = NearestNeighbors(n_neighbors=2).fit(x_z.values)
         m = x_z_neighbors.kneighbors(n_neighbors=1, return_distance=False).ravel()
         r_m = r_y[m]
```

### Comparing `xicorpy-0.1.2/xicorpy/correlation.py` & `xicorpy-0.2/xicorpy/correlation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import scipy.stats as ss
 
@@ -54,15 +55,15 @@
         self.y_df = convert_to_numeric(y_df)
 
         self._x = x
         self._y = y
 
     def compute_xi(
         self,
-        get_modified_xi: bool = True,
+        get_modified_xi: bool = None,
         m_nearest_neighbours: int = None,
         get_p_values: bool = False,
     ) -> Union[_RetType, Tuple[_RetType, _RetType]]:
         """
         Compute the Xi Coefficient (Chatterjee's Rank Correlation) between columns in X and Y.
 
         Xi Coefficient based on:
@@ -74,28 +75,46 @@
 
         The modified Xi Coefficient looks at M nearest neighbours to compute the correlation.
         This allows the coefficient to converge much faster. However, it is computationally slightly more intensive.
         For very large data, the two are likely to be very similar. We recommend using the modified Xi Coefficient.
 
         Args:
             get_modified_xi: Should the modified xi be computed?
-            m_nearest_neighbours: Only used if get_modified_xi is True.
+                    Defaults to True when there are no ties, and False when ties are present.
+            m_nearest_neighbours: Only used when get_modified_xi is True.
+                    Defaults to square-root of array size.
             get_p_values: Should the p-values be computed?
-                            The null hypothesis is that Y is completely independent of X (i.e., xi = 0).
+                    The null hypothesis is that Y is completely independent of X (i.e., xi = 0).
 
         Returns:
             float/np.ndarray/pd.DataFrame:
             - Xi Coefficient Values.
                 - If both X and Y are 1-d, returns a single float.
                 - If X is numpy object, returns a 2-D numpy array.
                 - Otherwise returns a pd.DataFrame.
-            - P-Values (only if get_p_values are true):
+            - P-Values (only when get_p_values are true):
                 - Same format at Xi
 
         """
+        if get_modified_xi is False:
+            pass
+        else:
+            ties = _check_ties(self.x_df, self.y_df)
+            if ties:
+                if get_modified_xi is True:
+                    warnings.warn(
+                        "Cannot use modified xi when there are ties present. Either explicitly set"
+                        "`get_modified_xi=False` or leave as `None` to accept automatic decision.",
+                        RuntimeWarning,
+                    )
+                else:
+                    get_modified_xi = False
+            elif get_modified_xi is None:
+                get_modified_xi = True
+
         ret = pd.DataFrame(0, index=self.x_df.columns, columns=self.y_df.columns)
         _, p = _get_p_no_ties(0, self.x_df.shape[0])
         p_values = pd.DataFrame(p, index=self.x_df.columns, columns=self.y_df.columns)
 
         for i in self.x_df.columns:
             i_col: pd.Series = self.x_df[i]
             if i_col.min() == i_col.max():  # pragma: no cover
@@ -155,15 +174,15 @@
 
         return ret
 
 
 def compute_xi_correlation(
     x: npt.ArrayLike,
     y: npt.ArrayLike = None,
-    get_modified_xi: bool = True,
+    get_modified_xi: bool = None,
     m_nearest_neighbours: int = None,
     get_p_values: bool = False,
 ) -> Union[_RetType, Tuple[_RetType, _RetType]]:
     """
     Helper function to compute the Xi Coefficient - uses the class machinery from `XiCorrelation`.
 
     Compute the Xi Coefficient (Chatterjee's Rank Correlation) between columns in X and Y.
@@ -183,15 +202,15 @@
     If Y is also passed, computes correlation between each column of X vs each column of Y.
 
     If only X is passed, X MUST be 2-d. Otherwise, both X and Y can be 1-d
 
     Args:
         x (npt.ArrayLike): A single list or list of lists or 1D/2D numpy array or pd.Series or pd.DataFrame.
         y (npt.ArrayLike): A single list or list of lists or 1D/2D numpy array or pd.Series or pd.DataFrame.
-        get_modified_xi: Should the modified xi be computed?
+        get_modified_xi: Should the modified xi be computed? By default this is True when there are no ties and False when ties are present
         m_nearest_neighbours: Only used if get_modified_xi is True.
         get_p_values: Should the p-values be computed?
                         The null hypothesis is that Y is completely independent of X (i.e., xi = 0).
 
     Returns:
         float/np.ndarray/pd.DataFrame:
         - Xi Coefficient Values.
@@ -248,16 +267,16 @@
         return _xi(y, get_p_value)
 
 
 def _xi(
     y: pd.Series, get_p_value: bool = False
 ) -> Union[float, Tuple[float, float, float]]:
     n = y.shape[0]
-    r = y.rank(method="max", ascending=True).values
-    l = y.rank(method="max", ascending=False).values
+    r = y.rank(method="max", ascending=True).values - 1
+    l = y.rank(method="max", ascending=False).values - 1
     num = n * np.abs(r[1:] - r[:-1]).sum()
     den = 2 * (l * (n - l)).sum()
     xi = 1 - num / den
     if get_p_value:
         sd, p = _get_p_value(xi, r, l, n)
         return xi, sd, p
     else:
@@ -319,7 +338,14 @@
     cq = np.cumsum(qfr)
     m = (cq + (n - ind) * qfr) / n
     b = (m * m).mean()
     v = (ai - 2 * b + ci ** 2) / cu ** 2
 
     p = 1 - ss.norm.cdf(np.sqrt(n) * xi / np.sqrt(v))
     return np.sqrt(v), p
+
+
+def _check_ties(*dfs: pd.DataFrame) -> bool:
+    df = pd.concat(dfs, ignore_index=True, axis="columns")
+    if len(df.drop_duplicates()) == len(df):
+        return False
+    return True
```

### Comparing `xicorpy-0.1.2/xicorpy/foci.py` & `xicorpy-0.2/xicorpy/foci.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-import logging
+import warnings
 from typing import List, Union
 
 import numpy.typing as npt
 
 from ._utils import validate_and_prepare_for_conditional_dependence
-from .conditional_dependence import (
-    compute_conditional_dependence,
-    compute_conditional_dependence_1d,
-)
-
-logger = logging.getLogger(__name__)
+from .conditional_dependence import compute_conditional_dependence_1d
 
 
 class FOCI:
     """Class for computing FOCI."""
 
     def __init__(self, y: npt.ArrayLike, x: npt.ArrayLike):
         """
@@ -44,92 +39,66 @@
 
         next_p = max(codec, key=lambda k: codec[k])
         return next_p, codec[next_p]
 
     def select_features(
         self,
         num_features: int = None,
-        auto_stop: bool = True,
         init_selection: List[Union[int, str]] = None,
     ) -> List[Union[int, str]]:
         """
         Selects features based on the Feature Ordering based on Conditional Independence (FOCI) algorithm in:
             [Azadkia and Chatterjee (2021). "A simple measure of conditional dependence", Annals of Statistics](https://arxiv.org/abs/1910.12327)
 
         Args:
             num_features: Maximum number of features to select. Defaults to the number of features in x.
-            auto_stop: Should the algorithm stop automatically when conditional dependence starts dropping?
             init_selection (list): Initial selection of features.
 
         Returns:
             list: List of selected features.
                 If x was `pd.DataFrame`, this will be column names.
                 Otherwise, this will be indices.
 
         """
         if num_features is None:  # pragma: no cover
             num_features = self.x_df.shape[1]
-            if not auto_stop:
-                raise ValueError(
-                    "If num_features is not specified, auto_stop MUST be True"
-                )
 
         current_selection = [i for i in (init_selection or [])]
         if len(current_selection) >= num_features:
-            logger.warning("Initial selection is already complete")
+            warnings.warn("Initial selection is already complete")
             return current_selection
 
-        if current_selection:
-            curr_t = compute_conditional_dependence(
-                self.y_, self.x_df[current_selection]
-            )
-        else:
-            next_p, curr_t = self._get_next_p(current_selection)
-            if curr_t <= 0:  # pragma: no cover
-                logger.warning("Unable to find the first feature")
-                return []
-            current_selection.append(next_p)
-
         stop = False
         while not stop and len(current_selection) < num_features:
             next_p, next_t = self._get_next_p(current_selection)
 
             if next_t <= 0:  # pragma: no cover
                 stop = True
-            elif auto_stop:
-                # Codec is decreasing! Stop!
-                if next_t - curr_t <= 0:
-                    stop = True
-                else:
-                    curr_t = next_t
-                    current_selection.append(next_p)
             else:
                 current_selection.append(next_p)
 
         return current_selection
 
 
 def select_features_using_foci(
     y: npt.ArrayLike,
     x: npt.ArrayLike,
     num_features: int = None,
-    auto_stop: bool = True,
     init_selection: List[Union[int, str]] = None,
 ) -> List[Union[int, str]]:
     """
     Implements the FOCI algorithm for feature selection.
 
     Azadkia and Chatterjee (2021). "A simple measure of conditional dependence", Annals of Statistics.
     https://arxiv.org/abs/1910.12327.
 
     Args:
         y (npt.ArrayLike): The dependent variable. A single list or 1D array or a pandas Series.
         x (npt.ArrayLike): The independent variables. A single list or list of lists or 1D/2D numpy array or pd.Series or pd.DataFrame.
         num_features: Max number of features to select. Defaults to ALL features.
-        auto_stop: If True, stops when the conditional dependence stops increasing.
         init_selection (list): Initial selection of features.
             If `x` is a `pd.DataFrame`, this is expected to be a list of column names.
             Otherwise, this is expected to be a list of indices.
 
     Returns:
         list: List of selected features.
             If x was `pd.DataFrame`, this will be column names.
@@ -138,8 +107,8 @@
     Raises:
         ValueError: If y is not 1d.
         ValueError: If x is not 1d or 2d.
         ValueError: If y and x have different lengths.
         ValueError: If there are <= 2 valid y values.
 
     """
-    return FOCI(y, x).select_features(num_features, auto_stop, init_selection)
+    return FOCI(y, x).select_features(num_features, init_selection)
```

### Comparing `xicorpy-0.1.2/PKG-INFO` & `xicorpy-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: xicorpy
-Version: 0.1.2
+Version: 0.2
 Summary: Python implementation of Chatterjee's Rank Correlation, its modifications, and other offshoots
 Home-page: https://swarnakumar.github.io/xicorpy
 License: MIT
 Author: Swarna Vallabhaneni
 Author-email: swarnakumar@gmail.com
 Maintainer: Swarna Vallabhaneni
 Maintainer-email: swarnakumar@gmail.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Provides-Extra: typings
-Requires-Dist: mkdocs-material (>=8.1,<8.2); extra == "docs"
-Requires-Dist: mkdocstrings (>=0.17,<0.18); extra == "docs"
-Requires-Dist: mypy (==0.931); extra == "typings"
+Requires-Dist: mkdocs-material (>=8.1,<8.2) ; extra == "docs"
+Requires-Dist: mkdocstrings (>=0.17,<0.18) ; extra == "docs"
+Requires-Dist: mypy (==0.931) ; extra == "typings"
 Requires-Dist: numpy (>=1.17,<2.0)
 Requires-Dist: pandas (>=1.2,<2.0)
 Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
 Requires-Dist: scipy (>=1.7,<2.0)
 Project-URL: Repository, https://github.com/swarnakumar/xicorpy
 Description-Content-Type: text/markdown
```

