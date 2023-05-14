# Comparing `tmp/axia-0.1.0.tar.gz` & `tmp/axia-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axia-0.1.0.tar", last modified: Sat May 13 23:15:26 2023, max compression
+gzip compressed data, was "axia-0.1.1.tar", last modified: Sun May 14 18:24:38 2023, max compression
```

## Comparing `axia-0.1.0.tar` & `axia-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-13 23:15:26.021928 axia-0.1.0/
--rw-r--r--   0 fernandonogueira   (501) staff       (20)     1074 2023-05-13 22:56:47.000000 axia-0.1.0/LICENSE
--rw-r--r--   0 fernandonogueira   (501) staff       (20)     2182 2023-05-13 23:15:26.021775 axia-0.1.0/PKG-INFO
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     1650 2023-05-13 20:35:16.000000 axia-0.1.0/README.md
-drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-13 23:15:26.020184 axia-0.1.0/axia/
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)       38 2023-05-12 20:48:52.000000 axia-0.1.0/axia/__init__.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     4340 2023-05-12 20:48:52.000000 axia-0.1.0/axia/dataset.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     2929 2023-05-12 20:48:52.000000 axia-0.1.0/axia/loader.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     3909 2023-05-12 20:48:52.000000 axia-0.1.0/axia/report.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)    16652 2023-05-12 20:48:52.000000 axia-0.1.0/axia/sbg_survival.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)    33343 2023-05-12 20:48:52.000000 axia-0.1.0/axia/shifted_beta_geometric.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)    34796 2023-05-12 20:48:52.000000 axia-0.1.0/axia/util.py
-drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-13 23:15:26.020923 axia-0.1.0/axia.egg-info/
--rw-r--r--   0 fernandonogueira   (501) staff       (20)     2182 2023-05-13 23:15:26.000000 axia-0.1.0/axia.egg-info/PKG-INFO
--rw-r--r--   0 fernandonogueira   (501) staff       (20)      339 2023-05-13 23:15:26.000000 axia-0.1.0/axia.egg-info/SOURCES.txt
--rw-r--r--   0 fernandonogueira   (501) staff       (20)        1 2023-05-13 23:15:26.000000 axia-0.1.0/axia.egg-info/dependency_links.txt
--rw-r--r--   0 fernandonogueira   (501) staff       (20)        5 2023-05-13 23:15:26.000000 axia-0.1.0/axia.egg-info/top_level.txt
--rw-r--r--   0 fernandonogueira   (501) staff       (20)      606 2023-05-13 23:00:59.000000 axia-0.1.0/pyproject.toml
--rw-r--r--   0 fernandonogueira   (501) staff       (20)       38 2023-05-13 23:15:26.021981 axia-0.1.0/setup.cfg
-drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-13 23:15:26.021540 axia-0.1.0/tests/
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     2579 2023-05-13 16:10:24.000000 axia-0.1.0/tests/test_fader_hardie.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     8132 2023-05-12 20:48:52.000000 axia-0.1.0/tests/test_report.py
--rw-rw-r--   0 fernandonogueira   (501) staff       (20)     6627 2023-05-12 20:48:52.000000 axia-0.1.0/tests/test_util.py
+drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-14 18:24:38.942932 axia-0.1.1/
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     1074 2023-05-13 22:56:47.000000 axia-0.1.1/LICENSE
+-rw-r--r--   0 fernandonogueira   (501) staff       (20)     1881 2023-05-14 18:24:38.942792 axia-0.1.1/PKG-INFO
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     1349 2023-05-13 23:25:25.000000 axia-0.1.1/README.md
+drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-14 18:24:38.941361 axia-0.1.1/axia/
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)       38 2023-05-12 20:48:52.000000 axia-0.1.1/axia/__init__.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     4340 2023-05-12 20:48:52.000000 axia-0.1.1/axia/dataset.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     2929 2023-05-12 20:48:52.000000 axia-0.1.1/axia/loader.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     3909 2023-05-12 20:48:52.000000 axia-0.1.1/axia/report.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)    16652 2023-05-12 20:48:52.000000 axia-0.1.1/axia/sbg_survival.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)    33343 2023-05-12 20:48:52.000000 axia-0.1.1/axia/shifted_beta_geometric.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)    34796 2023-05-12 20:48:52.000000 axia-0.1.1/axia/util.py
+drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-14 18:24:38.942029 axia-0.1.1/axia.egg-info/
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     1881 2023-05-14 18:24:38.000000 axia-0.1.1/axia.egg-info/PKG-INFO
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)      339 2023-05-14 18:24:38.000000 axia-0.1.1/axia.egg-info/SOURCES.txt
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)        1 2023-05-14 18:24:38.000000 axia-0.1.1/axia.egg-info/dependency_links.txt
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)        5 2023-05-14 18:24:38.000000 axia-0.1.1/axia.egg-info/top_level.txt
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)      606 2023-05-14 18:24:27.000000 axia-0.1.1/pyproject.toml
+-rw-r--r--   0 fernandonogueira   (501) staff       (20)       38 2023-05-14 18:24:38.942975 axia-0.1.1/setup.cfg
+drwxr-xr-x   0 fernandonogueira   (501) staff       (20)        0 2023-05-14 18:24:38.942596 axia-0.1.1/tests/
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     2579 2023-05-13 16:10:24.000000 axia-0.1.1/tests/test_fader_hardie.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     8132 2023-05-12 20:48:52.000000 axia-0.1.1/tests/test_report.py
+-rw-rw-r--   0 fernandonogueira   (501) staff       (20)     6627 2023-05-12 20:48:52.000000 axia-0.1.1/tests/test_util.py
```

### Comparing `axia-0.1.0/LICENSE` & `axia-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `axia-0.1.0/PKG-INFO` & `axia-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,49 @@
 Metadata-Version: 2.1
 Name: axia
-Version: 0.1.0
+Version: 0.1.1
 Summary: An alternative to survival analysis using the shifted beta-geometric model.
 Author-email: Fernando Nogueira <author@example.com>
 Project-URL: Homepage, https://github.com/fmfn/axia
 Project-URL: Bug Tracker, https://github.com/fmfn/axia/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
-  <img src="https://github.com/fmfn/axia/blob/master/.github/axia-logo-2.jpg"><br><br>
-  <!-- <img src="https://github.com/fmfn/axia/blob/master/github/axia-logo.png"><br><br> -->
+  <!-- <img src="https://github.com/fmfn/axia/blob/master/.github/axia-logo-2.jpg"><br><br> -->
+  <img src="https://github.com/fmfn/axia/blob/master/.github/axia-logo.png"><br><br>
 </div>
 
 -----------------
 
 The axia package provides an implementation of an extension  of
 the Shifted-Beta-Geometric model by P. Fader & B. Hardie [1] to individuals in
 contractual settings with multiple predictor variables.
 
-It will soon provide a lot more...
-
 Axia offers a survival analysis like approach to modeling the
 behaviour of individuals in contractual settings. Given a set of features, ages
 and status (alive or dead), this package builds on top of the model developed
 by P. Fader & B. Hardie [1], to infer hazard curves, retention curves and
 discounted-life-time-value.
 
 Head over to the examples folder to learn how to use axia.
 
 Installation
 ======
-Axia is not currently available on PyPi. To install the package,
-you will need to clone it and run the setup.py file. Use the following commands to
-get a copy from Github and install all dependencies:
-
-    git clone https://github.com/fmfn/axia.git
-    cd axia
-    python setup.py install
+```bash
+pip3 install axia
+```
+
 ### Dependencies
-* numpy
-* pandas
-* scipy
-* jupyter (for examples only)
+* numpy~=1.21.3
+* scipy~=1.7.1
+* pandas~=1.3.4
 
 References
 ===
 1. ["HOW TO PROJECT CUSTOMER RETENTION", P. Fader & B. Hardie](https://faculty.wharton.upenn.edu/wp-content/uploads/2012/04/Fader_hardie_jim_07.pdf)
 2. ["Customer-Base Valudation in a Contractual Setting: The Perils of Ignoring
 Heterogeneity", P. Fader & B. Hardie](https://pdfs.semanticscholar.org/d620/c9a463b9d09d433e01ecec4db083bb4a2ac9.pdf?_ga=2.242218690.1394399945.1550257837-1536596951.1529000020)
```

### Comparing `axia-0.1.0/README.md` & `axia-0.1.1/axia.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,49 @@
+Metadata-Version: 2.1
+Name: axia
+Version: 0.1.1
+Summary: An alternative to survival analysis using the shifted beta-geometric model.
+Author-email: Fernando Nogueira <author@example.com>
+Project-URL: Homepage, https://github.com/fmfn/axia
+Project-URL: Bug Tracker, https://github.com/fmfn/axia/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
-  <img src="https://github.com/fmfn/axia/blob/master/.github/axia-logo-2.jpg"><br><br>
-  <!-- <img src="https://github.com/fmfn/axia/blob/master/github/axia-logo.png"><br><br> -->
+  <!-- <img src="https://github.com/fmfn/axia/blob/master/.github/axia-logo-2.jpg"><br><br> -->
+  <img src="https://github.com/fmfn/axia/blob/master/.github/axia-logo.png"><br><br>
 </div>
 
 -----------------
 
 The axia package provides an implementation of an extension  of
 the Shifted-Beta-Geometric model by P. Fader & B. Hardie [1] to individuals in
 contractual settings with multiple predictor variables.
 
-It will soon provide a lot more...
-
 Axia offers a survival analysis like approach to modeling the
 behaviour of individuals in contractual settings. Given a set of features, ages
 and status (alive or dead), this package builds on top of the model developed
 by P. Fader & B. Hardie [1], to infer hazard curves, retention curves and
 discounted-life-time-value.
 
 Head over to the examples folder to learn how to use axia.
 
 Installation
 ======
-Axia is not currently available on PyPi. To install the package,
-you will need to clone it and run the setup.py file. Use the following commands to
-get a copy from Github and install all dependencies:
-
-    git clone https://github.com/fmfn/axia.git
-    cd axia
-    python setup.py install
+```bash
+pip3 install axia
+```
+
 ### Dependencies
-* numpy
-* pandas
-* scipy
-* jupyter (for examples only)
+* numpy~=1.21.3
+* scipy~=1.7.1
+* pandas~=1.3.4
 
 References
 ===
 1. ["HOW TO PROJECT CUSTOMER RETENTION", P. Fader & B. Hardie](https://faculty.wharton.upenn.edu/wp-content/uploads/2012/04/Fader_hardie_jim_07.pdf)
 2. ["Customer-Base Valudation in a Contractual Setting: The Perils of Ignoring
 Heterogeneity", P. Fader & B. Hardie](https://pdfs.semanticscholar.org/d620/c9a463b9d09d433e01ecec4db083bb4a2ac9.pdf?_ga=2.242218690.1394399945.1550257837-1536596951.1529000020)
```

### Comparing `axia-0.1.0/axia/dataset.py` & `axia-0.1.1/axia/dataset.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.0/axia/loader.py` & `axia-0.1.1/axia/loader.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.0/axia/report.py` & `axia-0.1.1/axia/report.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.0/axia/sbg_survival.py` & `axia-0.1.1/axia/sbg_survival.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.0/axia/shifted_beta_geometric.py` & `axia-0.1.1/axia/shifted_beta_geometric.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.0/axia/util.py` & `axia-0.1.1/axia/util.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.0/pyproject.toml` & `axia-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "axia"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Fernando Nogueira", email="author@example.com" },
 ]
 description = "An alternative to survival analysis using the shifted beta-geometric model."
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `axia-0.1.0/tests/test_fader_hardie.py` & `axia-0.1.1/tests/test_fader_hardie.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.0/tests/test_report.py` & `axia-0.1.1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `axia-0.1.0/tests/test_util.py` & `axia-0.1.1/tests/test_util.py`

 * *Files identical despite different names*

