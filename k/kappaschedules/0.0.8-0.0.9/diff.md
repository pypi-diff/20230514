# Comparing `tmp/kappaschedules-0.0.8.tar.gz` & `tmp/kappaschedules-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappaschedules-0.0.8.tar", last modified: Sun Feb 19 20:57:14 2023, max compression
+gzip compressed data, was "kappaschedules-0.0.9.tar", last modified: Thu Mar 16 19:24:00 2023, max compression
```

## Comparing `kappaschedules-0.0.8.tar` & `kappaschedules-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:57:14.637964 kappaschedules-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-19 20:57:14.637964 kappaschedules-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:57:14.633964 kappaschedules-0.0.8/kappaschedules/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-19 20:56:58.000000 kappaschedules-0.0.8/kappaschedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:57:14.637964 kappaschedules-0.0.8/kappaschedules/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:57:14.637964 kappaschedules-0.0.8/kappaschedules/schedules/base/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/base/decreasing_progress_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/base/increasing_progress_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/base/progress_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/base/schedule_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/constant_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/cosine_decreasing_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/cosine_increasing_schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:57:14.637964 kappaschedules-0.0.8/kappaschedules/schedules/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/functional/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/inverse_sqrt_decreasing_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/inverse_sqrt_increasing_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/linear_decreasing_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/linear_increasing_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/sequential_percent_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/sequential_step_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/step_fixed_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/kappaschedules/schedules/step_interval_schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:57:14.637964 kappaschedules-0.0.8/kappaschedules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-19 20:57:14.000000 kappaschedules-0.0.8/kappaschedules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-19 20:57:14.000000 kappaschedules-0.0.8/kappaschedules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 20:57:14.000000 kappaschedules-0.0.8/kappaschedules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-19 20:57:14.000000 kappaschedules-0.0.8/kappaschedules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-19 20:56:53.000000 kappaschedules-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-19 20:57:14.637964 kappaschedules-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:24:00.566570 kappaschedules-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-16 19:24:00.566570 kappaschedules-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:24:00.558570 kappaschedules-0.0.9/kappaschedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-16 19:23:43.000000 kappaschedules-0.0.9/kappaschedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:24:00.562570 kappaschedules-0.0.9/kappaschedules/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:24:00.566570 kappaschedules-0.0.9/kappaschedules/schedules/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/base/decreasing_progress_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/base/increasing_progress_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/base/progress_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/base/schedule_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/constant_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/cosine_decreasing_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/cosine_increasing_schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:24:00.566570 kappaschedules-0.0.9/kappaschedules/schedules/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/functional/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/inverse_sqrt_decreasing_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/inverse_sqrt_increasing_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/linear_decreasing_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/linear_increasing_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/sequential_percent_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/sequential_step_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/step_fixed_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/kappaschedules/schedules/step_interval_schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 19:24:00.558570 kappaschedules-0.0.9/kappaschedules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-16 19:24:00.000000 kappaschedules-0.0.9/kappaschedules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-16 19:24:00.000000 kappaschedules-0.0.9/kappaschedules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 19:24:00.000000 kappaschedules-0.0.9/kappaschedules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-16 19:24:00.000000 kappaschedules-0.0.9/kappaschedules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-16 19:23:38.000000 kappaschedules-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-16 19:24:00.566570 kappaschedules-0.0.9/setup.cfg
```

### Comparing `kappaschedules-0.0.8/LICENSE` & `kappaschedules-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kappaschedules-0.0.8/PKG-INFO` & `kappaschedules-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: kappaschedules
-Version: 0.0.8
+Version: 0.0.9
 Summary: schedules
 Home-page: https://github.com/BenediktAlkin/KappaSchedules
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaSchedules
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaSchedules/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KappaSchedules
+
+[![publish](https://github.com/BenediktAlkin/KappaSchedules/actions/workflows/publish.yaml/badge.svg)](https://github.com/BenediktAlkin/KappaSchedules/actions/workflows/publish.yaml)
```

### Comparing `kappaschedules-0.0.8/kappaschedules/__init__.py` & `kappaschedules-0.0.9/kappaschedules/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 # base
 from kappaschedules.schedules.base.schedule_base import ScheduleBase
 #
 from .schedules.constant_schedule import ConstantSchedule
 from .schedules.cosine_decreasing_schedule import CosineDecreasingSchedule
 from .schedules.cosine_increasing_schedule import CosineIncreasingSchedule
```

### Comparing `kappaschedules-0.0.8/kappaschedules/factory.py` & `kappaschedules-0.0.9/kappaschedules/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     SequentialStepSchedule,
     SequentialStepScheduleConfig,
 )
 from .schedules.base import ScheduleBase
 import inspect
 from copy import deepcopy
 
-def object_to_schedule(obj) -> ScheduleBase:
+def object_to_schedule(obj, **kwargs) -> ScheduleBase:
     if obj is None:
         return None
     if not isinstance(obj, (list, dict)):
         assert isinstance(obj, ScheduleBase)
         return obj
 
     # implicit sequential schedule
@@ -38,17 +38,17 @@
         else:
             raise NotImplementedError
 
         # sequential schedule
         schedule_configs = []
         for schedule_config in obj:
             assert "schedule" in schedule_config
-            schedule = object_to_schedule(schedule_config["schedule"])
-            kwargs = {k: v for k, v in schedule_config.items() if k != "schedule"}
-            schedule_configs.append(config_ctor(schedule=schedule, **kwargs))
+            schedule = object_to_schedule(schedule_config["schedule"], **kwargs)
+            cfg_kwargs = {k: v for k, v in schedule_config.items() if k != "schedule"}
+            schedule_configs.append(config_ctor(schedule=schedule, **cfg_kwargs))
         return ctor(schedule_configs)
 
     # single schedules
     assert "kind" in obj and isinstance(obj["kind"], str)
     obj = deepcopy(obj)
     kind = obj.pop("kind")
 
@@ -65,15 +65,15 @@
 
     # create SequentialScheduleConfig objects
     if ctor == SequentialPercentSchedule:
         obj["schedule_configs"] = _obj_to_schedule_configs(obj["schedule_configs"], SequentialPercentScheduleConfig)
     elif ctor == SequentialStepSchedule:
         obj["schedule_configs"] = _obj_to_schedule_configs(obj["schedule_configs"], SequentialStepScheduleConfig)
 
-    return ctor(**obj)
+    return ctor(**obj, **kwargs)
 
 def _obj_to_schedule_configs(obj, config_ctor):
     schedule_configs = []
     for schedule_config in obj:
         schedule = object_to_schedule(schedule_config.pop("schedule"))
         schedule_configs.append(config_ctor(schedule=schedule, **schedule_config))
     return schedule_configs
```

### Comparing `kappaschedules-0.0.8/kappaschedules/schedules/__init__.py` & `kappaschedules-0.0.9/kappaschedules/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `kappaschedules-0.0.8/kappaschedules/schedules/base/progress_schedule.py` & `kappaschedules-0.0.9/kappaschedules/schedules/base/progress_schedule.py`

 * *Files identical despite different names*

### Comparing `kappaschedules-0.0.8/kappaschedules/schedules/base/schedule_base.py` & `kappaschedules-0.0.9/kappaschedules/schedules/base/schedule_base.py`

 * *Files identical despite different names*

### Comparing `kappaschedules-0.0.8/kappaschedules/schedules/functional/schedules.py` & `kappaschedules-0.0.9/kappaschedules/schedules/functional/schedules.py`

 * *Files identical despite different names*

### Comparing `kappaschedules-0.0.8/kappaschedules/schedules/sequential_percent_schedule.py` & `kappaschedules-0.0.9/kappaschedules/schedules/sequential_percent_schedule.py`

 * *Files identical despite different names*

### Comparing `kappaschedules-0.0.8/kappaschedules/schedules/sequential_step_schedule.py` & `kappaschedules-0.0.9/kappaschedules/schedules/sequential_step_schedule.py`

 * *Files identical despite different names*

### Comparing `kappaschedules-0.0.8/kappaschedules/schedules/step_fixed_schedule.py` & `kappaschedules-0.0.9/kappaschedules/schedules/step_fixed_schedule.py`

 * *Files identical despite different names*

### Comparing `kappaschedules-0.0.8/kappaschedules/schedules/step_interval_schedule.py` & `kappaschedules-0.0.9/kappaschedules/schedules/step_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `kappaschedules-0.0.8/kappaschedules.egg-info/PKG-INFO` & `kappaschedules-0.0.9/kappaschedules.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: kappaschedules
-Version: 0.0.8
+Version: 0.0.9
 Summary: schedules
 Home-page: https://github.com/BenediktAlkin/KappaSchedules
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaSchedules
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaSchedules/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KappaSchedules
+
+[![publish](https://github.com/BenediktAlkin/KappaSchedules/actions/workflows/publish.yaml/badge.svg)](https://github.com/BenediktAlkin/KappaSchedules/actions/workflows/publish.yaml)
```

### Comparing `kappaschedules-0.0.8/kappaschedules.egg-info/SOURCES.txt` & `kappaschedules-0.0.9/kappaschedules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kappaschedules-0.0.8/setup.cfg` & `kappaschedules-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.8
+version = 0.0.9
 name = kappaschedules
 description = schedules
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BenediktAlkin/KappaSchedules
 project_urls = 
 	Source Code = https://github.com/BenediktAlkin/KappaSchedules
```

