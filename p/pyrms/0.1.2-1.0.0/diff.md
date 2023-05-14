# Comparing `tmp/pyrms-0.1.2.tar.gz` & `tmp/pyrms-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrms-0.1.2.tar", last modified: Tue Jul 21 13:37:18 2020, max compression
+gzip compressed data, was "/Users/mattjohnson/RMGCODE/pyrms/dist/.tmp-kib8rf1j/pyrms-1.0.0.tar", last modified: Sun May 14 04:02:31 2023, max compression
```

## Comparing `pyrms-0.1.2.tar` & `pyrms-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 mattjohnson   (501) staff       (20)        0 2020-07-21 13:37:18.000000 pyrms-0.1.2/
--rw-r--r--   0 mattjohnson   (501) staff       (20)     2114 2020-07-21 13:37:18.000000 pyrms-0.1.2/PKG-INFO
--rw-r--r--   0 mattjohnson   (501) staff       (20)     1518 2019-10-05 20:15:41.000000 pyrms-0.1.2/README.md
-drwxr-xr-x   0 mattjohnson   (501) staff       (20)        0 2020-07-21 13:37:18.000000 pyrms-0.1.2/pyrms/
--rw-r--r--   0 mattjohnson   (501) staff       (20)      441 2020-07-21 13:35:34.000000 pyrms-0.1.2/pyrms/__init__.py
--rw-r--r--   0 mattjohnson   (501) staff       (20)     1327 2019-10-04 23:41:51.000000 pyrms-0.1.2/pyrms/rms.py
--rw-r--r--   0 mattjohnson   (501) staff       (20)      736 2019-04-15 12:19:38.000000 pyrms-0.1.2/pyrms/rmsTest.py
-drwxr-xr-x   0 mattjohnson   (501) staff       (20)        0 2020-07-21 13:37:18.000000 pyrms-0.1.2/pyrms.egg-info/
--rw-r--r--   0 mattjohnson   (501) staff       (20)     2114 2020-07-21 13:37:18.000000 pyrms-0.1.2/pyrms.egg-info/PKG-INFO
--rw-r--r--   0 mattjohnson   (501) staff       (20)      182 2020-07-21 13:37:18.000000 pyrms-0.1.2/pyrms.egg-info/SOURCES.txt
--rw-r--r--   0 mattjohnson   (501) staff       (20)        1 2020-07-21 13:37:18.000000 pyrms-0.1.2/pyrms.egg-info/dependency_links.txt
--rw-r--r--   0 mattjohnson   (501) staff       (20)        6 2020-07-21 13:37:18.000000 pyrms-0.1.2/pyrms.egg-info/top_level.txt
--rw-r--r--   0 mattjohnson   (501) staff       (20)       38 2020-07-21 13:37:18.000000 pyrms-0.1.2/setup.cfg
--rw-r--r--   0 mattjohnson   (501) staff       (20)      612 2020-07-21 13:36:59.000000 pyrms-0.1.2/setup.py
+drwxr-xr-x   0 mattjohnson   (501) staff       (20)        0 2023-05-14 04:02:31.013157 pyrms-1.0.0/
+-rw-r--r--   0 mattjohnson   (501) staff       (20)     1068 2020-07-20 23:27:57.000000 pyrms-1.0.0/LICENSE
+-rw-r--r--   0 mattjohnson   (501) staff       (20)     2025 2023-05-14 04:02:31.012785 pyrms-1.0.0/PKG-INFO
+-rw-r--r--   0 mattjohnson   (501) staff       (20)     1672 2023-05-14 03:56:44.000000 pyrms-1.0.0/README.md
+drwxr-xr-x   0 mattjohnson   (501) staff       (20)        0 2023-05-14 04:02:31.009224 pyrms-1.0.0/pyrms/
+-rw-r--r--   0 mattjohnson   (501) staff       (20)       11 2023-05-14 03:56:39.000000 pyrms-1.0.0/pyrms/__init__.py
+-rw-r--r--   0 mattjohnson   (501) staff       (20)     3255 2023-05-14 03:57:11.000000 pyrms-1.0.0/pyrms/rms.py
+-rw-r--r--   0 mattjohnson   (501) staff       (20)      736 2019-04-15 12:19:38.000000 pyrms-1.0.0/pyrms/rmsTest.py
+drwxr-xr-x   0 mattjohnson   (501) staff       (20)        0 2023-05-14 04:02:31.012272 pyrms-1.0.0/pyrms.egg-info/
+-rw-r--r--   0 mattjohnson   (501) staff       (20)     2025 2023-05-14 04:02:30.000000 pyrms-1.0.0/pyrms.egg-info/PKG-INFO
+-rw-r--r--   0 mattjohnson   (501) staff       (20)      190 2023-05-14 04:02:31.000000 pyrms-1.0.0/pyrms.egg-info/SOURCES.txt
+-rw-r--r--   0 mattjohnson   (501) staff       (20)        1 2023-05-14 04:02:30.000000 pyrms-1.0.0/pyrms.egg-info/dependency_links.txt
+-rw-r--r--   0 mattjohnson   (501) staff       (20)        6 2023-05-14 04:02:30.000000 pyrms-1.0.0/pyrms.egg-info/top_level.txt
+-rw-r--r--   0 mattjohnson   (501) staff       (20)       38 2023-05-14 04:02:31.013254 pyrms-1.0.0/setup.cfg
+-rw-r--r--   0 mattjohnson   (501) staff       (20)      613 2023-05-14 04:02:15.000000 pyrms-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyrms-0.1.2/PKG-INFO` & `pyrms-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: pyrms
-Version: 0.1.2
-Summary: UNKNOWN
+Version: 1.0.0
 Home-page: https://github.com/ReactionMechanismGenerator/pyrms
 Author: mjohnson541
 Author-email: mjohnson541@gmail.com
-License: UNKNOWN
-Description: # <img align="top" src="https://github.com/ReactionMechanismGenerator/pyrms/blob/master/logos/rms-logo-small.png"> Py-RMS - Python Reaction Mechanism Simulator
-        
-        [![Build status](https://img.shields.io/travis/ReactionMechanismGenerator/pyrms/master.svg)](https://travis-ci.org/ReactionMechanismGenerator/pyrms)
-        [![codecov](https://codecov.io/gh/ReactionMechanismGenerator/pyrms/branch/master/graph/badge.svg)](https://codecov.io/gh/ReactionMechanismGenerator/pyrms)
-        
-        Python wrapper for the Reaction Mechanism Simulator (RMS) package for simulating and analyzing large chemical reaction mechanisms.  Currently only supports python 2.  
-        
-        In theory this wraps all functionality within RMS with two caveats:  
-        
-        1) In jupyter notebooks julia objects don't display the same way in the python kernel as they would in the julia kernel.  For example flux diagram generation had to be hard coded into this wrapper to display properly.  If this happens please make an issue.  
-        
-        2) There are ways to define julia functions that makes them impossible to call from python using the pyjulia.  In most cases this is easy to fix.  If you find a case where this happens please make an issue.  
-        
-        ## Installation Instructions:  
-        
-        Note:  
-          1) pyrms currently only supports python 2 so running `python` must open a python 2 kernel.  
-          2) Installing pyrms links/relinks your julia PyCall module to the python 2 being used.  
-        
-        To Install Run:  
-        ```
-        git clone https://github.com/ReactionMechanismGenerator/pyrms.git
-        cd pyrms
-        make install
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# <img align="top" src="https://github.com/ReactionMechanismGenerator/pyrms/blob/master/logos/rms-logo-small.png"> Py-RMS - Python Reaction Mechanism Simulator
+
+[![Build status](https://img.shields.io/travis/ReactionMechanismGenerator/pyrms/master.svg)](https://travis-ci.org/ReactionMechanismGenerator/pyrms)
+[![codecov](https://codecov.io/gh/ReactionMechanismGenerator/pyrms/branch/master/graph/badge.svg)](https://codecov.io/gh/ReactionMechanismGenerator/pyrms)
+
+Python wrapper for the Reaction Mechanism Simulator (RMS) package for simulating and analyzing large chemical reaction mechanisms. 
+
+In theory this wraps all functionality within RMS with two caveats:  
+
+1) In jupyter notebooks julia objects don't display the same way in the python kernel as they would in the julia kernel.  For example flux diagram generation had to be hard coded into this wrapper to display properly.  If this happens please make an issue.  
+
+2) There are ways to define julia functions that makes them impossible to call from python using the pyjulia.  In most cases this is easy to fix.  If you find a case where this happens please make an issue.  
+
+## Installation Instructions from Anaconda:  
+
+Note: We recommend installing pyrms in its own conda environment when convenient because getting pyjulia to work with conda python efficiently currently requires relinking 
+      the python executable to the python-jl executable, this usually isn't problematic, but it can be an issue in more complicated conda environments. 
+
+To Install Binaries with Conda Run:  
+```
+conda install -c rmg pyrms
+python -c "import pyrms; pyrms.install()"
+ln -sfn $(which python-jl) $(which python)
+```
```

### Comparing `pyrms-0.1.2/README.md` & `pyrms-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # <img align="top" src="https://github.com/ReactionMechanismGenerator/pyrms/blob/master/logos/rms-logo-small.png"> Py-RMS - Python Reaction Mechanism Simulator
 
 [![Build status](https://img.shields.io/travis/ReactionMechanismGenerator/pyrms/master.svg)](https://travis-ci.org/ReactionMechanismGenerator/pyrms)
 [![codecov](https://codecov.io/gh/ReactionMechanismGenerator/pyrms/branch/master/graph/badge.svg)](https://codecov.io/gh/ReactionMechanismGenerator/pyrms)
 
-Python wrapper for the Reaction Mechanism Simulator (RMS) package for simulating and analyzing large chemical reaction mechanisms.  Currently only supports python 2.  
+Python wrapper for the Reaction Mechanism Simulator (RMS) package for simulating and analyzing large chemical reaction mechanisms. 
 
 In theory this wraps all functionality within RMS with two caveats:  
 
 1) In jupyter notebooks julia objects don't display the same way in the python kernel as they would in the julia kernel.  For example flux diagram generation had to be hard coded into this wrapper to display properly.  If this happens please make an issue.  
 
 2) There are ways to define julia functions that makes them impossible to call from python using the pyjulia.  In most cases this is easy to fix.  If you find a case where this happens please make an issue.  
 
-## Installation Instructions:  
+## Installation Instructions from Anaconda:  
 
-Note:  
-  1) pyrms currently only supports python 2 so running `python` must open a python 2 kernel.  
-  2) Installing pyrms links/relinks your julia PyCall module to the python 2 being used.  
+Note: We recommend installing pyrms in its own conda environment when convenient because getting pyjulia to work with conda python efficiently currently requires relinking 
+      the python executable to the python-jl executable, this usually isn't problematic, but it can be an issue in more complicated conda environments. 
 
-To Install Run:  
+To Install Binaries with Conda Run:  
 ```
-git clone https://github.com/ReactionMechanismGenerator/pyrms.git
-cd pyrms
-make install
+conda install -c rmg pyrms
+python -c "import pyrms; pyrms.install()"
+ln -sfn $(which python-jl) $(which python)
 ```
```

### Comparing `pyrms-0.1.2/pyrms/rmsTest.py` & `pyrms-1.0.0/pyrms/rmsTest.py`

 * *Files identical despite different names*

### Comparing `pyrms-0.1.2/pyrms.egg-info/PKG-INFO` & `pyrms-1.0.0/pyrms.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: pyrms
-Version: 0.1.2
-Summary: UNKNOWN
+Version: 1.0.0
 Home-page: https://github.com/ReactionMechanismGenerator/pyrms
 Author: mjohnson541
 Author-email: mjohnson541@gmail.com
-License: UNKNOWN
-Description: # <img align="top" src="https://github.com/ReactionMechanismGenerator/pyrms/blob/master/logos/rms-logo-small.png"> Py-RMS - Python Reaction Mechanism Simulator
-        
-        [![Build status](https://img.shields.io/travis/ReactionMechanismGenerator/pyrms/master.svg)](https://travis-ci.org/ReactionMechanismGenerator/pyrms)
-        [![codecov](https://codecov.io/gh/ReactionMechanismGenerator/pyrms/branch/master/graph/badge.svg)](https://codecov.io/gh/ReactionMechanismGenerator/pyrms)
-        
-        Python wrapper for the Reaction Mechanism Simulator (RMS) package for simulating and analyzing large chemical reaction mechanisms.  Currently only supports python 2.  
-        
-        In theory this wraps all functionality within RMS with two caveats:  
-        
-        1) In jupyter notebooks julia objects don't display the same way in the python kernel as they would in the julia kernel.  For example flux diagram generation had to be hard coded into this wrapper to display properly.  If this happens please make an issue.  
-        
-        2) There are ways to define julia functions that makes them impossible to call from python using the pyjulia.  In most cases this is easy to fix.  If you find a case where this happens please make an issue.  
-        
-        ## Installation Instructions:  
-        
-        Note:  
-          1) pyrms currently only supports python 2 so running `python` must open a python 2 kernel.  
-          2) Installing pyrms links/relinks your julia PyCall module to the python 2 being used.  
-        
-        To Install Run:  
-        ```
-        git clone https://github.com/ReactionMechanismGenerator/pyrms.git
-        cd pyrms
-        make install
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# <img align="top" src="https://github.com/ReactionMechanismGenerator/pyrms/blob/master/logos/rms-logo-small.png"> Py-RMS - Python Reaction Mechanism Simulator
+
+[![Build status](https://img.shields.io/travis/ReactionMechanismGenerator/pyrms/master.svg)](https://travis-ci.org/ReactionMechanismGenerator/pyrms)
+[![codecov](https://codecov.io/gh/ReactionMechanismGenerator/pyrms/branch/master/graph/badge.svg)](https://codecov.io/gh/ReactionMechanismGenerator/pyrms)
+
+Python wrapper for the Reaction Mechanism Simulator (RMS) package for simulating and analyzing large chemical reaction mechanisms. 
+
+In theory this wraps all functionality within RMS with two caveats:  
+
+1) In jupyter notebooks julia objects don't display the same way in the python kernel as they would in the julia kernel.  For example flux diagram generation had to be hard coded into this wrapper to display properly.  If this happens please make an issue.  
+
+2) There are ways to define julia functions that makes them impossible to call from python using the pyjulia.  In most cases this is easy to fix.  If you find a case where this happens please make an issue.  
+
+## Installation Instructions from Anaconda:  
+
+Note: We recommend installing pyrms in its own conda environment when convenient because getting pyjulia to work with conda python efficiently currently requires relinking 
+      the python executable to the python-jl executable, this usually isn't problematic, but it can be an issue in more complicated conda environments. 
+
+To Install Binaries with Conda Run:  
+```
+conda install -c rmg pyrms
+python -c "import pyrms; pyrms.install()"
+ln -sfn $(which python-jl) $(which python)
+```
```

### Comparing `pyrms-0.1.2/setup.py` & `pyrms-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyrms", # Replace with your own username
-    version="0.1.2",
+    version="1.0.0",
     author="mjohnson541",
     author_email="mjohnson541@gmail.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ReactionMechanismGenerator/pyrms",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     python_requires='>=3.7',
-)
+)
```

