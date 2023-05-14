# Comparing `tmp/impetuous-gfa-0.97.8.tar.gz` & `tmp/impetuous-gfa-0.97.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impetuous-gfa-0.97.8.tar", last modified: Tue Dec 13 07:55:36 2022, max compression
+gzip compressed data, was "impetuous-gfa-0.97.9.tar", last modified: Tue Dec 13 07:59:12 2022, max compression
```

## Comparing `impetuous-gfa-0.97.8.tar` & `impetuous-gfa-0.97.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 rictjo    (1000) users      (998)        0 2022-12-13 07:55:36.802134 impetuous-gfa-0.97.8/
--rwxr-xr-x   0 rictjo    (1000) users      (998)    11357 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.8/LICENSE
--rw-r--r--   0 rictjo    (1000) users      (998)    60055 2022-12-13 07:55:36.802134 impetuous-gfa-0.97.8/PKG-INFO
--rwxr-xr-x   0 rictjo    (1000) users      (998)    59297 2022-11-23 20:37:51.000000 impetuous-gfa-0.97.8/README.md
-drwxr-xr-x   0 rictjo    (1000) users      (998)        0 2022-12-13 07:55:36.801134 impetuous-gfa-0.97.8/impetuous_gfa.egg-info/
--rw-r--r--   0 rictjo    (1000) users      (998)    60055 2022-12-13 07:55:36.000000 impetuous-gfa-0.97.8/impetuous_gfa.egg-info/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (998)      557 2022-12-13 07:55:36.000000 impetuous-gfa-0.97.8/impetuous_gfa.egg-info/SOURCES.txt
--rw-r--r--   0 rictjo    (1000) users      (998)        1 2022-12-13 07:55:36.000000 impetuous-gfa-0.97.8/impetuous_gfa.egg-info/dependency_links.txt
--rw-r--r--   0 rictjo    (1000) users      (998)       10 2022-12-13 07:55:36.000000 impetuous-gfa-0.97.8/impetuous_gfa.egg-info/top_level.txt
--rw-r--r--   0 rictjo    (1000) users      (998)       38 2022-12-13 07:55:36.802134 impetuous-gfa-0.97.8/setup.cfg
--rwxr-xr-x   0 rictjo    (1000) users      (998)     1314 2022-12-13 07:54:55.000000 impetuous-gfa-0.97.8/setup.py
-drwxr-xr-x   0 rictjo    (1000) users      (998)        0 2022-12-13 07:55:36.800134 impetuous-gfa-0.97.8/src/
-drwxr-xr-x   0 rictjo    (1000) users      (998)        0 2022-12-13 07:55:36.802134 impetuous-gfa-0.97.8/src/impetuous/
--rwxr-xr-x   0 rictjo    (1000) users      (998)       23 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.8/src/impetuous/__init__.py
--rwxr-xr-x   0 rictjo    (1000) users      (998)    61921 2022-12-13 07:54:55.000000 impetuous-gfa-0.97.8/src/impetuous/clustering.py
--rwxr-xr-x   0 rictjo    (1000) users      (998)    44696 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.8/src/impetuous/convert.py
--rw-r--r--   0 rictjo    (1000) users      (998)    28361 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.8/src/impetuous/fit.py
--rwxr-xr-x   0 rictjo    (1000) users      (998)    26782 2022-11-23 21:36:58.000000 impetuous-gfa-0.97.8/src/impetuous/hierarchical.py
--rwxr-xr-x   0 rictjo    (1000) users      (998)      811 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.8/src/impetuous/impetuous.py
--rw-r--r--   0 rictjo    (1000) users      (998)     8333 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.8/src/impetuous/optimisation.py
--rwxr-xr-x   0 rictjo    (1000) users      (998)    18762 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.8/src/impetuous/pathways.py
--rw-r--r--   0 rictjo    (1000) users      (998)     4708 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.8/src/impetuous/probabilistic.py
--rwxr-xr-x   0 rictjo    (1000) users      (998)    95482 2022-12-06 20:16:03.000000 impetuous-gfa-0.97.8/src/impetuous/quantification.py
--rw-r--r--   0 rictjo    (1000) users      (998)    20803 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.8/src/impetuous/reducer.py
--rw-r--r--   0 rictjo    (1000) users      (998)     9011 2022-12-06 20:16:03.000000 impetuous-gfa-0.97.8/src/impetuous/special.py
--rw-r--r--   0 rictjo    (1000) users      (998)     2344 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.8/src/impetuous/spectral.py
--rw-r--r--   0 rictjo    (1000) users      (998)    83710 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.8/src/impetuous/visualisation.py
+drwxr-xr-x   0 rictjo    (1000) users      (998)        0 2022-12-13 07:59:12.533063 impetuous-gfa-0.97.9/
+-rwxr-xr-x   0 rictjo    (1000) users      (998)    11357 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.9/LICENSE
+-rw-r--r--   0 rictjo    (1000) users      (998)    60055 2022-12-13 07:59:12.533063 impetuous-gfa-0.97.9/PKG-INFO
+-rwxr-xr-x   0 rictjo    (1000) users      (998)    59297 2022-11-23 20:37:51.000000 impetuous-gfa-0.97.9/README.md
+drwxr-xr-x   0 rictjo    (1000) users      (998)        0 2022-12-13 07:59:12.532063 impetuous-gfa-0.97.9/impetuous_gfa.egg-info/
+-rw-r--r--   0 rictjo    (1000) users      (998)    60055 2022-12-13 07:59:12.000000 impetuous-gfa-0.97.9/impetuous_gfa.egg-info/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (998)      557 2022-12-13 07:59:12.000000 impetuous-gfa-0.97.9/impetuous_gfa.egg-info/SOURCES.txt
+-rw-r--r--   0 rictjo    (1000) users      (998)        1 2022-12-13 07:59:12.000000 impetuous-gfa-0.97.9/impetuous_gfa.egg-info/dependency_links.txt
+-rw-r--r--   0 rictjo    (1000) users      (998)       10 2022-12-13 07:59:12.000000 impetuous-gfa-0.97.9/impetuous_gfa.egg-info/top_level.txt
+-rw-r--r--   0 rictjo    (1000) users      (998)       38 2022-12-13 07:59:12.533063 impetuous-gfa-0.97.9/setup.cfg
+-rwxr-xr-x   0 rictjo    (1000) users      (998)     1314 2022-12-13 07:59:04.000000 impetuous-gfa-0.97.9/setup.py
+drwxr-xr-x   0 rictjo    (1000) users      (998)        0 2022-12-13 07:59:12.531063 impetuous-gfa-0.97.9/src/
+drwxr-xr-x   0 rictjo    (1000) users      (998)        0 2022-12-13 07:59:12.533063 impetuous-gfa-0.97.9/src/impetuous/
+-rwxr-xr-x   0 rictjo    (1000) users      (998)       23 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.9/src/impetuous/__init__.py
+-rwxr-xr-x   0 rictjo    (1000) users      (998)    61923 2022-12-13 07:59:04.000000 impetuous-gfa-0.97.9/src/impetuous/clustering.py
+-rwxr-xr-x   0 rictjo    (1000) users      (998)    44696 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.9/src/impetuous/convert.py
+-rw-r--r--   0 rictjo    (1000) users      (998)    28361 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.9/src/impetuous/fit.py
+-rwxr-xr-x   0 rictjo    (1000) users      (998)    26782 2022-11-23 21:36:58.000000 impetuous-gfa-0.97.9/src/impetuous/hierarchical.py
+-rwxr-xr-x   0 rictjo    (1000) users      (998)      811 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.9/src/impetuous/impetuous.py
+-rw-r--r--   0 rictjo    (1000) users      (998)     8333 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.9/src/impetuous/optimisation.py
+-rwxr-xr-x   0 rictjo    (1000) users      (998)    18762 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.9/src/impetuous/pathways.py
+-rw-r--r--   0 rictjo    (1000) users      (998)     4708 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.9/src/impetuous/probabilistic.py
+-rwxr-xr-x   0 rictjo    (1000) users      (998)    95482 2022-12-06 20:16:03.000000 impetuous-gfa-0.97.9/src/impetuous/quantification.py
+-rw-r--r--   0 rictjo    (1000) users      (998)    20803 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.9/src/impetuous/reducer.py
+-rw-r--r--   0 rictjo    (1000) users      (998)     9011 2022-12-06 20:16:03.000000 impetuous-gfa-0.97.9/src/impetuous/special.py
+-rw-r--r--   0 rictjo    (1000) users      (998)     2344 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.9/src/impetuous/spectral.py
+-rw-r--r--   0 rictjo    (1000) users      (998)    83710 2022-10-16 07:47:16.000000 impetuous-gfa-0.97.9/src/impetuous/visualisation.py
```

### Comparing `impetuous-gfa-0.97.8/LICENSE` & `impetuous-gfa-0.97.9/LICENSE`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/PKG-INFO` & `impetuous-gfa-0.97.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impetuous-gfa
-Version: 0.97.8
+Version: 0.97.9
 Summary: Impetuous Quantification, a Statistical Learning library for Humans : Alignments, Clustering, Fast NodeGraph Searching, Enrichments and Group Analysis
 Home-page: https://github.com/richardtjornhammar/impetuous
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `impetuous-gfa-0.97.8/README.md` & `impetuous-gfa-0.97.9/README.md`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/impetuous_gfa.egg-info/PKG-INFO` & `impetuous-gfa-0.97.9/impetuous_gfa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impetuous-gfa
-Version: 0.97.8
+Version: 0.97.9
 Summary: Impetuous Quantification, a Statistical Learning library for Humans : Alignments, Clustering, Fast NodeGraph Searching, Enrichments and Group Analysis
 Home-page: https://github.com/richardtjornhammar/impetuous
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `impetuous-gfa-0.97.8/impetuous_gfa.egg-info/SOURCES.txt` & `impetuous-gfa-0.97.9/impetuous_gfa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/setup.py` & `impetuous-gfa-0.97.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "impetuous-gfa",
-    version = "0.97.8",
+    version = "0.97.9",
     author = "Richard Tjörnhammar",
     author_email = "richard.tjornhammar@gmail.com",
     description = "Impetuous Quantification, a Statistical Learning library for Humans : Alignments, Clustering, Fast NodeGraph Searching, Enrichments and Group Analysis",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/richardtjornhammar/impetuous",
     packages = setuptools.find_packages('src'),
```

### Comparing `impetuous-gfa-0.97.8/src/impetuous/clustering.py` & `impetuous-gfa-0.97.9/src/impetuous/clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1220,15 +1220,15 @@
         g2 = g1
     if len(g1) == 0 :
         g1 = g2
     #
     pS		= np.sum( allPairs(distm,g1,g1) )
     qS		= np.sum( allPairs(distm,g2,g2) )
     pqS		= np.sum( allPairs(distm,g1,g2) )
-    FS          = np.sum( allPairs(distm,*[g1,g2],*[g1,g2]) )
+    FS          = np.sum( allPairs(distm,[*g1,*g2],[*g1,*g2]) )
     p1122	= 1/len(g1)**2 * pS + 1/len(g2)**2 * qS
     p1212	= 2*1/len(g1) * 1/len(g2) * pqS # p2121 = p1212
     score	= p1212 - p1122
     norm_scores = np.array([pS,qS,pqS])/FS
     norm_scores = np.append(norm_scores, norm_scores[0] + norm_scores[1] - norm_scores[2] )
     #
     #	"QUADRATURE"	"TORQUE"	"NORMED DIFF"
```

### Comparing `impetuous-gfa-0.97.8/src/impetuous/convert.py` & `impetuous-gfa-0.97.9/src/impetuous/convert.py`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/src/impetuous/fit.py` & `impetuous-gfa-0.97.9/src/impetuous/fit.py`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/src/impetuous/hierarchical.py` & `impetuous-gfa-0.97.9/src/impetuous/hierarchical.py`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/src/impetuous/impetuous.py` & `impetuous-gfa-0.97.9/src/impetuous/impetuous.py`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/src/impetuous/optimisation.py` & `impetuous-gfa-0.97.9/src/impetuous/optimisation.py`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/src/impetuous/pathways.py` & `impetuous-gfa-0.97.9/src/impetuous/pathways.py`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/src/impetuous/probabilistic.py` & `impetuous-gfa-0.97.9/src/impetuous/probabilistic.py`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/src/impetuous/quantification.py` & `impetuous-gfa-0.97.9/src/impetuous/quantification.py`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/src/impetuous/reducer.py` & `impetuous-gfa-0.97.9/src/impetuous/reducer.py`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/src/impetuous/special.py` & `impetuous-gfa-0.97.9/src/impetuous/special.py`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/src/impetuous/spectral.py` & `impetuous-gfa-0.97.9/src/impetuous/spectral.py`

 * *Files identical despite different names*

### Comparing `impetuous-gfa-0.97.8/src/impetuous/visualisation.py` & `impetuous-gfa-0.97.9/src/impetuous/visualisation.py`

 * *Files identical despite different names*

