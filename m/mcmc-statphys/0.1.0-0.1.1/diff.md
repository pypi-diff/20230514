# Comparing `tmp/mcmc_statphys-0.1.0.tar.gz` & `tmp/mcmc_statphys-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcmc_statphys-0.1.0.tar", last modified: Sun May 14 08:56:06 2023, max compression
+gzip compressed data, was "mcmc_statphys-0.1.1.tar", last modified: Sun May 14 13:46:14 2023, max compression
```

## Comparing `mcmc_statphys-0.1.0.tar` & `mcmc_statphys-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 08:56:06.663652 mcmc_statphys-0.1.0/
--rw-rw-rw-   0        0        0      170 2023-05-14 08:17:00.000000 mcmc_statphys-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3721 2023-05-14 08:17:00.000000 mcmc_statphys-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-05-14 08:17:00.000000 mcmc_statphys-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2023-05-14 08:17:00.000000 mcmc_statphys-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-14 08:17:00.000000 mcmc_statphys-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2040 2023-05-14 08:56:06.665646 mcmc_statphys-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2023-05-14 08:17:00.000000 mcmc_statphys-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 08:56:06.568051 mcmc_statphys-0.1.0/docs/
--rw-rw-rw-   0        0        0      634 2023-05-14 08:17:01.000000 mcmc_statphys-0.1.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-14 08:17:01.000000 mcmc_statphys-0.1.0/docs/authors.rst
--rw-rw-rw-   0        0        0     5006 2023-05-14 08:17:01.000000 mcmc_statphys-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-14 08:17:01.000000 mcmc_statphys-0.1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-14 08:17:01.000000 mcmc_statphys-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      330 2023-05-14 08:17:01.000000 mcmc_statphys-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0     1209 2023-05-14 08:17:01.000000 mcmc_statphys-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0      811 2023-05-14 08:17:01.000000 mcmc_statphys-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-05-14 08:17:01.000000 mcmc_statphys-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0       88 2023-05-14 08:17:01.000000 mcmc_statphys-0.1.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 08:56:06.582247 mcmc_statphys-0.1.0/mcmc_statphys/
--rw-rw-rw-   0        0        0      137 2023-05-14 06:30:53.000000 mcmc_statphys-0.1.0/mcmc_statphys/__init__.py
--rw-rw-rw-   0        0        0      435 2023-05-14 06:30:49.000000 mcmc_statphys-0.1.0/mcmc_statphys/cli.py
--rw-rw-rw-   0        0        0    16740 2023-05-14 08:41:03.000000 mcmc_statphys-0.1.0/mcmc_statphys/mcmc_statphys.py
--rw-rw-rw-   0        0        0     6083 2023-05-14 03:28:20.000000 mcmc_statphys-0.1.0/mcmc_statphys/model.py
--rw-rw-rw-   0        0        0    11146 2023-05-14 07:39:06.000000 mcmc_statphys-0.1.0/mcmc_statphys/sample.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:56:06.654675 mcmc_statphys-0.1.0/mcmc_statphys.egg-info/
--rw-rw-rw-   0        0        0     2040 2023-05-14 08:56:06.000000 mcmc_statphys-0.1.0/mcmc_statphys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-05-14 08:56:06.000000 mcmc_statphys-0.1.0/mcmc_statphys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 08:56:06.000000 mcmc_statphys-0.1.0/mcmc_statphys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-14 08:56:06.000000 mcmc_statphys-0.1.0/mcmc_statphys.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-14 08:56:06.000000 mcmc_statphys-0.1.0/mcmc_statphys.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-05-14 08:56:06.000000 mcmc_statphys-0.1.0/mcmc_statphys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-14 08:56:06.000000 mcmc_statphys-0.1.0/mcmc_statphys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      408 2023-05-14 08:56:06.671629 mcmc_statphys-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1611 2023-05-14 08:52:04.000000 mcmc_statphys-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:56:06.659662 mcmc_statphys-0.1.0/tests/
--rw-rw-rw-   0        0        0       44 2023-05-14 08:17:01.000000 mcmc_statphys-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      927 2023-05-14 08:17:01.000000 mcmc_statphys-0.1.0/tests/test_mcmc_statphys.py
+drwxrwxrwx   0        0        0        0 2023-05-14 13:46:14.159690 mcmc_statphys-0.1.1/
+-rw-rw-rw-   0        0        0      170 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3721 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1989 2023-05-14 13:46:14.159690 mcmc_statphys-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 13:46:14.037117 mcmc_statphys-0.1.1/docs/
+-rw-rw-rw-   0        0        0      634 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     5006 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/history.rst
+-rw-rw-rw-   0        0        0      330 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1209 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      811 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       88 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 13:46:14.074634 mcmc_statphys-0.1.1/mcmc_statphys/
+-rw-rw-rw-   0        0        0      143 2023-05-14 12:02:25.000000 mcmc_statphys-0.1.1/mcmc_statphys/__init__.py
+-rw-rw-rw-   0        0        0      434 2023-05-14 12:02:25.000000 mcmc_statphys-0.1.1/mcmc_statphys/cli.py
+-rw-rw-rw-   0        0        0    10952 2023-05-14 10:14:57.000000 mcmc_statphys-0.1.1/mcmc_statphys/mcmc_statphys.py
+-rw-rw-rw-   0        0        0     6083 2023-05-14 09:16:12.000000 mcmc_statphys-0.1.1/mcmc_statphys/model.py
+drwxrwxrwx   0        0        0        0 2023-05-14 13:46:14.124783 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/
+-rw-rw-rw-   0        0        0     1989 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-14 13:46:13.000000 mcmc_statphys-0.1.1/mcmc_statphys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      408 2023-05-14 13:46:14.162684 mcmc_statphys-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1557 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 13:46:14.158692 mcmc_statphys-0.1.1/tests/
+-rw-rw-rw-   0        0        0       44 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      927 2023-05-14 13:37:58.000000 mcmc_statphys-0.1.1/tests/test_mcmc_statphys.py
```

### Comparing `mcmc_statphys-0.1.0/CONTRIBUTING.rst` & `mcmc_statphys-0.1.1/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 Look through the GitHub issues for features. Anything tagged with "enhancement"
 and "help wanted" is open to whoever wants to implement it.
 
 Write Documentation
 ~~~~~~~~~~~~~~~~~~~
 
-mcmc-statphys could always use more documentation, whether as part of the
-official mcmc-statphys docs, in docstrings, or even on the web in blog posts,
+mcmc_statphys could always use more documentation, whether as part of the
+official mcmc_statphys docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
 The best way to send feedback is to file an issue at https://github.com/uynajgi/mcmc_statphys/issues.
```

### Comparing `mcmc_statphys-0.1.0/LICENSE` & `mcmc_statphys-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.0/PKG-INFO` & `mcmc_statphys-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: mcmc_statphys
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library project of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).
 Home-page: https://github.com/uynajgi/mcmc_statphys
 Author: Uynaj GI
 Author-email: suquan12148@outlook.com
 License: MIT license
 Keywords: mcmc_statphys
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============
-mcmc-statphys
+mcmc_statphys
 =============
 
 
 .. image:: https://img.shields.io/pypi/v/mcmc_statphys.svg
         :target: https://pypi.python.org/pypi/mcmc_statphys
 
 .. image:: https://img.shields.io/travis/uynajgi/mcmc_statphys.svg
@@ -59,11 +58,11 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
-0.1.0 (2023-05-14)
+0.1.1 (2023-05-14)
 ------------------
 
 * First release on PyPI.
```

### Comparing `mcmc_statphys-0.1.0/README.rst` & `mcmc_statphys-0.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 =============
-mcmc-statphys
+mcmc_statphys
 =============
 
 
 .. image:: https://img.shields.io/pypi/v/mcmc_statphys.svg
         :target: https://pypi.python.org/pypi/mcmc_statphys
 
 .. image:: https://img.shields.io/travis/uynajgi/mcmc_statphys.svg
```

### Comparing `mcmc_statphys-0.1.0/docs/Makefile` & `mcmc_statphys-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.0/docs/conf.py` & `mcmc_statphys-0.1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 # source_suffix = ['.rst', '.md']
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = 'mcmc-statphys'
+project = 'mcmc_statphys'
 copyright = "2023, Uynaj GI"
 author = "Uynaj GI"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
@@ -124,38 +124,38 @@
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
     (master_doc, 'mcmc_statphys.tex',
-     'mcmc-statphys Documentation',
+     'mcmc_statphys Documentation',
      'Uynaj GI', 'manual'),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     (master_doc, 'mcmc_statphys',
-     'mcmc-statphys Documentation',
+     'mcmc_statphys Documentation',
      [author], 1)
 ]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (master_doc, 'mcmc_statphys',
-     'mcmc-statphys Documentation',
+     'mcmc_statphys Documentation',
      author,
      'mcmc_statphys',
      'One line description of project.',
      'Miscellaneous'),
 ]
```

### Comparing `mcmc_statphys-0.1.0/docs/installation.rst` & `mcmc_statphys-0.1.1/docs/installation.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 Installation
 ============
 
 
 Stable release
 --------------
 
-To install mcmc-statphys, run this command in your terminal:
+To install mcmc_statphys, run this command in your terminal:
 
 .. code-block:: console
 
     $ pip install mcmc_statphys
 
-This is the preferred method to install mcmc-statphys, as it will always install the most recent stable release.
+This is the preferred method to install mcmc_statphys, as it will always install the most recent stable release.
 
 If you don't have `pip`_ installed, this `Python installation guide`_ can guide
 you through the process.
 
 .. _pip: https://pip.pypa.io
 .. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
 
 
 From sources
 ------------
 
-The sources for mcmc-statphys can be downloaded from the `Github repo`_.
+The sources for mcmc_statphys can be downloaded from the `Github repo`_.
 
 You can either clone the public repository:
 
 .. code-block:: console
 
     $ git clone git://github.com/uynajgi/mcmc_statphys
```

### Comparing `mcmc_statphys-0.1.0/docs/make.bat` & `mcmc_statphys-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.0/mcmc_statphys/model.py` & `mcmc_statphys-0.1.1/mcmc_statphys/model.py`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.1.0/mcmc_statphys/sample.py` & `mcmc_statphys-0.1.1/mcmc_statphys/mcmc_statphys.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,8 @@
-# -*- encoding: utf-8 -*-
-'''
-@File    :   MCMC.py
-@Time    :   2023/05/13 21:07:49
-@Author  :   UynajGI
-@Version :   beta0.0.1
-@Contact :   betterWL@hotmail.com
-@License :   (CC-BY-4.0)Copyright 2023
-'''
+"""Main module."""
 
 import copy
 from collections import deque
 from typing import List, Tuple
 
 # here put the import lib
 import numpy as np
```

### Comparing `mcmc_statphys-0.1.0/mcmc_statphys.egg-info/PKG-INFO` & `mcmc_statphys-0.1.1/mcmc_statphys.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: mcmc-statphys
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library project of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).
 Home-page: https://github.com/uynajgi/mcmc_statphys
 Author: Uynaj GI
 Author-email: suquan12148@outlook.com
 License: MIT license
 Keywords: mcmc_statphys
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =============
-mcmc-statphys
+mcmc_statphys
 =============
 
 
 .. image:: https://img.shields.io/pypi/v/mcmc_statphys.svg
         :target: https://pypi.python.org/pypi/mcmc_statphys
 
 .. image:: https://img.shields.io/travis/uynajgi/mcmc_statphys.svg
@@ -59,11 +58,11 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
-0.1.0 (2023-05-14)
+0.1.1 (2023-05-14)
 ------------------
 
 * First release on PyPI.
```

### Comparing `mcmc_statphys-0.1.0/mcmc_statphys.egg-info/SOURCES.txt` & `mcmc_statphys-0.1.1/mcmc_statphys.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 mcmc_statphys/__init__.py
 mcmc_statphys/cli.py
 mcmc_statphys/mcmc_statphys.py
 mcmc_statphys/model.py
-mcmc_statphys/sample.py
 mcmc_statphys.egg-info/PKG-INFO
 mcmc_statphys.egg-info/SOURCES.txt
 mcmc_statphys.egg-info/dependency_links.txt
 mcmc_statphys.egg-info/entry_points.txt
 mcmc_statphys.egg-info/not-zip-safe
 mcmc_statphys.egg-info/requires.txt
 mcmc_statphys.egg-info/top_level.txt
```

### Comparing `mcmc_statphys-0.1.0/setup.py` & `mcmc_statphys-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 #!/usr/bin/env python
+
 """The setup script."""
 
-from setuptools import find_packages, setup
+from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = [
-    'Click>=7.0',
-]
+requirements = ['Click>=7.0', ]
 
-test_requirements = []
+test_requirements = [ ]
 
 setup(
     author="Uynaj GI",
     author_email='suquan12148@outlook.com',
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
     ],
     description="A library project of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).",
     entry_points={
         'console_scripts': [
             'mcmc_statphys=mcmc_statphys.cli:main',
         ],
     },
@@ -42,10 +40,10 @@
     include_package_data=True,
     keywords='mcmc_statphys',
     name='mcmc_statphys',
     packages=find_packages(include=['mcmc_statphys', 'mcmc_statphys.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/uynajgi/mcmc_statphys',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `mcmc_statphys-0.1.0/tests/test_mcmc_statphys.py` & `mcmc_statphys-0.1.1/tests/test_mcmc_statphys.py`

 * *Files identical despite different names*

