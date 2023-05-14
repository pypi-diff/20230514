# Comparing `tmp/betby-0.2.5.tar.gz` & `tmp/betby-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betby-0.2.5.tar", last modified: Thu May 11 10:22:07 2023, max compression
+gzip compressed data, was "betby-0.2.6.tar", last modified: Sun May 14 17:12:11 2023, max compression
```

## Comparing `betby-0.2.5.tar` & `betby-0.2.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 10:22:07.713113 betby-0.2.5/
--rw-rw-rw-   0        0        0      539 2023-05-11 10:22:07.712116 betby-0.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 10:22:07.691713 betby-0.2.5/betby/
--rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.5/betby/__init__.py
--rw-rw-rw-   0        0        0     6253 2023-05-11 10:20:23.000000 betby-0.2.5/betby/markets.py
-drwxrwxrwx   0        0        0        0 2023-05-11 10:22:07.708126 betby-0.2.5/betby.egg-info/
--rw-rw-rw-   0        0        0      539 2023-05-11 10:22:05.000000 betby-0.2.5/betby.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-05-11 10:22:07.000000 betby-0.2.5/betby.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 10:22:05.000000 betby-0.2.5/betby.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 10:22:05.000000 betby-0.2.5/betby.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 10:22:07.714110 betby-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      637 2023-05-11 10:20:41.000000 betby-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:12:11.106006 betby-0.2.6/
+-rw-rw-rw-   0        0        0      539 2023-05-14 17:12:11.104007 betby-0.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-14 17:12:11.078008 betby-0.2.6/betby/
+-rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.6/betby/__init__.py
+-rw-rw-rw-   0        0        0     6864 2023-05-14 17:10:07.000000 betby-0.2.6/betby/markets.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:12:11.100007 betby-0.2.6/betby.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-05-14 17:12:08.000000 betby-0.2.6/betby.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-14 17:12:10.000000 betby-0.2.6/betby.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 17:12:08.000000 betby-0.2.6/betby.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-14 17:12:08.000000 betby-0.2.6/betby.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 17:12:11.107008 betby-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      637 2023-05-14 17:08:16.000000 betby-0.2.6/setup.py
```

### Comparing `betby-0.2.5/PKG-INFO` & `betby-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.5
+Version: 0.2.6
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.5/betby/markets.py` & `betby-0.2.6/betby/markets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import numpy as np
 from math import exp, factorial
 
+
 class Get_markets:
     def __init__(self, avg_1, avg_2, score_1=0, score_2=0, time=0,
                  time_full=93, time_block=90, matrix=None, poisson=False,
                  result=None):
         self.avg_1 = avg_1
         self.avg_2 = avg_2
         self.score_1 = score_1
         self.score_2 = score_2
         self.time = time
         self.time_full = time_full
         self.time_block = time_block
         self.matrix = matrix
         self.poisson = poisson
         self.result = {} if result is None else result
+        self.poi_1 = len(matrix[0]) if not poisson else None
 
     # округление кэфов
     def kf_round(self, a, max):
         if a < 3.5:
             a = np.floor(a * 100) / 100
         elif a < 10:
             a = np.floor(a * 10) / 10
@@ -55,90 +57,97 @@
         avg_1 = self.avg_1 * (self.time_full - self.time) / self.time_full
         avg_2 = self.avg_2 * (self.time_full - self.time) / self.time_full
         if self.poisson:
             self.matrix = np.zeros((self.poisson, self.poisson))
             for i in range(self.poisson):
                 for j in range(self.poisson):
                     prob = (exp(-avg_1) * avg_1 ** i / factorial(i)) * (
-                                exp(-avg_2) * avg_2 ** j / factorial(j))
+                            exp(-avg_2) * avg_2 ** j / factorial(j))
                     self.matrix[i, j] = prob
-            return self.matrix
+        return self.matrix
 
     def total(self, mar=0.05, min_prob=0.2, max_odds=25):
         prob = 0
         self.result.update({'TOTAL': {'outcomes': []}})
-        for val in range(2 * self.poisson):
-            for i in range(self.poisson):
-                for j in range(self.poisson):
+        for val in range(2 * self.poisson or 2 * self.poi_1):
+            for i in range(self.poisson or self.poi_1):
+                for j in range(self.poisson or self.poi_1):
                     if i + j < val + 0.5:
                         prob += self.matrix[i, j]
             if prob >= min_prob and prob <= 1 - min_prob:
                 self.result['TOTAL']['outcomes'].append({
-                    'spec_' + str(val + 0.5): str(val + 0.5),
+                    'spec_' + str(
+                        val + 0.5 + self.score_1 + self.score_2): str(
+                        val + 0.5 + self.score_1 + self.score_2),
                     'over': {'prob': 1 - prob, 'margin': mar,
                              'ODDS': self.margin(
                                  1 / (1 - prob), mar, max_odds),
                              'block': 0},
                     'under': {'prob': prob, 'margin': mar,
                               'ODDS': self.margin(1 / prob, mar, max_odds),
                               'block': 0}
                 })
             prob = 0
 
     def handicap(self, mar=0.05, min_prob=0.2, max_odds=25):
         prob = 0
         self.result.update({'HANDICAP': {'outcomes': []}})
-        for val in range(1 - self.poisson, self.poisson):
-            for i in range(self.poisson):
-                for j in range(self.poisson):
+        for val in range(1 - (self.poisson or self.poi_1),
+                         self.poisson or self.poi_1):
+            for i in range(self.poisson or self.poi_1):
+                for j in range(self.poisson or self.poi_1):
                     if j - i > val + 0.5:
                         prob += self.matrix[i, j]
             if prob >= min_prob and prob <= 1 - min_prob:
                 self.result['HANDICAP']['outcomes'].append({
-                    'spec_' + str(val + 0.5): str(val + 0.5),
+                    'spec_' + str(
+                        val + 0.5 - self.score_1 + self.score_2): str(
+                        val + 0.5 - self.score_1 + self.score_2),
                     'H1': {'prob': 1 - prob, 'margin': mar,
                            'ODDS': self.margin(1 / (1 - prob), mar, max_odds),
                            'block': 0},
                     'H2': {'prob': prob, 'margin': mar,
                            'ODDS': self.margin(1 / prob, mar, max_odds),
                            'block': 0}
                 })
             prob = 0
 
     def home_total(self, mar=0.05, min_prob=0.2, max_odds=25):
         prob = 0
         self.result.update({'HOME_TOTAL': {'outcomes': []}})
-        for val in range(self.poisson):
-            for i in range(self.poisson):
-                for j in range(self.poisson):
+        for val in range(self.poisson or self.poi_1):
+            for i in range(self.poisson or self.poi_1):
+                for j in range(self.poisson or self.poi_1):
                     if i < val + 0.5:
                         prob += self.matrix[i, j]
             if prob >= min_prob and prob <= 1 - min_prob:
                 self.result['HOME_TOTAL']['outcomes'].append({
-                    'spec_' + str(val + 0.5): str(val + 0.5),
+                    'spec_' + str(val + 0.5 + self.score_1): str(
+                        val + 0.5 + self.score_1),
                     'over': {'prob': 1 - prob, 'margin': mar, 'ODDS':
                         self.margin(
                             1 / (1 - prob), mar, max_odds), 'block': 0},
                     'under': {'prob': prob, 'margin': mar, 'ODDS': self.margin(
                         1 / prob, mar, max_odds), 'block': 0}
                 })
             prob = 0
 
     def away_total(self, mar=0.05, min_prob=0.2, max_odds=25):
         prob = 0
         self.result.update({'AWAY_TOTAL': {'outcomes': []}})
-        for val in range(self.poisson):
-            for i in range(self.poisson):
-                for j in range(self.poisson):
+        for val in range(self.poisson or self.poi_1):
+            for i in range(self.poisson or self.poi_1):
+                for j in range(self.poisson or self.poi_1):
                     if j < val + 0.5:
                         prob += self.matrix[i, j]
             if prob >= min_prob and prob <= 1 - min_prob:
                 self.result['AWAY_TOTAL']['outcomes'].append({
-                    'spec_' + str(val + 0.5): str(val + 0.5),
+                    'spec_' + str(val + 0.5 + self.score_2): str(
+                        val + 0.5 + self.score_2),
                     'over': {'prob': 1 - prob, 'margin': mar,
                              'ODDS': self.margin(1 / (1 - prob), mar,
-                                            max_odds), 'block': 0},
+                                                 max_odds), 'block': 0},
                     'under': {'prob': prob, 'margin': mar,
                               'ODDS': self.margin(1 / prob, mar, max_odds),
                               'block': 0}
                 })
             prob = 0
```

### Comparing `betby-0.2.5/betby.egg-info/PKG-INFO` & `betby-0.2.6/betby.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.5
+Version: 0.2.6
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.5/setup.py` & `betby-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="betby",
-    version="0.2.5",
+    version="0.2.6",
     author="Ayrat Badrutdinov",
     author_email="a.badrutdinov@betby.com",
     description="Betby libraries",
     packages=["betby"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

