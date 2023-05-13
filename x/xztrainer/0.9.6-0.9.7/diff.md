# Comparing `tmp/xztrainer-0.9.6.tar.gz` & `tmp/xztrainer-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xztrainer-0.9.6.tar", max compression
+gzip compressed data, was "xztrainer-0.9.7.tar", max compression
```

## Comparing `xztrainer-0.9.6.tar` & `xztrainer-0.9.7.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      894 2023-05-07 23:51:55.750566 xztrainer-0.9.6/pyproject.toml
--rw-r--r--   0        0        0       46 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/__init__.py
--rw-r--r--   0        0        0      256 2023-03-14 15:54:26.631822 xztrainer-0.9.6/src/xztrainer/functional.py
--rw-r--r--   0        0        0     1414 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/logger/__init__.py
--rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/logger/compose.py
--rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/logger/null.py
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/logger/stream.py
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/logger/tensorboard.py
--rw-r--r--   0        0        0     1652 2023-05-07 23:51:35.263746 xztrainer-0.9.6/src/xztrainer/model.py
--rw-r--r--   0        0        0      743 2023-03-10 15:49:26.715934 xztrainer-0.9.6/src/xztrainer/rng.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 xztrainer-0.9.6/src/xztrainer/sampler.py
--rw-r--r--   0        0        0      409 2023-03-10 15:49:26.707934 xztrainer-0.9.6/src/xztrainer/setup_helper.py
--rw-r--r--   0        0        0    24069 2023-04-23 16:12:03.787658 xztrainer-0.9.6/src/xztrainer/xztrainer.py
--rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 xztrainer-0.9.6/setup.py
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 xztrainer-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0      894 2023-05-13 21:40:29.683483 xztrainer-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0       46 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/__init__.py
+-rw-r--r--   0        0        0      256 2023-03-14 15:54:26.631822 xztrainer-0.9.7/src/xztrainer/functional.py
+-rw-r--r--   0        0        0     1414 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/logger/__init__.py
+-rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/logger/compose.py
+-rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/logger/null.py
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/logger/stream.py
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/logger/tensorboard.py
+-rw-r--r--   0        0        0     1652 2023-05-07 23:51:35.263746 xztrainer-0.9.7/src/xztrainer/model.py
+-rw-r--r--   0        0        0      743 2023-03-10 15:49:26.715934 xztrainer-0.9.7/src/xztrainer/rng.py
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 xztrainer-0.9.7/src/xztrainer/sampler.py
+-rw-r--r--   0        0        0      409 2023-03-10 15:49:26.707934 xztrainer-0.9.7/src/xztrainer/setup_helper.py
+-rw-r--r--   0        0        0    24446 2023-05-13 21:39:53.718697 xztrainer-0.9.7/src/xztrainer/xztrainer.py
+-rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 xztrainer-0.9.7/PKG-INFO
```

### Comparing `xztrainer-0.9.6/pyproject.toml` & `xztrainer-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xztrainer"
-version = "0.9.6"
+version = "0.9.7"
 description = "A customizable training pipeline for PyTorch"
 authors = ["Maxim Afanasyev <mr.applexz@gmail.com>"]
 license = "MPL-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 tqdm = ">=4.62.3"
```

### Comparing `xztrainer-0.9.6/src/xztrainer/logger/__init__.py` & `xztrainer-0.9.7/src/xztrainer/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.6/src/xztrainer/logger/compose.py` & `xztrainer-0.9.7/src/xztrainer/logger/compose.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.6/src/xztrainer/logger/stream.py` & `xztrainer-0.9.7/src/xztrainer/logger/stream.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.6/src/xztrainer/logger/tensorboard.py` & `xztrainer-0.9.7/src/xztrainer/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.6/src/xztrainer/model.py` & `xztrainer-0.9.7/src/xztrainer/model.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.6/src/xztrainer/rng.py` & `xztrainer-0.9.7/src/xztrainer/rng.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.6/src/xztrainer/sampler.py` & `xztrainer-0.9.7/src/xztrainer/sampler.py`

 * *Files identical despite different names*

### Comparing `xztrainer-0.9.6/src/xztrainer/xztrainer.py` & `xztrainer-0.9.7/src/xztrainer/xztrainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,23 @@
             pin_memory=self.config.dataloader_pin_memory,
             **kwargs
         )
 
     def _calculate_reset_metrics(self, metrics: Dict[str, Metric]) -> Dict[str, float]:
         metric_values = {}
         for name, metric in metrics.items():
-            metric_values[name] = metric.compute()
+            metric_val = metric.compute()
+            metric_val_els = metric_val.numel()
+            if metric_val_els == 0:
+                raise ValueError(f'empty metric {name}')
+            elif metric_val_els == 1:
+                metric_values[name] = metric_val.item()
+            else:
+                for itm_i, itm in enumerate(metric_val.flatten()):
+                    metric_values[f'{name}_{itm_i}'] = itm.item()
             metric.reset()
         metric_values.update(self.trainable.calculate_composition_metrics(metric_values))
         return metric_values
 
     def _log_trainable(self, context: BaseTrainContext, metrics: Dict[str, Metric]):
         for k, v in self._calculate_reset_metrics(metrics).items():
             context.logger.log_scalar(k, v)
```

### Comparing `xztrainer-0.9.6/PKG-INFO` & `xztrainer-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xztrainer
-Version: 0.9.6
+Version: 0.9.7
 Summary: A customizable training pipeline for PyTorch
 License: MPL-2.0
 Author: Maxim Afanasyev
 Author-email: mr.applexz@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

