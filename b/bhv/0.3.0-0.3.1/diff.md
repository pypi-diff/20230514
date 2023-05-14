# Comparing `tmp/bhv-0.3.0.tar.gz` & `tmp/bhv-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.3.0.tar", last modified: Fri May 12 19:31:57 2023, max compression
+gzip compressed data, was "bhv-0.3.1.tar", last modified: Sun May 14 01:05:28 2023, max compression
```

## Comparing `bhv-0.3.0.tar` & `bhv-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-12 19:31:57.589482 bhv-0.3.0/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.3.0/LICENSE
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1002 2023-05-12 19:31:57.589482 bhv-0.3.0/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3202 2023-04-29 09:52:26.000000 bhv-0.3.0/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-12 19:31:57.589482 bhv-0.3.0/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.3.0/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    12914 2023-05-12 19:21:11.000000 bhv-0.3.0/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.3.0/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11610 2023-05-10 11:54:44.000000 bhv-0.3.0/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.3.0/bhv/poibin.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.3.0/bhv/positions.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8226 2023-05-02 19:26:10.000000 bhv-0.3.0/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2769 2023-05-03 12:10:28.000000 bhv-0.3.0/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1152 2023-04-24 02:20:49.000000 bhv-0.3.0/bhv/slice.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    24158 2023-05-05 11:23:02.000000 bhv-0.3.0/bhv/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3503 2023-05-10 11:50:50.000000 bhv-0.3.0/bhv/vanilla.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.3.0/bhv/visualization.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-12 19:31:57.589482 bhv-0.3.0/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1002 2023-05-12 19:31:57.000000 bhv-0.3.0/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      344 2023-05-12 19:31:57.000000 bhv-0.3.0/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-12 19:31:57.000000 bhv-0.3.0/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       45 2023-05-12 19:31:57.000000 bhv-0.3.0/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-12 19:31:57.000000 bhv-0.3.0/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-12 19:31:57.589482 bhv-0.3.0/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1290 2023-05-12 19:25:11.000000 bhv-0.3.0/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-14 01:05:28.014141 bhv-0.3.1/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.3.1/LICENSE
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1002 2023-05-14 01:05:28.014141 bhv-0.3.1/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3607 2023-05-14 00:49:43.000000 bhv-0.3.1/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-14 01:05:28.014141 bhv-0.3.1/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.3.1/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    12914 2023-05-12 20:34:13.000000 bhv-0.3.1/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.3.1/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11610 2023-05-10 11:54:44.000000 bhv-0.3.1/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.3.1/bhv/poibin.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.3.1/bhv/positions.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8226 2023-05-02 19:26:10.000000 bhv-0.3.1/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2769 2023-05-03 12:10:28.000000 bhv-0.3.1/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1152 2023-04-24 02:20:49.000000 bhv-0.3.1/bhv/slice.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    24409 2023-05-13 22:37:13.000000 bhv-0.3.1/bhv/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3505 2023-05-14 00:55:07.000000 bhv-0.3.1/bhv/vanilla.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.3.1/bhv/visualization.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-14 01:05:28.014141 bhv-0.3.1/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1002 2023-05-14 01:05:28.000000 bhv-0.3.1/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      344 2023-05-14 01:05:28.000000 bhv-0.3.1/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-14 01:05:28.000000 bhv-0.3.1/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       45 2023-05-14 01:05:28.000000 bhv-0.3.1/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-14 01:05:28.000000 bhv-0.3.1/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-14 01:05:28.014141 bhv-0.3.1/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1290 2023-05-14 00:43:56.000000 bhv-0.3.1/setup.py
```

### Comparing `bhv-0.3.0/LICENSE` & `bhv-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.3.0/PKG-INFO` & `bhv-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.3.0
+Version: 0.3.1
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.3.0/README.md` & `bhv-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,35 +22,40 @@
 - Three redundant implementations on NumPy for performance and correctness
 - A minimal abstraction for permutations with caching and composition
 - Very basic embeddings for other datatypes (more to come)
 - Graph visualization of distances in hyperdimensional space ([see example](examples/viz_distances.py)).
 - Boolean expression and network synthesis
 
 ## Installation
+Make sure you have an up-to-date Python version, 3.10 recommended.
+
 `pip install bhv`
 
 If you only want to work with plain Python, you're good to go with `from bhv.vanilla VanillaBHV as BHV`.
 
 Else you'll need
 `pip install numpy` or `pip install torch` with respectively `from bhv.np import NumPyPacked64BHV as BHV` or `from bhv.np import TorchBoolBHV as BHV`. 
 
 ## Getting started
 One way to start is with going over [Kanerva's initial paper](http://ww.robertdick.org/iesr/papers/kanerva09jan.pdf) together with the library.
 For that, multiple resources are provided:
 - [A notebook going over the very basics](examples/Kanerva09.ipynb)
-- [A Python file export of that](examples/kanerva09.py)
 - [The grandmother example](examples/grandmother_example.py)
 - [A Google Colab hosted reasoning by analogy example notebook](https://colab.research.google.com/drive/10gOc39TsM5CE-6u3kj2oe1t-8KZHr_bB?usp=sharing)
+- [A guide to picking metrics](examples/Metric_Picker.ipynb)
 
 If you like to dive into the code directly, I suggest the following entrypoints:
 - [Finite State Machine example](examples/state_machine.py)
 - [The base class AbstractBHV](bhv/abstract.py)
 - [The most idiomatic implementation NumPyBoolBHV](bhv/np.py)
 
 If you're comming at this from a Machine Learning angle, you may enjoy:
 - [A minimal implementation](examples/winnow_classification.py) of the [winnow algorithm](https://en.wikipedia.org/wiki/Winnow_(algorithm)) on a minimal problem
 - [A minimal implementation of classification based on the majority operator](examples/majority_classification.py) on a minimal problem
 - [A Google Colab hosted digit classification via plain majority notebook](https://colab.research.google.com/drive/1xYQAXxcdFw89RV5CsflcvFhx3zpmEUxk?usp=sharing)
+- [Graph classification notebook](https://colab.research.google.com/drive/1NrmCc99GrkmHm_VLs5nv9Q7BCbCLs0ar?usp=sharing) re-implementing [GraphHD](https://arxiv.org/abs/2205.07826)
 
 ## Note
 This repository is highly active, and a work-in-progress.
 Do expect changes to the naming, and even features to be swapped for more elegant alternatives.
+
+Also works with PyPy. Use the vanilla Python implementation. The numeric operations are slower than on CPython, but the symbolic ones are way faster.
```

### Comparing `bhv-0.3.0/bhv/abstract.py` & `bhv-0.3.1/bhv/abstract.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.0/bhv/embedding.py` & `bhv-0.3.1/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.0/bhv/np.py` & `bhv-0.3.1/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.0/bhv/poibin.py` & `bhv-0.3.1/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.0/bhv/positions.py` & `bhv-0.3.1/bhv/positions.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.0/bhv/pytorch.py` & `bhv-0.3.1/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.0/bhv/shared.py` & `bhv-0.3.1/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.0/bhv/slice.py` & `bhv-0.3.1/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.0/bhv/symbolic.py` & `bhv-0.3.1/bhv/symbolic.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,21 +102,23 @@
             counted[id(self)] = t
             return t
 
     def simplify(self, **kwargs):
         x = self
         while True:
             x_ = x.reduce(**kwargs)
+            if x_ is None:
+                raise RuntimeError(f"{x} reduced to non (under {kwargs})")
             if x == x_:
                 return x
             else:
                 x = x_
 
     def reduce(self, **kwargs):
-        return self
+        return self.reconstruct(*[c.simplify(**kwargs) for c, _ in self.children()])
 
     def preorder(self, p=lambda x: True):
         return [self]*p(self) + [v for c, _ in self.children() for v in c.preorder(p)]
 
     def truth_assignments(self, vars):
         configs = bitconfigs(len(vars))
 
@@ -540,14 +542,15 @@
         elif isinstance(self.l, Invert) and isinstance(self.r, Invert):
             return ~Xor(self.l.v.simplify(**kwargs), self.r.v.simplify(**kwargs))
         elif isinstance(self.l, And) and isinstance(self.r, And):
             if self.l.l == self.r.l: return And(self.l.l, Xor(self.l.r, self.r.r)).simplify(**kwargs)
             elif self.l.l == self.r.r: return And(self.l.l, Xor(self.l.r, self.r.l)).simplify(**kwargs)
             elif self.l.r == self.r.l: return And(self.l.r, Xor(self.l.l, self.r.r)).simplify(**kwargs)
             elif self.l.r == self.r.r: return And(self.l.r, Xor(self.l.l, self.r.l)).simplify(**kwargs)
+            else: return Xor(self.l.simplify(**kwargs), self.r.simplify(**kwargs))
         else:
             return Xor(self.l.simplify(**kwargs), self.r.simplify(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         afl = self.l.expected_active_fraction(**kwargs)
         afr = self.r.expected_active_fraction(**kwargs)
         return afl*(1. - afr) + (1. - afl)*afr
@@ -641,15 +644,15 @@
     cond: SymbolicBHV
     when1: SymbolicBHV
     when0: SymbolicBHV
 
     def reconstruct(self, c, w1, w0):
         return Select(c, w1, w0)
 
-    def nodename(self, compact_select=True, **kwargs):
+    def nodename(self, compact_select=False, **kwargs):
         return f"ON {self.cond.nodename()}" if compact_select else super().nodename(**kwargs)
 
     def children(self, compact_select=False, **kwargs):
         return [(self.when1, "1"), (self.when0, "0")] if compact_select else super().children(**kwargs)
 
     def show(self, **kwargs):
         return f"{self.cond.show(**kwargs)}.select({self.when1.show(**kwargs)}, {self.when0.show(**kwargs)})"
```

### Comparing `bhv-0.3.0/bhv/vanilla.py` & `bhv-0.3.1/bhv/vanilla.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         random.shuffle(p)
         return VanillaPermutation(p)
 
     def __mul__(self, other: 'VanillaPermutation') -> 'VanillaPermutation':
         return VanillaPermutation([self.data[other.data[i]] for i in range(DIMENSION//8)])
 
     def __invert__(self) -> 'VanillaPermutation':
-        p = [None]*DIMENSION//8
+        p = [None]*(DIMENSION//8)
         for i, j in enumerate(self.data):
             p[j] = i
         return VanillaPermutation(p)
 
     def __call__(self, hv: 'VanillaBHV') -> 'VanillaBHV':
         return hv.permute_bytes(self)
```

### Comparing `bhv-0.3.0/bhv/visualization.py` & `bhv-0.3.1/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.0/bhv.egg-info/PKG-INFO` & `bhv-0.3.1/bhv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.3.0
+Version: 0.3.1
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.3.0/setup.py` & `bhv-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.0'
+VERSION = '0.3.1'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
```

