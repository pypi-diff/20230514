# Comparing `tmp/pysyncon-0.2.1.tar.gz` & `tmp/pysyncon-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Code\pysyncon\dist\.tmp-lgezz1l7\pysyncon-0.2.1.tar", last modified: Wed Jan 18 21:53:21 2023, max compression
+gzip compressed data, was "C:\Code\pysyncon\dist\.tmp-lvvridfg\pysyncon-1.0.0.tar", last modified: Sun May 14 12:49:31 2023, max compression
```

## Comparing `pysyncon-0.2.1.tar` & `pysyncon-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-01-18 21:53:21.072232 pysyncon-0.2.1/
--rw-rw-rw-   0        0        0     1094 2023-01-07 12:49:27.000000 pysyncon-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1475 2023-01-18 21:53:21.072232 pysyncon-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2023-01-17 23:47:16.000000 pysyncon-0.2.1/README.md
--rw-rw-rw-   0        0        0       84 2023-01-07 12:49:27.000000 pysyncon-0.2.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-01-18 21:53:21.057272 pysyncon-0.2.1/pysyncon/
--rw-rw-rw-   0        0        0       90 2023-01-15 23:33:23.000000 pysyncon-0.2.1/pysyncon/__init__.py
--rw-rw-rw-   0        0        0     7110 2023-01-17 19:34:41.000000 pysyncon-0.2.1/pysyncon/augsynth.py
--rw-rw-rw-   0        0        0     6798 2023-01-17 23:47:16.000000 pysyncon-0.2.1/pysyncon/dataprep.py
--rw-rw-rw-   0        0        0     8043 2023-01-18 21:06:47.000000 pysyncon-0.2.1/pysyncon/synth.py
--rw-rw-rw-   0        0        0     1955 2023-01-17 19:34:41.000000 pysyncon-0.2.1/pysyncon/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-18 21:53:21.071234 pysyncon-0.2.1/pysyncon.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-01-18 21:53:21.000000 pysyncon-0.2.1/pysyncon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-01-18 21:53:21.000000 pysyncon-0.2.1/pysyncon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-18 21:53:21.000000 pysyncon-0.2.1/pysyncon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-01-18 21:53:21.000000 pysyncon-0.2.1/pysyncon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-18 21:53:21.000000 pysyncon-0.2.1/pysyncon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      550 2023-01-18 21:53:21.073228 pysyncon-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 12:49:31.016911 pysyncon-1.0.0/
+-rw-rw-rw-   0        0        0     1094 2023-01-07 12:49:27.000000 pysyncon-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2002 2023-05-14 12:49:31.016911 pysyncon-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-05-10 17:47:37.000000 pysyncon-1.0.0/README.md
+-rw-rw-rw-   0        0        0       84 2023-01-07 12:49:27.000000 pysyncon-1.0.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-14 12:49:30.988988 pysyncon-1.0.0/pysyncon/
+-rw-rw-rw-   0        0        0      162 2023-05-10 17:47:37.000000 pysyncon-1.0.0/pysyncon/__init__.py
+-rw-rw-rw-   0        0        0     4776 2023-05-10 17:47:37.000000 pysyncon-1.0.0/pysyncon/augsynth.py
+-rw-rw-rw-   0        0        0    10135 2023-05-14 10:56:56.000000 pysyncon-1.0.0/pysyncon/base.py
+-rw-rw-rw-   0        0        0    11029 2023-02-15 11:02:20.000000 pysyncon-1.0.0/pysyncon/dataprep.py
+-rw-rw-rw-   0        0        0     2727 2023-05-10 17:47:37.000000 pysyncon-1.0.0/pysyncon/penalized.py
+-rw-rw-rw-   0        0        0     3698 2023-05-10 17:47:37.000000 pysyncon-1.0.0/pysyncon/robust.py
+-rw-rw-rw-   0        0        0     8700 2023-05-11 21:07:11.000000 pysyncon-1.0.0/pysyncon/synth.py
+-rw-rw-rw-   0        0        0    12915 2023-05-14 10:56:56.000000 pysyncon-1.0.0/pysyncon/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-14 12:49:31.007938 pysyncon-1.0.0/pysyncon.egg-info/
+-rw-rw-rw-   0        0        0     2002 2023-05-14 12:49:30.000000 pysyncon-1.0.0/pysyncon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2023-05-14 12:49:30.000000 pysyncon-1.0.0/pysyncon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 12:49:30.000000 pysyncon-1.0.0/pysyncon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-14 12:49:30.000000 pysyncon-1.0.0/pysyncon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 12:49:30.000000 pysyncon-1.0.0/pysyncon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      550 2023-05-14 12:49:31.018907 pysyncon-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 12:49:31.016911 pysyncon-1.0.0/tests/
+-rw-rw-rw-   0        0        0     3232 2023-01-29 17:24:02.000000 pysyncon-1.0.0/tests/test_augsynth_basque.py
+-rw-rw-rw-   0        0        0    13196 2023-01-17 19:34:41.000000 pysyncon-1.0.0/tests/test_dataprep.py
+-rw-rw-rw-   0        0        0     3022 2023-05-10 17:47:37.000000 pysyncon-1.0.0/tests/test_penalized_basque.py
+-rw-rw-rw-   0        0        0     3168 2023-05-10 17:47:37.000000 pysyncon-1.0.0/tests/test_robust_basque.py
+-rw-rw-rw-   0        0        0     4758 2023-02-11 21:48:03.000000 pysyncon-1.0.0/tests/test_synth.py
+-rw-rw-rw-   0        0        0     7677 2023-05-14 10:56:56.000000 pysyncon-1.0.0/tests/test_synth_basque.py
+-rw-rw-rw-   0        0        0     3687 2023-01-29 17:24:02.000000 pysyncon-1.0.0/tests/test_synth_germany.py
+-rw-rw-rw-   0        0        0     4816 2023-01-29 17:24:02.000000 pysyncon-1.0.0/tests/test_synth_texas.py
+-rw-rw-rw-   0        0        0     5229 2023-05-14 10:56:51.000000 pysyncon-1.0.0/tests/test_utils.py
```

### Comparing `pysyncon-0.2.1/LICENSE` & `pysyncon-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysyncon-0.2.1/PKG-INFO` & `pysyncon-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 Metadata-Version: 2.1
 Name: pysyncon
-Version: 0.2.1
+Version: 1.0.0
 Home-page: https://github.com/sdfordham/pysyncon/
 Author: Stiofán Fordham
 License: MIT License
 Keywords: Synth,augsynth,synthetic-control-method,causal-inference
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 
-# pysyncon ![](https://img.shields.io/badge/python-3.8+-blue.svg) ![build](https://github.com/sdfordham/pysyncon/actions/workflows/build.yml/badge.svg)
+# pysyncon ![](https://img.shields.io/badge/python-3.8+-blue.svg) ![build](https://github.com/sdfordham/pysyncon/actions/workflows/main.yml/badge.svg)
 
-A python module for the synthetic control method that provides the same functionality as the R package [Synth](https://CRAN.R-project.org/package=Synth) and [augsynth](https://github.com/ebenmichael/augsynth) and eventually some other related methods (e.g. placebo tests).
+A python module for the synthetic control method that provides implementations of:
+
+- Synthetic Control Method (Abadie & Gardeazabal 2003)
+- Robust Synthetic Control Method (Amjad, Shah & Shen 2018)
+- Augmented Synthetic Control Method (Ben-Michael, Feller & Rothstein 2021)
+- Penalized Synthetic Control Method (Abadie & L'Hour 2021)
+
+The package also provides methods for performing placebo tests with the above.
+
+The implementations of the Synthetic Control method aims to be reconcilable with the R package [Synth](https://CRAN.R-project.org/package=Synth) and similarly the implementation of the Augmented Synthetic Control method and the R package [augsynth](https://github.com/ebenmichael/augsynth).
 
 ## Installation
 Install it from PyPI using pip:
 
 ````bash
 python -m pip install pysyncon
 ````
 
 ## Usage
 
-In the examples folder are notebooks reproducing the weights from:
+Documentation is available on [github-pages](https://sdfordham.github.io/pysyncon/). In the examples folder are notebooks reproducing the weights from:
 
 - The Economic Costs of Conflict: A Case Study of the Basque Country, Alberto Abadie and Javier Gardeazabal; The American Economic Review Vol. 93, No. 1 (Mar., 2003), pp. 113-132.
 - The worked example 'Prison construction and Black male incarceration' from the last chapter of 'Causal Inference: The Mixtape' by Scott Cunningham.
 - Comparative Politics and the Synthetic Control Method, Alberto Abadie, Alexis Diamond and Jens Hainmueller; American Journal of Political Science Vol. 59, No. 2 (April 2015), pp. 495-510.
```

### Comparing `pysyncon-0.2.1/README.md` & `pysyncon-1.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 
 
-# pysyncon ![](https://img.shields.io/badge/python-3.8+-blue.svg) ![build](https://github.com/sdfordham/pysyncon/actions/workflows/build.yml/badge.svg)
+# pysyncon ![](https://img.shields.io/badge/python-3.8+-blue.svg) ![build](https://github.com/sdfordham/pysyncon/actions/workflows/main.yml/badge.svg)
 
-A python module for the synthetic control method that provides the same functionality as the R package [Synth](https://CRAN.R-project.org/package=Synth) and [augsynth](https://github.com/ebenmichael/augsynth) and eventually some other related methods (e.g. placebo tests).
+A python module for the synthetic control method that provides implementations of:
+
+- Synthetic Control Method (Abadie & Gardeazabal 2003)
+- Robust Synthetic Control Method (Amjad, Shah & Shen 2018)
+- Augmented Synthetic Control Method (Ben-Michael, Feller & Rothstein 2021)
+- Penalized Synthetic Control Method (Abadie & L'Hour 2021)
+
+The package also provides methods for performing placebo tests with the above.
+
+The implementations of the Synthetic Control method aims to be reconcilable with the R package [Synth](https://CRAN.R-project.org/package=Synth) and similarly the implementation of the Augmented Synthetic Control method and the R package [augsynth](https://github.com/ebenmichael/augsynth).
 
 ## Installation
 Install it from PyPI using pip:
 
 ````bash
 python -m pip install pysyncon
 ````
 
 ## Usage
 
-In the examples folder are notebooks reproducing the weights from:
+Documentation is available on [github-pages](https://sdfordham.github.io/pysyncon/). In the examples folder are notebooks reproducing the weights from:
 
 - The Economic Costs of Conflict: A Case Study of the Basque Country, Alberto Abadie and Javier Gardeazabal; The American Economic Review Vol. 93, No. 1 (Mar., 2003), pp. 113-132.
 - The worked example 'Prison construction and Black male incarceration' from the last chapter of 'Causal Inference: The Mixtape' by Scott Cunningham.
 - Comparative Politics and the Synthetic Control Method, Alberto Abadie, Alexis Diamond and Jens Hainmueller; American Journal of Political Science Vol. 59, No. 2 (April 2015), pp. 495-510.
```

### Comparing `pysyncon-0.2.1/pysyncon.egg-info/PKG-INFO` & `pysyncon-1.0.0/pysyncon.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 Metadata-Version: 2.1
 Name: pysyncon
-Version: 0.2.1
+Version: 1.0.0
 Home-page: https://github.com/sdfordham/pysyncon/
 Author: Stiofán Fordham
 License: MIT License
 Keywords: Synth,augsynth,synthetic-control-method,causal-inference
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 
-# pysyncon ![](https://img.shields.io/badge/python-3.8+-blue.svg) ![build](https://github.com/sdfordham/pysyncon/actions/workflows/build.yml/badge.svg)
+# pysyncon ![](https://img.shields.io/badge/python-3.8+-blue.svg) ![build](https://github.com/sdfordham/pysyncon/actions/workflows/main.yml/badge.svg)
 
-A python module for the synthetic control method that provides the same functionality as the R package [Synth](https://CRAN.R-project.org/package=Synth) and [augsynth](https://github.com/ebenmichael/augsynth) and eventually some other related methods (e.g. placebo tests).
+A python module for the synthetic control method that provides implementations of:
+
+- Synthetic Control Method (Abadie & Gardeazabal 2003)
+- Robust Synthetic Control Method (Amjad, Shah & Shen 2018)
+- Augmented Synthetic Control Method (Ben-Michael, Feller & Rothstein 2021)
+- Penalized Synthetic Control Method (Abadie & L'Hour 2021)
+
+The package also provides methods for performing placebo tests with the above.
+
+The implementations of the Synthetic Control method aims to be reconcilable with the R package [Synth](https://CRAN.R-project.org/package=Synth) and similarly the implementation of the Augmented Synthetic Control method and the R package [augsynth](https://github.com/ebenmichael/augsynth).
 
 ## Installation
 Install it from PyPI using pip:
 
 ````bash
 python -m pip install pysyncon
 ````
 
 ## Usage
 
-In the examples folder are notebooks reproducing the weights from:
+Documentation is available on [github-pages](https://sdfordham.github.io/pysyncon/). In the examples folder are notebooks reproducing the weights from:
 
 - The Economic Costs of Conflict: A Case Study of the Basque Country, Alberto Abadie and Javier Gardeazabal; The American Economic Review Vol. 93, No. 1 (Mar., 2003), pp. 113-132.
 - The worked example 'Prison construction and Black male incarceration' from the last chapter of 'Causal Inference: The Mixtape' by Scott Cunningham.
 - Comparative Politics and the Synthetic Control Method, Alberto Abadie, Alexis Diamond and Jens Hainmueller; American Journal of Political Science Vol. 59, No. 2 (April 2015), pp. 495-510.
```

### Comparing `pysyncon-0.2.1/setup.cfg` & `pysyncon-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7973 796e 636f 6e0d 0a76 6572   = pysyncon..ver
-00000020: 7369 6f6e 203d 2030 2e32 2e31 0d0a 6175  sion = 0.2.1..au
+00000020: 7369 6f6e 203d 2031 2e30 2e30 0d0a 6175  sion = 1.0.0..au
 00000030: 7468 6f72 203d 2053 7469 6f66 c3a1 6e20  thor = Stiof..n 
 00000040: 466f 7264 6861 6d0d 0a75 726c 203d 2068  Fordham..url = h
 00000050: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00000060: 6d2f 7364 666f 7264 6861 6d2f 7079 7379  m/sdfordham/pysy
 00000070: 6e63 6f6e 2f0d 0a6c 6f6e 675f 6465 7363  ncon/..long_desc
 00000080: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000090: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
```

