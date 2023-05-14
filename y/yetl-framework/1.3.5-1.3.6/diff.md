# Comparing `tmp/yetl-framework-1.3.5.tar.gz` & `tmp/yetl-framework-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.3.5.tar", last modified: Sun May 14 09:17:12 2023, max compression
+gzip compressed data, was "yetl-framework-1.3.6.tar", last modified: Sun May 14 21:09:07 2023, max compression
```

## Comparing `yetl-framework-1.3.5.tar` & `yetl-framework-1.3.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/
--rw-r--r--   0 vsts      (1001) docker     (123)     5196 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4699 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.422930 yetl-framework-1.3.5/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      895 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.422930 yetl-framework-1.3.5/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3284 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7948 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4195 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5245 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3671 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5196 2023-05-14 09:17:12.000000 yetl-framework-1.3.5/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      902 2023-05-14 09:17:12.000000 yetl-framework-1.3.5/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 09:17:12.000000 yetl-framework-1.3.5/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 09:17:12.000000 yetl-framework-1.3.5/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       29 2023-05-14 09:17:12.000000 yetl-framework-1.3.5/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-14 09:17:12.000000 yetl-framework-1.3.5/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.044437 yetl-framework-1.3.6/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5196 2023-05-14 21:09:07.044437 yetl-framework-1.3.6/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4699 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-14 21:09:07.044437 yetl-framework-1.3.6/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.040437 yetl-framework-1.3.6/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      895 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.040437 yetl-framework-1.3.6/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.040437 yetl-framework-1.3.6/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3284 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7948 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.040437 yetl-framework-1.3.6/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4195 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6273 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3671 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.040437 yetl-framework-1.3.6/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-14 21:08:07.000000 yetl-framework-1.3.6/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 21:09:07.040437 yetl-framework-1.3.6/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5196 2023-05-14 21:09:06.000000 yetl-framework-1.3.6/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      902 2023-05-14 21:09:07.000000 yetl-framework-1.3.6/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 21:09:06.000000 yetl-framework-1.3.6/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 21:09:06.000000 yetl-framework-1.3.6/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       29 2023-05-14 21:09:06.000000 yetl-framework-1.3.6/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-14 21:09:06.000000 yetl-framework-1.3.6/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.3.5/PKG-INFO` & `yetl-framework-1.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.3.5
+Version: 1.3.6
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.3.5/README.md` & `yetl-framework-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/setup.py` & `yetl-framework-1.3.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.3.5",
+    version="1.3.6",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.3.5/yetl/__main__.py` & `yetl-framework-1.3.6/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/cli/_init.py` & `yetl-framework-1.3.6/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/__init__.py` & `yetl-framework-1.3.6/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/_config.py` & `yetl-framework-1.3.6/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/_decorators.py` & `yetl-framework-1.3.6/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/_logging_config.py` & `yetl-framework-1.3.6/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/_project.py` & `yetl-framework-1.3.6/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/_spark_context.py` & `yetl-framework-1.3.6/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/_tables.py` & `yetl-framework-1.3.6/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/_timeslice.py` & `yetl-framework-1.3.6/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/_utils.py` & `yetl-framework-1.3.6/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/deltalake.py` & `yetl-framework-1.3.6/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/table/_deltalake.py` & `yetl-framework-1.3.6/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/table/_factory.py` & `yetl-framework-1.3.6/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/config/table/_read.py` & `yetl-framework-1.3.6/yetl/config/table/_read.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from .._utils import JinjaVariables, render_jinja, get_ddl, load_schema, abs_config_path
 from typing import Any, Dict, List, Union
 from enum import Enum
 import os
 from pyspark.sql.types import StructType
 from pyspark.sql.streaming import StreamingQuery
 from pyspark.sql import DataFrame
+from pyspark.sql import functions as fn
 from .._stage_type import StageType
 from ._table import Table
+from ..deltalake import DeltaLakeFn
 
 
 class TriggerType(Enum):
     File = "file"
 
 
 class SliceDateFormat(Enum):
@@ -20,14 +22,40 @@
     PATH_DATE_FORMAT = JinjaVariables.PATH_DATE_FORMAT.value
 
 
 class Read(Table):
     _OPTION_CF_SCHEMA_HINTS = "cloudFiles.schemaHints"
     _OPTION_CORRUPT_RECORD_NAME = "columnNameOfCorruptRecord"
 
+    def add_timeslice(
+        self, df: DataFrame, filepath_column_name: str = "_metadata.file_path"
+    ):
+        if self.slice_date == SliceDateFormat.FILENAME_DATE_FORMAT:
+            date_format = self.path_date_format
+
+        if self.slice_date == SliceDateFormat.PATH_DATE_FORMAT:
+            date_format = self.filename_date_format
+
+        pattern = DeltaLakeFn.to_regex_search_pattern(date_format)
+        spark_format_string = DeltaLakeFn.to_spark_format_code(date_format)
+
+        df = (
+            df.withColumn(self.slice_date_column_name, fn.col(filepath_column_name))
+            .withColumn(
+                self.slice_date_column_name,
+                fn.regexp_extract(fn.col(self.slice_date_column_name), pattern, 0),
+            )
+            .withColumn(
+                self.slice_date_column_name,
+                fn.to_timestamp(self.slice_date_column_name, spark_format_string),
+            )
+        )
+
+        return df
+
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
         self._render()
         self.path = os.path.join(self.location, self.filename)
 
     _logger: Any = PrivateAttr(default=None)
```

### Comparing `yetl-framework-1.3.5/yetl/config/table/_table.py` & `yetl-framework-1.3.6/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.3.6/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.5/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.3.6/yetl_framework.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.3.5
+Version: 1.3.6
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.3.5/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.3.6/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

