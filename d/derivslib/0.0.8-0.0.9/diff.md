# Comparing `tmp/derivslib-0.0.8.tar.gz` & `tmp/derivslib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/derivslib-0.0.8.tar", last modified: Wed Apr  5 02:31:03 2023, max compression
+gzip compressed data, was "dist/derivslib-0.0.9.tar", last modified: Wed Apr  5 02:38:31 2023, max compression
```

## Comparing `derivslib-0.0.8.tar` & `derivslib-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 landon     (501) staff       (20)        0 2023-04-05 02:31:03.000000 derivslib-0.0.8/
--rw-r--r--   0 landon     (501) staff       (20)      942 2023-04-05 02:31:03.000000 derivslib-0.0.8/PKG-INFO
-drwxr-xr-x   0 landon     (501) staff       (20)        0 2023-04-05 02:31:03.000000 derivslib-0.0.8/data/
--rw-r--r--   0 landon     (501) staff       (20)        0 2023-04-05 02:29:33.000000 derivslib-0.0.8/data/__init__.py
-drwxr-xr-x   0 landon     (501) staff       (20)        0 2023-04-05 02:31:03.000000 derivslib-0.0.8/derivslib.egg-info/
--rw-r--r--   0 landon     (501) staff       (20)      942 2023-04-05 02:31:02.000000 derivslib-0.0.8/derivslib.egg-info/PKG-INFO
--rw-r--r--   0 landon     (501) staff       (20)      315 2023-04-05 02:31:02.000000 derivslib-0.0.8/derivslib.egg-info/SOURCES.txt
--rw-r--r--   0 landon     (501) staff       (20)        1 2023-04-05 02:31:02.000000 derivslib-0.0.8/derivslib.egg-info/dependency_links.txt
--rw-r--r--   0 landon     (501) staff       (20)      100 2023-04-05 02:31:02.000000 derivslib-0.0.8/derivslib.egg-info/requires.txt
--rw-r--r--   0 landon     (501) staff       (20)       23 2023-04-05 02:31:02.000000 derivslib-0.0.8/derivslib.egg-info/top_level.txt
-drwxr-xr-x   0 landon     (501) staff       (20)        0 2023-04-05 02:31:03.000000 derivslib-0.0.8/dist/
--rw-r--r--   0 landon     (501) staff       (20)        0 2023-04-05 02:29:48.000000 derivslib-0.0.8/dist/__init__.py
-drwxr-xr-x   0 landon     (501) staff       (20)        0 2023-04-05 02:31:03.000000 derivslib-0.0.8/examples/
--rw-r--r--   0 landon     (501) staff       (20)        0 2023-04-05 02:29:26.000000 derivslib-0.0.8/examples/__init__.py
--rw-r--r--   0 landon     (501) staff       (20)       38 2023-04-05 02:31:03.000000 derivslib-0.0.8/setup.cfg
--rw-r--r--   0 landon     (501) staff       (20)     1210 2023-04-05 02:30:23.000000 derivslib-0.0.8/setup.py
-drwxr-xr-x   0 landon     (501) staff       (20)        0 2023-04-05 02:31:03.000000 derivslib-0.0.8/src/
--rw-r--r--   0 landon     (501) staff       (20)        0 2023-04-05 02:29:17.000000 derivslib-0.0.8/src/__init__.py
--rw-r--r--   0 landon     (501) staff       (20)     6095 2023-04-03 19:50:16.000000 derivslib-0.0.8/src/cboe.py
--rw-r--r--   0 landon     (501) staff       (20)    80763 2023-04-03 19:55:52.000000 derivslib-0.0.8/src/derivslib.py
--rw-r--r--   0 landon     (501) staff       (20)    19076 2023-04-03 19:52:46.000000 derivslib-0.0.8/src/market.py
--rw-r--r--   0 landon     (501) staff       (20)    14715 2023-04-05 01:56:44.000000 derivslib-0.0.8/src/personal.py
--rw-r--r--   0 landon     (501) staff       (20)     3967 2023-04-03 18:29:31.000000 derivslib-0.0.8/src/utils.py
+drwxr-xr-x   0 landon     (501) staff       (20)        0 2023-04-05 02:38:31.000000 derivslib-0.0.9/
+-rw-r--r--   0 landon     (501) staff       (20)      942 2023-04-05 02:38:31.000000 derivslib-0.0.9/PKG-INFO
+drwxr-xr-x   0 landon     (501) staff       (20)        0 2023-04-05 02:38:31.000000 derivslib-0.0.9/data/
+-rw-r--r--   0 landon     (501) staff       (20)        0 2023-04-05 02:29:33.000000 derivslib-0.0.9/data/__init__.py
+drwxr-xr-x   0 landon     (501) staff       (20)        0 2023-04-05 02:38:31.000000 derivslib-0.0.9/derivslib.egg-info/
+-rw-r--r--   0 landon     (501) staff       (20)      942 2023-04-05 02:38:31.000000 derivslib-0.0.9/derivslib.egg-info/PKG-INFO
+-rw-r--r--   0 landon     (501) staff       (20)      298 2023-04-05 02:38:31.000000 derivslib-0.0.9/derivslib.egg-info/SOURCES.txt
+-rw-r--r--   0 landon     (501) staff       (20)        1 2023-04-05 02:38:31.000000 derivslib-0.0.9/derivslib.egg-info/dependency_links.txt
+-rw-r--r--   0 landon     (501) staff       (20)      110 2023-04-05 02:38:31.000000 derivslib-0.0.9/derivslib.egg-info/requires.txt
+-rw-r--r--   0 landon     (501) staff       (20)       18 2023-04-05 02:38:31.000000 derivslib-0.0.9/derivslib.egg-info/top_level.txt
+drwxr-xr-x   0 landon     (501) staff       (20)        0 2023-04-05 02:38:31.000000 derivslib-0.0.9/examples/
+-rw-r--r--   0 landon     (501) staff       (20)        0 2023-04-05 02:29:26.000000 derivslib-0.0.9/examples/__init__.py
+-rw-r--r--   0 landon     (501) staff       (20)       38 2023-04-05 02:38:31.000000 derivslib-0.0.9/setup.cfg
+-rw-r--r--   0 landon     (501) staff       (20)     1226 2023-04-05 02:38:08.000000 derivslib-0.0.9/setup.py
+drwxr-xr-x   0 landon     (501) staff       (20)        0 2023-04-05 02:38:31.000000 derivslib-0.0.9/src/
+-rw-r--r--   0 landon     (501) staff       (20)        0 2023-04-05 02:29:17.000000 derivslib-0.0.9/src/__init__.py
+-rw-r--r--   0 landon     (501) staff       (20)     6095 2023-04-03 19:50:16.000000 derivslib-0.0.9/src/cboe.py
+-rw-r--r--   0 landon     (501) staff       (20)    80763 2023-04-03 19:55:52.000000 derivslib-0.0.9/src/derivslib.py
+-rw-r--r--   0 landon     (501) staff       (20)    19076 2023-04-03 19:52:46.000000 derivslib-0.0.9/src/market.py
+-rw-r--r--   0 landon     (501) staff       (20)    14715 2023-04-05 01:56:44.000000 derivslib-0.0.9/src/personal.py
+-rw-r--r--   0 landon     (501) staff       (20)     3967 2023-04-03 18:29:31.000000 derivslib-0.0.9/src/utils.py
```

### Comparing `derivslib-0.0.8/PKG-INFO` & `derivslib-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: derivslib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Provides pricing tools and data for various derivative assets. I am not an attorney, accountant or financial advisor, nor am I holding myself out to be, and the information and tools contained in this package is not a substitute for financial advice from a professional who is aware of the facts and circumstances of your individual situation.
 Home-page: https://github.com/lwarner100/derivslib
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `derivslib-0.0.8/derivslib.egg-info/PKG-INFO` & `derivslib-0.0.9/derivslib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: derivslib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Provides pricing tools and data for various derivative assets. I am not an attorney, accountant or financial advisor, nor am I holding myself out to be, and the information and tools contained in this package is not a substitute for financial advice from a professional who is aware of the facts and circumstances of your individual situation.
 Home-page: https://github.com/lwarner100/derivslib
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `derivslib-0.0.8/setup.py` & `derivslib-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,20 @@
     'pandas',
     'plotly',
     'requests',
     'scipy',
     'seaborn',
     'wallstreet',
     'yfinance',
+    'derivslib'
 ]
 
 setup(
     name='derivslib',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=requirements,
     description='Provides pricing tools and data for various derivative assets. I am not an attorney, accountant or financial advisor, nor am I holding myself out to be, and the information and tools contained in this package is not a substitute for financial advice from a professional who is aware of the facts and circumstances of your individual situation.',
     url='https://github.com/lwarner100/derivslib',
     license='MIT',
     classifiers=[
         'Intended Audience :: Developers',
```

### Comparing `derivslib-0.0.8/src/cboe.py` & `derivslib-0.0.9/src/cboe.py`

 * *Files identical despite different names*

### Comparing `derivslib-0.0.8/src/derivslib.py` & `derivslib-0.0.9/src/derivslib.py`

 * *Files identical despite different names*

### Comparing `derivslib-0.0.8/src/market.py` & `derivslib-0.0.9/src/market.py`

 * *Files identical despite different names*

### Comparing `derivslib-0.0.8/src/personal.py` & `derivslib-0.0.9/src/personal.py`

 * *Files identical despite different names*

### Comparing `derivslib-0.0.8/src/utils.py` & `derivslib-0.0.9/src/utils.py`

 * *Files identical despite different names*

