# Comparing `tmp/knowledgebase-gsheet-gpt-1.1.1.tar.gz` & `tmp/knowledgebase-gsheet-gpt-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledgebase-gsheet-gpt-1.1.1.tar", last modified: Sun May 14 09:34:57 2023, max compression
+gzip compressed data, was "knowledgebase-gsheet-gpt-1.1.2.tar", last modified: Sun May 14 12:11:05 2023, max compression
```

## Comparing `knowledgebase-gsheet-gpt-1.1.1.tar` & `knowledgebase-gsheet-gpt-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 09:34:57.300608 knowledgebase-gsheet-gpt-1.1.1/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-14 09:34:57.300493 knowledgebase-gsheet-gpt-1.1.1/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 09:34:57.300310 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       98 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     4762 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-14 09:34:57.300642 knowledgebase-gsheet-gpt-1.1.1/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-14 09:34:57.000000 knowledgebase-gsheet-gpt-1.1.1/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 12:11:05.218661 knowledgebase-gsheet-gpt-1.1.2/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-14 12:11:05.218550 knowledgebase-gsheet-gpt-1.1.2/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-14 12:11:05.000000 knowledgebase-gsheet-gpt-1.1.2/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-14 12:11:05.218362 knowledgebase-gsheet-gpt-1.1.2/knowledgebase_gsheet_gpt.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-14 12:11:05.000000 knowledgebase-gsheet-gpt-1.1.2/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-14 12:11:05.000000 knowledgebase-gsheet-gpt-1.1.2/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-14 12:11:05.000000 knowledgebase-gsheet-gpt-1.1.2/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-14 12:11:05.000000 knowledgebase-gsheet-gpt-1.1.2/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       98 2023-05-14 12:11:05.000000 knowledgebase-gsheet-gpt-1.1.2/knowledgebase_gsheet_gpt.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-14 12:11:05.000000 knowledgebase-gsheet-gpt-1.1.2/knowledgebase_gsheet_gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     4762 2023-05-14 12:11:05.000000 knowledgebase-gsheet-gpt-1.1.2/knowledgebase_gsheet_gpt.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-14 12:11:05.218703 knowledgebase-gsheet-gpt-1.1.2/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-14 12:11:05.000000 knowledgebase-gsheet-gpt-1.1.2/setup.py
```

### Comparing `knowledgebase-gsheet-gpt-1.1.1/PKG-INFO` & `knowledgebase-gsheet-gpt-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.1.1
+Version: 1.1.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
```

### Comparing `knowledgebase-gsheet-gpt-1.1.1/README.md` & `knowledgebase-gsheet-gpt-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.egg-info/PKG-INFO` & `knowledgebase-gsheet-gpt-1.1.2/knowledgebase_gsheet_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.1.1
+Version: 1.1.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
```

### Comparing `knowledgebase-gsheet-gpt-1.1.1/knowledgebase_gsheet_gpt.py` & `knowledgebase-gsheet-gpt-1.1.2/knowledgebase_gsheet_gpt.py`

 * *Files identical despite different names*

### Comparing `knowledgebase-gsheet-gpt-1.1.1/setup.py` & `knowledgebase-gsheet-gpt-1.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="knowledgebase-gsheet-gpt",
-    version="1.1.1",
+    version="1.1.2",
     packages=find_packages(),
     py_modules=['knowledgebase_gsheet_gpt'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'knowledgebase_gsheet_gpt = knowledgebase_gsheet_gpt:main',
         ],
```

