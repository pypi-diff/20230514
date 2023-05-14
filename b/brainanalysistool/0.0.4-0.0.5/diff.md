# Comparing `tmp/brainanalysistool-0.0.4.tar.gz` & `tmp/brainanalysistool-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainanalysistool-0.0.4.tar", last modified: Sat Apr 22 06:32:21 2023, max compression
+gzip compressed data, was "brainanalysistool-0.0.5.tar", last modified: Sun May 14 13:17:17 2023, max compression
```

## Comparing `brainanalysistool-0.0.4.tar` & `brainanalysistool-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 06:32:21.150149 brainanalysistool-0.0.4/
--rw-rw-rw-   0        0        0     1088 2023-03-02 01:48:52.000000 brainanalysistool-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      677 2023-04-22 06:32:21.149844 brainanalysistool-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-03-14 00:14:53.000000 brainanalysistool-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 06:32:21.138848 brainanalysistool-0.0.4/brainanalysistool/
--rw-rw-rw-   0        0        0    10070 2023-04-02 09:12:15.000000 brainanalysistool-0.0.4/brainanalysistool/WaveAnalysisFun.py
--rw-rw-rw-   0        0        0     5899 2023-03-23 02:13:39.000000 brainanalysistool-0.0.4/brainanalysistool/WaveletFun.py
--rw-rw-rw-   0        0        0      492 2023-04-22 06:19:02.000000 brainanalysistool-0.0.4/brainanalysistool/__init__.py
--rw-rw-rw-   0        0        0    22078 2023-04-22 00:56:01.000000 brainanalysistool-0.0.4/brainanalysistool/plotting.py
--rw-rw-rw-   0        0        0     3548 2023-04-02 07:49:48.000000 brainanalysistool-0.0.4/brainanalysistool/preprocessing.py
-drwxrwxrwx   0        0        0        0 2023-04-22 06:32:21.147848 brainanalysistool-0.0.4/brainanalysistool.egg-info/
--rw-rw-rw-   0        0        0      677 2023-04-22 06:32:20.000000 brainanalysistool-0.0.4/brainanalysistool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-04-22 06:32:21.000000 brainanalysistool-0.0.4/brainanalysistool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 06:32:20.000000 brainanalysistool-0.0.4/brainanalysistool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-04-22 06:32:20.000000 brainanalysistool-0.0.4/brainanalysistool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-22 06:32:20.000000 brainanalysistool-0.0.4/brainanalysistool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 06:32:21.150149 brainanalysistool-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      968 2023-04-22 06:32:14.000000 brainanalysistool-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 13:17:17.166391 brainanalysistool-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2023-03-02 01:48:52.000000 brainanalysistool-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      677 2023-05-14 13:17:17.165801 brainanalysistool-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-03-14 00:14:53.000000 brainanalysistool-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 13:17:17.154801 brainanalysistool-0.0.5/brainanalysistool/
+-rw-rw-rw-   0        0        0    10070 2023-04-02 09:12:15.000000 brainanalysistool-0.0.5/brainanalysistool/WaveAnalysisFun.py
+-rw-rw-rw-   0        0        0     5899 2023-03-23 02:13:39.000000 brainanalysistool-0.0.5/brainanalysistool/WaveletFun.py
+-rw-rw-rw-   0        0        0      492 2023-05-14 13:16:21.000000 brainanalysistool-0.0.5/brainanalysistool/__init__.py
+-rw-rw-rw-   0        0        0    22078 2023-04-22 00:56:01.000000 brainanalysistool-0.0.5/brainanalysistool/plotting.py
+-rw-rw-rw-   0        0        0     3548 2023-04-02 07:49:48.000000 brainanalysistool-0.0.5/brainanalysistool/preprocessing.py
+drwxrwxrwx   0        0        0        0 2023-05-14 13:17:17.163927 brainanalysistool-0.0.5/brainanalysistool.egg-info/
+-rw-rw-rw-   0        0        0      677 2023-05-14 13:17:16.000000 brainanalysistool-0.0.5/brainanalysistool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-05-14 13:17:17.000000 brainanalysistool-0.0.5/brainanalysistool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 13:17:16.000000 brainanalysistool-0.0.5/brainanalysistool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-05-14 13:17:16.000000 brainanalysistool-0.0.5/brainanalysistool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-14 13:17:16.000000 brainanalysistool-0.0.5/brainanalysistool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 13:17:17.166802 brainanalysistool-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      969 2023-05-14 13:15:52.000000 brainanalysistool-0.0.5/setup.py
```

### Comparing `brainanalysistool-0.0.4/LICENSE` & `brainanalysistool-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `brainanalysistool-0.0.4/PKG-INFO` & `brainanalysistool-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainanalysistool
-Version: 0.0.4
+Version: 0.0.5
 Summary: Brain/Neuron/Ecog analysis tool
 Home-page: https://github.com/RunminGan1218/Brain-analysis-tool
 Author: Runmin Gan
 Author-email: 354613146@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `brainanalysistool-0.0.4/brainanalysistool/WaveAnalysisFun.py` & `brainanalysistool-0.0.5/brainanalysistool/WaveAnalysisFun.py`

 * *Files identical despite different names*

### Comparing `brainanalysistool-0.0.4/brainanalysistool/WaveletFun.py` & `brainanalysistool-0.0.5/brainanalysistool/WaveletFun.py`

 * *Files identical despite different names*

### Comparing `brainanalysistool-0.0.4/brainanalysistool/plotting.py` & `brainanalysistool-0.0.5/brainanalysistool/plotting.py`

 * *Files identical despite different names*

### Comparing `brainanalysistool-0.0.4/brainanalysistool/preprocessing.py` & `brainanalysistool-0.0.5/brainanalysistool/preprocessing.py`

 * *Files identical despite different names*

### Comparing `brainanalysistool-0.0.4/brainanalysistool.egg-info/PKG-INFO` & `brainanalysistool-0.0.5/brainanalysistool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainanalysistool
-Version: 0.0.4
+Version: 0.0.5
 Summary: Brain/Neuron/Ecog analysis tool
 Home-page: https://github.com/RunminGan1218/Brain-analysis-tool
 Author: Runmin Gan
 Author-email: 354613146@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `brainanalysistool-0.0.4/setup.py` & `brainanalysistool-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python
 from __future__ import print_function
 from setuptools import setup, find_packages
 import sys
  
 setup(
     name="brainanalysistool",
-    version="0.0.4",
+    version="0.0.5",
     author="Runmin Gan",
     author_email="354613146@qq.com",
     description="Brain/Neuron/Ecog analysis tool",
     long_description=open("README.md").read(),
     long_description_content_type='text/plain',
     license="MIT",
     url="https://github.com/RunminGan1218/Brain-analysis-tool",
     packages=['brainanalysistool'],
     install_requires=[
         "matplotlib>=3.6.2",
         "numpy>=1.23.5",
         "PyWavelets>=1.4.1",
         "scipy>=1.9.3",
         "pactools>= 0.3.1",
-        "pycwt>=0.3.0a22"
+        "pycwt>=0.3.0a22",
         "PyWavelets>=1.4.1"
         ],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

