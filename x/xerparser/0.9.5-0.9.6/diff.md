# Comparing `tmp/xerparser-0.9.5.tar.gz` & `tmp/xerparser-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xerparser-0.9.5.tar", max compression
+gzip compressed data, was "xerparser-0.9.6.tar", max compression
```

## Comparing `xerparser-0.9.5.tar` & `xerparser-0.9.6.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0    35149 2022-12-01 15:49:57.970889 xerparser-0.9.5/LICENSE
--rw-r--r--   0        0        0     5337 2023-05-13 15:23:27.047734 xerparser-0.9.5/README.md
--rw-r--r--   0        0        0      743 2023-05-13 15:23:42.137735 xerparser-0.9.5/pyproject.toml
--rw-r--r--   0        0        0      962 2023-05-13 15:23:42.137735 xerparser-0.9.5/xerparser/__init__.py
--rw-r--r--   0        0        0      465 2023-02-28 20:42:52.646081 xerparser-0.9.5/xerparser/schemas/__init__.py
--rw-r--r--   0        0        0     2643 2023-02-28 20:42:52.646081 xerparser-0.9.5/xerparser/schemas/account.py
--rw-r--r--   0        0        0     3247 2023-02-11 15:33:31.113595 xerparser-0.9.5/xerparser/schemas/actvcode.py
--rw-r--r--   0        0        0     1547 2023-01-21 16:07:16.794727 xerparser-0.9.5/xerparser/schemas/actvtype.py
--rw-r--r--   0        0        0    11154 2023-03-01 21:29:00.499182 xerparser-0.9.5/xerparser/schemas/calendars.py
--rw-r--r--   0        0        0      957 2023-02-28 20:42:52.646081 xerparser-0.9.5/xerparser/schemas/ermhdr.py
--rw-r--r--   0        0        0     1367 2023-01-21 16:07:16.794727 xerparser-0.9.5/xerparser/schemas/findates.py
--rw-r--r--   0        0        0      749 2023-01-21 15:04:28.694740 xerparser-0.9.5/xerparser/schemas/memotype.py
--rw-r--r--   0        0        0     1094 2023-02-25 17:15:29.004002 xerparser-0.9.5/xerparser/schemas/pcattype.py
--rw-r--r--   0        0        0     3227 2023-02-25 17:15:29.004002 xerparser-0.9.5/xerparser/schemas/pcatval.py
--rw-r--r--   0        0        0     8779 2023-05-13 15:23:42.137735 xerparser-0.9.5/xerparser/schemas/project.py
--rw-r--r--   0        0        0     2897 2023-02-28 20:42:52.646081 xerparser-0.9.5/xerparser/schemas/projwbs.py
--rw-r--r--   0        0        0     1103 2023-02-28 20:42:52.646081 xerparser-0.9.5/xerparser/schemas/rsrc.py
--rw-r--r--   0        0        0     2970 2023-02-28 20:42:52.646081 xerparser-0.9.5/xerparser/schemas/schedoptions.py
--rw-r--r--   0        0        0    16573 2023-05-13 15:23:27.047734 xerparser-0.9.5/xerparser/schemas/task.py
--rw-r--r--   0        0        0     1462 2023-03-05 18:22:40.262912 xerparser-0.9.5/xerparser/schemas/taskfin.py
--rw-r--r--   0        0        0      805 2023-01-15 15:17:45.767878 xerparser-0.9.5/xerparser/schemas/taskmemo.py
--rw-r--r--   0        0        0     2019 2023-01-21 16:07:16.794727 xerparser-0.9.5/xerparser/schemas/taskpred.py
--rw-r--r--   0        0        0     5063 2023-05-13 15:23:27.047734 xerparser-0.9.5/xerparser/schemas/taskrsrc.py
--rw-r--r--   0        0        0     1927 2023-01-21 16:07:16.794727 xerparser-0.9.5/xerparser/schemas/trsrcfin.py
--rw-r--r--   0        0        0     1524 2023-02-28 20:42:52.646081 xerparser-0.9.5/xerparser/schemas/udftype.py
--rw-r--r--   0        0        0        0 2022-12-19 19:22:23.085011 xerparser-0.9.5/xerparser/scripts/__init__.py
--rw-r--r--   0        0        0     1548 2023-01-15 15:17:45.767878 xerparser-0.9.5/xerparser/scripts/dates.py
--rw-r--r--   0        0        0      402 2023-01-21 16:07:16.794727 xerparser-0.9.5/xerparser/scripts/decorators.py
--rw-r--r--   0        0        0        0 2022-12-19 19:22:23.085011 xerparser-0.9.5/xerparser/src/__init__.py
--rw-r--r--   0        0        0     2851 2023-05-13 15:23:27.047734 xerparser-0.9.5/xerparser/src/errors.py
--rw-r--r--   0        0        0     2377 2023-05-13 15:23:27.047734 xerparser-0.9.5/xerparser/src/parser.py
--rw-r--r--   0        0        0      769 2023-05-13 15:23:27.047734 xerparser-0.9.5/xerparser/src/validators.py
--rw-r--r--   0        0        0    11062 2023-05-13 15:23:42.137735 xerparser-0.9.5/xerparser/src/xer.py
--rw-r--r--   0        0        0     6464 1970-01-01 00:00:00.000000 xerparser-0.9.5/setup.py
--rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 xerparser-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-03 05:25:25.921903 xerparser-0.9.6/LICENSE
+-rw-r--r--   0        0        0     5337 2023-04-19 13:53:53.195483 xerparser-0.9.6/README.md
+-rw-r--r--   0        0        0      743 2023-05-14 15:40:28.944059 xerparser-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0      962 2023-05-14 15:40:28.944059 xerparser-0.9.6/xerparser/__init__.py
+-rw-r--r--   0        0        0      465 2023-03-01 00:04:03.499449 xerparser-0.9.6/xerparser/schemas/__init__.py
+-rw-r--r--   0        0        0     2643 2023-03-01 00:04:28.289431 xerparser-0.9.6/xerparser/schemas/account.py
+-rw-r--r--   0        0        0     3247 2023-02-06 03:09:28.587242 xerparser-0.9.6/xerparser/schemas/actvcode.py
+-rw-r--r--   0        0        0     1547 2023-01-25 01:32:05.201004 xerparser-0.9.6/xerparser/schemas/actvtype.py
+-rw-r--r--   0        0        0    11154 2023-03-01 03:39:04.104780 xerparser-0.9.6/xerparser/schemas/calendars.py
+-rw-r--r--   0        0        0      957 2023-03-01 00:04:28.289431 xerparser-0.9.6/xerparser/schemas/ermhdr.py
+-rw-r--r--   0        0        0     1367 2023-01-25 01:32:05.211004 xerparser-0.9.6/xerparser/schemas/findates.py
+-rw-r--r--   0        0        0      749 2023-01-16 21:15:50.835852 xerparser-0.9.6/xerparser/schemas/memotype.py
+-rw-r--r--   0        0        0     1094 2023-02-26 04:48:17.672946 xerparser-0.9.6/xerparser/schemas/pcattype.py
+-rw-r--r--   0        0        0     3227 2023-02-26 04:48:17.672946 xerparser-0.9.6/xerparser/schemas/pcatval.py
+-rw-r--r--   0        0        0     9136 2023-05-14 15:40:28.944059 xerparser-0.9.6/xerparser/schemas/project.py
+-rw-r--r--   0        0        0     2897 2023-03-01 00:04:03.499449 xerparser-0.9.6/xerparser/schemas/projwbs.py
+-rw-r--r--   0        0        0     1103 2023-03-01 00:04:03.499449 xerparser-0.9.6/xerparser/schemas/rsrc.py
+-rw-r--r--   0        0        0     2970 2023-03-01 00:04:28.289431 xerparser-0.9.6/xerparser/schemas/schedoptions.py
+-rw-r--r--   0        0        0    16573 2023-03-17 20:28:16.137376 xerparser-0.9.6/xerparser/schemas/task.py
+-rw-r--r--   0        0        0     1462 2023-03-06 00:43:40.451659 xerparser-0.9.6/xerparser/schemas/taskfin.py
+-rw-r--r--   0        0        0      805 2022-12-26 20:40:30.667590 xerparser-0.9.6/xerparser/schemas/taskmemo.py
+-rw-r--r--   0        0        0     2019 2023-01-25 01:32:05.211004 xerparser-0.9.6/xerparser/schemas/taskpred.py
+-rw-r--r--   0        0        0     5063 2023-03-17 20:28:16.137376 xerparser-0.9.6/xerparser/schemas/taskrsrc.py
+-rw-r--r--   0        0        0     1927 2023-01-25 01:32:05.211004 xerparser-0.9.6/xerparser/schemas/trsrcfin.py
+-rw-r--r--   0        0        0     1524 2023-03-01 00:04:03.499449 xerparser-0.9.6/xerparser/schemas/udftype.py
+-rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.6/xerparser/scripts/__init__.py
+-rw-r--r--   0        0        0     1548 2022-12-30 22:42:20.878909 xerparser-0.9.6/xerparser/scripts/dates.py
+-rw-r--r--   0        0        0      402 2023-01-25 01:32:05.211004 xerparser-0.9.6/xerparser/scripts/decorators.py
+-rw-r--r--   0        0        0        0 2022-12-21 14:16:15.278744 xerparser-0.9.6/xerparser/src/__init__.py
+-rw-r--r--   0        0        0     2851 2023-04-08 15:29:35.029582 xerparser-0.9.6/xerparser/src/errors.py
+-rw-r--r--   0        0        0     2377 2023-04-08 15:29:35.029582 xerparser-0.9.6/xerparser/src/parser.py
+-rw-r--r--   0        0        0      769 2023-04-08 15:29:35.029582 xerparser-0.9.6/xerparser/src/validators.py
+-rw-r--r--   0        0        0    10822 2023-05-14 15:40:28.944059 xerparser-0.9.6/xerparser/src/xer.py
+-rw-r--r--   0        0        0     6062 1970-01-01 00:00:00.000000 xerparser-0.9.6/PKG-INFO
```

### Comparing `xerparser-0.9.5/LICENSE` & `xerparser-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/README.md` & `xerparser-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/pyproject.toml` & `xerparser-0.9.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xerparser"
-version = "0.9.5"
+version = "0.9.6"
 description = "Parse a P6 .xer file to a Python object."
 authors = ["Jesse <code@seqmanagement.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 keywords = ["primavera", "p6", "xer", "schedule", "scheduling", "planning", "project management", "project controls"]
 repository = "https://github.com/jjCode01/xerparser"
```

### Comparing `xerparser-0.9.5/xerparser/__init__.py` & `xerparser-0.9.6/xerparser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.5"
+__version__ = "0.9.6"
 
 from xerparser.src.errors import find_xer_errors, CorruptXerFile
 from xerparser.src.parser import parser, file_reader
 from xerparser.src.xer import Xer
 from xerparser.schemas.actvcode import ACTVCODE
 from xerparser.schemas.actvtype import ACTVTYPE
 from xerparser.schemas.calendars import CALENDAR
```

### Comparing `xerparser-0.9.5/xerparser/schemas/account.py` & `xerparser-0.9.6/xerparser/schemas/account.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/actvcode.py` & `xerparser-0.9.6/xerparser/schemas/actvcode.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/actvtype.py` & `xerparser-0.9.6/xerparser/schemas/actvtype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/calendars.py` & `xerparser-0.9.6/xerparser/schemas/calendars.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/ermhdr.py` & `xerparser-0.9.6/xerparser/schemas/ermhdr.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/findates.py` & `xerparser-0.9.6/xerparser/schemas/findates.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/memotype.py` & `xerparser-0.9.6/xerparser/schemas/memotype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/pcattype.py` & `xerparser-0.9.6/xerparser/schemas/pcattype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/pcatval.py` & `xerparser-0.9.6/xerparser/schemas/pcatval.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/project.py` & `xerparser-0.9.6/xerparser/schemas/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from xerparser.schemas.calendars import CALENDAR
 from xerparser.schemas.projwbs import PROJWBS
 from xerparser.schemas.pcattype import PCATTYPE
 from xerparser.schemas.pcatval import PCATVAL
 from xerparser.schemas.schedoptions import SCHEDOPTIONS
 from xerparser.schemas.task import TASK
 from xerparser.schemas.taskpred import TASKPRED
+from xerparser.schemas.taskrsrc import TASKRSRC
 from xerparser.schemas.udftype import UDFTYPE
 from xerparser.scripts.decorators import rounded
 from xerparser.src.validators import datetime_or_none, str_or_none, date_format
 
 
 class PROJECT:
     """
@@ -99,14 +100,15 @@
         # manually set from other tables
         self.activity_codes: list[ACTVTYPE] = []
         self.calendars: list[CALENDAR] = []
         self.name: str = ""
         self.project_codes: dict[PCATTYPE, PCATVAL] = {}
         self.tasks: list[TASK] = []
         self.relationships: list[TASKPRED] = []
+        self.resources: list[TASKRSRC] = []
         self.wbs_nodes: list[PROJWBS] = []
         self.user_defined_fields: dict[UDFTYPE, Any] = {}
 
     def __str__(self) -> str:
         return f"{self.short_name} - {self.name}"
 
     def __getitem__(self, obj: Any):
@@ -119,15 +121,16 @@
         if isinstance(obj, PROJWBS):
             return self.wbs_by_path.get(obj.full_code)
 
     @cached_property
     @rounded()
     def actual_cost(self) -> float:
         """Sum of task resource actual costs"""
-        return sum(task.actual_cost for task in self.tasks)
+        return sum(res.act_total_cost for res in self.resources)
+        # return sum(task.actual_cost for task in self.tasks)
 
     @property
     def actual_duration(self) -> int:
         """Project actual duration in calendar days from start date to data date"""
         return max((0, (self.data_date - self.actual_start).days))
 
     @cached_property
@@ -137,15 +140,16 @@
             return self.plan_start_date
         return min((task.start for task in self.tasks))
 
     @cached_property
     @rounded()
     def budgeted_cost(self) -> float:
         """Sum of task resource budgeted costs"""
-        return sum(task.budgeted_cost for task in self.tasks)
+        return sum(res.target_cost for res in self.resources)
+        # return sum(task.budgeted_cost for task in self.tasks)
 
     @property
     @rounded(ndigits=4)
     def duration_percent(self) -> float:
         """Project duration percent complete"""
         if self.original_duration == 0:
             return 0.0
@@ -189,15 +193,16 @@
     def relationships_by_hash(self) -> dict[int, TASKPRED]:
         return {hash(rel): rel for rel in self.relationships}
 
     @cached_property
     @rounded()
     def remaining_cost(self) -> float:
         """Sum of task resource remaining costs"""
-        return sum(task.remaining_cost for task in self.tasks)
+        return sum(res.remain_cost for res in self.resources)
+        # return sum(task.remaining_cost for task in self.tasks)
 
     @property
     def remaining_duration(self) -> int:
         """Project remaining duration in calendar days from data date to finish date"""
         return max((0, (self.finish_date - self.data_date).days))
 
     @cached_property
@@ -223,15 +228,16 @@
     def tasks_by_code(self) -> dict[str, TASK]:
         return {task.task_code: task for task in self.tasks}
 
     @cached_property
     @rounded()
     def this_period_cost(self) -> float:
         """Sum of task resource this period costs"""
-        return sum(task.this_period_cost for task in self.tasks)
+        return sum(res.act_this_per_cost for res in self.resources)
+        # return sum(task.this_period_cost for task in self.tasks)
 
     @cached_property
     def wbs_by_path(self) -> dict[str, PROJWBS]:
         return {node.full_code: node for node in self.wbs_nodes}
 
     def planned_progress(self, before_date: datetime) -> dict[str, list[TASK]]:
         """All planned progress through a given date.
```

### Comparing `xerparser-0.9.5/xerparser/schemas/projwbs.py` & `xerparser-0.9.6/xerparser/schemas/projwbs.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/rsrc.py` & `xerparser-0.9.6/xerparser/schemas/rsrc.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/schedoptions.py` & `xerparser-0.9.6/xerparser/schemas/schedoptions.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/task.py` & `xerparser-0.9.6/xerparser/schemas/task.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/taskfin.py` & `xerparser-0.9.6/xerparser/schemas/taskfin.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/taskmemo.py` & `xerparser-0.9.6/xerparser/schemas/taskmemo.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/taskpred.py` & `xerparser-0.9.6/xerparser/schemas/taskpred.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/taskrsrc.py` & `xerparser-0.9.6/xerparser/schemas/taskrsrc.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/trsrcfin.py` & `xerparser-0.9.6/xerparser/schemas/trsrcfin.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/schemas/udftype.py` & `xerparser-0.9.6/xerparser/schemas/udftype.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/scripts/dates.py` & `xerparser-0.9.6/xerparser/scripts/dates.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/src/errors.py` & `xerparser-0.9.6/xerparser/src/errors.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/src/parser.py` & `xerparser-0.9.6/xerparser/src/parser.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/src/validators.py` & `xerparser-0.9.6/xerparser/src/validators.py`

 * *Files identical despite different names*

### Comparing `xerparser-0.9.5/xerparser/src/xer.py` & `xerparser-0.9.6/xerparser/src/xer.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,20 +170,14 @@
     def _set_proj_calendars(self) -> None:
         for project in self.projects.values():
             cal_list = []
             for cal in self.calendars.values():
                 if not cal.proj_id or cal.proj_id == project.uid:
                     cal_list.append(cal)
             project.calendars = cal_list
-        # clndr_group = groupby(sorted(self.calendars.values(), key=proj_key), proj_key)
-        # for proj_id, clndrs in clndr_group:
-        #     if proj := self.projects.get(proj_id):
-        #         proj.calendars = list(clndrs)
-        #     for proje in self.projects.values():
-        #         proje.calendars = list
 
     def _set_proj_codes(self) -> None:
         for proj_code in self.tables.get("PROJPCAT", []):
             proj = self.projects.get(proj_code["proj_id"])
             code = self.project_code_values.get(proj_code["proj_catg_id"])
             if proj and code:
                 proj.project_codes.update({code.code_type: code})
@@ -245,16 +239,18 @@
         self.projects[task_pred.proj_id].relationships.append(task_pred)
         return task_pred
 
     def _set_taskrsrc(self, **kwargs) -> None:
         rsrc = self.resources[kwargs["rsrc_id"]]
         account = self.accounts.get(kwargs["acct_id"])
         task = self.tasks[kwargs["task_id"]]
+        proj = self.projects[kwargs["proj_id"]]
         taskrsrc = TASKRSRC(resource=rsrc, account=account, **kwargs)
         task.resources.update({taskrsrc.uid: taskrsrc})
+        proj.resources.append(taskrsrc)
 
     def _set_taskfin(self, **kwargs) -> None:
         period = self.financial_periods[kwargs["fin_dates_id"]]
         task_fin = TASKFIN(period=period, **kwargs)
         self.tasks[task_fin.task_id].periods.append(task_fin)
 
     def _set_taskrsrc_fin(self, **kwargs) -> None:
```

### Comparing `xerparser-0.9.5/PKG-INFO` & `xerparser-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xerparser
-Version: 0.9.5
+Version: 0.9.6
 Summary: Parse a P6 .xer file to a Python object.
 Home-page: https://github.com/jjCode01/xerparser
 License: GPL-3.0-only
 Keywords: primavera,p6,xer,schedule,scheduling,planning,project management,project controls
 Author: Jesse
 Author-email: code@seqmanagement.com
 Requires-Python: >=3.10,<4.0
```

