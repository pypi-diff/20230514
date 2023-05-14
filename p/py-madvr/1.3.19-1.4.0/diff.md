# Comparing `tmp/py_madvr-1.3.19.tar.gz` & `tmp/py_madvr-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.3.19.tar", last modified: Sun May 14 18:38:55 2023, max compression
+gzip compressed data, was "py_madvr-1.4.0.tar", last modified: Sun May 14 19:05:48 2023, max compression
```

## Comparing `py_madvr-1.3.19.tar` & `py_madvr-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:38:55.624011 py_madvr-1.3.19/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 18:38:44.000000 py_madvr-1.3.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 18:38:55.620011 py_madvr-1.3.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 18:38:44.000000 py_madvr-1.3.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:38:55.620011 py_madvr-1.3.19/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 18:38:44.000000 py_madvr-1.3.19/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 18:38:44.000000 py_madvr-1.3.19/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 18:38:44.000000 py_madvr-1.3.19/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-05-14 18:38:44.000000 py_madvr-1.3.19/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:38:55.620011 py_madvr-1.3.19/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-14 18:38:55.000000 py_madvr-1.3.19/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 18:38:55.000000 py_madvr-1.3.19/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:38:55.000000 py_madvr-1.3.19/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 18:38:55.000000 py_madvr-1.3.19/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 18:38:55.624011 py_madvr-1.3.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 18:38:44.000000 py_madvr-1.3.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:38:55.620011 py_madvr-1.3.19/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 18:38:44.000000 py_madvr-1.3.19/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 18:38:44.000000 py_madvr-1.3.19/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:05:48.981392 py_madvr-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 19:05:37.000000 py_madvr-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-14 19:05:48.981392 py_madvr-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-14 19:05:37.000000 py_madvr-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:05:48.981392 py_madvr-1.4.0/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 19:05:37.000000 py_madvr-1.4.0/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-14 19:05:37.000000 py_madvr-1.4.0/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 19:05:37.000000 py_madvr-1.4.0/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16160 2023-05-14 19:05:37.000000 py_madvr-1.4.0/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:05:48.981392 py_madvr-1.4.0/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-14 19:05:48.000000 py_madvr-1.4.0/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 19:05:48.000000 py_madvr-1.4.0/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 19:05:48.000000 py_madvr-1.4.0/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 19:05:48.000000 py_madvr-1.4.0/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 19:05:48.981392 py_madvr-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-14 19:05:37.000000 py_madvr-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:05:48.981392 py_madvr-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:05:37.000000 py_madvr-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 19:05:37.000000 py_madvr-1.4.0/tests/testMadVR.py
```

### Comparing `py_madvr-1.3.19/LICENSE` & `py_madvr-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.19/madvr/commands.py` & `py_madvr-1.4.0/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.3.19/madvr/madvr.py` & `py_madvr-1.4.0/madvr/madvr.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
                     )
             except ConnectionResetError:
                 self.logger.warning(
                     "Connection reset by peer. Attempting to reconnect..."
                 )
                 await self._reconnect()
             except (AttributeError, asyncio.TimeoutError, OSError) as err:
-                self.logger.warning(
+                self.logger.debug(
                     "Reading notifications failed or timed out: %s", err
                 )
                 await asyncio.sleep(5)
                 continue
 
             if not msg:
                 await asyncio.sleep(1)
```

### Comparing `py_madvr-1.3.19/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.4.0/py_madvr.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.3.19
+Version: 1.4.0
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Py MadVR
+# MadVR Envy Python Library
 
-Support for IP based controls for Envys''
+Support for IP based controls for MadVR Envy
 
-*Note: IP control does not work if there is no input signal, by design"
-
-Readme WIP
+Supports real time notifications and commands
 
 ## Commands
-same as the one in the docs like PowerOff. 
+Command structure follows the same in the manual https://madvrenvy.com/wp-content/uploads/EnvyIpControl.pdf?r=112a
 
-For things that take params, use a command -> KeyPress, MENU
+For things that take values, use a comma -> `["KeyPress, MENU"]`
 
-if you want to use power_off() you need to run it before turnging off other stuff bc render thread
-Recomend configuring update to be short, less than 5 seconds
+Not every single command is implemented, such as submenus or changing complicated options. You can use commands for all the typical stuff the remote can do.
```

### Comparing `py_madvr-1.3.19/setup.py` & `py_madvr-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.3.19",
+    version="1.4.0",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.3.19/tests/testMadVR.py` & `py_madvr-1.4.0/tests/testMadVR.py`

 * *Files identical despite different names*

