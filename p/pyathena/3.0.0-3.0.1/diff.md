# Comparing `tmp/pyathena-3.0.0.tar.gz` & `tmp/pyathena-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyathena-3.0.0.tar", max compression
+gzip compressed data, was "pyathena-3.0.1.tar", max compression
```

## Comparing `pyathena-3.0.0.tar` & `pyathena-3.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1055 2023-05-04 18:42:17.601809 pyathena-3.0.0/LICENSE
--rw-r--r--   0        0        0    70055 2023-05-04 18:42:17.601809 pyathena-3.0.0/README.rst
--rw-r--r--   0        0        0     1923 2023-05-04 18:42:17.601809 pyathena-3.0.0/pyathena/__init__.py
--rw-r--r--   0        0        0       24 2023-05-04 18:42:17.601809 pyathena-3.0.0/pyathena/arrow/__init__.py
--rw-r--r--   0        0        0     5157 2023-05-04 18:42:17.601809 pyathena-3.0.0/pyathena/arrow/async_cursor.py
--rw-r--r--   0        0        0     2554 2023-05-04 18:42:17.601809 pyathena-3.0.0/pyathena/arrow/converter.py
--rw-r--r--   0        0        0     7250 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/arrow/cursor.py
--rw-r--r--   0        0        0     9529 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/arrow/result_set.py
--rw-r--r--   0        0        0     2421 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/arrow/util.py
--rw-r--r--   0        0        0     5373 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/async_cursor.py
--rw-r--r--   0        0        0    21136 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/common.py
--rw-r--r--   0        0        0    10416 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/connection.py
--rw-r--r--   0        0        0     4209 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/converter.py
--rw-r--r--   0        0        0     5722 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/cursor.py
--rw-r--r--   0        0        0      660 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/error.py
--rw-r--r--   0        0        0       24 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/fastparquet/__init__.py
--rw-r--r--   0        0        0     2439 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/fastparquet/util.py
--rw-r--r--   0        0        0       24 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/filesystem/__init__.py
--rw-r--r--   0        0        0    20474 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/filesystem/s3.py
--rw-r--r--   0        0        0     1216 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/filesystem/s3_object.py
--rw-r--r--   0        0        0     6571 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/formatter.py
--rw-r--r--   0        0        0    16886 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/model.py
--rw-r--r--   0        0        0      220 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/pandas/__init__.py
--rw-r--r--   0        0        0     5829 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/pandas/async_cursor.py
--rw-r--r--   0        0        0     1830 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/pandas/converter.py
--rw-r--r--   0        0        0     8327 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/pandas/cursor.py
--rw-r--r--   0        0        0    13377 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/pandas/result_set.py
--rw-r--r--   0        0        0     9822 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/pandas/util.py
--rw-r--r--   0        0        0        0 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/py.typed
--rw-r--r--   0        0        0    24126 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/result_set.py
--rw-r--r--   0        0        0       24 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      661 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/arrow.py
--rw-r--r--   0        0        0    36892 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/base.py
--rw-r--r--   0        0        0      884 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/pandas.py
--rw-r--r--   0        0        0     2638 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/requirements.py
--rw-r--r--   0        0        0      173 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/rest.py
--rw-r--r--   0        0        0     1210 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/types.py
--rw-r--r--   0        0        0      142 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/sqlalchemy/util.py
--rw-r--r--   0        0        0     1948 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyathena/util.py
--rw-r--r--   0        0        0     3482 2023-05-04 18:42:17.605810 pyathena-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    71494 1970-01-01 00:00:00.000000 pyathena-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-05-14 14:29:12.112188 pyathena-3.0.1/LICENSE
+-rw-r--r--   0        0        0    70055 2023-05-14 14:29:12.116188 pyathena-3.0.1/README.rst
+-rw-r--r--   0        0        0     1923 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/arrow/__init__.py
+-rw-r--r--   0        0        0     5157 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/arrow/async_cursor.py
+-rw-r--r--   0        0        0     2554 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/arrow/converter.py
+-rw-r--r--   0        0        0     7250 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/arrow/cursor.py
+-rw-r--r--   0        0        0     9755 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/arrow/result_set.py
+-rw-r--r--   0        0        0     2421 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/arrow/util.py
+-rw-r--r--   0        0        0     5373 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/async_cursor.py
+-rw-r--r--   0        0        0    21136 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/common.py
+-rw-r--r--   0        0        0    10416 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/connection.py
+-rw-r--r--   0        0        0     4209 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/converter.py
+-rw-r--r--   0        0        0     5722 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/cursor.py
+-rw-r--r--   0        0        0      660 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/error.py
+-rw-r--r--   0        0        0       24 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/fastparquet/__init__.py
+-rw-r--r--   0        0        0     2439 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/fastparquet/util.py
+-rw-r--r--   0        0        0       24 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/filesystem/__init__.py
+-rw-r--r--   0        0        0    20474 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/filesystem/s3.py
+-rw-r--r--   0        0        0     1216 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/filesystem/s3_object.py
+-rw-r--r--   0        0        0     6571 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/formatter.py
+-rw-r--r--   0        0        0    17085 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/model.py
+-rw-r--r--   0        0        0      220 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/pandas/__init__.py
+-rw-r--r--   0        0        0     5829 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/pandas/async_cursor.py
+-rw-r--r--   0        0        0     1830 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/pandas/converter.py
+-rw-r--r--   0        0        0     8327 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/pandas/cursor.py
+-rw-r--r--   0        0        0    13589 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/pandas/result_set.py
+-rw-r--r--   0        0        0     9822 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/pandas/util.py
+-rw-r--r--   0        0        0        0 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/py.typed
+-rw-r--r--   0        0        0    24537 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/result_set.py
+-rw-r--r--   0        0        0       24 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      661 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/arrow.py
+-rw-r--r--   0        0        0    36892 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/base.py
+-rw-r--r--   0        0        0      884 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0     2638 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0      173 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/rest.py
+-rw-r--r--   0        0        0     1210 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/types.py
+-rw-r--r--   0        0        0      142 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/sqlalchemy/util.py
+-rw-r--r--   0        0        0     1948 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyathena/util.py
+-rw-r--r--   0        0        0     3482 2023-05-14 14:29:12.116188 pyathena-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    71494 1970-01-01 00:00:00.000000 pyathena-3.0.1/PKG-INFO
```

### Comparing `pyathena-3.0.0/LICENSE` & `pyathena-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/README.rst` & `pyathena-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/__init__.py` & `pyathena-3.0.1/pyathena/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING, FrozenSet, Type
 
 from pyathena.error import *  # noqa
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection
 
-__version__: str = "3.0.0"
+__version__: str = "3.0.1"
 user_agent_extra: str = f"PyAthena/{__version__}"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 2
 paramstyle: str = "pyformat"
```

### Comparing `pyathena-3.0.0/pyathena/arrow/async_cursor.py` & `pyathena-3.0.1/pyathena/arrow/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/arrow/converter.py` & `pyathena-3.0.1/pyathena/arrow/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/arrow/cursor.py` & `pyathena-3.0.1/pyathena/arrow/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/arrow/result_set.py` & `pyathena-3.0.1/pyathena/arrow/result_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,21 @@
         import pyarrow as pa
         from pyarrow import csv
 
         if not self.output_location:
             raise ProgrammingError("OutputLocation is none or empty.")
         if not self.output_location.endswith((".csv", ".txt")):
             return pa.Table.from_pydict(dict())
+        if self.substatement_type and self.substatement_type.upper() in (
+            "UPDATE",
+            "DELETE",
+            "MERGE",
+            "VACUUM_TABLE",
+        ):
+            return pa.Table.from_pydict(dict())
         length = self._get_content_length()
         if length and self.output_location.endswith(".txt"):
             description = self.description if self.description else []
             column_names = [d[0] for d in description]
             read_opts = csv.ReadOptions(
                 skip_rows=0,
                 column_names=column_names,
```

### Comparing `pyathena-3.0.0/pyathena/arrow/util.py` & `pyathena-3.0.1/pyathena/arrow/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/async_cursor.py` & `pyathena-3.0.1/pyathena/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/common.py` & `pyathena-3.0.1/pyathena/common.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/connection.py` & `pyathena-3.0.1/pyathena/connection.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/converter.py` & `pyathena-3.0.1/pyathena/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/cursor.py` & `pyathena-3.0.1/pyathena/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/error.py` & `pyathena-3.0.1/pyathena/error.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/fastparquet/util.py` & `pyathena-3.0.1/pyathena/fastparquet/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/filesystem/s3.py` & `pyathena-3.0.1/pyathena/filesystem/s3.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/filesystem/s3_object.py` & `pyathena-3.0.1/pyathena/filesystem/s3_object.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/formatter.py` & `pyathena-3.0.1/pyathena/formatter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/model.py` & `pyathena-3.0.1/pyathena/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         self._query_id: Optional[str] = query_execution.get("QueryExecutionId", None)
         if not self._query_id:
             raise DataError("KeyError `QueryExecutionId`")
         self._query: Optional[str] = query_execution.get("Query", None)
         if not self._query:
             raise DataError("KeyError `Query`")
         self._statement_type: Optional[str] = query_execution.get("StatementType", None)
+        self._substatement_type: Optional[str] = query_execution.get("SubstatementType", None)
         self._work_group: Optional[str] = query_execution.get("WorkGroup", None)
         self._execution_parameters: List[str] = query_execution.get("ExecutionParameters", [])
 
         status = query_execution.get("Status", None)
         if not status:
             raise DataError("KeyError `Status`")
         self._state: Optional[str] = status.get("State", None)
@@ -122,14 +123,18 @@
         return self._query
 
     @property
     def statement_type(self) -> Optional[str]:
         return self._statement_type
 
     @property
+    def substatement_type(self) -> Optional[str]:
+        return self._substatement_type
+
+    @property
     def work_group(self) -> Optional[str]:
         return self._work_group
 
     @property
     def execution_parameters(self) -> List[str]:
         return self._execution_parameters
```

### Comparing `pyathena-3.0.0/pyathena/pandas/async_cursor.py` & `pyathena-3.0.1/pyathena/pandas/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/pandas/converter.py` & `pyathena-3.0.1/pyathena/pandas/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/pandas/cursor.py` & `pyathena-3.0.1/pyathena/pandas/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/pandas/result_set.py` & `pyathena-3.0.1/pyathena/pandas/result_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,14 +253,21 @@
     def _read_csv(self) -> Union["TextFileReader", "DataFrame"]:
         import pandas as pd
 
         if not self.output_location:
             raise ProgrammingError("OutputLocation is none or empty.")
         if not self.output_location.endswith((".csv", ".txt")):
             return pd.DataFrame()
+        if self.substatement_type and self.substatement_type.upper() in (
+            "UPDATE",
+            "DELETE",
+            "MERGE",
+            "VACUUM_TABLE",
+        ):
+            return pd.DataFrame()
         length = self._get_content_length()
         if length and self.output_location.endswith(".txt"):
             sep = "\t"
             header = None
             description = self.description if self.description else []
             names = [d[0] for d in description]
         elif length and self.output_location.endswith(".csv"):
```

### Comparing `pyathena-3.0.0/pyathena/pandas/util.py` & `pyathena-3.0.1/pyathena/pandas/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/result_set.py` & `pyathena-3.0.1/pyathena/result_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,20 @@
     @property
     def statement_type(self) -> Optional[str]:
         if not self._query_execution:
             return None
         return self._query_execution.statement_type
 
     @property
+    def substatement_type(self) -> Optional[str]:
+        if not self._query_execution:
+            return None
+        return self._query_execution.substatement_type
+
+    @property
     def work_group(self) -> Optional[str]:
         if not self._query_execution:
             return None
         return self._query_execution.work_group
 
     @property
     def execution_parameters(self) -> List[str]:
@@ -548,14 +554,21 @@
     def statement_type(self) -> Optional[str]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.statement_type
 
     @property
+    def substatement_type(self) -> Optional[str]:
+        if not self.has_result_set:
+            return None
+        result_set = cast(AthenaResultSet, self.result_set)
+        return result_set.substatement_type
+
+    @property
     def work_group(self) -> Optional[str]:
         if not self.has_result_set:
             return None
         result_set = cast(AthenaResultSet, self.result_set)
         return result_set.work_group
 
     @property
```

### Comparing `pyathena-3.0.0/pyathena/sqlalchemy/arrow.py` & `pyathena-3.0.1/pyathena/sqlalchemy/arrow.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/sqlalchemy/base.py` & `pyathena-3.0.1/pyathena/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/sqlalchemy/pandas.py` & `pyathena-3.0.1/pyathena/sqlalchemy/pandas.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/sqlalchemy/requirements.py` & `pyathena-3.0.1/pyathena/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/sqlalchemy/types.py` & `pyathena-3.0.1/pyathena/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyathena/util.py` & `pyathena-3.0.1/pyathena/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.0/pyproject.toml` & `pyathena-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyAthena"
-version = "3.0.0"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
+version = "3.0.1"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
 description = "Python DB API 2.0 (PEP 249) client for Amazon Athena"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyathena-3.0.0/PKG-INFO` & `pyathena-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyathena
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python DB API 2.0 (PEP 249) client for Amazon Athena
 Home-page: https://github.com/laughingman7743/PyAthena/
 License: MIT
 Author: laughingman7743
 Author-email: laughingman7743@gmail.com
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
```

