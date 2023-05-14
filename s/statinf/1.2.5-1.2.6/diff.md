# Comparing `tmp/statinf-1.2.5.tar.gz` & `tmp/statinf-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statinf-1.2.5.tar", last modified: Fri May  5 14:18:57 2023, max compression
+gzip compressed data, was "statinf-1.2.6.tar", last modified: Sun May 14 17:41:12 2023, max compression
```

## Comparing `statinf-1.2.5.tar` & `statinf-1.2.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/
--rw-r--r--   0 florian   (1000) florian   (1000)     1070 2020-10-01 18:31:13.000000 statinf-1.2.5/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-05-05 14:18:57.601566 statinf-1.2.5/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     8337 2020-10-01 18:31:13.000000 statinf-1.2.5/README.md
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-05 14:18:57.601566 statinf-1.2.5/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)      781 2020-10-01 18:31:13.000000 statinf-1.2.5/setup.py
--rw-r--r--   0 florian   (1000) florian   (1000)      889 2023-05-05 14:18:57.000000 statinf-1.2.5/setup_new.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/
--rw-r--r--   0 florian   (1000) florian   (1000)       22 2023-05-05 14:18:57.000000 statinf-1.2.5/statinf/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/data/
--rw-r--r--   0 florian   (1000) florian   (1000)     2701 2023-02-03 18:48:52.000000 statinf-1.2.5/statinf/data/GenerateData.py
--rw-r--r--   0 florian   (1000) florian   (1000)    27132 2021-03-24 14:33:31.000000 statinf-1.2.5/statinf/data/ProcessData.py
--rw-r--r--   0 florian   (1000) florian   (1000)       55 2020-10-01 18:31:13.000000 statinf-1.2.5/statinf/data/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/distributions/
--rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-02-03 18:27:09.000000 statinf-1.2.5/statinf/distributions/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    25196 2023-05-05 14:18:00.000000 statinf-1.2.5/statinf/distributions/discrete.py
--rw-r--r--   0 florian   (1000) florian   (1000)       26 2021-06-27 12:48:10.000000 statinf-1.2.5/statinf/init_template.py
--rw-r--r--   0 florian   (1000) florian   (1000)     5107 2021-06-27 13:22:48.000000 statinf-1.2.5/statinf/misc.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/ml/
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2020-10-01 18:31:13.000000 statinf-1.2.5/statinf/ml/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2522 2021-03-07 06:24:49.000000 statinf-1.2.5/statinf/ml/activations.py
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-10-17 16:20:51.000000 statinf-1.2.5/statinf/ml/generative.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2892 2021-03-07 06:09:35.000000 statinf-1.2.5/statinf/ml/initializations.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3152 2021-03-07 06:45:42.000000 statinf-1.2.5/statinf/ml/losses.py
--rw-r--r--   0 florian   (1000) florian   (1000)    16863 2022-08-21 10:47:32.000000 statinf-1.2.5/statinf/ml/neuralnetwork.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11152 2021-03-07 08:40:43.000000 statinf-1.2.5/statinf/ml/optimizers.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6141 2021-06-27 13:22:59.000000 statinf-1.2.5/statinf/ml/performance.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/nonparametrics/
--rw-r--r--   0 florian   (1000) florian   (1000)       23 2020-11-01 11:38:35.000000 statinf-1.2.5/statinf/nonparametrics/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)      842 2020-11-01 18:05:22.000000 statinf-1.2.5/statinf/nonparametrics/kernels.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/regressions/
--rw-r--r--   0 florian   (1000) florian   (1000)    19249 2021-03-24 15:58:55.000000 statinf-1.2.5/statinf/regressions/LinearModels.py
--rw-r--r--   0 florian   (1000) florian   (1000)       51 2023-02-03 18:26:31.000000 statinf-1.2.5/statinf/regressions/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    18168 2021-03-24 15:54:37.000000 statinf-1.2.5/statinf/regressions/glm.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7060 2020-10-01 18:31:13.000000 statinf-1.2.5/statinf/regressions/glm_test.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf/stats/
--rw-r--r--   0 florian   (1000) florian   (1000)      126 2023-05-05 13:38:11.000000 statinf-1.2.5/statinf/stats/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6950 2020-11-01 18:03:36.000000 statinf-1.2.5/statinf/stats/bayesian.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4185 2020-10-01 18:31:13.000000 statinf-1.2.5/statinf/stats/descriptive.py
--rw-r--r--   0 florian   (1000) florian   (1000)    21520 2023-02-03 18:58:48.000000 statinf-1.2.5/statinf/stats/tests.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11524 2020-10-27 02:35:31.000000 statinf-1.2.5/statinf/stats/timeseries.py
--rw-r--r--   0 florian   (1000) florian   (1000)    10469 2020-11-01 18:02:58.000000 statinf-1.2.5/statinf/stats/unsupervised.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-05 14:18:57.601566 statinf-1.2.5/statinf.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-05-05 14:18:57.000000 statinf-1.2.5/statinf.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      966 2023-05-05 14:18:57.000000 statinf-1.2.5/statinf.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-05 14:18:57.000000 statinf-1.2.5/statinf.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      101 2023-05-05 14:18:57.000000 statinf-1.2.5/statinf.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-05 14:18:57.000000 statinf-1.2.5/statinf.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-14 17:41:12.462234 statinf-1.2.6/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1070 2020-10-01 18:31:13.000000 statinf-1.2.6/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-05-14 17:41:12.462234 statinf-1.2.6/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     8337 2020-10-01 18:31:13.000000 statinf-1.2.6/README.md
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-14 17:41:12.462234 statinf-1.2.6/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)      781 2020-10-01 18:31:13.000000 statinf-1.2.6/setup.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      889 2023-05-14 17:41:11.000000 statinf-1.2.6/setup_new.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-14 17:41:12.442234 statinf-1.2.6/statinf/
+-rw-r--r--   0 florian   (1000) florian   (1000)       22 2023-05-14 17:41:11.000000 statinf-1.2.6/statinf/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-14 17:41:12.442234 statinf-1.2.6/statinf/data/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2701 2023-02-03 18:48:52.000000 statinf-1.2.6/statinf/data/GenerateData.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    27132 2021-03-24 14:33:31.000000 statinf-1.2.6/statinf/data/ProcessData.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       55 2020-10-01 18:31:13.000000 statinf-1.2.6/statinf/data/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-14 17:41:12.442234 statinf-1.2.6/statinf/distributions/
+-rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-02-03 18:27:09.000000 statinf-1.2.6/statinf/distributions/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    25262 2023-05-14 17:30:24.000000 statinf-1.2.6/statinf/distributions/discrete.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       26 2021-06-27 12:48:10.000000 statinf-1.2.6/statinf/init_template.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     5107 2021-06-27 13:22:48.000000 statinf-1.2.6/statinf/misc.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-14 17:41:12.442234 statinf-1.2.6/statinf/ml/
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2020-10-01 18:31:13.000000 statinf-1.2.6/statinf/ml/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2522 2021-03-07 06:24:49.000000 statinf-1.2.6/statinf/ml/activations.py
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-10-17 16:20:51.000000 statinf-1.2.6/statinf/ml/generative.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2892 2021-03-07 06:09:35.000000 statinf-1.2.6/statinf/ml/initializations.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3152 2021-03-07 06:45:42.000000 statinf-1.2.6/statinf/ml/losses.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16863 2022-08-21 10:47:32.000000 statinf-1.2.6/statinf/ml/neuralnetwork.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11152 2021-03-07 08:40:43.000000 statinf-1.2.6/statinf/ml/optimizers.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6141 2021-06-27 13:22:59.000000 statinf-1.2.6/statinf/ml/performance.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-14 17:41:12.442234 statinf-1.2.6/statinf/nonparametrics/
+-rw-r--r--   0 florian   (1000) florian   (1000)       23 2020-11-01 11:38:35.000000 statinf-1.2.6/statinf/nonparametrics/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      842 2020-11-01 18:05:22.000000 statinf-1.2.6/statinf/nonparametrics/kernels.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-14 17:41:12.452234 statinf-1.2.6/statinf/regressions/
+-rw-r--r--   0 florian   (1000) florian   (1000)    19249 2021-03-24 15:58:55.000000 statinf-1.2.6/statinf/regressions/LinearModels.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       51 2023-02-03 18:26:31.000000 statinf-1.2.6/statinf/regressions/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    18168 2021-03-24 15:54:37.000000 statinf-1.2.6/statinf/regressions/glm.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7060 2020-10-01 18:31:13.000000 statinf-1.2.6/statinf/regressions/glm_test.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-14 17:41:12.462234 statinf-1.2.6/statinf/stats/
+-rw-r--r--   0 florian   (1000) florian   (1000)      126 2023-05-05 13:38:11.000000 statinf-1.2.6/statinf/stats/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6950 2020-11-01 18:03:36.000000 statinf-1.2.6/statinf/stats/bayesian.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4185 2020-10-01 18:31:13.000000 statinf-1.2.6/statinf/stats/descriptive.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    21520 2023-02-03 18:58:48.000000 statinf-1.2.6/statinf/stats/tests.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11524 2020-10-27 02:35:31.000000 statinf-1.2.6/statinf/stats/timeseries.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    10469 2020-11-01 18:02:58.000000 statinf-1.2.6/statinf/stats/unsupervised.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-14 17:41:12.442234 statinf-1.2.6/statinf.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-05-14 17:41:12.000000 statinf-1.2.6/statinf.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      966 2023-05-14 17:41:12.000000 statinf-1.2.6/statinf.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-14 17:41:12.000000 statinf-1.2.6/statinf.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      101 2023-05-14 17:41:12.000000 statinf-1.2.6/statinf.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-14 17:41:12.000000 statinf-1.2.6/statinf.egg-info/top_level.txt
```

### Comparing `statinf-1.2.5/LICENSE` & `statinf-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/PKG-INFO` & `statinf-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statinf
-Version: 1.2.5
+Version: 1.2.6
 Summary: A library for statistics and causal inference
 Home-page: https://www.florianfelice.com/statinf
 Author: Florian Felice
 Author-email: florian.felice@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statinf-1.2.5/README.md` & `statinf-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/setup.py` & `statinf-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/data/GenerateData.py` & `statinf-1.2.6/statinf/data/GenerateData.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/data/ProcessData.py` & `statinf-1.2.6/statinf/data/ProcessData.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/distributions/discrete.py` & `statinf-1.2.6/statinf/distributions/discrete.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,15 +309,15 @@
         self.j = j
 
         self._Z = None
 
         if (self.lambda_ is not None) & (self.nu_ is not None):
             assert self.lambda_ >= 0, ValueError('Value for parameter lambda must be strictly greater to 0 (lambda_ > 0)')
             assert self.nu_ >= 0, ValueError('Value for parameter nu must be greater or equal to 0 (nu_ >= 0)')
-            warnings.filterwarnings("error")
+            warnings.filterwarnings("ignore", message="overflow encountered")
             self._Z = self.Z(lambda_=self.lambda_, nu_=self.nu_, j=self.j)
             warnings.resetwarnings()
 
         self.nll_fun = lambda params, data, j: self.nloglike(params=params, data=data, j=j, Z=self.Z)
 
     def Z(self, lambda_, nu_, j=None, log=False) -> float:
         """Compute the :math:`Z` factor, normalizing constant.
@@ -455,18 +455,18 @@
         data = np.asarray(data)
         if bounds is None:
             bounds = [(self.eps, None), (self.eps, None)]
         if init_params == 'auto':
             _disp = data.mean() / data.var()
             init_params = np.array([data.mean(), _disp])
 
+        warnings.filterwarnings("ignore", message="overflow encountered")
         res = self._fit(data=data, bounds=bounds, method=method, init_params=init_params, args=(j,))
         self.lambda_ = res.x[0]
         self.nu_ = res.x[1]
-        warnings.filterwarnings("error")
         self._Z = self.Z(lambda_=self.lambda_, nu_=self.nu_, j=j)
         warnings.resetwarnings()
 
         out = {'lambda_': self.lambda_, 'nu_': self.nu_, 'convergence': res.success}
 
         if method in scipy_methods:
             out.update({'loglikelihood': self.ll})
```

### Comparing `statinf-1.2.5/statinf/misc.py` & `statinf-1.2.6/statinf/misc.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/ml/activations.py` & `statinf-1.2.6/statinf/ml/activations.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/ml/initializations.py` & `statinf-1.2.6/statinf/ml/initializations.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/ml/losses.py` & `statinf-1.2.6/statinf/ml/losses.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/ml/neuralnetwork.py` & `statinf-1.2.6/statinf/ml/neuralnetwork.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/ml/optimizers.py` & `statinf-1.2.6/statinf/ml/optimizers.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/ml/performance.py` & `statinf-1.2.6/statinf/ml/performance.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/nonparametrics/kernels.py` & `statinf-1.2.6/statinf/nonparametrics/kernels.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/regressions/LinearModels.py` & `statinf-1.2.6/statinf/regressions/LinearModels.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/regressions/glm.py` & `statinf-1.2.6/statinf/regressions/glm.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/regressions/glm_test.py` & `statinf-1.2.6/statinf/regressions/glm_test.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/stats/bayesian.py` & `statinf-1.2.6/statinf/stats/bayesian.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/stats/descriptive.py` & `statinf-1.2.6/statinf/stats/descriptive.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/stats/tests.py` & `statinf-1.2.6/statinf/stats/tests.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/stats/timeseries.py` & `statinf-1.2.6/statinf/stats/timeseries.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf/stats/unsupervised.py` & `statinf-1.2.6/statinf/stats/unsupervised.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.5/statinf.egg-info/PKG-INFO` & `statinf-1.2.6/statinf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statinf
-Version: 1.2.5
+Version: 1.2.6
 Summary: A library for statistics and causal inference
 Home-page: https://www.florianfelice.com/statinf
 Author: Florian Felice
 Author-email: florian.felice@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statinf-1.2.5/statinf.egg-info/SOURCES.txt` & `statinf-1.2.6/statinf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

