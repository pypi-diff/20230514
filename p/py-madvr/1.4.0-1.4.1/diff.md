# Comparing `tmp/py_madvr-1.4.0.tar.gz` & `tmp/py_madvr-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.4.0.tar", last modified: Sun May 14 19:05:48 2023, max compression
+gzip compressed data, was "py_madvr-1.4.1.tar", last modified: Sun May 14 20:42:14 2023, max compression
```

## Comparing `py_madvr-1.4.0.tar` & `py_madvr-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:05:48.981392 py_madvr-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 19:05:37.000000 py_madvr-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-14 19:05:48.981392 py_madvr-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-14 19:05:37.000000 py_madvr-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:05:48.981392 py_madvr-1.4.0/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 19:05:37.000000 py_madvr-1.4.0/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 19:05:37.000000 py_madvr-1.4.0/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 19:05:37.000000 py_madvr-1.4.0/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16160 2023-05-14 19:05:37.000000 py_madvr-1.4.0/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:05:48.981392 py_madvr-1.4.0/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-14 19:05:48.000000 py_madvr-1.4.0/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 19:05:48.000000 py_madvr-1.4.0/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 19:05:48.000000 py_madvr-1.4.0/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 19:05:48.000000 py_madvr-1.4.0/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 19:05:48.981392 py_madvr-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-14 19:05:37.000000 py_madvr-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:05:48.981392 py_madvr-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:05:37.000000 py_madvr-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 19:05:37.000000 py_madvr-1.4.0/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:42:14.495768 py_madvr-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 20:42:03.000000 py_madvr-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-14 20:42:14.495768 py_madvr-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-14 20:42:03.000000 py_madvr-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:42:14.491768 py_madvr-1.4.1/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 20:42:03.000000 py_madvr-1.4.1/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 20:42:03.000000 py_madvr-1.4.1/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 20:42:03.000000 py_madvr-1.4.1/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-05-14 20:42:03.000000 py_madvr-1.4.1/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:42:14.495768 py_madvr-1.4.1/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-14 20:42:14.000000 py_madvr-1.4.1/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 20:42:14.000000 py_madvr-1.4.1/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:42:14.000000 py_madvr-1.4.1/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 20:42:14.000000 py_madvr-1.4.1/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:42:14.495768 py_madvr-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-14 20:42:03.000000 py_madvr-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:42:14.495768 py_madvr-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 20:42:03.000000 py_madvr-1.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 20:42:03.000000 py_madvr-1.4.1/tests/testMadVR.py
```

### Comparing `py_madvr-1.4.0/LICENSE` & `py_madvr-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.4.0/PKG-INFO` & `py_madvr-1.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.4.0
+Version: 1.4.1
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.4.0/madvr/commands.py` & `py_madvr-1.4.1/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.4.0/madvr/madvr.py` & `py_madvr-1.4.1/madvr/madvr.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,15 +395,15 @@
         It uses about 30w idle on standby. I use IR via harmony to turn it on
 
         standby: bool -> standby instead of poweroff if true
         """
         # dont do anything if its off besides mark it off
         # sending command will open connection
         try:
-            res = await self.send_command("Standby" if standby else "PowerOff")
+            res = await self.send_command(["Standby"] if standby else ["PowerOff"])
             await self.close_connection()
             self.is_on = False
 
             return res
 
         except RetryExceededError:
             return "Retries Exceeded"
```

### Comparing `py_madvr-1.4.0/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.4.1/py_madvr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.4.0
+Version: 1.4.1
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.4.0/setup.py` & `py_madvr-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.4.0",
+    version="1.4.1",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.4.0/tests/testMadVR.py` & `py_madvr-1.4.1/tests/testMadVR.py`

 * *Files identical despite different names*

