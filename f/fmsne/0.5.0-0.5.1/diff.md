# Comparing `tmp/fmsne-0.5.0.tar.gz` & `tmp/fmsne-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmsne-0.5.0.tar", last modified: Sun May 14 09:55:11 2023, max compression
+gzip compressed data, was "fmsne-0.5.1.tar", last modified: Sun May 14 10:14:35 2023, max compression
```

## Comparing `fmsne-0.5.0.tar` & `fmsne-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-14 09:55:11.218449 fmsne-0.5.0/
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     1195 2023-05-13 08:50:57.000000 fmsne-0.5.0/LICENCE.md
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       67 2023-05-11 14:46:43.000000 fmsne-0.5.0/MANIFEST.in
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8690 2023-05-14 09:55:11.218449 fmsne-0.5.0/PKG-INFO
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8173 2023-05-13 09:10:50.000000 fmsne-0.5.0/README.md
-drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-14 09:55:11.218449 fmsne-0.5.0/fmsne/
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       44 2023-05-13 08:41:46.000000 fmsne-0.5.0/fmsne/__init__.py
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     3380 2023-05-11 14:46:43.000000 fmsne-0.5.0/fmsne/arithmetic_ansi.h
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8830 2023-05-11 14:46:43.000000 fmsne-0.5.0/fmsne/arithmetic_sse_double.h
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     9070 2023-05-11 14:46:43.000000 fmsne-0.5.0/fmsne/arithmetic_sse_float.h
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    40154 2023-05-11 14:46:48.000000 fmsne-0.5.0/fmsne/fmsne.py
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)  2010540 2023-05-14 09:45:02.000000 fmsne-0.5.0/fmsne/fmsne_implem.cpp
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)   171438 2023-05-11 14:46:43.000000 fmsne-0.5.0/fmsne/fmsne_implem.pyx
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    41095 2023-05-11 14:46:43.000000 fmsne-0.5.0/fmsne/lbfgs.c
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    32648 2023-05-11 14:46:43.000000 fmsne-0.5.0/fmsne/lbfgs.h
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    19367 2023-05-12 04:57:27.000000 fmsne-0.5.0/fmsne/vptree.h
-drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-14 09:55:11.218449 fmsne-0.5.0/fmsne.egg-info/
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8690 2023-05-14 09:55:11.000000 fmsne-0.5.0/fmsne.egg-info/PKG-INFO
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      400 2023-05-14 09:55:11.000000 fmsne-0.5.0/fmsne.egg-info/SOURCES.txt
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)        1 2023-05-14 09:55:11.000000 fmsne-0.5.0/fmsne.egg-info/dependency_links.txt
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       44 2023-05-14 09:55:11.000000 fmsne-0.5.0/fmsne.egg-info/requires.txt
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       19 2023-05-14 09:55:11.000000 fmsne-0.5.0/fmsne.egg-info/top_level.txt
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      506 2023-05-14 09:55:11.218449 fmsne-0.5.0/setup.cfg
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      997 2023-05-14 09:45:20.000000 fmsne-0.5.0/setup.py
+drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-14 10:14:35.257286 fmsne-0.5.1/
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     1195 2023-05-13 08:50:57.000000 fmsne-0.5.1/LICENCE.md
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       67 2023-05-11 14:46:43.000000 fmsne-0.5.1/MANIFEST.in
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8761 2023-05-14 10:14:35.257286 fmsne-0.5.1/PKG-INFO
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8173 2023-05-13 09:10:50.000000 fmsne-0.5.1/README.md
+drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-14 10:14:35.253286 fmsne-0.5.1/fmsne/
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       44 2023-05-14 10:13:40.000000 fmsne-0.5.1/fmsne/__init__.py
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     3380 2023-05-11 14:46:43.000000 fmsne-0.5.1/fmsne/arithmetic_ansi.h
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8830 2023-05-11 14:46:43.000000 fmsne-0.5.1/fmsne/arithmetic_sse_double.h
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     9070 2023-05-11 14:46:43.000000 fmsne-0.5.1/fmsne/arithmetic_sse_float.h
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    40154 2023-05-11 14:46:48.000000 fmsne-0.5.1/fmsne/fmsne.py
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)  2010540 2023-05-14 09:45:02.000000 fmsne-0.5.1/fmsne/fmsne_implem.cpp
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)   171438 2023-05-11 14:46:43.000000 fmsne-0.5.1/fmsne/fmsne_implem.pyx
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    41095 2023-05-11 14:46:43.000000 fmsne-0.5.1/fmsne/lbfgs.c
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    32648 2023-05-11 14:46:43.000000 fmsne-0.5.1/fmsne/lbfgs.h
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    19367 2023-05-12 04:57:27.000000 fmsne-0.5.1/fmsne/vptree.h
+drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-14 10:14:35.257286 fmsne-0.5.1/fmsne.egg-info/
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8761 2023-05-14 10:14:35.000000 fmsne-0.5.1/fmsne.egg-info/PKG-INFO
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      400 2023-05-14 10:14:35.000000 fmsne-0.5.1/fmsne.egg-info/SOURCES.txt
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)        1 2023-05-14 10:14:35.000000 fmsne-0.5.1/fmsne.egg-info/dependency_links.txt
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       44 2023-05-14 10:14:35.000000 fmsne-0.5.1/fmsne.egg-info/requires.txt
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       19 2023-05-14 10:14:35.000000 fmsne-0.5.1/fmsne.egg-info/top_level.txt
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      579 2023-05-14 10:14:35.257286 fmsne-0.5.1/setup.cfg
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      997 2023-05-14 09:45:20.000000 fmsne-0.5.1/setup.py
```

### Comparing `fmsne-0.5.0/LICENCE.md` & `fmsne-0.5.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `fmsne-0.5.0/PKG-INFO` & `fmsne-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: fmsne
-Version: 0.5.0
+Version: 0.5.1
 Summary: Fast Multi-Scale Neighbour Embedding
 Home-page: https://github.com/cdebodt/Fast_Multi-scale_NE
 Author: Cyril de Bodt
 Author-email: cyril.debodt@uclouvain.be
+Maintainer: Laurent Gatto
+Maintainer-email: laurent.gatto@uclouvain.be
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
```

### Comparing `fmsne-0.5.0/README.md` & `fmsne-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fmsne-0.5.0/fmsne/arithmetic_ansi.h` & `fmsne-0.5.1/fmsne/arithmetic_ansi.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.5.0/fmsne/arithmetic_sse_double.h` & `fmsne-0.5.1/fmsne/arithmetic_sse_double.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.5.0/fmsne/arithmetic_sse_float.h` & `fmsne-0.5.1/fmsne/arithmetic_sse_float.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.5.0/fmsne/fmsne.py` & `fmsne-0.5.1/fmsne/fmsne.py`

 * *Files identical despite different names*

### Comparing `fmsne-0.5.0/fmsne/fmsne_implem.cpp` & `fmsne-0.5.1/fmsne/fmsne_implem.cpp`

 * *Files identical despite different names*

### Comparing `fmsne-0.5.0/fmsne/fmsne_implem.pyx` & `fmsne-0.5.1/fmsne/fmsne_implem.pyx`

 * *Files identical despite different names*

### Comparing `fmsne-0.5.0/fmsne/lbfgs.c` & `fmsne-0.5.1/fmsne/lbfgs.c`

 * *Files identical despite different names*

### Comparing `fmsne-0.5.0/fmsne/lbfgs.h` & `fmsne-0.5.1/fmsne/lbfgs.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.5.0/fmsne/vptree.h` & `fmsne-0.5.1/fmsne/vptree.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.5.0/fmsne.egg-info/PKG-INFO` & `fmsne-0.5.1/fmsne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: fmsne
-Version: 0.5.0
+Version: 0.5.1
 Summary: Fast Multi-Scale Neighbour Embedding
 Home-page: https://github.com/cdebodt/Fast_Multi-scale_NE
 Author: Cyril de Bodt
 Author-email: cyril.debodt@uclouvain.be
+Maintainer: Laurent Gatto
+Maintainer-email: laurent.gatto@uclouvain.be
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
```

### Comparing `fmsne-0.5.0/setup.py` & `fmsne-0.5.1/setup.py`

 * *Files identical despite different names*

