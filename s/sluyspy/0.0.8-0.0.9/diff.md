# Comparing `tmp/sluyspy-0.0.8.tar.gz` & `tmp/sluyspy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sluyspy-0.0.8.tar", last modified: Mon Jan  9 16:48:35 2023, max compression
+gzip compressed data, was "sluyspy-0.0.9.tar", last modified: Mon Jan 16 10:26:13 2023, max compression
```

## Comparing `sluyspy-0.0.8.tar` & `sluyspy-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-01-09 16:48:35.213473 sluyspy-0.0.8/
--rw-r--r--   0 sluys     (1000) sluys     (1000)    13827 2022-11-09 13:13:47.000000 sluyspy-0.0.8/LICENCE
--rw-r--r--   0 sluys     (1000) sluys     (1000)     2530 2023-01-09 16:48:35.213473 sluyspy-0.0.8/PKG-INFO
--rw-r--r--   0 sluys     (1000) sluys     (1000)     1684 2022-11-09 13:13:47.000000 sluyspy-0.0.8/README.md
--rw-r--r--   0 sluys     (1000) sluys     (1000)       38 2023-01-09 16:48:35.213473 sluyspy-0.0.8/setup.cfg
--rwxr-xr-x   0 sluys     (1000) sluys     (1000)     1372 2023-01-09 16:45:43.000000 sluyspy-0.0.8/setup.py
-drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-01-09 16:48:35.212473 sluyspy-0.0.8/sluyspy/
--rw-r--r--   0 sluys     (1000) sluys     (1000)     1661 2023-01-09 16:05:47.000000 sluyspy-0.0.8/sluyspy/__init__.py
--rw-r--r--   0 sluys     (1000) sluys     (1000)      860 2023-01-09 16:05:47.000000 sluyspy-0.0.8/sluyspy/air_visual.py
--rw-r--r--   0 sluys     (1000) sluys     (1000)     2408 2023-01-09 16:05:47.000000 sluyspy-0.0.8/sluyspy/cli.py
--rw-r--r--   0 sluys     (1000) sluys     (1000)     1567 2023-01-09 16:05:47.000000 sluyspy-0.0.8/sluyspy/plot.py
--rw-r--r--   0 sluys     (1000) sluys     (1000)     1480 2023-01-09 16:27:50.000000 sluyspy-0.0.8/sluyspy/sys.py
--rw-r--r--   0 sluys     (1000) sluys     (1000)     2232 2023-01-09 16:05:47.000000 sluyspy-0.0.8/sluyspy/text.py
--rw-r--r--   0 sluys     (1000) sluys     (1000)     2011 2023-01-09 16:05:47.000000 sluyspy-0.0.8/sluyspy/weather.py
-drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-01-09 16:48:35.213473 sluyspy-0.0.8/sluyspy.egg-info/
--rw-r--r--   0 sluys     (1000) sluys     (1000)     2530 2023-01-09 16:48:35.000000 sluyspy-0.0.8/sluyspy.egg-info/PKG-INFO
--rw-r--r--   0 sluys     (1000) sluys     (1000)      303 2023-01-09 16:48:35.000000 sluyspy-0.0.8/sluyspy.egg-info/SOURCES.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)        1 2023-01-09 16:48:35.000000 sluyspy-0.0.8/sluyspy.egg-info/dependency_links.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)       33 2023-01-09 16:48:35.000000 sluyspy-0.0.8/sluyspy.egg-info/requires.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)        8 2023-01-09 16:48:35.000000 sluyspy-0.0.8/sluyspy.egg-info/top_level.txt
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-01-16 10:26:13.006322 sluyspy-0.0.9/
+-rw-r--r--   0 sluys     (1000) sluys     (1000)    13827 2022-11-09 13:13:47.000000 sluyspy-0.0.9/LICENCE
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     2535 2023-01-16 10:26:13.006322 sluyspy-0.0.9/PKG-INFO
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     1689 2023-01-16 08:40:18.000000 sluyspy-0.0.9/README.md
+-rw-r--r--   0 sluys     (1000) sluys     (1000)       38 2023-01-16 10:26:13.006322 sluyspy-0.0.9/setup.cfg
+-rwxr-xr-x   0 sluys     (1000) sluys     (1000)     1372 2023-01-16 08:40:42.000000 sluyspy-0.0.9/setup.py
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-01-16 10:26:13.006322 sluyspy-0.0.9/sluyspy/
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     1661 2023-01-09 16:05:47.000000 sluyspy-0.0.9/sluyspy/__init__.py
+-rw-r--r--   0 sluys     (1000) sluys     (1000)      860 2023-01-09 16:05:47.000000 sluyspy-0.0.9/sluyspy/air_visual.py
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     2418 2023-01-16 08:38:29.000000 sluyspy-0.0.9/sluyspy/cli.py
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     1567 2023-01-09 16:05:47.000000 sluyspy-0.0.9/sluyspy/plot.py
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     1480 2023-01-09 16:27:50.000000 sluyspy-0.0.9/sluyspy/sys.py
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     2232 2023-01-09 16:05:47.000000 sluyspy-0.0.9/sluyspy/text.py
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     2011 2023-01-09 16:05:47.000000 sluyspy-0.0.9/sluyspy/weather.py
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-01-16 10:26:13.006322 sluyspy-0.0.9/sluyspy.egg-info/
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     2535 2023-01-16 10:26:12.000000 sluyspy-0.0.9/sluyspy.egg-info/PKG-INFO
+-rw-r--r--   0 sluys     (1000) sluys     (1000)      303 2023-01-16 10:26:12.000000 sluyspy-0.0.9/sluyspy.egg-info/SOURCES.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)        1 2023-01-16 10:26:12.000000 sluyspy-0.0.9/sluyspy.egg-info/dependency_links.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)       33 2023-01-16 10:26:12.000000 sluyspy-0.0.9/sluyspy.egg-info/requires.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)        8 2023-01-16 10:26:12.000000 sluyspy-0.0.9/sluyspy.egg-info/top_level.txt
```

### Comparing `sluyspy-0.0.8/LICENCE` & `sluyspy-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `sluyspy-0.0.8/PKG-INFO` & `sluyspy-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sluyspy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Marc van der Sluys' personal Python modules.
 Home-page: https://github.com/MarcvdSluys/sluyspy
 Author: Marc van der Sluys
 License: EUPL 1.2
 Keywords: personal,private
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -64,8 +64,8 @@
 * Contact: http://marc.vandersluys.nl
 * Licence: [EUPL 1.2](https://www.eupl.eu/1.2/en/)
 
 
 ## References ##
 
 
-<sub>Copyright (c) 2022 Marc van der Sluys</sub>
+<sub>Copyright (c) 2022-2023 Marc van der Sluys</sub>
```

### Comparing `sluyspy-0.0.8/README.md` & `sluyspy-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 * Contact: http://marc.vandersluys.nl
 * Licence: [EUPL 1.2](https://www.eupl.eu/1.2/en/)
 
 
 ## References ##
 
 
-<sub>Copyright (c) 2022 Marc van der Sluys</sub>
+<sub>Copyright (c) 2022-2023 Marc van der Sluys</sub>
```

### Comparing `sluyspy-0.0.8/setup.py` & `sluyspy-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/bin/env python
 # -*- coding: utf-8 -*-
 
 """Setup.py for the sluyspy Python package."""
 
 
 # Package version:
-version='0.0.8'
+version='0.0.9'
 
 # Get long description from README.md:
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 # Set package properties:
 from setuptools import setup
```

### Comparing `sluyspy-0.0.8/sluyspy/__init__.py` & `sluyspy-0.0.9/sluyspy/__init__.py`

 * *Files identical despite different names*

### Comparing `sluyspy-0.0.8/sluyspy/air_visual.py` & `sluyspy-0.0.9/sluyspy/air_visual.py`

 * *Files identical despite different names*

### Comparing `sluyspy-0.0.8/sluyspy/cli.py` & `sluyspy-0.0.9/sluyspy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,26 +46,26 @@
     
     Parameters:
       message (str):        Message to print.
       exit_program (bool):  Exit the program or not, defaults to True.
       exit_code (int):      Exit code to exit the program with, defaults to 1.
     """
     
-    _sys.stderr.write('\n'+_clr('ERROR: '+message, 'white', 'on_red', attrs=['bold'])+'\n\n')
+    _sys.stderr.write('\n'+_clr('ERROR: '+str(message), 'white', 'on_red', attrs=['bold'])+'\n\n')
     
     if exit_program: exit(exit_code)
     return
 
 
 def warn(message, exit_program=False, exit_code=1):
     """Print a coloured warn message to stderr and exit.
     
     Parameters:
       message (str):        Message to print.
       exit_program (bool):  Exit the program or not, defaults to False.
       exit_code (int):      Exit code to exit the program with, defaults to 1.
     """
     
-    _sys.stderr.write('\n'+_clr('Warning: '+message, 'white', 'on_yellow', attrs=['bold'])+'\n\n')
+    _sys.stderr.write('\n'+_clr('Warning: '+str(message), 'white', 'on_yellow', attrs=['bold'])+'\n\n')
     
     if exit_program: exit(exit_code)
     return
```

### Comparing `sluyspy-0.0.8/sluyspy/plot.py` & `sluyspy-0.0.9/sluyspy/plot.py`

 * *Files identical despite different names*

### Comparing `sluyspy-0.0.8/sluyspy/sys.py` & `sluyspy-0.0.9/sluyspy/sys.py`

 * *Files identical despite different names*

### Comparing `sluyspy-0.0.8/sluyspy/text.py` & `sluyspy-0.0.9/sluyspy/text.py`

 * *Files identical despite different names*

### Comparing `sluyspy-0.0.8/sluyspy/weather.py` & `sluyspy-0.0.9/sluyspy/weather.py`

 * *Files identical despite different names*

### Comparing `sluyspy-0.0.8/sluyspy.egg-info/PKG-INFO` & `sluyspy-0.0.9/sluyspy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sluyspy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Marc van der Sluys' personal Python modules.
 Home-page: https://github.com/MarcvdSluys/sluyspy
 Author: Marc van der Sluys
 License: EUPL 1.2
 Keywords: personal,private
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -64,8 +64,8 @@
 * Contact: http://marc.vandersluys.nl
 * Licence: [EUPL 1.2](https://www.eupl.eu/1.2/en/)
 
 
 ## References ##
 
 
-<sub>Copyright (c) 2022 Marc van der Sluys</sub>
+<sub>Copyright (c) 2022-2023 Marc van der Sluys</sub>
```

