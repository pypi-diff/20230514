# Comparing `tmp/scranking-0.1.1.tar.gz` & `tmp/scranking-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scranking-0.1.1.tar", last modified: Sun Mar 26 00:33:30 2023, max compression
+gzip compressed data, was "scranking-0.1.2.tar", last modified: Sun May 14 02:47:06 2023, max compression
```

## Comparing `scranking-0.1.1.tar` & `scranking-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 joon      (1000) joon      (1000)        0 2023-03-26 00:33:30.685870 scranking-0.1.1/
--rw-r--r--   0 joon      (1000) joon      (1000)      433 2023-03-25 20:48:05.000000 scranking-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 joon      (1000) joon      (1000)     1065 2023-03-03 16:28:18.000000 scranking-0.1.1/LICENSE
--rw-r--r--   0 joon      (1000) joon      (1000)      371 2023-03-26 00:27:12.000000 scranking-0.1.1/MANIFEST.in
--rw-r--r--   0 joon      (1000) joon      (1000)     2276 2023-03-26 00:27:12.000000 scranking-0.1.1/Makefile
--rw-r--r--   0 joon      (1000) joon      (1000)     3039 2023-03-26 00:33:30.685870 scranking-0.1.1/PKG-INFO
--rw-r--r--   0 joon      (1000) joon      (1000)      952 2023-03-25 20:48:05.000000 scranking-0.1.1/README.md
--rw-r--r--   0 joon      (1000) joon      (1000)     2174 2023-03-25 20:48:05.000000 scranking-0.1.1/pyproject.toml
-drwxr-xr-x   0 joon      (1000) joon      (1000)        0 2023-03-26 00:33:30.675870 scranking-0.1.1/scranking/
--rw-r--r--   0 joon      (1000) joon      (1000)     2434 2023-03-25 18:59:47.000000 scranking-0.1.1/scranking/Swimmer.py
--rw-r--r--   0 joon      (1000) joon      (1000)        0 2023-03-04 00:39:51.000000 scranking-0.1.1/scranking/__init__.py
--rw-r--r--   0 joon      (1000) joon      (1000)       22 2023-03-25 20:48:05.000000 scranking-0.1.1/scranking/_version.py
-drwxr-xr-x   0 joon      (1000) joon      (1000)        0 2023-03-26 00:33:30.685870 scranking-0.1.1/scranking/test/
--rw-r--r--   0 joon      (1000) joon      (1000)   104653 2023-03-04 00:39:51.000000 scranking-0.1.1/scranking/test/schml.txt
--rw-r--r--   0 joon      (1000) joon      (1000)     1866 2023-03-25 18:59:47.000000 scranking-0.1.1/scranking/test/test_Swimmer.py
--rw-r--r--   0 joon      (1000) joon      (1000)      269 2023-03-25 18:59:47.000000 scranking-0.1.1/scranking/test/test_intergration.py
-drwxr-xr-x   0 joon      (1000) joon      (1000)        0 2023-03-26 00:33:30.675870 scranking-0.1.1/scranking.egg-info/
--rw-r--r--   0 joon      (1000) joon      (1000)     3039 2023-03-26 00:33:30.000000 scranking-0.1.1/scranking.egg-info/PKG-INFO
--rw-r--r--   0 joon      (1000) joon      (1000)      399 2023-03-26 00:33:30.000000 scranking-0.1.1/scranking.egg-info/SOURCES.txt
--rw-r--r--   0 joon      (1000) joon      (1000)        1 2023-03-26 00:33:30.000000 scranking-0.1.1/scranking.egg-info/dependency_links.txt
--rw-r--r--   0 joon      (1000) joon      (1000)      171 2023-03-26 00:33:30.000000 scranking-0.1.1/scranking.egg-info/requires.txt
--rw-r--r--   0 joon      (1000) joon      (1000)       10 2023-03-26 00:33:30.000000 scranking-0.1.1/scranking.egg-info/top_level.txt
--rw-r--r--   0 joon      (1000) joon      (1000)       38 2023-03-26 00:33:30.685870 scranking-0.1.1/setup.cfg
--rw-r--r--   0 joon      (1000) joon      (1000)       39 2023-03-04 00:39:51.000000 scranking-0.1.1/setup.py
+drwxr-xr-x   0 joon      (1000) joon      (1000)        0 2023-05-14 02:47:06.388657 scranking-0.1.2/
+-rw-r--r--   0 joon      (1000) joon      (1000)      580 2023-05-14 02:41:02.000000 scranking-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 joon      (1000) joon      (1000)     1065 2023-03-03 16:28:18.000000 scranking-0.1.2/LICENSE
+-rw-r--r--   0 joon      (1000) joon      (1000)      371 2023-03-26 00:27:12.000000 scranking-0.1.2/MANIFEST.in
+-rw-r--r--   0 joon      (1000) joon      (1000)     2276 2023-05-14 02:01:56.000000 scranking-0.1.2/Makefile
+-rw-r--r--   0 joon      (1000) joon      (1000)     4131 2023-05-14 02:47:06.388657 scranking-0.1.2/PKG-INFO
+-rw-r--r--   0 joon      (1000) joon      (1000)     2044 2023-05-14 02:41:02.000000 scranking-0.1.2/README.md
+-rw-r--r--   0 joon      (1000) joon      (1000)     2232 2023-05-14 02:41:02.000000 scranking-0.1.2/pyproject.toml
+drwxr-xr-x   0 joon      (1000) joon      (1000)        0 2023-05-14 02:47:06.378657 scranking-0.1.2/scranking/
+-rw-r--r--   0 joon      (1000) joon      (1000)     3010 2023-05-14 02:01:56.000000 scranking-0.1.2/scranking/Swimmer.py
+-rw-r--r--   0 joon      (1000) joon      (1000)        0 2023-03-04 00:39:51.000000 scranking-0.1.2/scranking/__init__.py
+-rw-r--r--   0 joon      (1000) joon      (1000)       22 2023-05-14 02:41:02.000000 scranking-0.1.2/scranking/_version.py
+drwxr-xr-x   0 joon      (1000) joon      (1000)        0 2023-05-14 02:47:06.388657 scranking-0.1.2/scranking/test/
+-rw-r--r--   0 joon      (1000) joon      (1000)     4581 2023-05-14 02:01:56.000000 scranking-0.1.2/scranking/test/test_Swimmer.py
+-rw-r--r--   0 joon      (1000) joon      (1000)      269 2023-03-25 18:59:47.000000 scranking-0.1.2/scranking/test/test_intergration.py
+drwxr-xr-x   0 joon      (1000) joon      (1000)        0 2023-05-14 02:47:06.388657 scranking-0.1.2/scranking.egg-info/
+-rw-r--r--   0 joon      (1000) joon      (1000)     4131 2023-05-14 02:47:06.000000 scranking-0.1.2/scranking.egg-info/PKG-INFO
+-rw-r--r--   0 joon      (1000) joon      (1000)      374 2023-05-14 02:47:06.000000 scranking-0.1.2/scranking.egg-info/SOURCES.txt
+-rw-r--r--   0 joon      (1000) joon      (1000)        1 2023-05-14 02:47:06.000000 scranking-0.1.2/scranking.egg-info/dependency_links.txt
+-rw-r--r--   0 joon      (1000) joon      (1000)      208 2023-05-14 02:47:06.000000 scranking-0.1.2/scranking.egg-info/requires.txt
+-rw-r--r--   0 joon      (1000) joon      (1000)       10 2023-05-14 02:47:06.000000 scranking-0.1.2/scranking.egg-info/top_level.txt
+-rw-r--r--   0 joon      (1000) joon      (1000)       38 2023-05-14 02:47:06.388657 scranking-0.1.2/setup.cfg
+-rw-r--r--   0 joon      (1000) joon      (1000)       39 2023-03-04 00:39:51.000000 scranking-0.1.2/setup.py
```

### Comparing `scranking-0.1.1/LICENSE` & `scranking-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scranking-0.1.1/Makefile` & `scranking-0.1.2/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 #########
 # TESTS #
 #########
 test: ## clean and run unit tests
 	python3 -m pytest -v $(TESTS)
 
 coverage:  ## clean and run unit tests with coverage
-	python3 -m pytest -v $(TESTS) --cov=$(SRC) --cov-branch --cov-fail-under=70 --cov-report term-missing
+	python3 -m pytest -v $(TESTS) --cov=$(SRC) --cov-branch --cov-fail-under=80 --cov-report term-missing
 
 # Alias
 tests: test
 
 ###########
 # VERSION #
 ###########
```

### Comparing `scranking-0.1.1/PKG-INFO` & `scranking-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scranking
-Version: 0.1.1
+Version: 0.1.2
 Summary: scranking is a python library that display ranking of the college swimmer
 Author-email: Joon Ahn <sa3883@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Joon Ahn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,21 +41,52 @@
 License-File: LICENSE
 
 # scranking
 
 scranking is a python library that display ranking of the college swimmer
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
-
 ![GitHub issues](https://img.shields.io/github/issues/joon0110/scranking)
 [![Build Status](https://github.com/joon0110/scranking/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/joon0110/scranking/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/joon0110/scranking/branch/main/graph/badge.svg)](https://codecov.io/gh/joon0110/scranking)
+[![PyPI](https://img.shields.io/pypi/v/scranking)](https://pypi.org/project/scranking/)
+[![Docs](https://readthedocs.org/projects/scranking/badge/?version=latest)](https://scranking.readthedocs.io/en/latest/)
 
 ## Overview
 
-Scranking is a library that scrapes data from a website such as [swimcloud](https://www.swimcloud.com/swimmer/549377/), which is website that shows times and ranking of the college swimmer. 
+Scranking is a library designed specifically for extracting data from [swimcloud](https://www.swimcloud.com/swimmer/549377/), a comprehensive website that showcases the times and rankings of high school and college swimmers.
 
 The library will allow users to simpily type the URL and get all the neccessary information of that swimmer.
 
 ## Install
 
-Install using 'pip install scranking' in the command line.
+Install using 'pip install scranking' in the command line and import it to your python file like all the others.
+
+## Quickstart of scranking
+
+```python
+from scranking import Swimmer
+
+    # Initialize the swimmer object with your swimcloud url
+    swimmer = Swimmer("url")
+
+    # Check if the browser is working
+    swimmer.get_http_status()
+
+    # Create a bf4 for that swimmer objecft
+    swimmer.get_soup()
+
+    # Save the html of the website into text file
+    swimmer.save_soup_to_file("soup", "filename.txt")
+
+    # Get the full name of that swimmer with the soup you created
+    swimmer.get_name("soup")
+
+    # Find a line html that contains swimmer's social network information and hometown
+    swimmer.get_info("infohtml")
+
+    # Get all the events for that swimmer with the best time
+    swimmer.get_event("soup")
+
+    # A search method for get_event method
+    swimmer.lookup_event("40 L Free")
+```
```

### Comparing `scranking-0.1.1/pyproject.toml` & `scranking-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "scranking"
 authors = [{name = "Joon Ahn", email = "sa3883@columbia.edu"}]
 description="scranking is a python library that display ranking of the college swimmer"
 readme = "README.md"
-version = '0.1.1'
+version = '0.1.2'
 requires-python = ">=3.8"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -45,14 +45,17 @@
     "flake8-pyproject",
     "mypy",
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
     "twine",
     "wheel",
     "beautifulsoup4",
+    "sphinx",
+    "sphinx_rtd_theme",
+    "recommonmark",
 ]
 
 [tool.black]
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
```

### Comparing `scranking-0.1.1/scranking.egg-info/PKG-INFO` & `scranking-0.1.2/scranking.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scranking
-Version: 0.1.1
+Version: 0.1.2
 Summary: scranking is a python library that display ranking of the college swimmer
 Author-email: Joon Ahn <sa3883@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Joon Ahn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,21 +41,52 @@
 License-File: LICENSE
 
 # scranking
 
 scranking is a python library that display ranking of the college swimmer
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
-
 ![GitHub issues](https://img.shields.io/github/issues/joon0110/scranking)
 [![Build Status](https://github.com/joon0110/scranking/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/joon0110/scranking/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/joon0110/scranking/branch/main/graph/badge.svg)](https://codecov.io/gh/joon0110/scranking)
+[![PyPI](https://img.shields.io/pypi/v/scranking)](https://pypi.org/project/scranking/)
+[![Docs](https://readthedocs.org/projects/scranking/badge/?version=latest)](https://scranking.readthedocs.io/en/latest/)
 
 ## Overview
 
-Scranking is a library that scrapes data from a website such as [swimcloud](https://www.swimcloud.com/swimmer/549377/), which is website that shows times and ranking of the college swimmer. 
+Scranking is a library designed specifically for extracting data from [swimcloud](https://www.swimcloud.com/swimmer/549377/), a comprehensive website that showcases the times and rankings of high school and college swimmers.
 
 The library will allow users to simpily type the URL and get all the neccessary information of that swimmer.
 
 ## Install
 
-Install using 'pip install scranking' in the command line.
+Install using 'pip install scranking' in the command line and import it to your python file like all the others.
+
+## Quickstart of scranking
+
+```python
+from scranking import Swimmer
+
+    # Initialize the swimmer object with your swimcloud url
+    swimmer = Swimmer("url")
+
+    # Check if the browser is working
+    swimmer.get_http_status()
+
+    # Create a bf4 for that swimmer objecft
+    swimmer.get_soup()
+
+    # Save the html of the website into text file
+    swimmer.save_soup_to_file("soup", "filename.txt")
+
+    # Get the full name of that swimmer with the soup you created
+    swimmer.get_name("soup")
+
+    # Find a line html that contains swimmer's social network information and hometown
+    swimmer.get_info("infohtml")
+
+    # Get all the events for that swimmer with the best time
+    swimmer.get_event("soup")
+
+    # A search method for get_event method
+    swimmer.lookup_event("40 L Free")
+```
```

