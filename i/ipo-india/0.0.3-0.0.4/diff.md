# Comparing `tmp/ipo_india-0.0.3.tar.gz` & `tmp/ipo_india-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipo_india-0.0.3.tar", last modified: Sun May 14 11:59:32 2023, max compression
+gzip compressed data, was "ipo_india-0.0.4.tar", last modified: Sun May 14 18:46:46 2023, max compression
```

## Comparing `ipo_india-0.0.3.tar` & `ipo_india-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:59:32.865297 ipo_india-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-14 11:59:32.865297 ipo_india-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:59:32.861297 ipo_india-0.0.3/ipo_india/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-14 11:59:27.000000 ipo_india-0.0.3/ipo_india/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-14 11:59:27.000000 ipo_india-0.0.3/ipo_india/ipo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-05-14 11:59:27.000000 ipo_india-0.0.3/ipo_india/ipo_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-14 11:59:27.000000 ipo_india-0.0.3/ipo_india/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:59:32.861297 ipo_india-0.0.3/ipo_india.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-14 11:59:32.000000 ipo_india-0.0.3/ipo_india.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-14 11:59:32.000000 ipo_india-0.0.3/ipo_india.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 11:59:32.000000 ipo_india-0.0.3/ipo_india.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-14 11:59:32.000000 ipo_india-0.0.3/ipo_india.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 11:59:32.000000 ipo_india-0.0.3/ipo_india.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 11:59:32.865297 ipo_india-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-14 11:59:27.000000 ipo_india-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:46:46.011348 ipo_india-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-14 18:46:46.011348 ipo_india-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:46:46.007348 ipo_india-0.0.4/ipo_india/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-14 18:46:40.000000 ipo_india-0.0.4/ipo_india/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-14 18:46:40.000000 ipo_india-0.0.4/ipo_india/ipo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-05-14 18:46:40.000000 ipo_india-0.0.4/ipo_india/ipo_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-14 18:46:40.000000 ipo_india-0.0.4/ipo_india/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:46:46.011348 ipo_india-0.0.4/ipo_india.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-14 18:46:45.000000 ipo_india-0.0.4/ipo_india.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-14 18:46:45.000000 ipo_india-0.0.4/ipo_india.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:46:45.000000 ipo_india-0.0.4/ipo_india.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-14 18:46:45.000000 ipo_india-0.0.4/ipo_india.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 18:46:45.000000 ipo_india-0.0.4/ipo_india.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 18:46:46.011348 ipo_india-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-14 18:46:40.000000 ipo_india-0.0.4/setup.py
```

### Comparing `ipo_india-0.0.3/ipo_india/ipo.py` & `ipo_india-0.0.4/ipo_india/ipo.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                 # Convert snake case of the keys to readable format
                 readable_key = property.replace('_', ' ').title()
                 if property in ['gmp', 'qib', 'rii', 'ret']:
                     readable_key = readable_key.upper()
                 if property in ['open_date', 'close_date']:
                     value = self.__datetime_to_readable_date(value)
                 if property == 'name':
-                    readable_ipo += f'{value}\n'
+                    readable_ipo += f'**{value}**\n'
                 else:
                     readable_ipo += f'{readable_key}: {value}\n'
         return readable_ipo
     
     def __datetime_to_readable_date(self, datetime_obj: datetime) -> str:
         '''
         Convert datetime object to date string
```

### Comparing `ipo_india-0.0.3/ipo_india/ipo_scraper.py` & `ipo_india-0.0.4/ipo_india/ipo_scraper.py`

 * *Files identical despite different names*

### Comparing `ipo_india-0.0.3/ipo_india/main.py` & `ipo_india-0.0.4/ipo_india/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ipo_india.ipo import Ipo
-from ipo_india.ipo_scraper import TopShareBrokersIPO
+from ipo import Ipo
+from ipo_scraper import TopShareBrokersIPO
 import logging
 def get_ipos(readable: bool = False,
              open_ipos: bool = False,
              retail: bool = False,
              sme: bool = False):
     try:
         if open_ipos:
```

### Comparing `ipo_india-0.0.3/setup.py` & `ipo_india-0.0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 setup(
     name='ipo_india',
     version=__version__,
 
     url='https://github.com/MichaelKim0407/tutorial-pip-package',
     author='Aman Agarwal',
     author_email='aman.agarwal150@gmail.com',
```

