# Comparing `tmp/geocontour-1.2.2.tar.gz` & `tmp/geocontour-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocontour-1.2.2.tar", last modified: Tue Mar 21 18:30:41 2023, max compression
+gzip compressed data, was "geocontour-1.3.0.tar", last modified: Sat May 13 23:56:59 2023, max compression
```

## Comparing `geocontour-1.2.2.tar` & `geocontour-1.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-03-21 18:30:41.062880 geocontour-1.2.2/
--rw-r--r--   0 bkrichman   (501) staff       (20)      190 2023-03-20 18:00:45.000000 geocontour-1.2.2/.gitignore
--rw-r--r--   0 bkrichman   (501) staff       (20)      581 2023-03-21 18:07:33.000000 geocontour-1.2.2/CITATION.cff
--rw-r--r--   0 bkrichman   (501) staff       (20)     1079 2023-03-07 20:16:09.000000 geocontour-1.2.2/LICENSE.txt
--rw-r--r--   0 bkrichman   (501) staff       (20)      314 2022-12-31 15:38:33.000000 geocontour-1.2.2/MANIFEST.in
--rw-r--r--   0 bkrichman   (501) staff       (20)    10542 2023-03-21 18:30:41.062406 geocontour-1.2.2/PKG-INFO
--rw-r--r--   0 bkrichman   (501) staff       (20)     9809 2023-03-21 18:07:18.000000 geocontour-1.2.2/README.md
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-03-21 18:30:40.988410 geocontour-1.2.2/geocontour/
--rw-r--r--   0 bkrichman   (501) staff       (20)      426 2023-03-20 16:17:38.000000 geocontour-1.2.2/geocontour/__init__.py
--rw-r--r--   0 bkrichman   (501) staff       (20)     7222 2023-03-20 16:17:38.000000 geocontour-1.2.2/geocontour/check.py
--rw-r--r--   0 bkrichman   (501) staff       (20)    39731 2023-03-20 16:17:38.000000 geocontour-1.2.2/geocontour/contourtrace.py
--rw-r--r--   0 bkrichman   (501) staff       (20)    11433 2023-03-20 16:17:38.000000 geocontour-1.2.2/geocontour/contourutil.py
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-03-21 18:30:40.995539 geocontour-1.2.2/geocontour/data/
--rw-r--r--   0 bkrichman   (501) staff       (20)   108990 2022-12-04 15:35:26.000000 geocontour-1.2.2/geocontour/data/MissBasin_boundary.npz
--rw-r--r--   0 bkrichman   (501) staff       (20)     3166 2022-12-04 15:26:13.000000 geocontour-1.2.2/geocontour/data/generic_boundary.npz
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-03-21 18:30:40.996333 geocontour-1.2.2/geocontour/examples/
--rw-r--r--   0 bkrichman   (501) staff       (20)     9417 2023-03-20 16:17:38.000000 geocontour-1.2.2/geocontour/examples/__init__.py
--rw-r--r--   0 bkrichman   (501) staff       (20)     5977 2023-03-20 16:17:38.000000 geocontour-1.2.2/geocontour/geocontour.py
--rw-r--r--   0 bkrichman   (501) staff       (20)     9263 2023-03-20 16:17:38.000000 geocontour-1.2.2/geocontour/grid.py
--rw-r--r--   0 bkrichman   (501) staff       (20)    14461 2023-03-20 16:17:38.000000 geocontour-1.2.2/geocontour/masksearch.py
--rw-r--r--   0 bkrichman   (501) staff       (20)     9951 2023-03-20 16:17:38.000000 geocontour-1.2.2/geocontour/maskutil.py
--rw-r--r--   0 bkrichman   (501) staff       (20)    29100 2023-03-20 16:17:38.000000 geocontour-1.2.2/geocontour/output.py
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-03-21 18:30:40.997986 geocontour-1.2.2/geocontour/tests/
--rw-r--r--   0 bkrichman   (501) staff       (20)     6903 2023-03-20 16:17:38.000000 geocontour-1.2.2/geocontour/tests/__init__.py
--rw-r--r--   0 bkrichman   (501) staff       (20)    12681 2023-03-20 16:17:38.000000 geocontour-1.2.2/geocontour/tests/timing.py
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-03-21 18:30:40.992203 geocontour-1.2.2/geocontour.egg-info/
--rw-r--r--   0 bkrichman   (501) staff       (20)    10542 2023-03-21 18:30:40.000000 geocontour-1.2.2/geocontour.egg-info/PKG-INFO
--rw-r--r--   0 bkrichman   (501) staff       (20)     1101 2023-03-21 18:30:40.000000 geocontour-1.2.2/geocontour.egg-info/SOURCES.txt
--rw-r--r--   0 bkrichman   (501) staff       (20)        1 2023-03-21 18:30:40.000000 geocontour-1.2.2/geocontour.egg-info/dependency_links.txt
--rw-r--r--   0 bkrichman   (501) staff       (20)       41 2023-03-21 18:30:40.000000 geocontour-1.2.2/geocontour.egg-info/requires.txt
--rw-r--r--   0 bkrichman   (501) staff       (20)       11 2023-03-21 18:30:40.000000 geocontour-1.2.2/geocontour.egg-info/top_level.txt
-drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-03-21 18:30:41.061046 geocontour-1.2.2/images/
--rwxrwxr--   0 bkrichman   (501) staff       (20)  1720228 2022-12-19 01:54:17.000000 geocontour-1.2.2/images/example_large_boundary+mask.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)  1499990 2022-12-19 01:54:17.000000 geocontour-1.2.2/images/example_large_contour.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)  1723815 2022-12-19 01:54:17.000000 geocontour-1.2.2/images/example_large_contoursearch.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)  3480862 2022-12-19 01:54:17.000000 geocontour-1.2.2/images/example_large_geocontour+bordfeat.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)  4377349 2022-12-19 01:54:17.000000 geocontour-1.2.2/images/example_large_geocontour+natfeat.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)  1736596 2022-12-19 01:54:17.000000 geocontour-1.2.2/images/example_large_geocontour.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)   148016 2022-12-19 01:54:17.000000 geocontour-1.2.2/images/example_small_boundary+mask.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)    95607 2022-12-19 01:54:17.000000 geocontour-1.2.2/images/example_small_contour.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)   161593 2022-12-19 01:54:17.000000 geocontour-1.2.2/images/example_small_contoursearch.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)   142525 2022-12-19 01:54:17.000000 geocontour-1.2.2/images/example_small_geocontour.png
--rwxrwxr--   0 bkrichman   (501) staff       (20)   143125 2022-12-19 01:54:17.000000 geocontour-1.2.2/images/example_small_geocontour_simp.png
--rw-r--r--   0 bkrichman   (501) staff       (20)    13364 2022-12-04 21:44:14.000000 geocontour-1.2.2/images/icon_geocontour.png
--rw-r--r--   0 bkrichman   (501) staff       (20)      331 2023-03-21 16:47:22.000000 geocontour-1.2.2/requirements+cartopy.txt
--rw-r--r--   0 bkrichman   (501) staff       (20)      269 2023-03-21 16:46:18.000000 geocontour-1.2.2/requirements.txt
--rw-r--r--   0 bkrichman   (501) staff       (20)       38 2023-03-21 18:30:41.063034 geocontour-1.2.2/setup.cfg
--rw-r--r--   0 bkrichman   (501) staff       (20)     1125 2023-03-21 16:47:45.000000 geocontour-1.2.2/setup.py
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.249652 geocontour-1.3.0/
+-rw-r--r--   0 bkrichman   (501) staff       (20)      190 2023-03-20 18:00:45.000000 geocontour-1.3.0/.gitignore
+-rw-r--r--   0 bkrichman   (501) staff       (20)      559 2023-05-13 23:45:44.000000 geocontour-1.3.0/CITATION.cff
+-rw-r--r--   0 bkrichman   (501) staff       (20)     1079 2023-03-07 20:16:09.000000 geocontour-1.3.0/LICENSE.txt
+-rw-r--r--   0 bkrichman   (501) staff       (20)      314 2022-12-31 15:38:33.000000 geocontour-1.3.0/MANIFEST.in
+-rw-r--r--   0 bkrichman   (501) staff       (20)    11470 2023-05-13 23:56:59.248463 geocontour-1.3.0/PKG-INFO
+-rw-r--r--   0 bkrichman   (501) staff       (20)    10737 2023-05-13 23:52:27.000000 geocontour-1.3.0/README.md
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.164192 geocontour-1.3.0/geocontour/
+-rw-r--r--   0 bkrichman   (501) staff       (20)      426 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/__init__.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)     7222 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/check.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)    54078 2023-05-13 23:30:17.000000 geocontour-1.3.0/geocontour/contourtrace.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)    11433 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/contourutil.py
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.179152 geocontour-1.3.0/geocontour/data/
+-rw-r--r--   0 bkrichman   (501) staff       (20)   108990 2022-12-04 15:35:26.000000 geocontour-1.3.0/geocontour/data/MissBasin_boundary.npz
+-rw-r--r--   0 bkrichman   (501) staff       (20)     3166 2022-12-04 15:26:13.000000 geocontour-1.3.0/geocontour/data/generic_boundary.npz
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.180234 geocontour-1.3.0/geocontour/examples/
+-rw-r--r--   0 bkrichman   (501) staff       (20)     9417 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/examples/__init__.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)     5977 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/geocontour.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)     9263 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/grid.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)    14461 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/masksearch.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)     9951 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/maskutil.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)    29100 2023-03-20 16:17:38.000000 geocontour-1.3.0/geocontour/output.py
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.182896 geocontour-1.3.0/geocontour/tests/
+-rw-r--r--   0 bkrichman   (501) staff       (20)     7285 2023-05-13 23:30:17.000000 geocontour-1.3.0/geocontour/tests/__init__.py
+-rw-r--r--   0 bkrichman   (501) staff       (20)    13553 2023-05-13 23:30:17.000000 geocontour-1.3.0/geocontour/tests/timing.py
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.176411 geocontour-1.3.0/geocontour.egg-info/
+-rw-r--r--   0 bkrichman   (501) staff       (20)    11470 2023-05-13 23:56:59.000000 geocontour-1.3.0/geocontour.egg-info/PKG-INFO
+-rw-r--r--   0 bkrichman   (501) staff       (20)     1101 2023-05-13 23:56:59.000000 geocontour-1.3.0/geocontour.egg-info/SOURCES.txt
+-rw-r--r--   0 bkrichman   (501) staff       (20)        1 2023-05-13 23:56:59.000000 geocontour-1.3.0/geocontour.egg-info/dependency_links.txt
+-rw-r--r--   0 bkrichman   (501) staff       (20)       41 2023-05-13 23:56:59.000000 geocontour-1.3.0/geocontour.egg-info/requires.txt
+-rw-r--r--   0 bkrichman   (501) staff       (20)       11 2023-05-13 23:56:59.000000 geocontour-1.3.0/geocontour.egg-info/top_level.txt
+drwxr-xr-x   0 bkrichman   (501) staff       (20)        0 2023-05-13 23:56:59.246876 geocontour-1.3.0/images/
+-rwxrwxr--   0 bkrichman   (501) staff       (20)  1720228 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_large_boundary+mask.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)  1499990 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_large_contour.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)  1723815 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_large_contoursearch.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)  3480862 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_large_geocontour+bordfeat.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)  4377349 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_large_geocontour+natfeat.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)  1736596 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_large_geocontour.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)   148016 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_small_boundary+mask.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)    95607 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_small_contour.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)   161593 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_small_contoursearch.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)   142525 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_small_geocontour.png
+-rwxrwxr--   0 bkrichman   (501) staff       (20)   143125 2022-12-19 01:54:17.000000 geocontour-1.3.0/images/example_small_geocontour_simp.png
+-rw-r--r--   0 bkrichman   (501) staff       (20)    13364 2022-12-04 21:44:14.000000 geocontour-1.3.0/images/icon_geocontour.png
+-rw-r--r--   0 bkrichman   (501) staff       (20)      330 2023-05-13 23:42:27.000000 geocontour-1.3.0/requirements+cartopy.txt
+-rw-r--r--   0 bkrichman   (501) staff       (20)      269 2023-05-13 23:41:02.000000 geocontour-1.3.0/requirements.txt
+-rw-r--r--   0 bkrichman   (501) staff       (20)       38 2023-05-13 23:56:59.249816 geocontour-1.3.0/setup.cfg
+-rw-r--r--   0 bkrichman   (501) staff       (20)     1125 2023-05-13 23:34:09.000000 geocontour-1.3.0/setup.py
```

### Comparing `geocontour-1.2.2/CITATION.cff` & `geocontour-1.3.0/CITATION.cff`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-cff-version: 1.2.2
+cff-version: 1.3.0
 message: "If you use this software, please cite it as below."
-abstract: "Utilities for masking, contour tracing, and geocontour construction for flux calculations from gridded geographic data"
+abstract: "Utilities for masking, contour tracing, and geocontour construction with gridded geographic data"
 authors:
   -
     family-names: Krichman
     given-names: Benjamin
     orcid: "https://orcid.org/0000-0002-7481-8281"
 title: "geocontour"
-date-released: 2023-03-21
-doi: "10.5281/zenodo.7757447"
+date-released: 2023-05-13
+doi: "10.5281/zenodo.7402714"
 keywords:
   - python
   - geospatial
   - masking
   - contour-tracing
   - gridded-data
 license: MIT
 repository-code: "https://github.com/benkrichman/geocontour"
-version: "1.2.2"
+version: "1.3.0"
```

### Comparing `geocontour-1.2.2/LICENSE.txt` & `geocontour-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/PKG-INFO` & `geocontour-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocontour
-Version: 1.2.2
+Version: 1.3.0
 Summary: Utilities for masking, contour tracing, and geocontour construction with gridded geographic data
 Home-page: https://github.com/benkrichman/geocontour
 Author: Benjamin Krichman
 Author-email: benkrichman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -48,28 +48,28 @@
 
 Find the full documentation hosted [here](https://geocontour.readthedocs.io/en/latest/index.html).
 
 ## Citation
 
 If geocontour played a significant role in your work and you would like to cite it, the following is suggested (APA):
 
-Krichman, B. (2023). *geocontour* (Version 1.2.2) [Computer Software]. https://doi.org/10.5281/zenodo.7757447
+Krichman, B. (2023). *geocontour* (Version 1.3.0) [Computer Software]. https://doi.org/10.5281/zenodo.7402714
 
 Bibtex:
 
 ```latex
 @software{geocontour,
 author={Krichman, Benjamin},
-doi={10.5281/zenodo.7757447},
+doi={10.5281/zenodo.7402714},
 license={MIT},
-month={3},
+month={5},
 year={2023},
 title={{geocontour}},
 url={https://github.com/benkrichman/geocontour},
-version={1.2.2},
+version={1.3.0},
 note = {Computer Software}
 }
 ```
 
 ## Features
 
 ### Masks
@@ -82,21 +82,23 @@
 Useful mask operators
 - return mask connectivity (and null connectivity)
 - return mask edge cells
 - return mask vertex points
 
 ### Contours
 
-Implements 4 existing algorithms for contour tracing, and two improvements on known algorithms
-- square tracing [^1][^2]
-- moore neighbor tracing [^1][^2]
+Implements 6 existing algorithms for contour tracing, and two improvements on known algorithms
+- square tracing (a.k.a. simple boundary follower/Papert's turtle algorithm) [^3][^4][^5][^7][^8]
+- moore neighbor tracing [^3][^8]
 - improved moore neighbor tracing (capturing inside corners)
-- pavlidis tracing [^1][^3]
+- pavlidis tracing [^3][^6]
 - improved pavlidis tracing (capturing inside corners)
-- fast representative tracing [^4]
+- modified simple boundary follower [^1][^2][^4]
+- improved simple boundary follower [^1][^2][^7]
+- fast representative tracing [^7]
 
 Tuning of contours created from tracing input masks
 - trace direction
 - selectable and adjustable stopping conditions
 - automatic or manual selection of starting cell
 - selectable connection type (cell to cell or cell edge to cell center)
 - simplification of output contour (removal of repeating cells)
@@ -200,14 +202,24 @@
 
 ```python
 geocontour.output.plot(latitudes,longitudes,geocontour=geocontour,title='Example Geocontour\nMississippi River Basin',outname='example_large_geocontour+bordfeat',features='borders')
 ```
 
 <img src=https://github.com/benkrichman/geocontour/raw/main/images/example_large_geocontour%2Bbordfeat.png width="800">
 
-[^1]: Ghuneim, A.G. (2000). *Contour Tracing*. McGill University. <https://www.imageprocessingplace.com/downloads_V3/root_downloads/tutorials/contour_tracing_Abeer_George_Ghuneim/alg.html>
+[^1]: Cheong, C.-H., & Han, T.-D. (2006). Improved Simple Boundary Following Algorithm. Journal of KIISE: Software and Applications, 33(4), 427–439. <https://koreascience.kr/article/JAKO200622219415761.pdf>
 
-[^2]: Toussaint, G.T. (2010). *Grids Connectivity and Contour Tracing* [Lesson Notes]. McGill University. <http://www-cgrl.cs.mcgill.ca/~godfried/teaching/mir-reading-assignments/Chapter-2-Grids-Connectivity-Contour-Tracing.pdf>
+[^2]: Cheong, C.-H., Seo, J., & Han, T.-D. (2006). Advanced Contour Tracing Algorithms based on Analysis of Tracing Conditions. Proceedings of the 33rd KISS Fall Conference, 33, 431–436. <https://koreascience.kr/article/CFKO200614539217302.pdf>
+
+[^3]: Ghuneim, A.G. (2000). *Contour Tracing*. McGill University. <https://www.imageprocessingplace.com/downloads_V3/root_downloads/tutorials/contour_tracing_Abeer_George_Ghuneim/alg.html>
+
+[^4]: Gose, E., Johnsonbaugh, R., & Jost, S. (1996). Pattern recognition and image analysis. Prentice Hall PTR.
+
+[^5]: Papert, S. (1973). Uses of Technology to Enhance Education (No. 298; Artificial Intelligence). Massachusetts Institute of Technology. <https://dspace.mit.edu/handle/1721.1/6213>
+
+[^6]: Pavlidis, T. (1982) Algorithms for Graphics and Image Processing. Computer Science Press, New York, NY. <https://doi.org/10.1007/978-3-642-93208-3>
+
+[^7]: Seo, J., Chae, S., Shim, J., Kim, D., Cheong, C., & Han, T.-D. (2016). Fast Contour-Tracing Algorithm Based on a Pixel-Following Method for Image Sensors. Sensors, 16(3), 353. <https://doi.org/10.3390/s16030353>
+
+[^8]: Toussaint, G.T. (2010). *Grids Connectivity and Contour Tracing* [Lesson Notes]. McGill University. <http://www-cgrl.cs.mcgill.ca/~godfried/teaching/mir-reading-assignments/Chapter-2-Grids-Connectivity-Contour-Tracing.pdf>
 
-[^3]: Pavlidis, T. (1982) Algorithms for Graphics and Image Processing. Computer Science Press, New York, NY. <https://doi.org/10.1007/978-3-642-93208-3>
 
-[^4]: Seo, J., Chae, S., Shim, J., Kim, D., Cheong, C., & Han, T.-D. (2016). Fast Contour-Tracing Algorithm Based on a Pixel-Following Method for Image Sensors. Sensors, 16(3), 353. <https://doi.org/10.3390/s16030353>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geocontour-1.2.2/README.md` & `geocontour-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,28 +30,28 @@
 
 Find the full documentation hosted [here](https://geocontour.readthedocs.io/en/latest/index.html).
 
 ## Citation
 
 If geocontour played a significant role in your work and you would like to cite it, the following is suggested (APA):
 
-Krichman, B. (2023). *geocontour* (Version 1.2.2) [Computer Software]. https://doi.org/10.5281/zenodo.7757447
+Krichman, B. (2023). *geocontour* (Version 1.3.0) [Computer Software]. https://doi.org/10.5281/zenodo.7402714
 
 Bibtex:
 
 ```latex
 @software{geocontour,
 author={Krichman, Benjamin},
-doi={10.5281/zenodo.7757447},
+doi={10.5281/zenodo.7402714},
 license={MIT},
-month={3},
+month={5},
 year={2023},
 title={{geocontour}},
 url={https://github.com/benkrichman/geocontour},
-version={1.2.2},
+version={1.3.0},
 note = {Computer Software}
 }
 ```
 
 ## Features
 
 ### Masks
@@ -64,21 +64,23 @@
 Useful mask operators
 - return mask connectivity (and null connectivity)
 - return mask edge cells
 - return mask vertex points
 
 ### Contours
 
-Implements 4 existing algorithms for contour tracing, and two improvements on known algorithms
-- square tracing [^1][^2]
-- moore neighbor tracing [^1][^2]
+Implements 6 existing algorithms for contour tracing, and two improvements on known algorithms
+- square tracing (a.k.a. simple boundary follower/Papert's turtle algorithm) [^3][^4][^5][^7][^8]
+- moore neighbor tracing [^3][^8]
 - improved moore neighbor tracing (capturing inside corners)
-- pavlidis tracing [^1][^3]
+- pavlidis tracing [^3][^6]
 - improved pavlidis tracing (capturing inside corners)
-- fast representative tracing [^4]
+- modified simple boundary follower [^1][^2][^4]
+- improved simple boundary follower [^1][^2][^7]
+- fast representative tracing [^7]
 
 Tuning of contours created from tracing input masks
 - trace direction
 - selectable and adjustable stopping conditions
 - automatic or manual selection of starting cell
 - selectable connection type (cell to cell or cell edge to cell center)
 - simplification of output contour (removal of repeating cells)
@@ -182,14 +184,24 @@
 
 ```python
 geocontour.output.plot(latitudes,longitudes,geocontour=geocontour,title='Example Geocontour\nMississippi River Basin',outname='example_large_geocontour+bordfeat',features='borders')
 ```
 
 <img src=https://github.com/benkrichman/geocontour/raw/main/images/example_large_geocontour%2Bbordfeat.png width="800">
 
-[^1]: Ghuneim, A.G. (2000). *Contour Tracing*. McGill University. <https://www.imageprocessingplace.com/downloads_V3/root_downloads/tutorials/contour_tracing_Abeer_George_Ghuneim/alg.html>
+[^1]: Cheong, C.-H., & Han, T.-D. (2006). Improved Simple Boundary Following Algorithm. Journal of KIISE: Software and Applications, 33(4), 427–439. <https://koreascience.kr/article/JAKO200622219415761.pdf>
 
-[^2]: Toussaint, G.T. (2010). *Grids Connectivity and Contour Tracing* [Lesson Notes]. McGill University. <http://www-cgrl.cs.mcgill.ca/~godfried/teaching/mir-reading-assignments/Chapter-2-Grids-Connectivity-Contour-Tracing.pdf>
+[^2]: Cheong, C.-H., Seo, J., & Han, T.-D. (2006). Advanced Contour Tracing Algorithms based on Analysis of Tracing Conditions. Proceedings of the 33rd KISS Fall Conference, 33, 431–436. <https://koreascience.kr/article/CFKO200614539217302.pdf>
+
+[^3]: Ghuneim, A.G. (2000). *Contour Tracing*. McGill University. <https://www.imageprocessingplace.com/downloads_V3/root_downloads/tutorials/contour_tracing_Abeer_George_Ghuneim/alg.html>
+
+[^4]: Gose, E., Johnsonbaugh, R., & Jost, S. (1996). Pattern recognition and image analysis. Prentice Hall PTR.
+
+[^5]: Papert, S. (1973). Uses of Technology to Enhance Education (No. 298; Artificial Intelligence). Massachusetts Institute of Technology. <https://dspace.mit.edu/handle/1721.1/6213>
+
+[^6]: Pavlidis, T. (1982) Algorithms for Graphics and Image Processing. Computer Science Press, New York, NY. <https://doi.org/10.1007/978-3-642-93208-3>
+
+[^7]: Seo, J., Chae, S., Shim, J., Kim, D., Cheong, C., & Han, T.-D. (2016). Fast Contour-Tracing Algorithm Based on a Pixel-Following Method for Image Sensors. Sensors, 16(3), 353. <https://doi.org/10.3390/s16030353>
+
+[^8]: Toussaint, G.T. (2010). *Grids Connectivity and Contour Tracing* [Lesson Notes]. McGill University. <http://www-cgrl.cs.mcgill.ca/~godfried/teaching/mir-reading-assignments/Chapter-2-Grids-Connectivity-Contour-Tracing.pdf>
 
-[^3]: Pavlidis, T. (1982) Algorithms for Graphics and Image Processing. Computer Science Press, New York, NY. <https://doi.org/10.1007/978-3-642-93208-3>
 
-[^4]: Seo, J., Chae, S., Shim, J., Kim, D., Cheong, C., & Han, T.-D. (2016). Fast Contour-Tracing Algorithm Based on a Pixel-Following Method for Image Sensors. Sensors, 16(3), 353. <https://doi.org/10.3390/s16030353>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geocontour-1.2.2/geocontour/check.py` & `geocontour-1.3.0/geocontour/check.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/geocontour/contourtrace.py` & `geocontour-1.3.0/geocontour/contourtrace.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 import geocontour.check as gcc
 import geocontour.maskutil as gcmu
 import geocontour.contourutil as gccu
 
 def square(mask,latitudes=None,longitudes=None,direction='cw',start='auto',stop='either',startvisits=3,checkconn=False,remcontourrepeat=True,remsearchrepeat=False,closecontour=True):
     """
     Find the contour of a mask using the square tracing algorithm
+    
+    Also known as:
+
+        - Papert's turtle algorithm
+        - simple boundary follower (SBF)
 
     Parameters
     ----------
     mask : ndarray
         2D MxN bool array where M=len(`latitudes`) and
         N=len(`longitudes`)
     latitudes : ndarray, optional
@@ -74,28 +79,42 @@
     --------
     geocontour.contourutil.findstart
     geocontour.contourutil.setstop
     moore
     moore_imp
     pavlidis
     pavlidis_imp
+    MSBF
+    ISBF
     TSR
 
     Notes
     -----
     - If `latitudes`/`longitudes` not provided, returned
       `contour`/`contoursearch` will be indices of the input mask
     - `startvisits` parameter will only be utilized when `stop`
       parameter is set to 'Nvisits' or 'either'
 
     References
     ----------
     Ghuneim, A.G. (2000). Contour Tracing. McGill University.
     <https://www.imageprocessingplace.com/downloads_V3/root_downloads/tutorials/contour_tracing_Abeer_George_Ghuneim/alg.html>
 
+    Gose, E., Johnsonbaugh, R., & Jost, S. (1996). Pattern recognition
+    and image analysis. Prentice Hall PTR.
+
+    Papert, S. (1973). Uses of Technology to Enhance Education (No. 298;
+    Artificial Intelligence). Massachusetts Institute of Technology.
+    <https://dspace.mit.edu/handle/1721.1/6213>
+
+    Seo, J., Chae, S., Shim, J., Kim, D., Cheong, C., & Han, T.-D.
+    (2016). Fast Contour-Tracing Algorithm Based on a Pixel-Following
+    Method for Image Sensors. Sensors, 16(3), 353.
+    <https://doi.org/10.3390/s16030353>
+
     Toussaint, G.T. (2010). Grids Connectivity and Contour Tracing
     [Lesson Notes]. McGill University.
     <http://www-cgrl.cs.mcgill.ca/~godfried/teaching/mir-reading-assignments/Chapter-2-Grids-Connectivity-Contour-Tracing.pdf>
     """
     if latitudes is not None and longitudes is not None:
         gcc.cmask(mask,latitudes,longitudes)
     else:
@@ -211,14 +230,16 @@
     --------
     geocontour.contourutil.findstart
     geocontour.contourutil.setstop
     square
     moore_imp
     pavlidis
     pavlidis_imp
+    MSBF
+    ISBF
     TSR
 
     Notes
     -----
     - If `latitudes`/`longitudes` not provided, returned
       `contour`/`contoursearch` will be indices of the input mask
     - `startvisits` parameter will only be utilized when `stop`
@@ -358,14 +379,16 @@
     --------
     geocontour.contourutil.findstart
     geocontour.contourutil.setstop
     square
     moore
     pavlidis
     pavlidis_imp
+    MSBF
+    ISBF
     TSR
 
     Notes
     -----
     - If `latitudes`/`longitudes` not provided, returned
       `contour`/`contoursearch` will be indices of the input mask
     - `startvisits` parameter will only be utilized when `stop`
@@ -505,14 +528,16 @@
     --------
     geocontour.contourutil.findstart
     geocontour.contourutil.setstop
     square
     moore
     moore_imp
     pavlidis_imp
+    MSBF
+    ISBF
     TSR
 
     Notes
     -----
     - If `latitudes`/`longitudes` not provided, returned
       `contour`/`contoursearch` will be indices of the input mask
     - `startvisits` parameter will only be utilized when `stop`
@@ -680,14 +705,16 @@
     --------
     geocontour.contourutil.findstart
     geocontour.contourutil.setstop
     square
     moore
     moore_imp
     pavlidis
+    MSBF
+    ISBF
     TSR
 
     Notes
     -----
     - If `latitudes`/`longitudes` not provided, returned
       `contour`/`contoursearch` will be indices of the input mask
     - `startvisits` parameter will only be utilized when `stop`
@@ -786,14 +813,356 @@
             orientation=insideturn(orientation)
             rotations+=1
         if rotations>3:
             sys.exit('ERROR - Stuck on isolated cell '+str(cell))
     contour,contoursearch=gccu.clean(contourcells,searchcells,latitudes=latitudes,longitudes=longitudes,closecontour=closecontour,remcontourrepeat=remcontourrepeat,remsearchrepeat=remsearchrepeat)
     return contour,contoursearch
 
+def MSBF(mask,latitudes=None,longitudes=None,direction='cw',start='auto',stop='either',startvisits=4,remcontourrepeat=True,remsearchrepeat=False,closecontour=True):
+    """
+    Find the contour of a mask using the modified simple boundary
+    following algorithm
+
+    Parameters
+    ----------
+    mask : ndarray
+        2D MxN bool array where M=len(`latitudes`) and
+        N=len(`longitudes`)
+    latitudes : ndarray, optional
+        1D Nx1 array of latitude points (degrees)
+    longitudes : ndarray, optional
+        1D Nx1 array of longitude points (degrees)
+    direction : {'cw', 'ccw'}, default='cw'
+        select the direction of contour tracing
+    start : {'auto', array_like}, default='auto' 
+        either a selection for automatic start cell assignment or a
+        manual assignment via a 2x2 array describing the start cell and
+        orientation
+
+            row 1: indices of the start cell
+                e.g. for start cell [2,3] second row (lat) and third
+                column (lon)
+            row 2: the start orientation
+                e.g. orientation [0,1] points right, [1,0] points down
+    stop : {'Elisoff', 'Nvisits', 'either'}, default='either'
+        selector for the stopping criterion
+
+            ``Elisoff``
+                stops when the start cell has been re-visited with the
+                same orientation as started with
+            ``Nvisits``
+                stops when the start cell has been re-visited N number
+                of times (N set by `startvisits` parameter)
+            ``either``
+                stops when either Elisoff or Nvisits has been satisfied
+    startvisits : int, default=3
+        the number of times re-visiting the start cell will trigger an
+        end to the search
+    checkconn : bool, default=False
+        select whether to check connectivity and warn the user of
+        potential issues, default=False
+    remcontourrepeat : bool, default=True
+        select whether to remove consecutive repeating cells in the
+        output `contour`
+    remsearchrepeat : bool, default=False
+        select whether to remove consecutive repeating cells in the
+        output `contoursearch`
+    closecontour : bool, default=True
+        select whether to close the output `contour` (first cell = last
+        cell)
+
+    Returns
+    -------
+    contour : ndarray
+        2D Nx2 array of ordered latitude/longitude points (degrees)
+        describing the edge of a mask
+    contoursearch : ndarray
+        2D Nx2 array of ordered latitude/longitude points (degrees)
+        describing the cells searched during contour tracing
+    
+    See Also
+    --------
+    geocontour.contourutil.findstart
+    geocontour.contourutil.setstop
+    square
+    moore
+    moore_imp
+    pavlidis
+    pavlidis_imp
+    ISBF
+    TSR
+
+    Notes
+    -----
+    - If `latitudes`/`longitudes` not provided, returned
+      `contour`/`contoursearch` will be indices of the input mask
+    - `startvisits` parameter will only be utilized when `stop`
+      parameter is set to 'Nvisits' or 'either'
+
+    References
+    ----------
+    Cheong, C.-H., & Han, T.-D. (2006). Improved Simple Boundary
+    Following Algorithm. Journal of KIISE: Software and Applications,
+    33(4), 427–439.
+    <https://koreascience.kr/article/JAKO200622219415761.pdf>
+
+    Cheong, C.-H., Seo, J., & Han, T.-D. (2006). Advanced Contour
+    Tracing Algorithms based on Analysis of Tracing Conditions.
+    Proceedings of the 33rd KISS Fall Conference, 33, 431–436.
+    <https://koreascience.kr/article/CFKO200614539217302.pdf>
+
+    Gose, E., Johnsonbaugh, R., & Jost, S. (1996). Pattern recognition
+    and image analysis. Prentice Hall PTR.
+    """
+    if latitudes is not None and longitudes is not None:
+        gcc.cmask(mask,latitudes,longitudes)
+    else:
+        gcc.cmask(mask)
+    buffermask=np.full((tuple(np.array(mask.shape)+2)),False)
+    buffermask[1:-1,1:-1]=mask
+    if direction=='cw':
+        def outsideturn(orientation):
+            return orientation[::-1]*np.array([-1,1])
+        def insideturn(orientation):
+            return orientation[::-1]*np.array([1,-1])
+        searchdir='ru'
+    elif direction=='ccw':
+        def outsideturn(orientation):
+            return orientation[::-1]*np.array([1,-1])
+        def insideturn(orientation):
+            return orientation[::-1]*np.array([-1,1])
+        searchdir='rd'
+    else:
+        sys.exit('ERROR - direction=\''+direction+'\' is not a valid selection, valid selections are \'cw\'/\'ccw\'')
+    if type(start) is not str:
+        startcell,startorientation=gccu.parsestart(start,buffermask)
+    elif start=='auto':
+        startcell,startorientation=gccu.findstart(buffermask,searchdir=searchdir)
+    else:
+        sys.exit('ERROR - start=\''+start+'\' is not a valid selection, valid selections are \'auto\' or a 2x2 array describing start cell index and start orientation')
+    checkbreak=gccu.setstop(stop,startvisits,startcell,startorientation)
+    orientation=startorientation
+    cell=startcell
+    searchcells=[]
+    contourcells=[]
+    contourcells.append(cell)
+    Nvisits=0
+    breakloop=False
+    tag=False
+    while not breakloop:
+        searchcells.append(cell)
+        if buffermask[cell[0],cell[1]]==True:
+            contourcells.append(cell)
+            O=cell+outsideturn(orientation)
+            R=cell-orientation
+            RO=O-orientation
+            if tag==False and buffermask[O[0],O[1]]==False and buffermask[RO[0],RO[1]]==True and buffermask[R[0],R[1]]==False:
+                orientation=-orientation
+                cell=RO
+                tag=True
+            else:
+                orientation=outsideturn(orientation)
+                cell=O
+                tag=False
+        else:
+            orientation=insideturn(orientation)
+            cell=cell+orientation
+            tag=False
+        if (cell==startcell).all():
+            Nvisits+=1
+        breakloop=checkbreak(cell,orientation,Nvisits)
+    contour,contoursearch=gccu.clean(contourcells,searchcells,latitudes=latitudes,longitudes=longitudes,closecontour=closecontour,remcontourrepeat=remcontourrepeat,remsearchrepeat=remsearchrepeat)
+    return contour,contoursearch
+
+def ISBF(mask,latitudes=None,longitudes=None,direction='cw',start='auto',stop='either',startvisits=4,remcontourrepeat=True,remsearchrepeat=False,closecontour=True):
+    """
+    Find the contour of a mask using the improved simple boundary
+    following algorithm
+
+    Parameters
+    ----------
+    mask : ndarray
+        2D MxN bool array where M=len(`latitudes`) and
+        N=len(`longitudes`)
+    latitudes : ndarray, optional
+        1D Nx1 array of latitude points (degrees)
+    longitudes : ndarray, optional
+        1D Nx1 array of longitude points (degrees)
+    direction : {'cw', 'ccw'}, default='cw'
+        select the direction of contour tracing
+    start : {'auto', array_like}, default='auto' 
+        either a selection for automatic start cell assignment or a
+        manual assignment via a 2x2 array describing the start cell and
+        orientation
+
+            row 1: indices of the start cell
+                e.g. for start cell [2,3] second row (lat) and third
+                column (lon)
+            row 2: the start orientation
+                e.g. orientation [0,1] points right, [1,0] points down
+    stop : {'Elisoff', 'Nvisits', 'either'}, default='either'
+        selector for the stopping criterion
+
+            ``Elisoff``
+                stops when the start cell has been re-visited with the
+                same orientation as started with
+            ``Nvisits``
+                stops when the start cell has been re-visited N number
+                of times (N set by `startvisits` parameter)
+            ``either``
+                stops when either Elisoff or Nvisits has been satisfied
+    startvisits : int, default=3
+        the number of times re-visiting the start cell will trigger an
+        end to the search
+    checkconn : bool, default=False
+        select whether to check connectivity and warn the user of
+        potential issues, default=False
+    remcontourrepeat : bool, default=True
+        select whether to remove consecutive repeating cells in the
+        output `contour`
+    remsearchrepeat : bool, default=False
+        select whether to remove consecutive repeating cells in the
+        output `contoursearch`
+    closecontour : bool, default=True
+        select whether to close the output `contour` (first cell = last
+        cell)
+
+    Returns
+    -------
+    contour : ndarray
+        2D Nx2 array of ordered latitude/longitude points (degrees)
+        describing the edge of a mask
+    contoursearch : ndarray
+        2D Nx2 array of ordered latitude/longitude points (degrees)
+        describing the cells searched during contour tracing
+    
+    See Also
+    --------
+    geocontour.contourutil.findstart
+    geocontour.contourutil.setstop
+    square
+    moore
+    moore_imp
+    pavlidis
+    pavlidis_imp
+    MSBF
+    TSR
+
+    Notes
+    -----
+    - If `latitudes`/`longitudes` not provided, returned
+      `contour`/`contoursearch` will be indices of the input mask
+    - `startvisits` parameter will only be utilized when `stop`
+      parameter is set to 'Nvisits' or 'either'
+
+    References
+    ----------
+    Cheong, C.-H., & Han, T.-D. (2006). Improved Simple Boundary
+    Following Algorithm. Journal of KIISE: Software and Applications,
+    33(4), 427–439.
+    <https://koreascience.kr/article/JAKO200622219415761.pdf>
+
+    Cheong, C.-H., Seo, J., & Han, T.-D. (2006). Advanced Contour
+    Tracing Algorithms based on Analysis of Tracing Conditions.
+    Proceedings of the 33rd KISS Fall Conference, 33, 431–436.
+    <https://koreascience.kr/article/CFKO200614539217302.pdf>
+
+    Seo, J., Chae, S., Shim, J., Kim, D., Cheong, C., & Han, T.-D.
+    (2016). Fast Contour-Tracing Algorithm Based on a Pixel-Following
+    Method for Image Sensors. Sensors, 16(3), 353.
+    <https://doi.org/10.3390/s16030353>
+    """
+    if latitudes is not None and longitudes is not None:
+        gcc.cmask(mask,latitudes,longitudes)
+    else:
+        gcc.cmask(mask)
+    buffermask=np.full((tuple(np.array(mask.shape)+2)),False)
+    buffermask[1:-1,1:-1]=mask
+    if direction=='cw':
+        def outsideturn(orientation):
+            return orientation[::-1]*np.array([-1,1])
+        def insideturn(orientation):
+            return orientation[::-1]*np.array([1,-1])
+        searchdir='ru'
+    elif direction=='ccw':
+        def outsideturn(orientation):
+            return orientation[::-1]*np.array([1,-1])
+        def insideturn(orientation):
+            return orientation[::-1]*np.array([-1,1])
+        searchdir='rd'
+    else:
+        sys.exit('ERROR - direction=\''+direction+'\' is not a valid selection, valid selections are \'cw\'/\'ccw\'')
+    if type(start) is not str:
+        startcell,startorientation=gccu.parsestart(start,buffermask)
+    elif start=='auto':
+        startcell,startorientation=gccu.findstart(buffermask,searchdir=searchdir)
+    else:
+        sys.exit('ERROR - start=\''+start+'\' is not a valid selection, valid selections are \'auto\' or a 2x2 array describing start cell index and start orientation')
+    checkbreak=gccu.setstop(stop,startvisits,startcell,startorientation)
+    orientation=startorientation
+    cell=startcell
+    searchcells=[]
+    contourcells=[]
+    searchcells.append(cell)
+    contourcells.append(cell)
+    Nvisits=0
+    breakloop=False
+    #following 2006 paper/conf (2016 paper missing tag component - goes into infinite loop on case 4b)
+    tag=False
+    while not breakloop:
+        O=cell+outsideturn(orientation)
+        if buffermask[O[0],O[1]]==True: #Case A
+            searchcells.append(O)
+            contourcells.append(O)
+            cell=O
+            orientation=outsideturn(orientation)
+            tag=False
+        else:
+            R=cell-orientation
+            RO=O-orientation
+            if buffermask[RO[0],RO[1]]==True and buffermask[R[0],R[1]]==False and tag==False: #Case B
+                searchcells.append(O)
+                searchcells.append(R)
+                searchcells.append(RO)
+                contourcells.append(RO)
+                cell=RO
+                orientation=-orientation
+                tag=True
+            else:
+                searchcells.append(RO)
+                searchcells.append(O)
+                F=cell+orientation
+                FO=O+orientation
+                if buffermask[FO[0],FO[1]]==True:
+                    searchcells.append(F)
+                    searchcells.append(FO)
+                    if buffermask[F[0],F[1]]==True: #Case D
+                        contourcells.append(F)
+                        contourcells.append(FO)
+                    else: #Case C
+                        contourcells.append(FO)
+                    cell=FO
+                elif buffermask[F[0],F[1]]==True: #Case E
+                    searchcells.append(FO)
+                    searchcells.append(F)
+                    contourcells.append(F)
+                    cell=F
+                    orientation=insideturn(orientation)
+                else: #Case F
+                    searchcells.append(FO)
+                    searchcells.append(F)
+                    searchcells.append(cell)
+                    orientation=-orientation
+                tag=False
+        if (cell==startcell).all():
+            Nvisits+=1
+        breakloop=checkbreak(cell,orientation,Nvisits)
+    contour,contoursearch=gccu.clean(contourcells,searchcells,latitudes=latitudes,longitudes=longitudes,closecontour=closecontour,remcontourrepeat=remcontourrepeat,remsearchrepeat=remsearchrepeat)
+    return contour,contoursearch
+
 def TSR(mask,latitudes=None,longitudes=None,direction='cw',start='auto',stop='either',startvisits=4,remcontourrepeat=True,remsearchrepeat=False,closecontour=True):
     """
     Find the contour of a mask using the two-step representative tracing
     algorithm
 
     Parameters
     ----------
@@ -857,14 +1226,16 @@
     geocontour.contourutil.findstart
     geocontour.contourutil.setstop
     square
     moore
     moore_imp
     pavlidis
     pavlidis_imp
+    MSBF
+    ISBF
 
     Notes
     -----
     - If `latitudes`/`longitudes` not provided, returned
       `contour`/`contoursearch` will be indices of the input mask
     - `startvisits` parameter will only be utilized when `stop`
       parameter is set to 'Nvisits' or 'either'
@@ -908,50 +1279,50 @@
     searchcells=[]
     contourcells=[]
     searchcells.append(cell)
     contourcells.append(cell)
     Nvisits=0
     breakloop=False
     while not breakloop:
-        L=cell+outsideturn(orientation)
-        RL=cell-orientation+outsideturn(orientation)
+        O=cell+outsideturn(orientation)
+        RO=O-orientation
         #Stage 1
-        if buffermask[RL[0],RL[1]]==True:
-            searchcells.append(L)
-            searchcells.append(RL)
-            if buffermask[L[0],L[1]]==True: #Case 1
-                contourcells.append(L)
-                contourcells.append(RL)
+        if buffermask[RO[0],RO[1]]==True:
+            searchcells.append(O)
+            searchcells.append(RO)
+            if buffermask[O[0],O[1]]==True: #Case 1
+                contourcells.append(O)
+                contourcells.append(RO)
             else: #Case 2
-                contourcells.append(RL)
-            cell=RL
+                contourcells.append(RO)
+            cell=RO
             orientation=-orientation
         else:
-            searchcells.append(RL)
-            searchcells.append(L)
-            if buffermask[L[0],L[1]]==True: #Case 3
-                contourcells.append(L)
-                cell=L
+            searchcells.append(RO)
+            searchcells.append(O)
+            if buffermask[O[0],O[1]]==True: #Case 3
+                contourcells.append(O)
+                cell=O
                 orientation=outsideturn(orientation)
             else: #Case 4
                 pass
         #Stage 2
         F=cell+orientation
-        FL=cell+orientation+outsideturn(orientation)
-        if buffermask[FL[0],FL[1]]==True:
+        FO=F+outsideturn(orientation)
+        if buffermask[FO[0],FO[1]]==True:
             searchcells.append(F)
-            searchcells.append(FL)
+            searchcells.append(FO)
             if buffermask[F[0],F[1]]==True: #Case 6
                 contourcells.append(F)
-                contourcells.append(FL)
+                contourcells.append(FO)
             else: #Case 5
-                contourcells.append(FL)
-            cell=FL
+                contourcells.append(FO)
+            cell=FO
         else:
-            searchcells.append(FL)
+            searchcells.append(FO)
             searchcells.append(F)
             if buffermask[F[0],F[1]]==True: #Case 7
                 contourcells.append(F)
                 cell=F
                 orientation=insideturn(orientation)
             else: #Case 8
                 orientation=-orientation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geocontour-1.2.2/geocontour/contourutil.py` & `geocontour-1.3.0/geocontour/contourutil.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/geocontour/data/MissBasin_boundary.npz` & `geocontour-1.3.0/geocontour/data/MissBasin_boundary.npz`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/geocontour/data/generic_boundary.npz` & `geocontour-1.3.0/geocontour/data/generic_boundary.npz`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/geocontour/examples/__init__.py` & `geocontour-1.3.0/geocontour/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/geocontour/geocontour.py` & `geocontour-1.3.0/geocontour/geocontour.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/geocontour/grid.py` & `geocontour-1.3.0/geocontour/grid.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/geocontour/masksearch.py` & `geocontour-1.3.0/geocontour/masksearch.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/geocontour/maskutil.py` & `geocontour-1.3.0/geocontour/maskutil.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/geocontour/output.py` & `geocontour-1.3.0/geocontour/output.py`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/geocontour/tests/__init__.py` & `geocontour-1.3.0/geocontour/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,22 @@
     contour,contoursearch=gc.contourtrace.pavlidis(mask,latitudes=latitudes,longitudes=longitudes)
     print('contour:')
     print(contour)
     print('\n\nTest geocontour.contourtrace.pavlidis_imp()\n')
     contour,contoursearch=gc.contourtrace.pavlidis_imp(mask,latitudes=latitudes,longitudes=longitudes)
     print('contour:')
     print(contour)
+    print('\n\nTest geocontour.contourtrace.MSBF()\n')
+    contour,contoursearch=gc.contourtrace.MSBF(mask,latitudes=latitudes,longitudes=longitudes)
+    print('contour:')
+    print(contour)
+    print('\n\nTest geocontour.contourtrace.ISBF()\n')
+    contour,contoursearch=gc.contourtrace.ISBF(mask,latitudes=latitudes,longitudes=longitudes)
+    print('contour:')
+    print(contour)
     print('\n\nTest geocontour.contourtrace.TSR()\n')
     contour,contoursearch=gc.contourtrace.TSR(mask,latitudes=latitudes,longitudes=longitudes)
     print('contour:')
     print(contour)
     #Test Geocontour Funcs
     print('\n\n***TEST GEOCONTOUR FUNCS***\n')
     print('\n\nTest geocontour.build()\n')
```

### Comparing `geocontour-1.2.2/geocontour/tests/timing.py` & `geocontour-1.3.0/geocontour/tests/timing.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,30 +178,34 @@
         select to plot results
     logax : bool, default=False
         select to use log axes (if plotting)
 
     Returns
     -------
     results : ndarray
-        2D Nx7 array of timing results in units of seconds where N is
+        2D Nx9 array of timing results in units of seconds where N is
         equal to len(`spacing`)
  
             column1: number of cells in mask
 
             column2: square() timing
 
             column3: moore() timing
 
             column4: moore_imp() timing
 
             column5: pavlidis() timing
 
             column6: pavlidis_imp() timing
 
-            column7: TSR() timing
+            column7: MSBF() timing
+
+            column8: ISBF() timing
+
+            column9: TSR() timing
 
     See Also
     --------
     masksearch
     geocontour.contourtrace
 
     Notes
@@ -244,60 +248,76 @@
         moore_imptimes=TM.repeat(numtests,runspertest)
         pavlidisfunc=(lambda: gcct.pavlidis(mask,lats,lons))
         TM=tm.Timer(pavlidisfunc)
         pavlidistimes=TM.repeat(numtests,runspertest)
         pavlidis_impfunc=(lambda: gcct.pavlidis_imp(mask,lats,lons))
         TM=tm.Timer(pavlidis_impfunc)
         pavlidis_imptimes=TM.repeat(numtests,runspertest)
+        MSBFfunc=(lambda: gcct.MSBF(mask,lats,lons))
+        TM=tm.Timer(MSBFfunc)
+        MSBFtimes=TM.repeat(numtests,runspertest)
+        ISBFfunc=(lambda: gcct.ISBF(mask,lats,lons))
+        TM=tm.Timer(ISBFfunc)
+        ISBFtimes=TM.repeat(numtests,runspertest)
         TSRfunc=(lambda: gcct.TSR(mask,lats,lons))
         TM=tm.Timer(TSRfunc)
         TSRtimes=TM.repeat(numtests,runspertest)
         if stat=='mean':
             squaretime=np.mean(squaretimes)
             mooretime=np.mean(mooretimes)
             moore_imptime=np.mean(moore_imptimes)
             pavlidistime=np.mean(pavlidistimes)
             pavlidis_imptime=np.mean(pavlidis_imptimes)
+            MSBFtime=np.mean(MSBFtimes)
+            ISBFtime=np.mean(ISBFtimes)
             TSRtime=np.mean(TSRtimes)
         elif stat=='median':
             squaretime=np.median(squaretimes)
             mooretime=np.median(mooretimes)
             moore_imptime=np.median(moore_imptimes)
             pavlidistime=np.median(pavlidistimes)
             pavlidis_imptime=np.median(pavlidis_imptimes)
+            MSBFtime=np.median(MSBFtimes)
+            ISBFtime=np.median(ISBFtimes)
             TSRtime=np.median(TSRtimes)
         elif stat=='min':
             squaretime=np.min(squaretimes)
             mooretime=np.min(mooretimes)
             moore_imptime=np.min(moore_imptimes)
             pavlidistime=np.min(pavlidistimes)
             pavlidis_imptime=np.min(pavlidis_imptimes)
+            MSBFtime=np.min(MSBFtimes)
+            ISBFtime=np.min(ISBFtimes)
             TSRtime=np.min(TSRtimes)
         elif stat=='max':
             squaretime=np.max(squaretimes)
             mooretime=np.max(mooretimes)
             moore_imptime=np.max(moore_imptimes)
             pavlidistime=np.max(pavlidistimes)
             pavlidis_imptime=np.max(pavlidis_imptimes)
+            MSBFtime=np.max(MSBFtimes)
+            ISBFtime=np.max(ISBFtimes)
             TSRtime=np.max(TSRtimes)
         else:
             sys.exit('ERROR - stat=\''+stat+'\' is not a valid selection, valid selections are \'mean\'/\'median\'/\'min\'/\'max\'')
-        output.append([numcells,squaretime,mooretime,moore_imptime,pavlidistime,pavlidis_imptime,TSRtime])
-        print('\n'+str(numcells)+' cells in mask:\n   '+stat+' square time: '+str(squaretime)+'\n   '+stat+' moore time: '+str(mooretime)+'\n   '+stat+' moore_imp time: '+str(moore_imptime)+'\n   '+stat+' pavlidis time: '+str(pavlidistime)+'\n   '+stat+' pavlidis_imp time: '+str(pavlidis_imptime)+'\n   '+stat+' TSR time: '+str(TSRtime))
+        output.append([numcells,squaretime,mooretime,moore_imptime,pavlidistime,pavlidis_imptime,MSBFtime,ISBFtime,TSRtime])
+        print('\n'+str(numcells)+' cells in mask:\n   '+stat+' square time: '+str(squaretime)+'\n   '+stat+' moore time: '+str(mooretime)+'\n   '+stat+' moore_imp time: '+str(moore_imptime)+'\n   '+stat+' pavlidis time: '+str(pavlidistime)+'\n   '+stat+' pavlidis_imp time: '+str(pavlidis_imptime)+'\n   '+stat+' MSBF time: '+str(MSBFtime)+'\n   '+stat+' ISBF time: '+str(ISBFtime)+'\n   '+stat+' TSR time: '+str(TSRtime))
     
     results=np.array(output)
     if plot==True:
         fig=plt.figure()
         ax=fig.add_subplot(1,1,1)
         ax.plot(results[:,0],results[:,1],label='square')
         ax.plot(results[:,0],results[:,2],label='moore')
         ax.plot(results[:,0],results[:,3],label='moore_imp')
         ax.plot(results[:,0],results[:,4],label='pavlidis')
         ax.plot(results[:,0],results[:,5],label='pavlidis_imp')
-        ax.plot(results[:,0],results[:,6],label='TSR')
+        ax.plot(results[:,0],results[:,6],label='MSBF')
+        ax.plot(results[:,0],results[:,7],label='ISBF')
+        ax.plot(results[:,0],results[:,8],label='TSR')
         ax.grid()
         if logax==True:
             ax.set_xscale('log')
             ax.set_yscale('log')
         ax.legend()
         ax.set_title('Contour Trace Times\n'+stat+' of '+str(numtests)+' tests of '+str(runspertest)+' calls each')
         ax.set_ylabel('time (s)')
```

### Comparing `geocontour-1.2.2/geocontour.egg-info/PKG-INFO` & `geocontour-1.3.0/geocontour.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocontour
-Version: 1.2.2
+Version: 1.3.0
 Summary: Utilities for masking, contour tracing, and geocontour construction with gridded geographic data
 Home-page: https://github.com/benkrichman/geocontour
 Author: Benjamin Krichman
 Author-email: benkrichman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -48,28 +48,28 @@
 
 Find the full documentation hosted [here](https://geocontour.readthedocs.io/en/latest/index.html).
 
 ## Citation
 
 If geocontour played a significant role in your work and you would like to cite it, the following is suggested (APA):
 
-Krichman, B. (2023). *geocontour* (Version 1.2.2) [Computer Software]. https://doi.org/10.5281/zenodo.7757447
+Krichman, B. (2023). *geocontour* (Version 1.3.0) [Computer Software]. https://doi.org/10.5281/zenodo.7402714
 
 Bibtex:
 
 ```latex
 @software{geocontour,
 author={Krichman, Benjamin},
-doi={10.5281/zenodo.7757447},
+doi={10.5281/zenodo.7402714},
 license={MIT},
-month={3},
+month={5},
 year={2023},
 title={{geocontour}},
 url={https://github.com/benkrichman/geocontour},
-version={1.2.2},
+version={1.3.0},
 note = {Computer Software}
 }
 ```
 
 ## Features
 
 ### Masks
@@ -82,21 +82,23 @@
 Useful mask operators
 - return mask connectivity (and null connectivity)
 - return mask edge cells
 - return mask vertex points
 
 ### Contours
 
-Implements 4 existing algorithms for contour tracing, and two improvements on known algorithms
-- square tracing [^1][^2]
-- moore neighbor tracing [^1][^2]
+Implements 6 existing algorithms for contour tracing, and two improvements on known algorithms
+- square tracing (a.k.a. simple boundary follower/Papert's turtle algorithm) [^3][^4][^5][^7][^8]
+- moore neighbor tracing [^3][^8]
 - improved moore neighbor tracing (capturing inside corners)
-- pavlidis tracing [^1][^3]
+- pavlidis tracing [^3][^6]
 - improved pavlidis tracing (capturing inside corners)
-- fast representative tracing [^4]
+- modified simple boundary follower [^1][^2][^4]
+- improved simple boundary follower [^1][^2][^7]
+- fast representative tracing [^7]
 
 Tuning of contours created from tracing input masks
 - trace direction
 - selectable and adjustable stopping conditions
 - automatic or manual selection of starting cell
 - selectable connection type (cell to cell or cell edge to cell center)
 - simplification of output contour (removal of repeating cells)
@@ -200,14 +202,24 @@
 
 ```python
 geocontour.output.plot(latitudes,longitudes,geocontour=geocontour,title='Example Geocontour\nMississippi River Basin',outname='example_large_geocontour+bordfeat',features='borders')
 ```
 
 <img src=https://github.com/benkrichman/geocontour/raw/main/images/example_large_geocontour%2Bbordfeat.png width="800">
 
-[^1]: Ghuneim, A.G. (2000). *Contour Tracing*. McGill University. <https://www.imageprocessingplace.com/downloads_V3/root_downloads/tutorials/contour_tracing_Abeer_George_Ghuneim/alg.html>
+[^1]: Cheong, C.-H., & Han, T.-D. (2006). Improved Simple Boundary Following Algorithm. Journal of KIISE: Software and Applications, 33(4), 427–439. <https://koreascience.kr/article/JAKO200622219415761.pdf>
 
-[^2]: Toussaint, G.T. (2010). *Grids Connectivity and Contour Tracing* [Lesson Notes]. McGill University. <http://www-cgrl.cs.mcgill.ca/~godfried/teaching/mir-reading-assignments/Chapter-2-Grids-Connectivity-Contour-Tracing.pdf>
+[^2]: Cheong, C.-H., Seo, J., & Han, T.-D. (2006). Advanced Contour Tracing Algorithms based on Analysis of Tracing Conditions. Proceedings of the 33rd KISS Fall Conference, 33, 431–436. <https://koreascience.kr/article/CFKO200614539217302.pdf>
+
+[^3]: Ghuneim, A.G. (2000). *Contour Tracing*. McGill University. <https://www.imageprocessingplace.com/downloads_V3/root_downloads/tutorials/contour_tracing_Abeer_George_Ghuneim/alg.html>
+
+[^4]: Gose, E., Johnsonbaugh, R., & Jost, S. (1996). Pattern recognition and image analysis. Prentice Hall PTR.
+
+[^5]: Papert, S. (1973). Uses of Technology to Enhance Education (No. 298; Artificial Intelligence). Massachusetts Institute of Technology. <https://dspace.mit.edu/handle/1721.1/6213>
+
+[^6]: Pavlidis, T. (1982) Algorithms for Graphics and Image Processing. Computer Science Press, New York, NY. <https://doi.org/10.1007/978-3-642-93208-3>
+
+[^7]: Seo, J., Chae, S., Shim, J., Kim, D., Cheong, C., & Han, T.-D. (2016). Fast Contour-Tracing Algorithm Based on a Pixel-Following Method for Image Sensors. Sensors, 16(3), 353. <https://doi.org/10.3390/s16030353>
+
+[^8]: Toussaint, G.T. (2010). *Grids Connectivity and Contour Tracing* [Lesson Notes]. McGill University. <http://www-cgrl.cs.mcgill.ca/~godfried/teaching/mir-reading-assignments/Chapter-2-Grids-Connectivity-Contour-Tracing.pdf>
 
-[^3]: Pavlidis, T. (1982) Algorithms for Graphics and Image Processing. Computer Science Press, New York, NY. <https://doi.org/10.1007/978-3-642-93208-3>
 
-[^4]: Seo, J., Chae, S., Shim, J., Kim, D., Cheong, C., & Han, T.-D. (2016). Fast Contour-Tracing Algorithm Based on a Pixel-Following Method for Image Sensors. Sensors, 16(3), 353. <https://doi.org/10.3390/s16030353>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geocontour-1.2.2/geocontour.egg-info/SOURCES.txt` & `geocontour-1.3.0/geocontour.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/images/example_large_boundary+mask.png` & `geocontour-1.3.0/images/example_large_boundary+mask.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/images/example_large_contour.png` & `geocontour-1.3.0/images/example_large_contour.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/images/example_large_contoursearch.png` & `geocontour-1.3.0/images/example_large_contoursearch.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/images/example_large_geocontour+bordfeat.png` & `geocontour-1.3.0/images/example_large_geocontour+bordfeat.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/images/example_large_geocontour+natfeat.png` & `geocontour-1.3.0/images/example_large_geocontour+natfeat.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/images/example_large_geocontour.png` & `geocontour-1.3.0/images/example_large_geocontour.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/images/example_small_boundary+mask.png` & `geocontour-1.3.0/images/example_small_boundary+mask.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/images/example_small_contour.png` & `geocontour-1.3.0/images/example_small_contour.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/images/example_small_contoursearch.png` & `geocontour-1.3.0/images/example_small_contoursearch.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/images/example_small_geocontour.png` & `geocontour-1.3.0/images/example_small_geocontour.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/images/example_small_geocontour_simp.png` & `geocontour-1.3.0/images/example_small_geocontour_simp.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/images/icon_geocontour.png` & `geocontour-1.3.0/images/icon_geocontour.png`

 * *Files identical despite different names*

### Comparing `geocontour-1.2.2/setup.py` & `geocontour-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools as st
 
 with open('README.md','r') as ldf:
     longdesc=ldf.read()
 
 st.setup(
     name='geocontour',
-    version='1.2.2',
+    version='1.3.0',
     license='MIT',
     url='https://github.com/benkrichman/geocontour',
     description='Utilities for masking, contour tracing, and geocontour construction with gridded geographic data',
     long_description=longdesc,
     long_description_content_type="text/markdown",
     author='Benjamin Krichman',
     author_email='benkrichman@gmail.com',
```

