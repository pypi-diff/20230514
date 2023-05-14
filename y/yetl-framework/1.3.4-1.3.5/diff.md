# Comparing `tmp/yetl-framework-1.3.4.tar.gz` & `tmp/yetl-framework-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.3.4.tar", last modified: Sat May 13 19:49:17 2023, max compression
+gzip compressed data, was "yetl-framework-1.3.5.tar", last modified: Sun May 14 09:17:12 2023, max compression
```

## Comparing `yetl-framework-1.3.4.tar` & `yetl-framework-1.3.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-13 19:49:17.833384 yetl-framework-1.3.4/
--rw-r--r--   0 vsts      (1001) docker     (123)     5196 2023-05-13 19:49:17.833384 yetl-framework-1.3.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4699 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-13 19:49:17.833384 yetl-framework-1.3.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-13 19:49:17.829384 yetl-framework-1.3.4/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      895 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-13 19:49:17.829384 yetl-framework-1.3.4/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-13 19:49:17.829384 yetl-framework-1.3.4/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3284 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7948 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-13 19:49:17.829384 yetl-framework-1.3.4/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4195 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4935 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3671 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-13 19:49:17.833384 yetl-framework-1.3.4/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-13 19:48:28.000000 yetl-framework-1.3.4/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-13 19:49:17.833384 yetl-framework-1.3.4/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5196 2023-05-13 19:49:17.000000 yetl-framework-1.3.4/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      902 2023-05-13 19:49:17.000000 yetl-framework-1.3.4/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-13 19:49:17.000000 yetl-framework-1.3.4/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-13 19:49:17.000000 yetl-framework-1.3.4/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       29 2023-05-13 19:49:17.000000 yetl-framework-1.3.4/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-13 19:49:17.000000 yetl-framework-1.3.4/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5196 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4699 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1112 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.422930 yetl-framework-1.3.5/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      895 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.422930 yetl-framework-1.3.5/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      558 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3284 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7948 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4195 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1162 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5245 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3671 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      114 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-14 09:16:19.000000 yetl-framework-1.3.5/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 09:17:12.426930 yetl-framework-1.3.5/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5196 2023-05-14 09:17:12.000000 yetl-framework-1.3.5/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      902 2023-05-14 09:17:12.000000 yetl-framework-1.3.5/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 09:17:12.000000 yetl-framework-1.3.5/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 09:17:12.000000 yetl-framework-1.3.5/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       29 2023-05-14 09:17:12.000000 yetl-framework-1.3.5/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-14 09:17:12.000000 yetl-framework-1.3.5/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.3.4/PKG-INFO` & `yetl-framework-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.3.4
+Version: 1.3.5
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.3.4/README.md` & `yetl-framework-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/setup.py` & `yetl-framework-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.3.4",
+    version="1.3.5",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.3.4/yetl/__main__.py` & `yetl-framework-1.3.5/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/cli/_init.py` & `yetl-framework-1.3.5/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/__init__.py` & `yetl-framework-1.3.5/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/_config.py` & `yetl-framework-1.3.5/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/_decorators.py` & `yetl-framework-1.3.5/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/_logging_config.py` & `yetl-framework-1.3.5/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/_project.py` & `yetl-framework-1.3.5/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/_spark_context.py` & `yetl-framework-1.3.5/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/_tables.py` & `yetl-framework-1.3.5/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/_timeslice.py` & `yetl-framework-1.3.5/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/_utils.py` & `yetl-framework-1.3.5/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/deltalake.py` & `yetl-framework-1.3.5/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/table/_deltalake.py` & `yetl-framework-1.3.5/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/table/_factory.py` & `yetl-framework-1.3.5/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/config/table/_read.py` & `yetl-framework-1.3.5/yetl/config/table/_read.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 from ._table import Table
 
 
 class TriggerType(Enum):
     File = "file"
 
 
+class SliceDateFormat(Enum):
+    FILENAME_DATE_FORMAT = JinjaVariables.FILENAME_DATE_FORMAT.value
+    PATH_DATE_FORMAT = JinjaVariables.PATH_DATE_FORMAT.value
+
+
 class Read(Table):
     _OPTION_CF_SCHEMA_HINTS = "cloudFiles.schemaHints"
     _OPTION_CORRUPT_RECORD_NAME = "columnNameOfCorruptRecord"
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
@@ -35,14 +40,16 @@
     filename_date_format: str = Field(...)
     path_date_format: str = Field(...)
     format: str = Field(...)
     spark_schema: Union[StructType, str] = Field(default=None)
     ddl: List[str] = Field(default=None)
     headerless_ddl: List[str] = Field(default=None)
     stage: StageType = Field(...)
+    slice_date: SliceDateFormat = Field(default=SliceDateFormat.FILENAME_DATE_FORMAT)
+    slice_date_column_name: str = Field(default="_slice_date")
 
     def _render(self):
         super()._render()
         self._replacements[
             JinjaVariables.FILENAME_DATE_FORMAT
         ] = self.timeslice.strftime(self.filename_date_format)
         self._replacements[JinjaVariables.PATH_DATE_FORMAT] = self.timeslice.strftime(
```

### Comparing `yetl-framework-1.3.4/yetl/config/table/_table.py` & `yetl-framework-1.3.5/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.3.5/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.3.4/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.3.5/yetl_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.3.4
+Version: 1.3.5
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.3.4/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.3.5/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

