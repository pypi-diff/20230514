# Comparing `tmp/lmo-0.2.1.tar.gz` & `tmp/lmo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmo-0.2.1.tar", max compression
+gzip compressed data, was "lmo-0.3.0.tar", max compression
```

## Comparing `lmo-0.2.1.tar` & `lmo-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.2.1/LICENSE
--rw-r--r--   0        0        0      754 2023-05-11 19:25:30.130399 lmo-0.2.1/README.md
--rw-r--r--   0        0        0      199 2023-05-02 23:21:30.443482 lmo-0.2.1/lmo/__init__.py
--rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.2.1/lmo/_meta.py
--rw-r--r--   0        0        0      128 2023-04-30 12:42:37.998900 lmo-0.2.1/lmo/_typing.py
--rw-r--r--   0        0        0     7036 2023-05-04 02:29:29.090059 lmo-0.2.1/lmo/multivariate.py
--rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.2.1/lmo/py.typed
--rw-r--r--   0        0        0      987 2023-05-04 01:04:36.508186 lmo-0.2.1/lmo/stats.py
--rw-r--r--   0        0        0     5850 2023-05-11 18:57:22.207683 lmo-0.2.1/lmo/univariate.py
--rw-r--r--   0        0        0     1482 2023-05-03 23:50:48.397361 lmo-0.2.1/lmo/weights.py
--rw-r--r--   0        0        0     1916 2023-05-11 19:28:18.473947 lmo-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 lmo-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.3.0/LICENSE
+-rw-r--r--   0        0        0      754 2023-05-11 19:25:30.130399 lmo-0.3.0/README.md
+-rw-r--r--   0        0        0      199 2023-05-02 23:21:30.443482 lmo-0.3.0/lmo/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.3.0/lmo/_meta.py
+-rw-r--r--   0        0        0      415 2023-05-14 01:14:00.711613 lmo-0.3.0/lmo/_utils.py
+-rw-r--r--   0        0        0     6933 2023-05-14 00:52:05.975764 lmo-0.3.0/lmo/multivariate.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.3.0/lmo/py.typed
+-rw-r--r--   0        0        0     1099 2023-05-14 01:14:00.735614 lmo-0.3.0/lmo/stats.py
+-rw-r--r--   0        0        0     1217 2023-05-14 00:52:26.476196 lmo-0.3.0/lmo/typing.py
+-rw-r--r--   0        0        0     5727 2023-05-14 00:52:47.956648 lmo-0.3.0/lmo/univariate.py
+-rw-r--r--   0        0        0     1527 2023-05-14 01:14:00.743614 lmo-0.3.0/lmo/weights.py
+-rw-r--r--   0        0        0     1949 2023-05-14 01:18:45.937664 lmo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 lmo-0.3.0/PKG-INFO
```

### Comparing `lmo-0.2.1/LICENSE` & `lmo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmo-0.2.1/README.md` & `lmo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lmo-0.2.1/lmo/multivariate.py` & `lmo-0.3.0/lmo/multivariate.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,25 +25,24 @@
 
 from typing import Any, cast
 
 import numpy as np
 from numpy import typing as npt
 
 from . import tl_moment
-from ._typing import SortKind
+from .typing import AnyMatrix, SortKind, Trimming
 from .weights import tl_weights
 
 
 # noinspection PyPep8Naming
 def tl_comoment(
-    a: npt.ArrayLike,
+    a: AnyMatrix,
     r: int,
     /,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     *,
     rowvar: bool = True,
     sort: SortKind | None = None,
 ) -> npt.NDArray[np.float_]:
     """
     Multivariate extension of the sample TL-moments: the TL-comoment matrix.
 
@@ -51,17 +50,16 @@
     Modified to be compatible with (the more general) TL-moments.
 
     Args:
         a: A 1-D or 2-D array containing `m` variables and `n` observations.
           Each row of `a` represents a variable, and each column a single
           observation of all those variables. Also see `rowvar` below.
         r: The order of the TL-moment; strictly positive integer.
-
-        s (optional): Amount of samples to trim at the start, default is 1.
-        t (optional): Amount of samples to trim at the end, default is 1.
+        trim: Amount of samples to trim on both sides, or a tuple of the amount
+            to trim on the left and right sides. Default is 1.
 
         rowvar (optional): If `rowvar` is True (default), then each row
           represents a variable, with observations in the columns. Otherwise,
           the relationship is transposed: each column represents a variable,
           while the rows contain observations.
         sort (opional): Sorting algorithm to use, default is 'quicksort'. See
           `numpy.sort` for more info.
@@ -90,196 +88,190 @@
     if not m or not x.size:
         return np.empty((0, 0), dtype)
 
     if r == 0:
         # The zeroth (TL-)co-moment matrix is the identity matrix, right..?
         return np.eye(m, dtype=dtype)
 
-    w = tl_weights(n, r, s, t)
+    w = tl_weights(n, r, trim)
 
     L_ji = np.empty((m, m), dtype=dtype)
     for j, ii in enumerate(np.argsort(x, kind=sort)):
         L_ji[j] = x[:, ii] @ w
 
     return L_ji.T
 
 
 # noinspection PyPep8Naming
 def tl_coratio(
-    a: npt.ArrayLike,
+    a: AnyMatrix,
     r: int,
     /,
     k: int = 2,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     **kwargs: Any,
 ) -> npt.NDArray[np.float_]:
     """
     TL-comoment ratio matrix `L_r[i, j] / l_k[j]`.
 
     References:
         * Serfling, R. and Xiao, P., 2006. A Contribution to Multivariate
           L-Moments: L-Comoment Matrices.
 
     """
-    L_k = tl_comoment(a, r, s, t, **kwargs)
+    L_k = tl_comoment(a, r, trim, **kwargs)
 
     if k == 0:
         return L_k
 
     l_r = L_k.diagonal() if k == r else cast(
-        npt.NDArray[np.float_], tl_moment(a, r, s, t, **kwargs)
+        npt.NDArray[np.float_], tl_moment(a, r, trim, **kwargs)
     )
 
     return L_k / l_r[:, np.newaxis]
 
 
 def tl_coloc(
-    a: npt.ArrayLike,
+    a: AnyMatrix,
     /,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     **kwargs: Any,
 ) -> npt.NDArray[np.float_]:
     """
     TL-co-locations; the 1st TL-comoment matrix.
 
     Notes:
         * If you figure out how to interpret this, or how this can be applied,
           please tell me (github: @jorenham).
 
     """
-    return tl_comoment(a, 1, s, t, **kwargs)
+    return tl_comoment(a, 1, trim, **kwargs)
 
 
 def tl_coscale(
-    a: npt.ArrayLike,
+    a: AnyMatrix,
     /,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     **kwargs: Any,
 ) -> npt.NDArray[np.float_]:
     """
     TL-coscale coefficients; the 2nd TL-comoment matrix.
 
     Analogous to the (auto-) covariance matrix, the TL-coscale matrix is
     positive semi-definite, and its main diagonal contains the TL-scale's.
     But unlike the variance-covariance matrix, the TL-coscale matrix is not
     symmetric.
     """
-    return tl_comoment(a, 2, s, t, **kwargs)
+    return tl_comoment(a, 2, trim, **kwargs)
 
 
 def tl_corr(
-    a: npt.ArrayLike,
+    a: AnyMatrix,
     /,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     **kwargs: Any,
 ) -> npt.NDArray[np.float_]:
     """
     Sample TL-correlation coefficient matrix; the ratio of the TL-coscale
     matrix over the TL-scale **column**-vectors, i.e. the TL-correlation matrix
     is typically asymmetric.
 
     The diagonal contains only ones.
 
     Notes:
         Where the pearson correlation coefficient measures linearity, the
         (T)L-correlation coefficient measures monotonicity.
 
     """
-    return tl_coratio(a, 2, s=s, t=t, **kwargs)
+    return tl_coratio(a, 2, trim=trim, **kwargs)
 
 
 def tl_coskew(
-    a: npt.ArrayLike,
+    a: AnyMatrix,
     /,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     **kwargs: Any,
 ) -> npt.NDArray[np.float_]:
     """
     TL-coskewness coefficients; the 3rd TL-comoment ratio matrix.
 
     The main diagonal cantains the TL-skewness coefficients.
     """
-    return tl_coratio(a, 3, s=s, t=t, **kwargs)
+    return tl_coratio(a, 3, trim=trim, **kwargs)
 
 
 def tl_cokurt(
-    a: npt.ArrayLike,
+    a: AnyMatrix,
     /,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     **kwargs: Any,
 ) -> npt.NDArray[np.float_]:
     """
     TL-cokurtosis coefficients; the 4th TL-comoment ratio matrix.
 
     The main diagonal contains the TL-kurtosis coefficients.
     """
-    return tl_coratio(a, 4, s=s, t=t, **kwargs)
+    return tl_coratio(a, 4, trim=trim, **kwargs)
 
 
 def l_comoment(
-    a: npt.ArrayLike,
+    a: AnyMatrix,
     r: int,
     /,
     **kwargs: Any,
 ) -> npt.NDArray[np.float_]:
     """
     The r-th sample L-comoment matrix.
     Alias for ``tl_comoment(a, r, 0, 0, **kwargs)``.
     """
-    return tl_comoment(a, r, 0, 0, **kwargs)
+    return tl_comoment(a, r, 0, **kwargs)
 
 
 def l_coratio(
-    a: npt.ArrayLike,
+    a: AnyMatrix,
     r: int,
     k: int = 2,
     /,
     **kwargs: Any,
 ) -> npt.NDArray[np.float_]:
     """
     L-comoment ratio matrix `L_r[i, j] / l_k[j]`.
     Alias for ``tl_coratio(a, r, k, 0, 0, **kwargs)``.
     """
-    return tl_coratio(a, r, k, 0, 0, **kwargs)
+    return tl_coratio(a, r, k, 0, **kwargs)
 
 
-def l_coloc(a: npt.ArrayLike, /, **kwargs: Any) -> npt.NDArray[np.float_]:
+def l_coloc(a: AnyMatrix, /, **kwargs: Any) -> npt.NDArray[np.float_]:
     """
     L-colocation matrix, i.e. each `L[i, j]` is the sample mean of `a[i]`.
     """
     return l_comoment(a, 1, **kwargs)
 
 
-def l_coscale(a: npt.ArrayLike, /, **kwargs: Any) -> npt.NDArray[np.float_]:
+def l_coscale(a: AnyMatrix, /, **kwargs: Any) -> npt.NDArray[np.float_]:
     """
     L-scale: the second L-comoment matrix.
     """
     return l_comoment(a, 2, **kwargs)
 
 
-def l_corr(a: npt.ArrayLike, /, **kwargs: Any) -> npt.NDArray[np.float_]:
+def l_corr(a: AnyMatrix, /, **kwargs: Any) -> npt.NDArray[np.float_]:
     """
     L-correlation coefficients; the 2nd L-comoment ratio matrix.
 
     Unlike the TL-correlation, the L-correlation is bounded within [-1, 1].
     """
     return l_coratio(a, 2, **kwargs)
 
 
-def l_coskew(a: npt.ArrayLike, /, **kwargs: Any) -> npt.NDArray[np.float_]:
+def l_coskew(a: AnyMatrix, /, **kwargs: Any) -> npt.NDArray[np.float_]:
     """
     L-coskewness coefficients; the 3rd L-comoment ratio matrix.
     """
     return l_coratio(a, 3, **kwargs)
 
 
-def l_cokurt(a: npt.ArrayLike, /, **kwargs: Any) -> npt.NDArray[np.float_]:
+def l_cokurt(a: AnyMatrix, /, **kwargs: Any) -> npt.NDArray[np.float_]:
     """
     L-cokurtosis coefficients; the 4th L-comoment ratio matrix.
     """
     return l_coratio(a, 4, **kwargs)
```

### Comparing `lmo-0.2.1/lmo/univariate.py` & `lmo-0.3.0/lmo/univariate.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,65 +26,57 @@
 """
 
 __all__ = (
     'l_moment', 'l_ratio', 'l_loc', 'l_scale', 'l_skew', 'l_kurt',
     'tl_moment', 'tl_ratio', 'tl_loc', 'tl_scale', 'tl_skew', 'tl_kurt',
 )
 
-from typing import Any, TypeAlias
+from typing import Any
 
 import numpy as np
-import numpy.typing as npt
 
+from .typing import AnyTensor, ScalarOrArray, SortKind, Trimming
 from .weights import tl_weights
-from ._typing import SortKind
-
-_AnyFloat: TypeAlias = np.floating[Any]
-_NumOrArr: TypeAlias = _AnyFloat | npt.NDArray[_AnyFloat]
 
 
 def tl_moment(
-    a: npt.ArrayLike,
+    a: AnyTensor,
     r: int,
     /,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     *,
     axis: int | None = None,
     sort: SortKind | None = None,
-) -> np.float_ | npt.NDArray[np.float_]:
+) -> ScalarOrArray[np.float_]:
     """
     The r-th sample TL-moment.
 
     Args:
         a: Array-like with samples.
         r: The order of the TL-moment; strictly positive integer.
-
-        s: Amount of samples to trim at the start, default is 1.
-        t: Amount of samples to trim at the end, default is 1.
+        trim: Amount of samples to trim on both sides, or a tuple of the amount
+            to trim on the left and right sides.
 
         axis: Axis along wich to calculate the TL-moments.
             If `None` (default), all samples in the array will be used.
         sort: Sorting algorithm to use, default is `'quicksort'`. See
             `numpy.sort` for more info.
 
     Returns:
         Scalar or array; the r-th TL-moment(s).
 
     """
-    x = np.sort(a, axis=axis, kind=sort)
+    x = np.sort(np.asanyarray(a), axis=axis, kind=sort)
     n = x.shape[axis or 0]
 
     if r == 0:
         # zeroth (TL-)moment is 1
-        # noinspection PyTypeChecker
-        dt: np.dtype[_AnyFloat] = np.find_common_type([x.dtype], [np.float_])
-        return np.ones(x.size // n, dtype=dt) if x.ndim > 1 else dt.type(1)
+        return np.ones(x.size // n) if x.ndim > 1 else np.float_(1)
 
-    w = tl_weights(n, r, s, t)
+    w = tl_weights(n, r, trim)
 
     _axis = (axis or 0) % x.ndim
     assert _axis >= 0
 
     if _axis == 0:
         # apply along the first axis
         return w @ x
@@ -93,145 +85,146 @@
         # apply along the last axis
         return x @ w
 
     return np.apply_along_axis(np.inner, _axis, x, w)
 
 
 def tl_ratio(
-    a: npt.ArrayLike,
+    a: AnyTensor,
     r: int,
     /,
     k: int = 2,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     *,
     axis: int | None = None,
     sort: SortKind | None = None,
-) -> _NumOrArr:
+) -> ScalarOrArray[np.float_]:
     """
     Ratio of the r-th and k-th (2nd by default) sample TL-moments.
     """
-    x = np.sort(a, axis=axis, kind=sort)
+    x = np.sort(np.asanyarray(a), axis=axis, kind=sort)
 
-    l_r = tl_moment(x, r, s, t, axis=axis)
+    l_r = tl_moment(x, r, trim, axis=axis)
 
     if k == 0:
         return l_r
     if k == r:
         return np.ones_like(l_r)[()]
 
-    l_k = l_r if k == r else tl_moment(x, k, s, t, axis=axis)
+    l_k = l_r if k == r else tl_moment(x, k, trim, axis=axis)
 
     # i.e. `x / 0 = 0 if x == 0 else np.nan`
     return np.divide(
         l_r,
         l_k,
         out=np.where(l_r == 0, 0.0, np.nan),
         where=l_k != 0
     )[()]  # [()] converts any 0-dimensional arrays to scalar
 
 
 def tl_loc(
-    a: npt.ArrayLike,
+    a: AnyTensor,
     /,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     **kwargs: Any,
-) -> _NumOrArr:
+) -> ScalarOrArray[np.float_]:
     """
     TL-location: the first sample TL-moment. Analogous to the sample mean.
     """
-    return tl_moment(a, 1, s, t, **kwargs)
+    return tl_moment(a, 1, trim, **kwargs)
 
 
 def tl_scale(
-    a: npt.ArrayLike,
+    a: AnyTensor,
     /,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     **kwargs: Any,
-) -> _NumOrArr:
+) -> ScalarOrArray[np.float_]:
     """
     TL-scale: the second TL-moment. Analogous to the sample standard deviation.
     """
-    return tl_moment(a, 2, s, t, **kwargs)
+    return tl_moment(a, 2, trim, **kwargs)
 
 
 def tl_skew(
-    a: npt.ArrayLike,
+    a: AnyTensor,
     /,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     **kwargs: Any,
-) -> _NumOrArr:
+) -> ScalarOrArray[np.float_]:
     """
     TL-skewness coefficient; the ratio of the 3rd and 2nd sample TL-moments.
     """
-    return tl_ratio(a, 3, s=s, t=t, **kwargs)
+    return tl_ratio(a, 3, trim=trim, **kwargs)
 
 
 def tl_kurt(
-    a: npt.ArrayLike,
+    a: AnyTensor,
     /,
-    s: int = 1,
-    t: int = 1,
+    trim: Trimming = 1,
     **kwargs: Any,
-) -> _NumOrArr:
+) -> ScalarOrArray[np.float_]:
     """
     TL-kurtosis coefficient; the ratio of the 4th and 2nd sample TL-moments.
     """
-    return tl_ratio(a, 4, s=s, t=t, **kwargs)
+    return tl_ratio(a, 4, trim=trim, **kwargs)
 
 
 # L-moment aliasses
 
-def l_moment(a: npt.ArrayLike, r: int, /, **kwargs: Any) -> _NumOrArr:
+def l_moment(
+    a: AnyTensor,
+    r: int,
+    /,
+    **kwargs: Any,
+) -> ScalarOrArray[np.float_]:
     """
     The r-th sample L-moment.
-    Alias for ``tl_moment(a, r, 0, 0, **kwargs)``.
+    Alias for ``tl_moment(a, r, 0, **kwargs)``.
     """
-    return tl_moment(a, r, 0, 0, **kwargs)
+    return tl_moment(a, r, 0, **kwargs)
 
 
 def l_ratio(
-    a: npt.ArrayLike,
-    r: int, k: int = 2,
+    a: AnyTensor,
+    r: int,
+    k: int = 2,
     /,
     **kwargs: Any,
-) -> _NumOrArr:
+) -> ScalarOrArray[np.float_]:
     """
     Ratio of the r-th and k-th L-moments.
-    Alias for ``tl_ratio(a, r, k, 0, 0, **kwargs)``.
+    Alias for ``tl_ratio(a, r, k, 0, **kwargs)``.
 
     For k > 0, the L-moment ratio's are bounded within [-1, 1].
     """
-    return tl_ratio(a, r, k, 0, 0, **kwargs)
+    return tl_ratio(a, r, k, 0, **kwargs)
 
 
-def l_loc(a: npt.ArrayLike, /, **kwargs: Any) -> _NumOrArr:
+def l_loc(a: AnyTensor, /, **kwargs: Any) -> ScalarOrArray[np.float_]:
     """
     L-location: the first sample L-moment.
     Equivalent to the sample mean.
     """
     return l_moment(a, 1, **kwargs)
 
 
-def l_scale(a: npt.ArrayLike, /, **kwargs: Any) -> _NumOrArr:
+def l_scale(a: AnyTensor, /, **kwargs: Any) -> ScalarOrArray[np.float_]:
     """
     L-scale: the second L-moment.
     Equivalent to half the mean absolute difference.
     """
     return l_moment(a, 2, **kwargs)
 
 
-def l_skew(a: npt.ArrayLike, /, **kwargs: Any) -> _NumOrArr:
+def l_skew(a: AnyTensor, /, **kwargs: Any) -> ScalarOrArray[np.float_]:
     """
     L-skewness coefficient; the ratio of the 3rd and 2nd sample L-moments.
     """
     return l_ratio(a, 3, **kwargs)
 
 
-def l_kurt(a: npt.ArrayLike, /, **kwargs: Any) -> _NumOrArr:
+def l_kurt(a: AnyTensor, /, **kwargs: Any) -> ScalarOrArray[np.float_]:
     """
     L-kurtosis coefficient; the ratio of the 4th and 2nd sample L-moments.
     """
     return l_ratio(a, 4, **kwargs)
```

### Comparing `lmo-0.2.1/lmo/weights.py` & `lmo-0.3.0/lmo/weights.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 __all__ = 'tl_weights', 'l_weights'
 
 from math import comb, fsum
 
 import numpy as np
 import numpy.typing as npt
 
+from ._utils import expand_trimming
+from .typing import Trimming
 
-def tl_weights(n: int, r: int, /, s: int, t: int) -> npt.NDArray[np.float_]:
+
+def tl_weights(n: int, r: int, /, trim: Trimming) -> npt.NDArray[np.float_]:
     """
     Linear sample weights for calculation of the r-th TL(s, t)-moment.
 
     Args:
         n: Sample size.
         r: L-moment order, e.g. 1 for location, and 2 for scale.
-        s: Amount of samples to trim at the start/left.
-        t: Amount of samples to trim at the end/right.
+        trim: Amount of samples to trim on both sides, or a tuple of the amount
+            to trim on the left and right sides. Default is 1.
 
     Returns:
         w_j: A vector of size `n`, with linear weights for each of the
             (ordered) samples.
 
     """
     if r <= 0:
         raise ValueError(f'expected r > 0, got {r} <= 0')
-    if min(s, t) < 0:
-        raise ValueError(f'expected s >= 0 and t >= 0, got min{s, t} < 0')
-    if n < r + s + t:
-        raise ValueError(f'expected n >= r + s + t, got {n} < {r + s + t}')
+
+    tl, tr = expand_trimming(trim)
+
+    if n < r + tl + tr:
+        raise ValueError(f'expected n >= r + s + t, got {n} < {r + tl + tr}')
 
     # pre-calculate the terms that are independent on j
-    m = r * comb(n, r + s + t)
+    m = r * comb(n, r + tl + tr)
     w_k = np.empty(r)
     for k in range(r):
         w_k[k] = (-1) ** k * comb(r - 1, k) / m
 
     # sample weights
     w_j = np.zeros(n)
-    for j in range(s, n - t):
+    for j in range(tl, n - tr):
         # divide inside the loop, to avoid overflows
         w_j[j] = fsum(
-            comb(j, r + s - k - 1) * comb(n - j - 1, t + k) * w_k[k]
+            comb(j, r + tl - k - 1) * comb(n - j - 1, tr + k) * w_k[k]
             for k in range(r)
         )
 
     return w_j
 
 
 def l_weights(n: int, r: int, /) -> npt.NDArray[np.float_]:
     """
     Alias for `tl_weights(n, r, 0, 0)`.
     """
-    return tl_weights(n, r, 0, 0)
+    return tl_weights(n, r, 0)
```

### Comparing `lmo-0.2.1/PKG-INFO` & `lmo-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: lmo
-Version: 0.2.1
+Version: 0.3.0
 Summary: L-Moments for robust statistics.
-Home-page: https://github.com/jorenham/lmo/
+Home-page: https://jorenham.github.io/lmo/
 License: BSD-3-Clause
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: numpy (>=1.21)
+Requires-Dist: numpy (>=1.20,<2.0)
 Project-URL: Bug Tracker, https://github.com/jorenham/lmo/issues
+Project-URL: Documentation, https://jorenham.github.io/lmo/
 Project-URL: Repository, https://github.com/jorenham/lmo/
 Description-Content-Type: text/markdown
 
 <img src="./docs/static/lmo.svg" alt="jorenham/lmo" width="128" align="right">
 
 # Lmo
```

