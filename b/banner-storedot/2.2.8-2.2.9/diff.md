# Comparing `tmp/banner-storedot-2.2.8.tar.gz` & `tmp/banner-storedot-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banner-storedot-2.2.8.tar", last modified: Mon Jan 30 14:59:43 2023, max compression
+gzip compressed data, was "banner-storedot-2.2.9.tar", last modified: Mon Jan 30 15:25:50 2023, max compression
```

## Comparing `banner-storedot-2.2.8.tar` & `banner-storedot-2.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 14:59:43.310567 banner-storedot-2.2.8/
--rw-rwSr--   0 gil       (1008) developers  (1234)     1073 2021-08-19 08:44:05.000000 banner-storedot-2.2.8/LICENSE
--rw-r--r--   0 gil       (1008) developers  (1234)     8235 2023-01-30 14:59:43.310567 banner-storedot-2.2.8/PKG-INFO
--rw-rwSr--   0 gil       (1008) developers  (1234)     7782 2022-07-18 10:09:00.000000 banner-storedot-2.2.8/README.md
--rw-rwSr--   0 gil       (1008) developers  (1234)      122 2021-08-19 10:21:45.000000 banner-storedot-2.2.8/pyproject.toml
--rw-r--r--   0 gil       (1008) developers  (1234)      672 2023-01-30 14:59:43.310567 banner-storedot-2.2.8/setup.cfg
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 14:59:43.302567 banner-storedot-2.2.8/src/
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 14:59:43.306567 banner-storedot-2.2.8/src/banner/
--rw-rwSr--   0 gil       (1008) developers  (1234)      161 2022-11-08 14:34:28.000000 banner-storedot-2.2.8/src/banner/__init__.py
--rw-r--r--   0 gil       (1008) developers  (1234)    26627 2023-01-30 14:58:49.000000 banner-storedot-2.2.8/src/banner/connection.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     6049 2023-01-08 12:31:38.000000 banner-storedot-2.2.8/src/banner/pandas_decorator.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     2121 2022-01-09 16:04:35.000000 banner-storedot-2.2.8/src/banner/pandas_wrap.py
--rw-rwSr--   0 gil       (1008) developers  (1234)    47841 2023-01-29 14:03:26.000000 banner-storedot-2.2.8/src/banner/queries.py
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 14:59:43.306567 banner-storedot-2.2.8/src/banner/utils/
--rw-rwSr--   0 gil       (1008) developers  (1234)        0 2021-08-19 11:04:29.000000 banner-storedot-2.2.8/src/banner/utils/__init__.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     3798 2022-12-22 09:12:51.000000 banner-storedot-2.2.8/src/banner/utils/const.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     1739 2022-12-27 13:22:40.000000 banner-storedot-2.2.8/src/banner/utils/misc.py
--rw-rwSr--   0 gil       (1008) developers  (1234)    10084 2023-01-19 13:06:13.000000 banner-storedot-2.2.8/src/banner/utils/neware.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     1952 2022-08-17 11:13:16.000000 banner-storedot-2.2.8/src/banner/utils/pandas.py
--rw-rwSr--   0 gil       (1008) developers  (1234)   166397 2023-01-12 11:46:42.000000 banner-storedot-2.2.8/src/banner/utils/web2py.py
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 14:59:43.310567 banner-storedot-2.2.8/src/banner_storedot.egg-info/
--rw-rwSr--   0 gil       (1008) developers  (1234)     8235 2023-01-30 14:59:43.000000 banner-storedot-2.2.8/src/banner_storedot.egg-info/PKG-INFO
--rw-rwSr--   0 gil       (1008) developers  (1234)      544 2023-01-30 14:59:43.000000 banner-storedot-2.2.8/src/banner_storedot.egg-info/SOURCES.txt
--rw-rwSr--   0 gil       (1008) developers  (1234)        1 2023-01-30 14:59:43.000000 banner-storedot-2.2.8/src/banner_storedot.egg-info/dependency_links.txt
--rw-rwSr--   0 gil       (1008) developers  (1234)       75 2023-01-30 14:59:43.000000 banner-storedot-2.2.8/src/banner_storedot.egg-info/requires.txt
--rw-rwSr--   0 gil       (1008) developers  (1234)        7 2023-01-30 14:59:43.000000 banner-storedot-2.2.8/src/banner_storedot.egg-info/top_level.txt
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 15:25:50.740200 banner-storedot-2.2.9/
+-rw-rwSr--   0 gil       (1008) developers  (1234)     1073 2021-08-19 08:44:05.000000 banner-storedot-2.2.9/LICENSE
+-rw-r--r--   0 gil       (1008) developers  (1234)     8235 2023-01-30 15:25:50.740200 banner-storedot-2.2.9/PKG-INFO
+-rw-rwSr--   0 gil       (1008) developers  (1234)     7782 2022-07-18 10:09:00.000000 banner-storedot-2.2.9/README.md
+-rw-rwSr--   0 gil       (1008) developers  (1234)      122 2021-08-19 10:21:45.000000 banner-storedot-2.2.9/pyproject.toml
+-rw-r--r--   0 gil       (1008) developers  (1234)      672 2023-01-30 15:25:50.740200 banner-storedot-2.2.9/setup.cfg
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 15:25:50.736199 banner-storedot-2.2.9/src/
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 15:25:50.736199 banner-storedot-2.2.9/src/banner/
+-rw-rwSr--   0 gil       (1008) developers  (1234)      161 2022-11-08 14:34:28.000000 banner-storedot-2.2.9/src/banner/__init__.py
+-rw-r--r--   0 gil       (1008) developers  (1234)    26651 2023-01-30 15:23:16.000000 banner-storedot-2.2.9/src/banner/connection.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     6049 2023-01-08 12:31:38.000000 banner-storedot-2.2.9/src/banner/pandas_decorator.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     2121 2022-01-09 16:04:35.000000 banner-storedot-2.2.9/src/banner/pandas_wrap.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)    47841 2023-01-29 14:03:26.000000 banner-storedot-2.2.9/src/banner/queries.py
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 15:25:50.740200 banner-storedot-2.2.9/src/banner/utils/
+-rw-rwSr--   0 gil       (1008) developers  (1234)        0 2021-08-19 11:04:29.000000 banner-storedot-2.2.9/src/banner/utils/__init__.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     3798 2022-12-22 09:12:51.000000 banner-storedot-2.2.9/src/banner/utils/const.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     1739 2022-12-27 13:22:40.000000 banner-storedot-2.2.9/src/banner/utils/misc.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)    10084 2023-01-19 13:06:13.000000 banner-storedot-2.2.9/src/banner/utils/neware.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     1952 2022-08-17 11:13:16.000000 banner-storedot-2.2.9/src/banner/utils/pandas.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)   166397 2023-01-12 11:46:42.000000 banner-storedot-2.2.9/src/banner/utils/web2py.py
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 15:25:50.740200 banner-storedot-2.2.9/src/banner_storedot.egg-info/
+-rw-rwSr--   0 gil       (1008) developers  (1234)     8235 2023-01-30 15:25:50.000000 banner-storedot-2.2.9/src/banner_storedot.egg-info/PKG-INFO
+-rw-rwSr--   0 gil       (1008) developers  (1234)      544 2023-01-30 15:25:50.000000 banner-storedot-2.2.9/src/banner_storedot.egg-info/SOURCES.txt
+-rw-rwSr--   0 gil       (1008) developers  (1234)        1 2023-01-30 15:25:50.000000 banner-storedot-2.2.9/src/banner_storedot.egg-info/dependency_links.txt
+-rw-rwSr--   0 gil       (1008) developers  (1234)       75 2023-01-30 15:25:50.000000 banner-storedot-2.2.9/src/banner_storedot.egg-info/requires.txt
+-rw-rwSr--   0 gil       (1008) developers  (1234)        7 2023-01-30 15:25:50.000000 banner-storedot-2.2.9/src/banner_storedot.egg-info/top_level.txt
```

### Comparing `banner-storedot-2.2.8/LICENSE` & `banner-storedot-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.8/PKG-INFO` & `banner-storedot-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banner-storedot
-Version: 2.2.8
+Version: 2.2.9
 Summary: light dal package
 Home-page: https://https://github.com/storedot/banner
 Author: GB
 Author-email: gilb@store-dot.com
 Project-URL: Bug Tracker, https://https://github.com/storedot/banner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `banner-storedot-2.2.8/README.md` & `banner-storedot-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.8/setup.cfg` & `banner-storedot-2.2.9/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = banner-storedot
-version = 2.2.8
+version = 2.2.9
 author = GB
 author_email = gilb@store-dot.com
 description = light dal package
 long_description = file: README.md
 url = https://https://github.com/storedot/banner
 project_urls = 
 	Bug Tracker = https://https://github.com/storedot/banner/issues
```

### Comparing `banner-storedot-2.2.8/src/banner/connection.py` & `banner-storedot-2.2.9/src/banner/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -811,15 +811,16 @@
             
             for column in df.filter(like='updated_on').columns:
                 df[column] = df[column].astype('datetime64[ms]')
                 
             return df.convert_dtypes()
         
         except (
-            KeyError, IndexError, TypeError, AttributeError, 
+            KeyError, IndexError, TypeError, 
+            AttributeError, ValueError,
             UndefinedVariableError, redis.ResponseError
         ):
             return DataFrame()
         
 
 
 QUERY_TO_STORAGE_CONTROL = dict(
```

### Comparing `banner-storedot-2.2.8/src/banner/pandas_decorator.py` & `banner-storedot-2.2.9/src/banner/pandas_decorator.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.8/src/banner/pandas_wrap.py` & `banner-storedot-2.2.9/src/banner/pandas_wrap.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.8/src/banner/queries.py` & `banner-storedot-2.2.9/src/banner/queries.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.8/src/banner/utils/const.py` & `banner-storedot-2.2.9/src/banner/utils/const.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.8/src/banner/utils/misc.py` & `banner-storedot-2.2.9/src/banner/utils/misc.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.8/src/banner/utils/neware.py` & `banner-storedot-2.2.9/src/banner/utils/neware.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.8/src/banner/utils/pandas.py` & `banner-storedot-2.2.9/src/banner/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.8/src/banner/utils/web2py.py` & `banner-storedot-2.2.9/src/banner/utils/web2py.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.8/src/banner_storedot.egg-info/PKG-INFO` & `banner-storedot-2.2.9/src/banner_storedot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banner-storedot
-Version: 2.2.8
+Version: 2.2.9
 Summary: light dal package
 Home-page: https://https://github.com/storedot/banner
 Author: GB
 Author-email: gilb@store-dot.com
 Project-URL: Bug Tracker, https://https://github.com/storedot/banner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `banner-storedot-2.2.8/src/banner_storedot.egg-info/SOURCES.txt` & `banner-storedot-2.2.9/src/banner_storedot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

