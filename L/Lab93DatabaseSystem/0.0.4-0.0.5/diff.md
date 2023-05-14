# Comparing `tmp/Lab93DatabaseSystem-0.0.4.tar.gz` & `tmp/Lab93DatabaseSystem-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lab93DatabaseSystem-0.0.4.tar", last modified: Thu May 11 23:58:52 2023, max compression
+gzip compressed data, was "Lab93DatabaseSystem-0.0.5.tar", last modified: Sun May 14 20:06:50 2023, max compression
```

## Comparing `Lab93DatabaseSystem-0.0.4.tar` & `Lab93DatabaseSystem-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-11 23:58:52.335261 Lab93DatabaseSystem-0.0.4/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      917 2023-05-11 23:58:52.331928 Lab93DatabaseSystem-0.0.4/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      628 2023-05-11 23:57:49.000000 Lab93DatabaseSystem-0.0.4/pyproject.toml
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      386 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.4/readme.md
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-05-11 23:58:52.335261 Lab93DatabaseSystem-0.0.4/setup.cfg
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-11 23:58:52.305263 Lab93DatabaseSystem-0.0.4/src/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-11 23:58:52.308596 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     5661 2023-05-10 00:02:51.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-11 23:58:52.325262 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-11 23:58:52.331928 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/DatabaseAPI/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     8703 2023-05-11 23:40:49.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      928 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/DatabaseAPI/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-11 23:58:52.321929 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem.egg-info/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      917 2023-05-11 23:58:52.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem.egg-info/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      469 2023-05-11 23:58:52.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem.egg-info/SOURCES.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-05-11 23:58:52.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem.egg-info/dependency_links.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       20 2023-05-11 23:58:52.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem.egg-info/top_level.txt
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-14 20:06:50.772989 Lab93DatabaseSystem-0.0.5/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      915 2023-05-14 20:06:50.769656 Lab93DatabaseSystem-0.0.5/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      626 2023-05-14 20:06:13.000000 Lab93DatabaseSystem-0.0.5/pyproject.toml
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      386 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.5/readme.md
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-05-14 20:06:50.772989 Lab93DatabaseSystem-0.0.5/setup.cfg
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-14 20:06:50.749656 Lab93DatabaseSystem-0.0.5/src/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-14 20:06:50.756322 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     5724 2023-05-14 19:22:15.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-14 20:06:50.762989 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-14 20:06:50.769656 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/DatabaseAPI/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     8791 2023-05-14 20:03:54.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      928 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/DatabaseAPI/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-14 20:06:50.759656 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem.egg-info/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      915 2023-05-14 20:06:50.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem.egg-info/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      469 2023-05-14 20:06:50.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem.egg-info/SOURCES.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-05-14 20:06:50.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem.egg-info/dependency_links.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       20 2023-05-14 20:06:50.000000 Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem.egg-info/top_level.txt
```

### Comparing `Lab93DatabaseSystem-0.0.4/PKG-INFO` & `Lab93DatabaseSystem-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: Lab93DatabaseSystem
-Version: 0.0.4
+Version: 0.0.5
 Summary: An API for object persistence scriptability.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
-Project-URL: Homepage, https://github.com/guyyatsu/Lab93-Database-System
-Project-URL: Bug Tracker, https://github.com/guyyatsu/Lab93-Database-System/issues
+Project-URL: Homepage, https://github.com/guyyatsu/Lab93-DatabaseSystem
+Project-URL: Bug Tracker, https://github.com/guyyatsu/Lab93-DatabaseSystem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Lab-93 SQLite3 Databse API
```

### Comparing `Lab93DatabaseSystem-0.0.4/pyproject.toml` & `Lab93DatabaseSystem-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Lab93DatabaseSystem"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Hunter Dale", email="hunter@guyyatsu.me" },
 ]
 
 description = "An API for object persistence scriptability."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/guyyatsu/Lab93-Database-System"
-"Bug Tracker" = "https://github.com/guyyatsu/Lab93-Database-System/issues"
+"Homepage" = "https://github.com/guyyatsu/Lab93-DatabaseSystem"
+"Bug Tracker" = "https://github.com/guyyatsu/Lab93-DatabaseSystem/issues"
```

### Comparing `Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/__init__.py` & `Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,16 @@
                                  "columns": { "last_name":     "REQUIRED TEXT",
                                               "email_address": "TEXT",
                                               "phone_number":  "TEXT",
                                               "github":        "TEXT",
                                               "website":       "TEXT",
                                             },
                                },
+                  "income": {},
+                  "hours": {},
                  }
 
     # Iterate through every top-level key and validate it's existence.
     #NOTE:
     ''' Each key must also be a dictionary containing:
 
             1.  - A key representing the name of the default column within the
```

### Comparing `Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py` & `Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 
     # Curate a list of headers for a given table.
     'queryHeaderList': "SELECT name FROM sqlite_master WHERE type='table'",
 
     # Add a new row to a specific table.
     'createNewUniqueRow': "INSERT OR IGNORE INTO {}({}) VALUES({});",
 
-    'querySelectRow': "SELECT * FROM {} WHERE {}='{}';"
+    'querySelectRow': "SELECT {} FROM {} WHERE {}='{}';"
 }
-
+`
 
 def newColumn( database,
                table: str="test_table_one",
                column: str="test_column_one",
                column_type: str="UNIQUE PRIMARY TEXT" ) -> None:
     """
     SQLite3_Statements.newColumn will create a new header within a table of your choosing.
@@ -208,21 +208,23 @@
                                           column.lower() )            )\
                    .fetchall()[0][0]
 
 # NOTE: New function for version 0.0.4
 # TODO: This should actually be a querySpecificRow.
 def selectRow( database,
               table,
-              row,
+              column,
+              header,
               value ):
     database = databaseConnection(database)
     return database.cursor\
                    .execute( statements['querySelectRow']\
-                                 .format( table.lower(),
-                                          row.lower(),
+                                 .format( column.lower(),
+                                          table.lower(),
+                                          header.lower(),
                                           value         )     )\
                    .fetchall()
 
 
 def new_uniqueRow( database,
                    table: str="test_table_one",
                    columns: str="test_column_one, test_column_two",
```

### Comparing `Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py` & `Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py`

 * *Files identical despite different names*

### Comparing `Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem.egg-info/PKG-INFO` & `Lab93DatabaseSystem-0.0.5/src/Lab93DatabaseSystem.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: Lab93DatabaseSystem
-Version: 0.0.4
+Version: 0.0.5
 Summary: An API for object persistence scriptability.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
-Project-URL: Homepage, https://github.com/guyyatsu/Lab93-Database-System
-Project-URL: Bug Tracker, https://github.com/guyyatsu/Lab93-Database-System/issues
+Project-URL: Homepage, https://github.com/guyyatsu/Lab93-DatabaseSystem
+Project-URL: Bug Tracker, https://github.com/guyyatsu/Lab93-DatabaseSystem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Lab-93 SQLite3 Databse API
```

