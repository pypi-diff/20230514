# Comparing `tmp/pydeps-1.9.8.tar.gz` & `tmp/pydeps-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pydeps-1.9.8.tar", last modified: Fri Aug 21 22:11:45 2020, max compression
+gzip compressed data, was "dist\pydeps-1.9.9.tar", last modified: Thu Sep  3 11:23:23 2020, max compression
```

## Comparing `pydeps-1.9.8.tar` & `pydeps-1.9.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2020-08-21 22:11:45.000000 pydeps-1.9.8/
--rw-rw-rw-   0        0        0    20362 2020-08-21 22:11:45.000000 pydeps-1.9.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2020-08-21 22:11:45.000000 pydeps-1.9.8/pydeps/
--rw-rw-rw-   0        0        0     5396 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/arguments.py
--rw-rw-rw-   0        0        0     8916 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/cli.py
--rw-rw-rw-   0        0        0     4316 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/colors.py
--rw-rw-rw-   0        0        0    14628 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/depgraph.py
--rw-rw-rw-   0        0        0     4638 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/depgraph2dot.py
--rw-rw-rw-   0        0        0     2603 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/dot.py
--rw-rw-rw-   0        0        0     4710 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/dummymodule.py
--rw-rw-rw-   0        0        0    27716 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/mf27.py
--rw-rw-rw-   0        0        0     1157 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/package_names.py
--rw-rw-rw-   0        0        0    10071 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/py2depgraph.py
--rw-rw-rw-   0        0        0      295 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/pycompat.py
--rw-rw-rw-   0        0        0     5089 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/pydeps.py
--rw-rw-rw-   0        0        0     1201 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/pystdlib.py
--rw-rw-rw-   0        0        0    10055 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/render_context.py
--rw-rw-rw-   0        0        0     3379 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/target.py
--rw-rw-rw-   0        0        0      204 2020-08-21 22:08:10.000000 pydeps-1.9.8/pydeps/__init__.py
--rw-rw-rw-   0        0        0       36 2020-08-21 22:07:42.000000 pydeps-1.9.8/pydeps/__main__.py
-drwxrwxrwx   0        0        0        0 2020-08-21 22:11:45.000000 pydeps-1.9.8/pydeps.egg-info/
--rw-rw-rw-   0        0        0        1 2020-08-21 22:11:45.000000 pydeps-1.9.8/pydeps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2020-08-21 22:11:45.000000 pydeps-1.9.8/pydeps.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    20362 2020-08-21 22:11:45.000000 pydeps-1.9.8/pydeps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       46 2020-08-21 22:11:45.000000 pydeps-1.9.8/pydeps.egg-info/requires.txt
--rw-rw-rw-   0        0        0      526 2020-08-21 22:11:45.000000 pydeps-1.9.8/pydeps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2020-08-21 22:11:45.000000 pydeps-1.9.8/pydeps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    16067 2020-08-21 22:07:42.000000 pydeps-1.9.8/README.rst
--rw-rw-rw-   0        0        0       42 2020-08-21 22:11:45.000000 pydeps-1.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1868 2020-08-21 22:08:10.000000 pydeps-1.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-09-03 11:23:23.000000 pydeps-1.9.9/
+-rw-rw-rw-   0        0        0    20760 2020-09-03 11:23:23.000000 pydeps-1.9.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2020-09-03 11:23:23.000000 pydeps-1.9.9/pydeps/
+-rw-rw-rw-   0        0        0     5396 2019-08-21 08:56:39.000000 pydeps-1.9.9/pydeps/arguments.py
+-rw-rw-rw-   0        0        0     8916 2020-07-31 12:40:20.000000 pydeps-1.9.9/pydeps/cli.py
+-rw-rw-rw-   0        0        0     4316 2019-12-05 08:29:04.000000 pydeps-1.9.9/pydeps/colors.py
+-rw-rw-rw-   0        0        0    14628 2020-05-06 08:43:25.000000 pydeps-1.9.9/pydeps/depgraph.py
+-rw-rw-rw-   0        0        0     4638 2020-05-06 08:43:25.000000 pydeps-1.9.9/pydeps/depgraph2dot.py
+-rw-rw-rw-   0        0        0     2603 2020-09-03 11:09:41.000000 pydeps-1.9.9/pydeps/dot.py
+-rw-rw-rw-   0        0        0     4710 2019-08-21 08:56:39.000000 pydeps-1.9.9/pydeps/dummymodule.py
+-rw-rw-rw-   0        0        0    27716 2019-08-21 08:56:39.000000 pydeps-1.9.9/pydeps/mf27.py
+-rw-rw-rw-   0        0        0     1157 2019-10-28 08:24:08.000000 pydeps-1.9.9/pydeps/package_names.py
+-rw-rw-rw-   0        0        0    10071 2019-08-21 08:56:39.000000 pydeps-1.9.9/pydeps/py2depgraph.py
+-rw-rw-rw-   0        0        0      295 2019-08-21 08:56:39.000000 pydeps-1.9.9/pydeps/pycompat.py
+-rw-rw-rw-   0        0        0     5089 2020-09-03 11:09:41.000000 pydeps-1.9.9/pydeps/pydeps.py
+-rw-rw-rw-   0        0        0     1201 2019-08-21 08:56:39.000000 pydeps-1.9.9/pydeps/pystdlib.py
+-rw-rw-rw-   0        0        0    10055 2020-05-06 08:43:25.000000 pydeps-1.9.9/pydeps/render_context.py
+-rw-rw-rw-   0        0        0     3379 2019-11-25 08:41:50.000000 pydeps-1.9.9/pydeps/target.py
+-rw-rw-rw-   0        0        0      204 2020-09-03 11:21:57.000000 pydeps-1.9.9/pydeps/__init__.py
+-rw-rw-rw-   0        0        0       36 2019-08-21 08:56:39.000000 pydeps-1.9.9/pydeps/__main__.py
+drwxrwxrwx   0        0        0        0 2020-09-03 11:23:23.000000 pydeps-1.9.9/pydeps.egg-info/
+-rw-rw-rw-   0        0        0        1 2020-09-03 11:23:22.000000 pydeps-1.9.9/pydeps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2020-09-03 11:23:22.000000 pydeps-1.9.9/pydeps.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    20760 2020-09-03 11:23:22.000000 pydeps-1.9.9/pydeps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2020-09-03 11:23:22.000000 pydeps-1.9.9/pydeps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      526 2020-09-03 11:23:22.000000 pydeps-1.9.9/pydeps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2020-09-03 11:23:22.000000 pydeps-1.9.9/pydeps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    16393 2020-09-03 11:21:34.000000 pydeps-1.9.9/README.rst
+-rw-rw-rw-   0        0        0       42 2020-09-03 11:23:23.000000 pydeps-1.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1868 2020-09-03 11:21:57.000000 pydeps-1.9.9/setup.py
```

### Comparing `pydeps-1.9.8/PKG-INFO` & `pydeps-1.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 1.1
 Name: pydeps
-Version: 1.9.8
+Version: 1.9.9
 Summary: Display module dependencies
 Home-page: https://github.com/thebjorn/pydeps
 Author: bjorn
 Author-email: bp@datakortet.no
 License: BSD
-Description: 
-        pydeps
+Description: pydeps
         ======
         
         .. image:: https://readthedocs.org/projects/pydeps/badge/?version=latest
            :target: https://readthedocs.org/projects/pydeps/?badge=latest
            :alt: Documentation Status
         
         .. image:: https://travis-ci.org/thebjorn/pydeps.svg
@@ -24,16 +23,19 @@
         .. image:: https://pepy.tech/badge/pydeps
            :target: https://pepy.tech/project/pydeps
            :alt: Downloads
         
         Python module dependency visualization. This package installs the ``pydeps``
         command, and normal usage will be to use it from the command line.
         
+        .. contents::
+           :depth: 2
+        
         How to install
-        ==============
+        --------------
         ::
         
             pip install pydeps
         
         Basic Usage
         -----------
         From the shell::
@@ -73,14 +75,18 @@
         
         Please report bugs and feature requests on GitHub at
         https://github.com/thebjorn/pydeps/issues
         
         Version history
         ---------------
         
+        **Version 1.9.8** Fix for ``maximum recursion depth exceeded`` when using large
+        frameworks (like ``sympy``).  Thanks to tanujkhattar_ for finding the fix and to
+        balopat_ for reporting it.
+        
         **Version 1.9.7** Check ``PYDEPS_DISPLAY`` and ``BROWSER`` for a program to open
         the graph, PR by jhermann_
         
         **Version 1.9.6** ``--no-show`` and ``--no-dot`` as aliases for ``--noshow``
         and ``--nodot``, PR by jhermann_
         
         .. 
@@ -174,16 +180,16 @@
         
         This is the result of running ``pydeps`` on itself (``pydeps pydeps``):
         
         .. image:: https://raw.githubusercontent.com/thebjorn/pydeps/master/docs/_static/pydeps.svg?sanitize=true
         
         (full disclosure: this is for an early version of pydeps)
         
-        Bacon
-        ~~~~~
+        Bacon (Scoring)
+        ---------------
         
         ``pydeps`` also contains an Erdős-like scoring function (a.k.a. Bacon
         number, from Six degrees of Kevin Bacon
         (http://en.wikipedia.org/wiki/Six_Degrees_of_Kevin_Bacon) that lets
         you filter out modules that are more than a given number of 'hops'
         away from the module you're interested in.  This is useful for finding
         the interface a module has to the rest of the world.
@@ -403,14 +409,16 @@
         .. _eight04: https://github.com/eight04
         .. _tomasito665: https://github.com/Tomasito665
         .. _aroberge: https://github.com/aroberge
         .. _pawamoy: https://github.com/pawamoy
         .. _kinow: https://github.com/kinow
         .. _ewen-lbh: https://github.com/ewen-lbh
         .. _jhermann: https://github.com/jhermann
+        .. _balopat: https://github.com/balopat
+        .. _tanujkhattar: https://github.com/tanujkhattar
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `pydeps-1.9.8/pydeps/arguments.py` & `pydeps-1.9.9/pydeps/arguments.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/cli.py` & `pydeps-1.9.9/pydeps/cli.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/colors.py` & `pydeps-1.9.9/pydeps/colors.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/depgraph.py` & `pydeps-1.9.9/pydeps/depgraph.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/depgraph2dot.py` & `pydeps-1.9.9/pydeps/depgraph2dot.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/dot.py` & `pydeps-1.9.9/pydeps/dot.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/dummymodule.py` & `pydeps-1.9.9/pydeps/dummymodule.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/mf27.py` & `pydeps-1.9.9/pydeps/mf27.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/package_names.py` & `pydeps-1.9.9/pydeps/package_names.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/py2depgraph.py` & `pydeps-1.9.9/pydeps/py2depgraph.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/pydeps.py` & `pydeps-1.9.9/pydeps/pydeps.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/pystdlib.py` & `pydeps-1.9.9/pydeps/pystdlib.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/render_context.py` & `pydeps-1.9.9/pydeps/render_context.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps/target.py` & `pydeps-1.9.9/pydeps/target.py`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/pydeps.egg-info/PKG-INFO` & `pydeps-1.9.9/pydeps.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 1.1
 Name: pydeps
-Version: 1.9.8
+Version: 1.9.9
 Summary: Display module dependencies
 Home-page: https://github.com/thebjorn/pydeps
 Author: bjorn
 Author-email: bp@datakortet.no
 License: BSD
-Description: 
-        pydeps
+Description: pydeps
         ======
         
         .. image:: https://readthedocs.org/projects/pydeps/badge/?version=latest
            :target: https://readthedocs.org/projects/pydeps/?badge=latest
            :alt: Documentation Status
         
         .. image:: https://travis-ci.org/thebjorn/pydeps.svg
@@ -24,16 +23,19 @@
         .. image:: https://pepy.tech/badge/pydeps
            :target: https://pepy.tech/project/pydeps
            :alt: Downloads
         
         Python module dependency visualization. This package installs the ``pydeps``
         command, and normal usage will be to use it from the command line.
         
+        .. contents::
+           :depth: 2
+        
         How to install
-        ==============
+        --------------
         ::
         
             pip install pydeps
         
         Basic Usage
         -----------
         From the shell::
@@ -73,14 +75,18 @@
         
         Please report bugs and feature requests on GitHub at
         https://github.com/thebjorn/pydeps/issues
         
         Version history
         ---------------
         
+        **Version 1.9.8** Fix for ``maximum recursion depth exceeded`` when using large
+        frameworks (like ``sympy``).  Thanks to tanujkhattar_ for finding the fix and to
+        balopat_ for reporting it.
+        
         **Version 1.9.7** Check ``PYDEPS_DISPLAY`` and ``BROWSER`` for a program to open
         the graph, PR by jhermann_
         
         **Version 1.9.6** ``--no-show`` and ``--no-dot`` as aliases for ``--noshow``
         and ``--nodot``, PR by jhermann_
         
         .. 
@@ -174,16 +180,16 @@
         
         This is the result of running ``pydeps`` on itself (``pydeps pydeps``):
         
         .. image:: https://raw.githubusercontent.com/thebjorn/pydeps/master/docs/_static/pydeps.svg?sanitize=true
         
         (full disclosure: this is for an early version of pydeps)
         
-        Bacon
-        ~~~~~
+        Bacon (Scoring)
+        ---------------
         
         ``pydeps`` also contains an Erdős-like scoring function (a.k.a. Bacon
         number, from Six degrees of Kevin Bacon
         (http://en.wikipedia.org/wiki/Six_Degrees_of_Kevin_Bacon) that lets
         you filter out modules that are more than a given number of 'hops'
         away from the module you're interested in.  This is useful for finding
         the interface a module has to the rest of the world.
@@ -403,14 +409,16 @@
         .. _eight04: https://github.com/eight04
         .. _tomasito665: https://github.com/Tomasito665
         .. _aroberge: https://github.com/aroberge
         .. _pawamoy: https://github.com/pawamoy
         .. _kinow: https://github.com/kinow
         .. _ewen-lbh: https://github.com/ewen-lbh
         .. _jhermann: https://github.com/jhermann
+        .. _balopat: https://github.com/balopat
+        .. _tanujkhattar: https://github.com/tanujkhattar
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `pydeps-1.9.8/pydeps.egg-info/SOURCES.txt` & `pydeps-1.9.9/pydeps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydeps-1.9.8/README.rst` & `pydeps-1.9.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 pydeps
 ======
 
 .. image:: https://readthedocs.org/projects/pydeps/badge/?version=latest
    :target: https://readthedocs.org/projects/pydeps/?badge=latest
    :alt: Documentation Status
 
@@ -16,16 +15,19 @@
 .. image:: https://pepy.tech/badge/pydeps
    :target: https://pepy.tech/project/pydeps
    :alt: Downloads
 
 Python module dependency visualization. This package installs the ``pydeps``
 command, and normal usage will be to use it from the command line.
 
+.. contents::
+   :depth: 2
+
 How to install
-==============
+--------------
 ::
 
     pip install pydeps
 
 Basic Usage
 -----------
 From the shell::
@@ -65,14 +67,18 @@
 
 Please report bugs and feature requests on GitHub at
 https://github.com/thebjorn/pydeps/issues
 
 Version history
 ---------------
 
+**Version 1.9.8** Fix for ``maximum recursion depth exceeded`` when using large
+frameworks (like ``sympy``).  Thanks to tanujkhattar_ for finding the fix and to
+balopat_ for reporting it.
+
 **Version 1.9.7** Check ``PYDEPS_DISPLAY`` and ``BROWSER`` for a program to open
 the graph, PR by jhermann_
 
 **Version 1.9.6** ``--no-show`` and ``--no-dot`` as aliases for ``--noshow``
 and ``--nodot``, PR by jhermann_
 
 .. 
@@ -166,16 +172,16 @@
 
 This is the result of running ``pydeps`` on itself (``pydeps pydeps``):
 
 .. image:: https://raw.githubusercontent.com/thebjorn/pydeps/master/docs/_static/pydeps.svg?sanitize=true
 
 (full disclosure: this is for an early version of pydeps)
 
-Bacon
-~~~~~
+Bacon (Scoring)
+---------------
 
 ``pydeps`` also contains an Erdős-like scoring function (a.k.a. Bacon
 number, from Six degrees of Kevin Bacon
 (http://en.wikipedia.org/wiki/Six_Degrees_of_Kevin_Bacon) that lets
 you filter out modules that are more than a given number of 'hops'
 away from the module you're interested in.  This is useful for finding
 the interface a module has to the rest of the world.
@@ -395,7 +401,9 @@
 .. _eight04: https://github.com/eight04
 .. _tomasito665: https://github.com/Tomasito665
 .. _aroberge: https://github.com/aroberge
 .. _pawamoy: https://github.com/pawamoy
 .. _kinow: https://github.com/kinow
 .. _ewen-lbh: https://github.com/ewen-lbh
 .. _jhermann: https://github.com/jhermann
+.. _balopat: https://github.com/balopat
+.. _tanujkhattar: https://github.com/tanujkhattar
```

### Comparing `pydeps-1.9.8/setup.py` & `pydeps-1.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import io
 import sys
 
 import setuptools
 from distutils.core import setup
 from setuptools.command.test import test as TestCommand
 
-version='1.9.8'
+version='1.9.9'
 
 
 class PyTest(TestCommand):
     user_options = [('pytest-args=', 'a', "Arguments to pass to py.test")]
 
     def initialize_options(self):
         TestCommand.initialize_options(self)
```

