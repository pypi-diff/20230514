# Comparing `tmp/pytheus-0.0.8.tar.gz` & `tmp/pytheus-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytheus-0.0.8.tar", last modified: Thu Apr 13 00:45:36 2023, max compression
+gzip compressed data, was "pytheus-0.0.9.tar", last modified: Sat Apr 15 09:54:15 2023, max compression
```

## Comparing `pytheus-0.0.8.tar` & `pytheus-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-13 00:45:36.964037 pytheus-0.0.8/
--rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.0.8/LICENSE
--rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-13 00:45:36.963844 pytheus-0.0.8/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)    12050 2023-04-12 19:36:26.000000 pytheus-0.0.8/README.md
--rw-r--r--   0 llandy     (501) staff       (20)     1089 2023-04-13 00:45:03.000000 pytheus-0.0.8/pyproject.toml
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-13 00:45:36.961103 pytheus-0.0.8/pytheus/
--rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.0.8/pytheus/__init__.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-13 00:45:36.962678 pytheus-0.0.8/pytheus/backends/
--rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.0.8/pytheus/backends/__init__.py
--rw-r--r--   0 llandy     (501) staff       (20)     4148 2023-04-04 00:38:41.000000 pytheus-0.0.8/pytheus/backends/base.py
--rw-r--r--   0 llandy     (501) staff       (20)     3142 2023-04-04 00:38:41.000000 pytheus-0.0.8/pytheus/backends/redis.py
--rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.0.8/pytheus/exceptions.py
--rw-r--r--   0 llandy     (501) staff       (20)     2058 2023-04-12 22:30:13.000000 pytheus-0.0.8/pytheus/exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    18655 2023-04-13 00:44:01.000000 pytheus-0.0.8/pytheus/metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     3051 2023-04-03 00:08:23.000000 pytheus-0.0.8/pytheus/registry.py
--rw-r--r--   0 llandy     (501) staff       (20)      230 2023-04-12 22:36:32.000000 pytheus-0.0.8/pytheus/utils.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-13 00:45:36.961861 pytheus-0.0.8/pytheus.egg-info/
--rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-13 00:45:36.000000 pytheus-0.0.8/pytheus.egg-info/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)      465 2023-04-13 00:45:36.000000 pytheus-0.0.8/pytheus.egg-info/SOURCES.txt
--rw-r--r--   0 llandy     (501) staff       (20)        1 2023-04-13 00:45:36.000000 pytheus-0.0.8/pytheus.egg-info/dependency_links.txt
--rw-r--r--   0 llandy     (501) staff       (20)      176 2023-04-13 00:45:36.000000 pytheus-0.0.8/pytheus.egg-info/requires.txt
--rw-r--r--   0 llandy     (501) staff       (20)        8 2023-04-13 00:45:36.000000 pytheus-0.0.8/pytheus.egg-info/top_level.txt
--rw-r--r--   0 llandy     (501) staff       (20)       38 2023-04-13 00:45:36.964082 pytheus-0.0.8/setup.cfg
--rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.0.8/setup.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-13 00:45:36.963477 pytheus-0.0.8/tests/
--rw-r--r--   0 llandy     (501) staff       (20)     5852 2023-04-12 22:30:37.000000 pytheus-0.0.8/tests/test_exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    22719 2023-04-13 00:36:59.000000 pytheus-0.0.8/tests/test_metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.0.8/tests/test_registry.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-15 09:54:15.198875 pytheus-0.0.9/
+-rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.0.9/LICENSE
+-rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-15 09:54:15.198684 pytheus-0.0.9/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)    12050 2023-04-12 19:36:26.000000 pytheus-0.0.9/README.md
+-rw-r--r--   0 llandy     (501) staff       (20)     1089 2023-04-15 09:53:06.000000 pytheus-0.0.9/pyproject.toml
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-15 09:54:15.184860 pytheus-0.0.9/pytheus/
+-rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.0.9/pytheus/__init__.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-15 09:54:15.186201 pytheus-0.0.9/pytheus/backends/
+-rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.0.9/pytheus/backends/__init__.py
+-rw-r--r--   0 llandy     (501) staff       (20)     4148 2023-04-04 00:38:41.000000 pytheus-0.0.9/pytheus/backends/base.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3142 2023-04-15 09:52:20.000000 pytheus-0.0.9/pytheus/backends/redis.py
+-rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.0.9/pytheus/exceptions.py
+-rw-r--r--   0 llandy     (501) staff       (20)     2058 2023-04-12 22:30:13.000000 pytheus-0.0.9/pytheus/exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    18841 2023-04-13 22:40:07.000000 pytheus-0.0.9/pytheus/metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3051 2023-04-03 00:08:23.000000 pytheus-0.0.9/pytheus/registry.py
+-rw-r--r--   0 llandy     (501) staff       (20)      568 2023-04-13 22:40:07.000000 pytheus-0.0.9/pytheus/utils.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-15 09:54:15.185633 pytheus-0.0.9/pytheus.egg-info/
+-rw-r--r--   0 llandy     (501) staff       (20)    12494 2023-04-15 09:54:15.000000 pytheus-0.0.9/pytheus.egg-info/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)      485 2023-04-15 09:54:15.000000 pytheus-0.0.9/pytheus.egg-info/SOURCES.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        1 2023-04-15 09:54:15.000000 pytheus-0.0.9/pytheus.egg-info/dependency_links.txt
+-rw-r--r--   0 llandy     (501) staff       (20)      176 2023-04-15 09:54:15.000000 pytheus-0.0.9/pytheus.egg-info/requires.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        8 2023-04-15 09:54:15.000000 pytheus-0.0.9/pytheus.egg-info/top_level.txt
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2023-04-15 09:54:15.198913 pytheus-0.0.9/setup.cfg
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.0.9/setup.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-15 09:54:15.198292 pytheus-0.0.9/tests/
+-rw-r--r--   0 llandy     (501) staff       (20)     5857 2023-04-13 22:30:11.000000 pytheus-0.0.9/tests/test_exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    23523 2023-04-13 22:40:07.000000 pytheus-0.0.9/tests/test_metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.0.9/tests/test_registry.py
+-rw-r--r--   0 llandy     (501) staff       (20)      349 2023-04-13 22:40:07.000000 pytheus-0.0.9/tests/test_utils.py
```

### Comparing `pytheus-0.0.8/LICENSE` & `pytheus-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.8/PKG-INFO` & `pytheus-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytheus
-Version: 0.0.8
+Version: 0.0.9
 Summary: playing with metrics
 Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
 Project-URL: Homepage, https://github.com/Llandy3d/pytheus
 Project-URL: Documentation, https://pythe.us
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pytheus-0.0.8/README.md` & `pytheus-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.8/pyproject.toml` & `pytheus-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytheus"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Llandy Riveron Del Risco", email="llandy3d@gmail.com" },
 ]
 description = "playing with metrics"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pytheus-0.0.8/pytheus/backends/base.py` & `pytheus-0.0.9/pytheus/backends/base.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.8/pytheus/backends/redis.py` & `pytheus-0.0.9/pytheus/backends/redis.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.8/pytheus/exposition.py` & `pytheus-0.0.9/pytheus/exposition.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.8/pytheus/metrics.py` & `pytheus-0.0.9/pytheus/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pytheus.backends import get_backend
 from pytheus.exceptions import (
     BucketException,
     LabelValidationException,
     UnobservableMetricException,
 )
 from pytheus.registry import REGISTRY, Collector, Registry
-from pytheus.utils import MetricType
+from pytheus.utils import InfFloat, MetricType
 
 Labels = dict[str, str]
 
 
 metric_name_re = re.compile(r"[a-zA-Z_:][a-zA-Z0-9_:]*")
 label_name_re = re.compile(r"[a-zA-Z_][a-zA-Z0-9_]*")
 
@@ -456,17 +456,22 @@
 
         sorted_buckets = sorted(buckets)
         if buckets != sorted_buckets:
             raise BucketException(
                 f"buckets values are not in sorted order. {buckets} != {sorted_buckets}"
             )
 
-        # +inf is required so we always add it
-        if buckets[-1] != float("inf"):
-            buckets.append(float("inf"))
+        # +Inf is required so we always add it
+        last_bucket_value = buckets[-1]
+        if isinstance(last_bucket_value, InfFloat):
+            pass
+        elif last_bucket_value == float("inf"):
+            buckets[-1] = InfFloat("inf")
+        else:
+            buckets.append(InfFloat("inf"))
 
         self._upper_bounds = buckets
 
         # create bucket values
         self._buckets = None
         self._sum = None
         self._count = None
```

### Comparing `pytheus-0.0.8/pytheus/registry.py` & `pytheus-0.0.9/pytheus/registry.py`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.8/pytheus.egg-info/PKG-INFO` & `pytheus-0.0.9/pytheus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytheus
-Version: 0.0.8
+Version: 0.0.9
 Summary: playing with metrics
 Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
 Project-URL: Homepage, https://github.com/Llandy3d/pytheus
 Project-URL: Documentation, https://pythe.us
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pytheus-0.0.8/tests/test_exposition.py` & `pytheus-0.0.9/tests/test_exposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,37 +53,37 @@
         registry = CollectorRegistry()
         REGISTRY.set_registry(registry)
 
         histogram = Histogram("hello", "world")
         histogram.observe(0.4)
         metrics_text = generate_metrics()
         assert metrics_text == (
-            '# HELP hello world\n# TYPE hello histogram\nhello_bucket{le="0.005"} 0.0\nhello_bucket{le="0.01"} 0.0\nhello_bucket{le="0.025"} 0.0\nhello_bucket{le="0.05"} 0.0\nhello_bucket{le="0.1"} 0.0\nhello_bucket{le="0.25"} 0.0\nhello_bucket{le="0.5"} 1.0\nhello_bucket{le="1"} 1.0\nhello_bucket{le="2.5"} 1.0\nhello_bucket{le="5"} 1.0\nhello_bucket{le="10"} 1.0\nhello_bucket{le="inf"} 1.0\nhello_sum 0.4\nhello_count 1.0\n'
+            '# HELP hello world\n# TYPE hello histogram\nhello_bucket{le="0.005"} 0.0\nhello_bucket{le="0.01"} 0.0\nhello_bucket{le="0.025"} 0.0\nhello_bucket{le="0.05"} 0.0\nhello_bucket{le="0.1"} 0.0\nhello_bucket{le="0.25"} 0.0\nhello_bucket{le="0.5"} 1.0\nhello_bucket{le="1"} 1.0\nhello_bucket{le="2.5"} 1.0\nhello_bucket{le="5"} 1.0\nhello_bucket{le="10"} 1.0\nhello_bucket{le="+Inf"} 1.0\nhello_sum 0.4\nhello_count 1.0\n'
         )
 
     def test_generate_metrics_histogram_with_labels(self):
         registry = CollectorRegistry()
         REGISTRY.set_registry(registry)
 
         histogram = Histogram("hello", "world", required_labels=["bob"])
         histogram_a = histogram.labels({"bob": "a"})
         histogram_b = histogram.labels({"bob": "b"})
         histogram_a.observe(0.4)
         histogram_b.observe(7)
         metrics_text = generate_metrics()
         assert metrics_text == (
-            '# HELP hello world\n# TYPE hello histogram\nhello_bucket{bob="a",le="0.005"} 0.0\nhello_bucket{bob="a",le="0.01"} 0.0\nhello_bucket{bob="a",le="0.025"} 0.0\nhello_bucket{bob="a",le="0.05"} 0.0\nhello_bucket{bob="a",le="0.1"} 0.0\nhello_bucket{bob="a",le="0.25"} 0.0\nhello_bucket{bob="a",le="0.5"} 1.0\nhello_bucket{bob="a",le="1"} 1.0\nhello_bucket{bob="a",le="2.5"} 1.0\nhello_bucket{bob="a",le="5"} 1.0\nhello_bucket{bob="a",le="10"} 1.0\nhello_bucket{bob="a",le="inf"} 1.0\nhello_sum{bob="a"} 0.4\nhello_count{bob="a"} 1.0\nhello_bucket{bob="b",le="0.005"} 0.0\nhello_bucket{bob="b",le="0.01"} 0.0\nhello_bucket{bob="b",le="0.025"} 0.0\nhello_bucket{bob="b",le="0.05"} 0.0\nhello_bucket{bob="b",le="0.1"} 0.0\nhello_bucket{bob="b",le="0.25"} 0.0\nhello_bucket{bob="b",le="0.5"} 0.0\nhello_bucket{bob="b",le="1"} 0.0\nhello_bucket{bob="b",le="2.5"} 0.0\nhello_bucket{bob="b",le="5"} 0.0\nhello_bucket{bob="b",le="10"} 1.0\nhello_bucket{bob="b",le="inf"} 1.0\nhello_sum{bob="b"} 7.0\nhello_count{bob="b"} 1.0\n'
+            '# HELP hello world\n# TYPE hello histogram\nhello_bucket{bob="a",le="0.005"} 0.0\nhello_bucket{bob="a",le="0.01"} 0.0\nhello_bucket{bob="a",le="0.025"} 0.0\nhello_bucket{bob="a",le="0.05"} 0.0\nhello_bucket{bob="a",le="0.1"} 0.0\nhello_bucket{bob="a",le="0.25"} 0.0\nhello_bucket{bob="a",le="0.5"} 1.0\nhello_bucket{bob="a",le="1"} 1.0\nhello_bucket{bob="a",le="2.5"} 1.0\nhello_bucket{bob="a",le="5"} 1.0\nhello_bucket{bob="a",le="10"} 1.0\nhello_bucket{bob="a",le="+Inf"} 1.0\nhello_sum{bob="a"} 0.4\nhello_count{bob="a"} 1.0\nhello_bucket{bob="b",le="0.005"} 0.0\nhello_bucket{bob="b",le="0.01"} 0.0\nhello_bucket{bob="b",le="0.025"} 0.0\nhello_bucket{bob="b",le="0.05"} 0.0\nhello_bucket{bob="b",le="0.1"} 0.0\nhello_bucket{bob="b",le="0.25"} 0.0\nhello_bucket{bob="b",le="0.5"} 0.0\nhello_bucket{bob="b",le="1"} 0.0\nhello_bucket{bob="b",le="2.5"} 0.0\nhello_bucket{bob="b",le="5"} 0.0\nhello_bucket{bob="b",le="10"} 1.0\nhello_bucket{bob="b",le="+Inf"} 1.0\nhello_sum{bob="b"} 7.0\nhello_count{bob="b"} 1.0\n'
         )
 
     def test_generate_metrics_histogram_with_labels_and_default_labels(self):
         registry = CollectorRegistry()
         REGISTRY.set_registry(registry)
 
         histogram = Histogram(
             "hello", "world", required_labels=["bob"], default_labels={"bob": "default"}
         )
         histogram = histogram.labels({"bob": "a"})
         histogram.observe(0.4)
         metrics_text = generate_metrics()
         assert metrics_text == (
-            '# HELP hello world\n# TYPE hello histogram\nhello_bucket{bob="a",le="0.005"} 0.0\nhello_bucket{bob="a",le="0.01"} 0.0\nhello_bucket{bob="a",le="0.025"} 0.0\nhello_bucket{bob="a",le="0.05"} 0.0\nhello_bucket{bob="a",le="0.1"} 0.0\nhello_bucket{bob="a",le="0.25"} 0.0\nhello_bucket{bob="a",le="0.5"} 1.0\nhello_bucket{bob="a",le="1"} 1.0\nhello_bucket{bob="a",le="2.5"} 1.0\nhello_bucket{bob="a",le="5"} 1.0\nhello_bucket{bob="a",le="10"} 1.0\nhello_bucket{bob="a",le="inf"} 1.0\nhello_sum{bob="a"} 0.4\nhello_count{bob="a"} 1.0\nhello_bucket{bob="default",le="0.005"} 0.0\nhello_bucket{bob="default",le="0.01"} 0.0\nhello_bucket{bob="default",le="0.025"} 0.0\nhello_bucket{bob="default",le="0.05"} 0.0\nhello_bucket{bob="default",le="0.1"} 0.0\nhello_bucket{bob="default",le="0.25"} 0.0\nhello_bucket{bob="default",le="0.5"} 0.0\nhello_bucket{bob="default",le="1"} 0.0\nhello_bucket{bob="default",le="2.5"} 0.0\nhello_bucket{bob="default",le="5"} 0.0\nhello_bucket{bob="default",le="10"} 0.0\nhello_bucket{bob="default",le="inf"} 0.0\nhello_sum{bob="default"} 0.0\nhello_count{bob="default"} 0.0\n'
+            '# HELP hello world\n# TYPE hello histogram\nhello_bucket{bob="a",le="0.005"} 0.0\nhello_bucket{bob="a",le="0.01"} 0.0\nhello_bucket{bob="a",le="0.025"} 0.0\nhello_bucket{bob="a",le="0.05"} 0.0\nhello_bucket{bob="a",le="0.1"} 0.0\nhello_bucket{bob="a",le="0.25"} 0.0\nhello_bucket{bob="a",le="0.5"} 1.0\nhello_bucket{bob="a",le="1"} 1.0\nhello_bucket{bob="a",le="2.5"} 1.0\nhello_bucket{bob="a",le="5"} 1.0\nhello_bucket{bob="a",le="10"} 1.0\nhello_bucket{bob="a",le="+Inf"} 1.0\nhello_sum{bob="a"} 0.4\nhello_count{bob="a"} 1.0\nhello_bucket{bob="default",le="0.005"} 0.0\nhello_bucket{bob="default",le="0.01"} 0.0\nhello_bucket{bob="default",le="0.025"} 0.0\nhello_bucket{bob="default",le="0.05"} 0.0\nhello_bucket{bob="default",le="0.1"} 0.0\nhello_bucket{bob="default",le="0.25"} 0.0\nhello_bucket{bob="default",le="0.5"} 0.0\nhello_bucket{bob="default",le="1"} 0.0\nhello_bucket{bob="default",le="2.5"} 0.0\nhello_bucket{bob="default",le="5"} 0.0\nhello_bucket{bob="default",le="10"} 0.0\nhello_bucket{bob="default",le="+Inf"} 0.0\nhello_sum{bob="default"} 0.0\nhello_count{bob="default"} 0.0\n'
         )
```

### Comparing `pytheus-0.0.8/tests/test_metrics.py` & `pytheus-0.0.9/tests/test_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pytheus.exceptions import (
     BucketException,
     LabelValidationException,
     UnobservableMetricException,
 )
 from pytheus.metrics import Counter, CustomCollector, Gauge, Histogram, _Metric, _MetricCollector
 from pytheus.registry import REGISTRY, CollectorRegistry
-from pytheus.utils import MetricType
+from pytheus.utils import InfFloat, MetricType
 
 
 @pytest.fixture
 def set_empty_registry():
     """
     As the REGISTRY object is global by default, we might have data from other tests.
     So with this fixture we just set a new empty one.
@@ -481,23 +481,39 @@
     def test_create_histogram_with_default_labels(self):
         Histogram("name", "desc", required_labels=["bob", "cat"])
 
     def test_histogram_fails_with_le_label(self):
         with pytest.raises(LabelValidationException):
             Histogram("name", "desc", required_labels=["bob", "le"])
 
-    def test_buckets_adds_inf_implicitly(self):
+    def test_buckets_adds_inf_implicitly_float_number(self):
         buckets = [0.2, 0.5, 1]
+        expected = [0.2, 0.5, 1, InfFloat("inf")]
         histogram = Histogram("name", "desc", buckets=buckets)
-        assert histogram._upper_bounds[-1] == float("inf")
+        assert histogram._upper_bounds == expected
+        assert isinstance(histogram._upper_bounds[-1], InfFloat)
+
+    def test_buckets_adds_inf_implicitly_float_inf(self):
+        buckets = [0.2, 0.5, 1, float("inf")]
+        expected = [0.2, 0.5, 1, InfFloat("inf")]
+        histogram = Histogram("name", "desc", buckets=buckets)
+        assert histogram._upper_bounds == expected
+        assert isinstance(histogram._upper_bounds[-1], InfFloat)
+
+    def test_buckets_adds_inf_implicitly_inf_float(self):
+        buckets = [0.2, 0.5, 1, InfFloat("inf")]
+        expected = [0.2, 0.5, 1, InfFloat("inf")]
+        histogram = Histogram("name", "desc", buckets=buckets)
+        assert histogram._upper_bounds == expected
+        assert isinstance(histogram._upper_bounds[-1], InfFloat)
 
     def test_buckets_with_sorted_order(self):
         buckets = [0.2, 0.5, 1]
         histogram = Histogram("name", "desc", buckets=buckets)
-        assert histogram._upper_bounds == buckets + [float("inf")]
+        assert histogram._upper_bounds == buckets + [InfFloat("inf")]
 
     def test_buckets_with_unsorted_order_fails(self):
         with pytest.raises(BucketException):
             Histogram("name", "desc", buckets=(0.2, 1, 0.5))
 
     def test_buckets_empty_uses_default_buckets(self):
         histogram = Histogram("name", "desc", buckets=[])
```

### Comparing `pytheus-0.0.8/tests/test_registry.py` & `pytheus-0.0.9/tests/test_registry.py`

 * *Files identical despite different names*

