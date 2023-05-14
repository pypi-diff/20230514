# Comparing `tmp/ipo_india-0.0.2.tar.gz` & `tmp/ipo_india-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipo_india-0.0.2.tar", last modified: Sat May 13 13:57:43 2023, max compression
+gzip compressed data, was "ipo_india-0.0.3.tar", last modified: Sun May 14 11:59:32 2023, max compression
```

## Comparing `ipo_india-0.0.2.tar` & `ipo_india-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 quartic   (1000) quartic   (1000)        0 2023-05-13 13:57:43.595608 ipo_india-0.0.2/
--rw-rw-r--   0 quartic   (1000) quartic   (1000)      265 2023-05-13 13:57:43.595608 ipo_india-0.0.2/PKG-INFO
-drwxrwxr-x   0 quartic   (1000) quartic   (1000)        0 2023-05-13 13:57:43.595608 ipo_india-0.0.2/ipo_india/
--rw-rw-r--   0 quartic   (1000) quartic   (1000)       89 2023-05-13 11:41:36.000000 ipo_india-0.0.2/ipo_india/__init__.py
--rw-rw-r--   0 quartic   (1000) quartic   (1000)     2337 2023-05-13 11:33:48.000000 ipo_india-0.0.2/ipo_india/ipo.py
--rw-rw-r--   0 quartic   (1000) quartic   (1000)     5603 2023-05-13 11:33:48.000000 ipo_india-0.0.2/ipo_india/ipo_scraper.py
--rw-rw-r--   0 quartic   (1000) quartic   (1000)      989 2023-05-13 13:55:54.000000 ipo_india-0.0.2/ipo_india/main.py
-drwxrwxr-x   0 quartic   (1000) quartic   (1000)        0 2023-05-13 13:57:43.595608 ipo_india-0.0.2/ipo_india.egg-info/
--rw-rw-r--   0 quartic   (1000) quartic   (1000)      265 2023-05-13 13:57:43.000000 ipo_india-0.0.2/ipo_india.egg-info/PKG-INFO
--rw-rw-r--   0 quartic   (1000) quartic   (1000)      254 2023-05-13 13:57:43.000000 ipo_india-0.0.2/ipo_india.egg-info/SOURCES.txt
--rw-rw-r--   0 quartic   (1000) quartic   (1000)        1 2023-05-13 13:57:43.000000 ipo_india-0.0.2/ipo_india.egg-info/dependency_links.txt
--rw-rw-r--   0 quartic   (1000) quartic   (1000)       95 2023-05-13 13:57:43.000000 ipo_india-0.0.2/ipo_india.egg-info/requires.txt
--rw-rw-r--   0 quartic   (1000) quartic   (1000)       10 2023-05-13 13:57:43.000000 ipo_india-0.0.2/ipo_india.egg-info/top_level.txt
--rw-rw-r--   0 quartic   (1000) quartic   (1000)       38 2023-05-13 13:57:43.595608 ipo_india-0.0.2/setup.cfg
--rw-rw-r--   0 quartic   (1000) quartic   (1000)      512 2023-05-13 13:57:01.000000 ipo_india-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:59:32.865297 ipo_india-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-14 11:59:32.865297 ipo_india-0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:59:32.861297 ipo_india-0.0.3/ipo_india/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-14 11:59:27.000000 ipo_india-0.0.3/ipo_india/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-14 11:59:27.000000 ipo_india-0.0.3/ipo_india/ipo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-05-14 11:59:27.000000 ipo_india-0.0.3/ipo_india/ipo_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-14 11:59:27.000000 ipo_india-0.0.3/ipo_india/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:59:32.861297 ipo_india-0.0.3/ipo_india.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-14 11:59:32.000000 ipo_india-0.0.3/ipo_india.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-14 11:59:32.000000 ipo_india-0.0.3/ipo_india.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 11:59:32.000000 ipo_india-0.0.3/ipo_india.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-14 11:59:32.000000 ipo_india-0.0.3/ipo_india.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 11:59:32.000000 ipo_india-0.0.3/ipo_india.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 11:59:32.865297 ipo_india-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-14 11:59:27.000000 ipo_india-0.0.3/setup.py
```

### Comparing `ipo_india-0.0.2/ipo_india/ipo_scraper.py` & `ipo_india-0.0.3/ipo_india/ipo_scraper.py`

 * *Files identical despite different names*

### Comparing `ipo_india-0.0.2/ipo_india/main.py` & `ipo_india-0.0.3/ipo_india/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ipo_india.ipo import Ipo
 from ipo_india.ipo_scraper import TopShareBrokersIPO
-
+import logging
 def get_ipos(readable: bool = False,
              open_ipos: bool = False,
              retail: bool = False,
              sme: bool = False):
     try:
         if open_ipos:
             if retail:
@@ -21,10 +21,11 @@
         else:
             ipos = [Ipo(name=ipo_name, **ipo_data) for ipo_name, ipo_data in ipos.items()]
 
         return ipos
     except Exception:
         raise Exception("Faield to get IPOs")
 
-# ipos = get_ipos(readable=True, open_ipos=False)
-# ipos = get_ipos(open_ipos=False)
-# print(ipos)
+if __name__ == "__main__":
+    ipos = get_ipos(readable=True, open_ipos=False)
+    logging.info(ipos)
+
```

### Comparing `ipo_india-0.0.2/setup.py` & `ipo_india-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 setup(
     name='ipo_india',
     version=__version__,
 
     url='https://github.com/MichaelKim0407/tutorial-pip-package',
     author='Aman Agarwal',
     author_email='aman.agarwal150@gmail.com',
@@ -14,8 +14,8 @@
         "html5lib==1.1",
         "pydantic==1.10.7",
         "pytz==2023.3",
         "requests==2.30.0",
     ],
     packages=find_packages(),
     python_requires='>=3.9',
-)
+)
```

