# Comparing `tmp/n0struct-0.2.96.tar.gz` & `tmp/n0struct-0.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\n0struct-0.2.96.tar", last modified: Sat May 13 12:24:15 2023, max compression
+gzip compressed data, was "dist\n0struct-0.2.97.tar", last modified: Sun May 14 20:42:10 2023, max compression
```

## Comparing `n0struct-0.2.96.tar` & `n0struct-0.2.97.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 12:24:15.367426 n0struct-0.2.96/
--rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.96/LICENSE
--rw-rw-rw-   0        0        0     1060 2023-05-13 12:24:15.368456 n0struct-0.2.96/PKG-INFO
--rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.96/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 12:24:15.335914 n0struct-0.2.96/n0struct/
--rw-rw-rw-   0        0        0      988 2023-05-13 11:12:54.000000 n0struct-0.2.96/n0struct/__init__.py
--rw-rw-rw-   0        0        0     3671 2023-05-12 12:43:36.000000 n0struct-0.2.96/n0struct/n0struct_arrays.py
--rw-rw-rw-   0        0        0     2104 2023-05-13 11:27:25.000000 n0struct-0.2.96/n0struct/n0struct_comprehensions.py
--rw-rw-rw-   0        0        0    13176 2023-04-25 08:08:57.000000 n0struct-0.2.96/n0struct/n0struct_date.py
--rw-rw-rw-   0        0        0     3389 2023-05-13 05:52:52.000000 n0struct-0.2.96/n0struct/n0struct_files.py
--rw-rw-rw-   0        0        0    29362 2023-05-13 11:55:07.000000 n0struct-0.2.96/n0struct/n0struct_files_csv.py
--rw-rw-rw-   0        0        0     7117 2023-05-13 11:56:28.000000 n0struct-0.2.96/n0struct/n0struct_files_fwf.py
--rw-rw-rw-   0        0        0    15648 2023-05-13 11:36:31.000000 n0struct-0.2.96/n0struct/n0struct_findall.py
--rw-rw-rw-   0        0        0     4070 2023-04-25 08:08:57.000000 n0struct-0.2.96/n0struct/n0struct_git.py
--rw-rw-rw-   0        0        0    20873 2023-05-13 12:00:24.000000 n0struct-0.2.96/n0struct/n0struct_logging.py
--rw-rw-rw-   0        0        0     2287 2023-04-25 08:08:57.000000 n0struct-0.2.96/n0struct/n0struct_mask.py
--rw-rw-rw-   0        0        0    12168 2023-04-25 08:08:57.000000 n0struct-0.2.96/n0struct/n0struct_n0dict_.py
--rw-rw-rw-   0        0        0    17116 2023-05-13 12:19:09.000000 n0struct-0.2.96/n0struct/n0struct_n0dict__.py
--rw-rw-rw-   0        0        0     7519 2023-05-13 11:50:12.000000 n0struct-0.2.96/n0struct/n0struct_n0list_.py
--rw-rw-rw-   0        0        0    75645 2023-05-13 12:22:04.000000 n0struct-0.2.96/n0struct/n0struct_n0list_n0dict.py
--rw-rw-rw-   0        0        0      917 2023-04-25 08:08:57.000000 n0struct-0.2.96/n0struct/n0struct_random.py
--rw-rw-rw-   0        0        0     3852 2023-04-25 08:08:57.000000 n0struct-0.2.96/n0struct/n0struct_references.py
--rw-rw-rw-   0        0        0     3235 2023-05-12 12:49:17.000000 n0struct-0.2.96/n0struct/n0struct_transform_structure.py
--rw-rw-rw-   0        0        0    18067 2023-05-13 12:20:41.000000 n0struct-0.2.96/n0struct/n0struct_utils.py
--rw-rw-rw-   0        0        0     6659 2023-05-12 12:42:29.000000 n0struct-0.2.96/n0struct/n0struct_utils_compare.py
--rw-rw-rw-   0        0        0     4120 2023-05-12 12:42:54.000000 n0struct-0.2.96/n0struct/n0struct_utils_find.py
-drwxrwxrwx   0        0        0        0 2023-05-13 12:24:15.367426 n0struct-0.2.96/n0struct/test/
--rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.96/n0struct/test/__init__.py
--rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.96/n0struct/test/__main__.py
--rw-rw-rw-   0        0        0    33051 2023-05-13 12:06:10.000000 n0struct-0.2.96/n0struct/test/test_n0struct.py
--rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.96/n0struct/test/test_n0struct2.py
--rw-rw-rw-   0        0        0      890 2023-05-13 12:07:38.000000 n0struct-0.2.96/n0struct/test/test_n0struct3.py
--rw-rw-rw-   0        0        0     1490 2023-05-13 12:23:25.000000 n0struct-0.2.96/n0struct/test/test_n0struct4.py
-drwxrwxrwx   0        0        0        0 2023-05-13 12:24:15.360401 n0struct-0.2.96/n0struct.egg-info/
--rw-rw-rw-   0        0        0     1060 2023-05-13 12:24:15.000000 n0struct-0.2.96/n0struct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1032 2023-05-13 12:24:15.000000 n0struct-0.2.96/n0struct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 12:24:15.000000 n0struct-0.2.96/n0struct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-13 12:24:15.000000 n0struct-0.2.96/n0struct.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-05-13 12:24:15.000000 n0struct-0.2.96/n0struct.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-13 12:24:15.000000 n0struct-0.2.96/n0struct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 12:24:15.378396 n0struct-0.2.96/setup.cfg
--rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.96/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:42:10.493233 n0struct-0.2.97/
+-rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.97/LICENSE
+-rw-rw-rw-   0        0        0     1060 2023-05-14 20:42:10.508854 n0struct-0.2.97/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.97/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 20:42:10.462022 n0struct-0.2.97/n0struct/
+-rw-rw-rw-   0        0        0      988 2023-05-13 11:12:54.000000 n0struct-0.2.97/n0struct/__init__.py
+-rw-rw-rw-   0        0        0     3671 2023-05-12 12:43:36.000000 n0struct-0.2.97/n0struct/n0struct_arrays.py
+-rw-rw-rw-   0        0        0     2104 2023-05-13 11:27:25.000000 n0struct-0.2.97/n0struct/n0struct_comprehensions.py
+-rw-rw-rw-   0        0        0    13176 2023-04-25 08:08:57.000000 n0struct-0.2.97/n0struct/n0struct_date.py
+-rw-rw-rw-   0        0        0     3389 2023-05-13 05:52:52.000000 n0struct-0.2.97/n0struct/n0struct_files.py
+-rw-rw-rw-   0        0        0    29365 2023-05-14 20:33:53.000000 n0struct-0.2.97/n0struct/n0struct_files_csv.py
+-rw-rw-rw-   0        0        0     7117 2023-05-13 11:56:28.000000 n0struct-0.2.97/n0struct/n0struct_files_fwf.py
+-rw-rw-rw-   0        0        0    15648 2023-05-13 11:36:31.000000 n0struct-0.2.97/n0struct/n0struct_findall.py
+-rw-rw-rw-   0        0        0     4070 2023-04-25 08:08:57.000000 n0struct-0.2.97/n0struct/n0struct_git.py
+-rw-rw-rw-   0        0        0    20960 2023-05-14 20:41:00.000000 n0struct-0.2.97/n0struct/n0struct_logging.py
+-rw-rw-rw-   0        0        0     2287 2023-04-25 08:08:57.000000 n0struct-0.2.97/n0struct/n0struct_mask.py
+-rw-rw-rw-   0        0        0    12168 2023-04-25 08:08:57.000000 n0struct-0.2.97/n0struct/n0struct_n0dict_.py
+-rw-rw-rw-   0        0        0    17116 2023-05-13 12:19:09.000000 n0struct-0.2.97/n0struct/n0struct_n0dict__.py
+-rw-rw-rw-   0        0        0     7519 2023-05-13 11:50:12.000000 n0struct-0.2.97/n0struct/n0struct_n0list_.py
+-rw-rw-rw-   0        0        0    75645 2023-05-13 12:22:04.000000 n0struct-0.2.97/n0struct/n0struct_n0list_n0dict.py
+-rw-rw-rw-   0        0        0      917 2023-04-25 08:08:57.000000 n0struct-0.2.97/n0struct/n0struct_random.py
+-rw-rw-rw-   0        0        0     3852 2023-04-25 08:08:57.000000 n0struct-0.2.97/n0struct/n0struct_references.py
+-rw-rw-rw-   0        0        0     3235 2023-05-12 12:49:17.000000 n0struct-0.2.97/n0struct/n0struct_transform_structure.py
+-rw-rw-rw-   0        0        0    18218 2023-05-14 15:31:16.000000 n0struct-0.2.97/n0struct/n0struct_utils.py
+-rw-rw-rw-   0        0        0     6659 2023-05-12 12:42:29.000000 n0struct-0.2.97/n0struct/n0struct_utils_compare.py
+-rw-rw-rw-   0        0        0     4120 2023-05-12 12:42:54.000000 n0struct-0.2.97/n0struct/n0struct_utils_find.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:42:10.493233 n0struct-0.2.97/n0struct/test/
+-rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.97/n0struct/test/__init__.py
+-rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.97/n0struct/test/__main__.py
+-rw-rw-rw-   0        0        0    33051 2023-05-13 12:06:10.000000 n0struct-0.2.97/n0struct/test/test_n0struct.py
+-rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.97/n0struct/test/test_n0struct2.py
+-rw-rw-rw-   0        0        0      890 2023-05-13 12:07:38.000000 n0struct-0.2.97/n0struct/test/test_n0struct3.py
+-rw-rw-rw-   0        0        0     1490 2023-05-13 12:23:25.000000 n0struct-0.2.97/n0struct/test/test_n0struct4.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:42:10.477641 n0struct-0.2.97/n0struct.egg-info/
+-rw-rw-rw-   0        0        0     1060 2023-05-14 20:42:10.000000 n0struct-0.2.97/n0struct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1032 2023-05-14 20:42:10.000000 n0struct-0.2.97/n0struct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 20:42:10.000000 n0struct-0.2.97/n0struct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 20:42:10.000000 n0struct-0.2.97/n0struct.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-05-14 20:42:10.000000 n0struct-0.2.97/n0struct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 20:42:10.000000 n0struct-0.2.97/n0struct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 20:42:10.508854 n0struct-0.2.97/setup.cfg
+-rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.97/setup.py
```

### Comparing `n0struct-0.2.96/LICENSE` & `n0struct-0.2.97/LICENSE`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/PKG-INFO` & `n0struct-0.2.97/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.96
+Version: 0.2.97
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.96/README.md` & `n0struct-0.2.97/README.md`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/__init__.py` & `n0struct-0.2.97/n0struct/__init__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_arrays.py` & `n0struct-0.2.97/n0struct/n0struct_arrays.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_comprehensions.py` & `n0struct-0.2.97/n0struct/n0struct_comprehensions.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_date.py` & `n0struct-0.2.97/n0struct/n0struct_date.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_files.py` & `n0struct-0.2.97/n0struct/n0struct_files.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_files_csv.py` & `n0struct-0.2.97/n0struct/n0struct_files_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         return_original_line = return_original_line,
         parse_csv_line       = parse_csv_line,
         encoding             = encoding,
         read_mode            = read_mode,
         header_is_mandatory  = header_is_mandatory,
     )
 # ******************************************************************************
-def generate_comlex_csv_row(
+def generate_complex_csv_row(
     row: list,
     delimiter: str = ',',
     EOL: str = '\n',
 ) -> str:
     generated_csv_row = ""
     for field_value in row:
         if field_value is None:
@@ -371,15 +371,15 @@
             elif isinstance(list_of_items[0], dict):
                 header = list(list_of_items[0].keys())
             mapping_dict = {column_name: column_name for column_name in header}
         else:
             header = list(mapping_dict.keys())
 
         if save_to and show_header:
-            out_filehandler.write(generate_comlex_csv_row(header, delimiter))
+            out_filehandler.write(generate_complex_csv_row(header, delimiter))
 
         for found_item in list_of_items:  # found_item == row in case of CSV list or item node in case of XML structure
             if isinstance(found_item, dict):
                 found_item = n0dict(found_item) # to have ability to use .first(xpath)
             elif isinstance(found_item, list):
                 found_item = n0list(found_item) # to have ability to use .first(xpath)
 
@@ -392,15 +392,15 @@
                     found_value = found_item.first(xpath, "")
                     if found_value:
                         break
                 csv_row.append(found_value)
             csv_table.append(csv_row)
 
             if save_to:
-                out_filehandler.write(generate_comlex_csv_row(csv_row, delimiter))
+                out_filehandler.write(generate_complex_csv_row(csv_row, delimiter))
 
     if save_to:
         out_filehandler.close
 
     return csv_table
 # ******************************************************************************
 def remove_colums_in_csv(
```

### Comparing `n0struct-0.2.96/n0struct/n0struct_files_fwf.py` & `n0struct-0.2.97/n0struct/n0struct_files_fwf.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_findall.py` & `n0struct-0.2.97/n0struct/n0struct_findall.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_git.py` & `n0struct-0.2.97/n0struct/n0struct_git.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_logging.py` & `n0struct-0.2.97/n0struct/n0struct_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 
 __main_log_filename = None
 def init_logger(
         debug_level: str = "TRACE",
         debug_output = sys.stderr,
         debug_timeformat: str = "YYYY-MM-DD HH:mm:ss.SSS",
-        debug_show_object_type = True,
-        debug_show_object_id = True,
+        debug_show_object_type = False,
+        debug_show_object_id = False,
         debug_show_item_count = True,
         debug_logtofile = False,
         log_file_name: str = None,
     ):
     logger.level("DEBUG", color="<white>")  # Change default color of DEBUG messages from blue into light gray
 
     global __main_log_filename
@@ -358,15 +358,17 @@
     :return:
     """
     prefix = (
                 (str(type(var_object)) or "").replace("<class '", "<").replace("'>", ">")
                 if __debug_show_object_type
                 else ""
              ) + (
-                f" id={id(var_object)}"
+                (
+                    (" " if __debug_show_object_type else "") + f"id={id(var_object)}"
+                )
                 if __debug_show_object_id
                 else ""
              )
     if prefix:
         prefix += " "
 
     n0print(
```

### Comparing `n0struct-0.2.96/n0struct/n0struct_mask.py` & `n0struct-0.2.97/n0struct/n0struct_mask.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_n0dict_.py` & `n0struct-0.2.97/n0struct/n0struct_n0dict_.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_n0dict__.py` & `n0struct-0.2.97/n0struct/n0struct_n0dict__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_n0list_.py` & `n0struct-0.2.97/n0struct/n0struct_n0list_.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_n0list_n0dict.py` & `n0struct-0.2.97/n0struct/n0struct_n0list_n0dict.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_random.py` & `n0struct-0.2.97/n0struct/n0struct_random.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_references.py` & `n0struct-0.2.97/n0struct/n0struct_references.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_transform_structure.py` & `n0struct-0.2.97/n0struct/n0struct_transform_structure.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_utils.py` & `n0struct-0.2.97/n0struct/n0struct_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,20 +369,25 @@
         value = "A"
         validate_values(value.upper(), ("A", "B", "C")) == "A"
         value = "c"
         validate_values(value.upper(), ("A", "B", "C")) == "C"
         value = "D"
         validate_values(value.upper(), ("A", "B", "C")) == "C"
     '''
-    if not isinstance(possible_values_the_last_is_default, (list, tuple)) or not possible_values_the_last_is_default:
-        return return_if_wrong_input
+    if not possible_values_the_last_is_default or not isinstance(possible_values_the_last_is_default, (list, tuple)):
+        if return_if_wrong_input:
+            return return_if_wrong_input
+        raise ValueError(f"{possible_values_the_last_is_default=} must be not empty list/tuple")
+
     if value in possible_values_the_last_is_default:
         return value
+        
     if isinstance(raise_if_not_found, Exception):
         raise raise_if_not_found
+
     return possible_values_the_last_is_default[-1]
 # ******************************************************************************
 def raise_exception(ex: Exception):
     raise ex
 # ******************************************************************************
 def catch_exception(func: callable, result_in_case_of_exception: typing.Any = None, **kw):
     """
```

### Comparing `n0struct-0.2.96/n0struct/n0struct_utils_compare.py` & `n0struct-0.2.97/n0struct/n0struct_utils_compare.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/n0struct_utils_find.py` & `n0struct-0.2.97/n0struct/n0struct_utils_find.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/test/test_n0struct.py` & `n0struct-0.2.97/n0struct/test/test_n0struct.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/test/test_n0struct2.py` & `n0struct-0.2.97/n0struct/test/test_n0struct2.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/test/test_n0struct3.py` & `n0struct-0.2.97/n0struct/test/test_n0struct3.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct/test/test_n0struct4.py` & `n0struct-0.2.97/n0struct/test/test_n0struct4.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/n0struct.egg-info/PKG-INFO` & `n0struct-0.2.97/n0struct.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.96
+Version: 0.2.97
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.96/n0struct.egg-info/SOURCES.txt` & `n0struct-0.2.97/n0struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.96/setup.py` & `n0struct-0.2.97/setup.py`

 * *Files identical despite different names*

