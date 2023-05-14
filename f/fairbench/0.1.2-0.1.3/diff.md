# Comparing `tmp/fairbench-0.1.2-py3-none-any.whl.zip` & `tmp/fairbench-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,31 @@
-Zip file size: 17113 bytes, number of entries: 25
+Zip file size: 19500 bytes, number of entries: 29
 -rw-rw-rw-  2.0 fat      165 b- defN 23-Jan-15 16:08 fairbench/__init__.py
 -rw-rw-rw-  2.0 fat      512 b- defN 23-Jan-15 16:07 fairbench/accumulate.py
 -rw-rw-rw-  2.0 fat     1790 b- defN 23-Jan-15 16:07 fairbench/algorithms.py
 -rw-rw-rw-  2.0 fat     1817 b- defN 23-Jan-19 20:24 fairbench/export.py
 -rw-rw-rw-  2.0 fat     9339 b- defN 23-Jan-14 23:06 fairbench/fork.py
 -rw-rw-rw-  2.0 fat     1744 b- defN 23-Jan-15 16:07 fairbench/output.py
 -rw-rw-rw-  2.0 fat     2393 b- defN 23-Jan-15 16:07 fairbench/reduction.py
 -rw-rw-rw-  2.0 fat     1146 b- defN 23-Jan-15 16:07 fairbench/reporting.py
 -rw-rw-rw-  2.0 fat       79 b- defN 23-Jan-15 16:19 fairbench/forks/__init__.py
--rw-rw-rw-  2.0 fat     1801 b- defN 23-Jan-19 20:24 fairbench/forks/explanation.py
--rw-rw-rw-  2.0 fat    13023 b- defN 23-Jan-19 20:21 fairbench/forks/fork.py
+-rw-rw-rw-  2.0 fat     1845 b- defN 23-Feb-03 12:23 fairbench/forks/explanation.py
+-rw-rw-rw-  2.0 fat    14417 b- defN 23-Feb-20 09:13 fairbench/forks/fork.py
 -rw-rw-rw-  2.0 fat      154 b- defN 23-Jan-14 23:08 fairbench/metrics/__init__.py
 -rw-rw-rw-  2.0 fat     1816 b- defN 23-Jan-19 20:21 fairbench/metrics/classification.py
 -rw-rw-rw-  2.0 fat     2007 b- defN 23-Jan-15 16:07 fairbench/metrics/disparate_impact.py
 -rw-rw-rw-  2.0 fat     1450 b- defN 23-Jan-15 16:07 fairbench/metrics/disparate_mistreatment.py
 -rw-rw-rw-  2.0 fat      207 b- defN 23-Jan-15 14:06 fairbench/reports/__init__.py
 -rw-rw-rw-  2.0 fat      753 b- defN 23-Jan-15 17:03 fairbench/reports/accumulate.py
--rw-rw-rw-  2.0 fat     1557 b- defN 23-Jan-15 17:03 fairbench/reports/adhoc.py
+-rw-rw-rw-  2.0 fat     1547 b- defN 23-Feb-20 09:13 fairbench/reports/adhoc.py
 -rw-rw-rw-  2.0 fat     1411 b- defN 23-Jan-15 17:07 fairbench/reports/base.py
 -rw-rw-rw-  2.0 fat     4980 b- defN 23-Jan-15 17:07 fairbench/reports/reduction.py
--rw-rw-rw-  2.0 fat      859 b- defN 23-Jan-15 16:08 fairbench/reports/surrogate.py
--rw-rw-rw-  2.0 fat      714 b- defN 23-Jan-19 20:26 fairbench-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-19 20:26 fairbench-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jan-19 20:26 fairbench-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2056 b- defN 23-Jan-19 20:26 fairbench-0.1.2.dist-info/RECORD
-25 files, 51875 bytes uncompressed, 13797 bytes compressed:  73.4%
+-rw-rw-rw-  2.0 fat      862 b- defN 23-Jan-23 12:46 fairbench/reports/surrogate.py
+-rw-rw-rw-  2.0 fat      155 b- defN 23-Feb-20 08:42 fairbench/reports/reduction/__init__.py
+-rw-rw-rw-  2.0 fat      856 b- defN 23-Feb-20 08:37 fairbench/reports/reduction/expanders.py
+-rw-rw-rw-  2.0 fat     1587 b- defN 23-Feb-20 08:42 fairbench/reports/reduction/reduce.py
+-rw-rw-rw-  2.0 fat     2604 b- defN 23-Feb-20 08:40 fairbench/reports/reduction/reducers.py
+-rw-rw-rw-  2.0 fat      714 b- defN 23-Feb-20 09:14 fairbench-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-20 09:14 fairbench-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Feb-20 09:14 fairbench-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2437 b- defN 23-Feb-20 09:14 fairbench-0.1.3.dist-info/RECORD
+29 files, 58889 bytes uncompressed, 15570 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -57,20 +57,32 @@
 
 Filename: fairbench/reports/reduction.py
 Comment: 
 
 Filename: fairbench/reports/surrogate.py
 Comment: 
 
-Filename: fairbench-0.1.2.dist-info/METADATA
+Filename: fairbench/reports/reduction/__init__.py
 Comment: 
 
-Filename: fairbench-0.1.2.dist-info/WHEEL
+Filename: fairbench/reports/reduction/expanders.py
 Comment: 
 
-Filename: fairbench-0.1.2.dist-info/top_level.txt
+Filename: fairbench/reports/reduction/reduce.py
 Comment: 
 
-Filename: fairbench-0.1.2.dist-info/RECORD
+Filename: fairbench/reports/reduction/reducers.py
+Comment: 
+
+Filename: fairbench-0.1.3.dist-info/METADATA
+Comment: 
+
+Filename: fairbench-0.1.3.dist-info/WHEEL
+Comment: 
+
+Filename: fairbench-0.1.3.dist-info/top_level.txt
+Comment: 
+
+Filename: fairbench-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fairbench/forks/explanation.py

```diff
@@ -13,14 +13,15 @@
         from fairbench.forks import Fork
 
         self.value = value
         self.explain = Fork(kwargs) if explain is None else explain
         self.desc = desc
         if (
             not isinstance(value, float)
+            and not isinstance(value, int)
             and "tensor" not in value.__class__.__name__.lower()
             and "array" not in value.__class__.__name__
         ):
             raise Exception("Can not set non-numeric as explainable", value)
         if explain is not None and kwargs:
             raise Exception("Cannot create explainable with both kwargs and a Fork")
```

## fairbench/forks/fork.py

```diff
@@ -11,36 +11,52 @@
     assert backend_name in ["torch", "tensorflow", "jax", "numpy"]
     global _backend
     _backend = backend_name
 
 
 def tobackend(value):
     global _backend
-    name = type(value.raw if isinstance(value, ep.Tensor) else value).__module__.split(".")[0]
+    name = type(value.raw if isinstance(value, ep.Tensor) else value).__module__.split(
+        "."
+    )[0]
     m = sys.modules
     if name != _backend:
         value = value.raw if isinstance(value, ep.Tensor) else value
         if name == "torch" and isinstance(value, m[name].Tensor):  # type: ignore
             value = value.detach().numpy()
         elif name == "tensorflow" and isinstance(value, m[name].Tensor):  # type: ignore
             value = value.numpy()
         if (name == "jax" or name == "jaxlib") and isinstance(value, m["jax"].numpy.ndarray):  # type: ignore
             value = np.array(value)
         if _backend == "torch":
             import torch
+
             value = torch.from_numpy(value)
         elif _backend == "tensorflow":
             import tensorflow
+
             value = tensorflow.convert_to_tensor(value)
         elif _backend == "jax":
             import jax.numpy as jnp
+
             value = jnp.array(value)
     return ep.astensor(value)
 
 
+def istensor(value, _allow_explanation=False) -> bool:
+    if value.__class__.__name__ == "Explainable" and not _allow_explanation:
+        value = value.value
+    if (
+        "tensor" not in value.__class__.__name__.lower()
+        and "array" not in value.__class__.__name__.lower()
+    ):
+        return False
+    return True
+
+
 def astensor(value, _allow_explanation=False) -> ep.Tensor:
     if value.__class__.__name__ == "Explainable" and not _allow_explanation:
         value = value.value
     if (
         "tensor" not in value.__class__.__name__.lower()
         and "array" not in value.__class__.__name__.lower()
     ):
@@ -48,28 +64,29 @@
     if isinstance(value, list):
         value = np.array(value, dtype=np.float)
     value = tobackend(value)
     if value.ndim != 0:
         value = value.flatten()
     return value.float64()
 
+
 def fromtensor(value):
     # TODO: maybe applying this as a wrapper to methods instead of submitting to dask can be faster
     if isinstance(value, ep.Tensor):
         return value.raw
 
     return value
 
 
 class Fork(object):
     def __init__(self, *args, **branches):
         for arg in args:
             if not isinstance(arg, dict):
                 raise TypeError(
-                    "Forks can only support dicts of branches as positional arguments"
+                    "Forks can only support dicts (holding branch values) as positional arguments"
                 )
             for k, v in arg.items():
                 if k in branches:
                     raise TypeError(f"Branch {k} provided multiple times")
                 branches[k] = v
         self._branches = branches
 
@@ -369,14 +386,46 @@
                 + str(e)
                 + " branch that other inputs have"
             )
 
     return wrapper
 
 
+def multibranch_tensors(method):
+    @wraps(method)
+    def wrapper(*args, **kwargs):
+        branches = set(
+            [
+                branch
+                for arg in list(args) + list(kwargs.values())
+                if isinstance(arg, Fork)
+                for branch in arg._branches
+            ]
+        )
+        if not branches:
+            raise Exception(
+                f"Method {method} annotated as @multibranch_tensors and requires at least one Fork input"
+            )
+        args = [
+            arg
+            if isinstance(arg, Fork) or not istensor(arg, True)
+            else Fork(**{branch: astensor(arg) for branch in branches})
+            for arg in args
+        ]
+        kwargs = {
+            key: arg
+            if isinstance(arg, Fork) or not istensor(arg)
+            else Fork(**{branch: astensor(arg) for branch in branches})
+            for key, arg in kwargs.items()
+        }
+        return method(*args, **kwargs)
+
+    return wrapper
+
+
 def combine(*args):
     ret = {}
     for arg in args:
         assert isinstance(arg, Fork)
         ret |= arg._branches
     return Fork(ret)
```

## fairbench/reports/adhoc.py

```diff
@@ -2,48 +2,42 @@
 from fairbench.reports import reduction as fb
 from fairbench.reports.accumulate import kwargs as tokwargs
 from fairbench.forks.fork import combine
 from fairbench.reports.surrogate import surrogate_positives
 from fairbench import metrics
 
 
-def accreport(*args, **kwargs):
-    return report(
-        *args,
-        metrics=(metrics.accuracy, metrics.pr, metrics.tpr, metrics.tnr),
-        **kwargs
-    )
+common_metrics = (metrics.accuracy, metrics.prule, metrics.dfpr, metrics.dfnr)
 
 
-def binreport(*args, **kwargs):
-    return report(
-        *args,
-        metrics=(metrics.accuracy, metrics.prule, metrics.dfpr, metrics.dfnr),
-        **kwargs
-    )
+def accreport(*args, metrics=common_metrics, **kwargs):
+    return report(*args, metrics=metrics, **kwargs)
 
 
-def multireport(*args, **kwargs):
-    base = report(
-        *args,
-        metrics=(metrics.accuracy, metrics.pr, metrics.tpr, metrics.tnr),
-        **kwargs
-    )
+def binreport(*args, metrics=common_metrics, **kwargs):
+    return report(*args, metrics=metrics, **kwargs)
+
+
+def multireport(*args, metrics=common_metrics, **kwargs):
+    base = report(*args, metrics=metrics, **kwargs)
     return combine(
         fb.reduce(base, fb.mean),
         fb.reduce(base, fb.min, expand=fb.ratio),
         fb.reduce(base, fb.max, expand=fb.diff),
     )
 
 
 def isecreport(*args, **kwargs):
-    params = dict()
-    for arg in args:
-        params = params | arg
-    params = params | kwargs
+    if len(args) == 0:
+        params = tokwargs(**kwargs)
+    else:
+        params = dict()
+        for arg in args:
+            params = params | arg
+        params = params | kwargs
 
     bayesian = fb.reduce(
         surrogate_positives(params["predictions"], params["sensitive"]),
         fb.min,
         fb.ratio,
         name="bayesian",
     )
```

## fairbench/reports/surrogate.py

```diff
@@ -1,15 +1,15 @@
 from fairbench.reports import reduce, todata, identical
-from fairbench.forks.fork import Fork
+from fairbench.forks.fork import Fork, multibranch_tensors
 from sklearn.linear_model import LogisticRegression
 import numpy as np
 
 
+@multibranch_tensors
 def surrogate_positives(predictions, sensitive, surrogate_model=LogisticRegression()):
-    assert isinstance(sensitive, Fork)
     predictions = np.round(reduce(predictions, identical, name=None).numpy())
     X = reduce(sensitive, todata, name=None).numpy()
     surrogate_model = surrogate_model.fit(X, predictions)
     prediction_branches = dict()
     for branches in sensitive.intersections():
         Xbranch = np.array(
             [[1 if branch in branches else 0 for branch in sensitive._branches]]
```

## Comparing `fairbench-0.1.2.dist-info/METADATA` & `fairbench-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbench
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fairness model assessment framework
 Home-page: https://github.com/maniospas/FairBench
 Author: Emmanouil (Manios) Krasanakis
 Author-email: maniospas@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

