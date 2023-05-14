# Comparing `tmp/lilit-1.2.1.tar.gz` & `tmp/lilit-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lilit-1.2.1.tar", last modified: Sun May 14 13:44:23 2023, max compression
+gzip compressed data, was "lilit-1.2.2.tar", last modified: Sun May 14 19:49:01 2023, max compression
```

## Comparing `lilit-1.2.1.tar` & `lilit-1.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 13:44:23.921509 lilit-1.2.1/
--rw-rw-r--   0 jack      (1000) jack      (1000)      107 2023-05-14 10:52:53.000000 lilit-1.2.1/.gitignore
--rw-rw-r--   0 jack      (1000) jack      (1000)    35149 2023-03-30 14:20:30.000000 lilit-1.2.1/LICENSE
--rw-rw-r--   0 jack      (1000) jack      (1000)     9231 2023-05-14 13:44:23.921509 lilit-1.2.1/PKG-INFO
--rw-rw-r--   0 jack      (1000) jack      (1000)     7972 2023-05-14 10:01:30.000000 lilit-1.2.1/README.md
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 13:44:23.921509 lilit-1.2.1/docs/
--rw-rw-r--   0 jack      (1000) jack      (1000)      136 2023-04-04 10:36:24.000000 lilit-1.2.1/docs/index.html
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 13:44:23.921509 lilit-1.2.1/docs/lilit/
--rw-rw-r--   0 jack      (1000) jack      (1000)   701863 2023-04-04 10:36:24.000000 lilit-1.2.1/docs/lilit/likelihood.html
--rw-rw-r--   0 jack      (1000) jack      (1000)    62222 2023-04-04 10:36:23.000000 lilit-1.2.1/docs/lilit.html
--rw-rw-r--   0 jack      (1000) jack      (1000)   196905 2023-04-04 10:36:24.000000 lilit-1.2.1/docs/search.js
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 13:44:23.921509 lilit-1.2.1/examples/
--rw-rw-r--   0 jack      (1000) jack      (1000)    10552 2023-03-13 10:51:04.000000 lilit-1.2.1/examples/experiments.yaml
--rw-rw-r--   0 jack      (1000) jack      (1000)     3863 2023-03-10 18:35:00.000000 lilit-1.2.1/examples/logBB.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)     4660 2023-03-10 19:11:31.000000 lilit-1.2.1/examples/logTTTEEE.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)     5102 2023-03-13 10:12:49.000000 lilit-1.2.1/examples/logTTTEEEBB.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)    13218 2023-03-25 19:08:04.000000 lilit-1.2.1/examples/other_simple_likelihood.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    11698 2023-03-03 18:27:08.000000 lilit-1.2.1/examples/planck_2018.ini
--rw-rw-r--   0 jack      (1000) jack      (1000)     3124 2023-05-14 12:34:24.000000 lilit-1.2.1/examples/samplingBB.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     5041 2023-03-25 19:13:19.000000 lilit-1.2.1/examples/samplingFULL.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     4797 2023-05-14 12:30:17.000000 lilit-1.2.1/examples/samplingTTTEEE.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 13:44:23.921509 lilit-1.2.1/lilit/
--rw-rw-r--   0 jack      (1000) jack      (1000)     8129 2023-05-14 13:41:06.000000 lilit-1.2.1/lilit/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    10552 2023-04-28 08:54:33.000000 lilit-1.2.1/lilit/experiments.yaml
--rw-rw-r--   0 jack      (1000) jack      (1000)    10441 2023-05-14 13:38:08.000000 lilit-1.2.1/lilit/functions.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    39823 2023-05-14 12:38:14.000000 lilit-1.2.1/lilit/likelihood.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    11698 2023-03-03 18:27:08.000000 lilit-1.2.1/lilit/planck_2018.ini
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 13:44:23.921509 lilit-1.2.1/lilit.egg-info/
--rw-rw-r--   0 jack      (1000) jack      (1000)     9231 2023-05-14 13:44:23.000000 lilit-1.2.1/lilit.egg-info/PKG-INFO
--rw-rw-r--   0 jack      (1000) jack      (1000)      586 2023-05-14 13:44:23.000000 lilit-1.2.1/lilit.egg-info/SOURCES.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-05-14 13:44:23.000000 lilit-1.2.1/lilit.egg-info/dependency_links.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)       43 2023-05-14 13:44:23.000000 lilit-1.2.1/lilit.egg-info/requires.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)        6 2023-05-14 13:44:23.000000 lilit-1.2.1/lilit.egg-info/top_level.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)       38 2023-05-14 13:44:23.921509 lilit-1.2.1/setup.cfg
--rw-rw-r--   0 jack      (1000) jack      (1000)     1005 2023-04-04 09:43:31.000000 lilit-1.2.1/setup.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 19:49:01.616921 lilit-1.2.2/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      107 2023-05-14 17:32:19.000000 lilit-1.2.2/.gitignore
+-rw-rw-r--   0 jack      (1000) jack      (1000)    35149 2023-05-14 17:32:19.000000 lilit-1.2.2/LICENSE
+-rw-rw-r--   0 jack      (1000) jack      (1000)     9231 2023-05-14 19:49:01.616921 lilit-1.2.2/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)     7972 2023-05-14 19:35:00.000000 lilit-1.2.2/README.md
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 19:49:01.616921 lilit-1.2.2/docs/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      136 2023-05-14 17:32:19.000000 lilit-1.2.2/docs/index.html
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 19:49:01.616921 lilit-1.2.2/docs/lilit/
+-rw-rw-r--   0 jack      (1000) jack      (1000)   701863 2023-05-14 17:32:19.000000 lilit-1.2.2/docs/lilit/likelihood.html
+-rw-rw-r--   0 jack      (1000) jack      (1000)    62222 2023-05-14 17:32:19.000000 lilit-1.2.2/docs/lilit.html
+-rw-rw-r--   0 jack      (1000) jack      (1000)   196905 2023-05-14 17:32:19.000000 lilit-1.2.2/docs/search.js
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 19:49:01.616921 lilit-1.2.2/examples/
+-rw-rw-r--   0 jack      (1000) jack      (1000)    10552 2023-05-14 17:32:19.000000 lilit-1.2.2/examples/experiments.yaml
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3863 2023-05-14 17:32:19.000000 lilit-1.2.2/examples/logBB.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4660 2023-05-14 17:32:19.000000 lilit-1.2.2/examples/logTTTEEE.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5102 2023-05-14 17:32:19.000000 lilit-1.2.2/examples/logTTTEEEBB.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)    13218 2023-05-14 17:32:19.000000 lilit-1.2.2/examples/other_simple_likelihood.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    11698 2023-05-14 17:32:19.000000 lilit-1.2.2/examples/planck_2018.ini
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3124 2023-05-14 19:35:00.000000 lilit-1.2.2/examples/samplingBB.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5041 2023-05-14 17:32:19.000000 lilit-1.2.2/examples/samplingFULL.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4696 2023-05-14 19:35:00.000000 lilit-1.2.2/examples/samplingTTTEEE.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 19:49:01.616921 lilit-1.2.2/lilit/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      244 2023-05-14 19:43:26.000000 lilit-1.2.2/lilit/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    10552 2023-05-14 17:32:19.000000 lilit-1.2.2/lilit/experiments.yaml
+-rw-rw-r--   0 jack      (1000) jack      (1000)    10263 2023-05-14 19:43:09.000000 lilit-1.2.2/lilit/functions.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    24051 2023-05-14 19:47:04.000000 lilit-1.2.2/lilit/likelihood.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    11698 2023-05-14 17:32:19.000000 lilit-1.2.2/lilit/planck_2018.ini
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 19:49:01.616921 lilit-1.2.2/lilit.egg-info/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     9231 2023-05-14 19:49:01.000000 lilit-1.2.2/lilit.egg-info/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)      586 2023-05-14 19:49:01.000000 lilit-1.2.2/lilit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-05-14 19:49:01.000000 lilit-1.2.2/lilit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       43 2023-05-14 19:49:01.000000 lilit-1.2.2/lilit.egg-info/requires.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)        6 2023-05-14 19:49:01.000000 lilit-1.2.2/lilit.egg-info/top_level.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       38 2023-05-14 19:49:01.616921 lilit-1.2.2/setup.cfg
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1005 2023-05-14 17:32:19.000000 lilit-1.2.2/setup.py
```

### Comparing `lilit-1.2.1/LICENSE` & `lilit-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/PKG-INFO` & `lilit-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilit
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python package encoding a likelihood for LiteBIRD.
 Home-page: https://github.com/ggalloni/LiLit
 Author: Galloni, Giacomo
 Author-email: giacomo.galloni@roma2.infn.it
 License: GNU General Public License v3.0
 Description: # LiLit: Likelihood for LiteBIRD
```

### Comparing `lilit-1.2.1/README.md` & `lilit-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/docs/lilit/likelihood.html` & `lilit-1.2.2/docs/lilit/likelihood.html`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/docs/lilit.html` & `lilit-1.2.2/docs/lilit.html`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/docs/search.js` & `lilit-1.2.2/docs/search.js`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/examples/experiments.yaml` & `lilit-1.2.2/examples/experiments.yaml`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/examples/logBB.txt` & `lilit-1.2.2/examples/logBB.txt`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/examples/logTTTEEE.txt` & `lilit-1.2.2/examples/logTTTEEE.txt`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/examples/logTTTEEEBB.txt` & `lilit-1.2.2/examples/logTTTEEEBB.txt`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/examples/other_simple_likelihood.py` & `lilit-1.2.2/examples/other_simple_likelihood.py`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/examples/planck_2018.ini` & `lilit-1.2.2/examples/planck_2018.ini`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/examples/samplingBB.py` & `lilit-1.2.2/examples/samplingBB.py`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/examples/samplingFULL.py` & `lilit-1.2.2/examples/samplingFULL.py`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/examples/samplingTTTEEE.py` & `lilit-1.2.2/examples/samplingTTTEEE.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 """Sample on CMB temperature and E-modes."""
 import time
 from mpi4py import MPI
 from cobaya.run import run
 from cobaya.log import LoggedError
-import lilit
 from lilit import LiLit
-
-from lilit import functions as func
-
-print(func.get_keys(["t", "e"]))
-
-print(lilit.__version__)
+from lilit import CAMBres2dict
 
 debug = True
 name = "TTTEEE"
 
 # Note that the order of these list has to be the same of the fields keyword
 lmin = [2, 20]
 lmax = [1500, 1200]
@@ -28,25 +22,25 @@
     nside=256,
     lmin=lmin,
     lmax=lmax,
     fsky=fsky,
     debug=debug,
 )
 
-# gaussTTTEEE = LiLit(
-#     name=name,
-#     fields=["t", "e"],
-#     like="gaussian",
-#     experiment="PTEPLiteBIRD",
-#     nside=256,
-#     lmin=lmin,
-#     lmax=lmax,
-#     fsky=fsky,
-#     debug=debug,
-# )
+gaussTTTEEE = LiLit(
+    name=name,
+    fields=["t", "e"],
+    like="gaussian",
+    experiment="PTEPLiteBIRD",
+    nside=256,
+    lmin=lmin,
+    lmax=lmax,
+    fsky=fsky,
+    debug=debug,
+)
 
 info = {
     "likelihood": {name: exactTTTEEE},
     "params": {
         "As": {"latex": "A_\\mathrm{s}", "value": "lambda logA: 1e-10*np.exp(logA)"},
         "H0": {"latex": "H_0", "max": 100, "min": 20},
         # "H0": 67.32117,
@@ -55,53 +49,53 @@
             "value": "lambda theta_MC_100: 1.e-2*theta_MC_100",
         },
         "logA": {
             "drop": True,
             "latex": "\\log(10^{10} A_\\mathrm{s})",
             "prior": {"max": 3.91, "min": 1.61},
             "proposal": 0.001,
-            # "ref": {"dist": "norm", "loc": 3.04478383213, "scale": 0.0001},
-            "ref": 3.04478383213,
+            "ref": {"dist": "norm", "loc": 3.04478383213, "scale": 0.0001},
+            # "ref": 3.04478383213,
         },
         "mnu": 0.06,
         "ns": {
             "latex": "n_\\mathrm{s}",
             "prior": {"max": 1.2, "min": 0.8},
             "proposal": 0.002,
-            # "ref": {"dist": "norm", "loc": 0.9660499, "scale": 0.0004},
-            "ref": 0.9660499,
+            "ref": {"dist": "norm", "loc": 0.9660499, "scale": 0.0004},
+            # "ref": 0.9660499,
         },
         "ombh2": {
             "latex": "\\Omega_\\mathrm{b} h^2",
             "prior": {"max": 0.1, "min": 0.005},
             "proposal": 0.0001,
-            # "ref": {"dist": "norm", "loc": 0.0223828, "scale": 0.00001},
-            "ref": 0.0223828,
+            "ref": {"dist": "norm", "loc": 0.0223828, "scale": 0.00001},
+            # "ref": 0.0223828,
         },
         "omch2": {
             "latex": "\\Omega_\\mathrm{c} h^2",
             "prior": {"max": 0.99, "min": 0.001},
             "proposal": 0.0005,
-            # "ref": {"dist": "norm", "loc": 0.1201075, "scale": 0.0001},
-            "ref": 0.1201075,
+            "ref": {"dist": "norm", "loc": 0.1201075, "scale": 0.0001},
+            # "ref": 0.1201075,
         },
         "tau": {
             "latex": "\\tau_\\mathrm{reio}",
             "prior": {"max": 0.8, "min": 0.01},
             "proposal": 0.003,
-            # "ref": {"dist": "norm", "loc": 0.05430842, "scale": 0.0006},
-            "ref": 0.05430842,
+            "ref": {"dist": "norm", "loc": 0.05430842, "scale": 0.0006},
+            # "ref": 0.05430842,
         },
         "theta_MC_100": {
             "drop": True,
             "latex": "100\\theta_\\mathrm{MC}",
             "prior": {"max": 10, "min": 0.5},
             "proposal": 0.0002,
-            # "ref": {"dist": "norm", "loc": 1.04109, "scale": 0.00004},
-            "ref": 1.041456798,
+            "ref": {"dist": "norm", "loc": 1.04109, "scale": 0.00004},
+            # "ref": 1.041456798,
             "renames": "theta",
         },
     },
     "output": f"chains/exact{name}_lmax{lmax}",
     "force": True,
     "resume": False,
     # "debug": True,
```

### Comparing `lilit-1.2.1/lilit/__init__.py` & `lilit-1.2.2/lilit.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,110 +1,116 @@
-"""# Welcome to LiLit!
-
-A Python package encoding the likelihood for LiteBIRD.
-
-In this repository I provide some basic examples of forecasting likelihoods for LiteBIRD. These are implemented to be used a [Cobaya](https://github.com/CobayaSampler/cobaya) context ([J. Torrado and A. Lewis, 2020](https://arxiv.org/abs/2005.05290)), which encapsulates [CosmoMC](https://github.com/cmbant/CosmoMC) in a Python framework. The idea of this repository is to ease the creation of common framework among different  LiteBIRDers, trying to homogenize the post-PTEP works as we recently discussed among the collaboration. The main product of this repository is the Likelihood for LiteBIRD (LiLit), which you can find [here](lilit/likelihood.py). Within LiLit, the most relevant study cases of LiteBIRD (T, E, B) are already tested and working. So, if you need to work with those, you should not need to look into the actual definition of the likelihood function, since you can proptly start running your MCMCs. Despite this, you should provide to the likelihood some file where to find the proper LiteBIRD noise power spectra, given that LiLit is implementing a simple inverse noise weighting just as a place-holder for something more realistic. As regards lensing, LiLit will need you to pass the reconstruction noise, since its computation is not coded, thus there is no place-holder for lensing.
-
-This repository should also give to new Cobaya-users a good starting point to build upon (see [this](examples/other_simple_likelihood.py)). 
-
-The repository can be found at [https://github.com/ggalloni/LiLit](https://github.com/ggalloni/LiLit).
-
-## Installation
-
-To install the LiLit package it is sufficient to do:
-
-```
-pip install lilit
-```
-
-Then, to access the LiLit class, it is sufficient to import it as:
-
-```
-from lilit import LiLit
-```
-
-## Some further details on LiLit
-
-If you want to start using LiLit, here are some further details on what you can do with it. Firstly, LiLit is independent of the number of fields considered and can be dynamically modified at declaration. Thus, it makes no difference if you want to use B-modes alone, or if you want to use CMB temperature, E-modes, lensing, etc. The only constraint is that the Boltzmann code you are using to provide the spectra should understand the fields you are asking to LiLit. Each of these fields may have their own $\ell_{\rm min}$, $\ell_{\rm max}$ and $f_{\rm sky}$. So, I implemented the possibility to pass all these quantities as lists to LiLit, which will then take case of the proper multipoles cuts and so on. The only requirement is that you should pass these lists following the order in which you passes the requested fields. For example:
-
-```
-fields = ["t", "e", "b"]
-
-# lmax = [lmaxTT, lmaxEE, lmaxBB]
-lmax = [1500, 1200, 900]
-
-# lmin = [lminTT, lminEE, lminBB]
-lmin = [20, 2, 2]
-
-# fsky = [fskyTT, fskyEE, fskyBB]
-fsky = [1.0, 0.8, 0.6]
-```
-
-If you do not want to pass custom fiducial power spectra for the fields you requested, you can exploit the fact that LiLit will internally compute every spectra according to _Planck_ 2018 best-fit values of the cosmological parameters. Note that if you requested B-modes, you must provide the value you want to assign to the tensor-to-scalar ratio $r$ (be careful on what pivot scale you are using here). If you do not pass the spectral index $n_t$, it will follow the standard consistency relation. 
-
-As regards noise, as mentioned above you should pass realistic power spectra according to what you are working on. Just as a mere place-holder, LiLit will compute the inverse-weighted noise ([P. Campeti et al., 2020](https://arxiv.org/abs/2007.04241)) over each channel of LiteBIRD ([E. Allys et al., 2022](https://arxiv.org/abs/2202.02773)).
-
-Once you have fixed all these quantities, you are ready to define your likelihood. The only remaining things to decide are what approximation you want to use to compute the $\chi^2$ and the actual name of the likelihood. LiLit implements the exact likelihood ([S. Hamimeche and A. Lewis, 2008](https://arxiv.org/abs/0801.0554)) and the Gaussian one. Thus, you can define your likelihood with:
-
-```
-name = exampleTEB
-
-# using the exact likelihood approximation
-exampleTEB = LiLit(name=name, fields=fields, like="exact", nl_file="/path/to/noise.pkl", lmax=lmax, fsky=fsky, debug=False)
-
-# using the Gaussian likelihood approximation
-exampleTEB = LiLit(name=name, fields=fields, like="gaussian", nl_file="/path/to/noise.pkl", lmax=lmax, fsky=fsky, debug=False)
-```
-
-Note that you may want to set debug to True in order to check that everything is OK.
-
-I tried to be as modular as possible so that you can plug whatever existing function you have. Also, this should make parallelization easier if you need it.
-
-## Other simple likelihood
-
-[Here](examples/other_simple_likelihood.py), you can find two very simple examples of the skeleton of a single-field likelihood and a two-field one. If you are new to Cobaya, you may want to have a look at these before jumping to LiLit. 
-
-As regards the single-field likelihood, what you can find there is a very basic example of how to run Cobaya on a generic field X. Some parts of this may require additional attention before running, however this should give you an idea of how to work with this package. For instance, here I am considering a very simple case in which I do not need to pass anything to the likelihood class but the spectra, and in which the likelihood does not provide any derived parameters.
-
-## Examples
-
-I provide also few working examples of the usage of LiLit. Some particular attention should be given to the dictionaries defined in the sampling scripts. If you are not familiar with their structure, have a look at Cobaya's [documentation](https://cobaya.readthedocs.io/en/latest/). Then, I customized these to maximize accordance with the fiducial _Planck_ 2018 spectra. These also assume that you will be using [CAMB](https://github.com/cmbant/CAMB) ([A. Lewis et al., 2000](https://arxiv.org/abs/astro-ph/9911177)); for the [CLASS](https://github.com/lesgourg/class_public) ([D. Blas et al., 2011](https://arxiv.org/abs/1104.2933)) equivalent of this, refer again to documentiation, since some of the parameters are renamed. Note that Cobaya will understand whatever newly defined parameter you added to the Boltzmann code.
-
-In the parameters block of the sampling dictionary, parameters with a prior will be interpreted as open parameters, while all the others are essentially derived ones. Cobaya will figure out by itself whether it has to ask for some of them to the theory code (CAMB) or to other parameters. Also, it will figure out what parts of the routines need certain parameters. For example, you can pass $A_s$ to the likelihood function and do something with it, but at the same time it will pass it also to CAMB to compute the spectra.
-
-Once you have finished preparing your sampling.py file, you can run it simply by using: 
-
-`python sampling.py > log.txt`
-
-Sending the inline output to a text file might help in recovering information on how the run is going. If you want to run it parallely, you may want to use something like:
-
-`mpirun -np 4 --cpus-per-proc 4 python sampling.py > log.txt`
-
-The number of processess translates on the number of chains that will be runned simultaneously.
-
-## Dependencies
-* cobaya
-* numpy
-* healpy
-* pyyaml
-* matplotlib
-* camb
-
-## Documentation
-
-The documentation can be found at [https://ggalloni.github.io/LiLit](https://ggalloni.github.io/LiLit).
-
-## Developing the code
-
-If you want to help developing the code, feel free to send a pull request. Also, feel free to write me so that we can discuss on eventual major developments.
-
-## Support
-
-For additional details on how Cobaya works, I suggest to see the [documentation](https://cobaya.readthedocs.io/en/latest/), which is very good to find whatever is not working in you case. If you cannot find the problem there, feel free to open an issue.
-"""
-
-from .likelihood import LiLit
-from .functions import CAMBres2dict
-
-__author__ = "Giacomo Galloni"
-__version__ = "1.2.1"
-__docformat__ = "numpy"
+Metadata-Version: 2.1
+Name: lilit
+Version: 1.2.2
+Summary: A Python package encoding a likelihood for LiteBIRD.
+Home-page: https://github.com/ggalloni/LiLit
+Author: Galloni, Giacomo
+Author-email: giacomo.galloni@roma2.infn.it
+License: GNU General Public License v3.0
+Description: # LiLit: Likelihood for LiteBIRD
+        
+        Author: Giacomo Galloni
+        
+        ## Overview
+        
+        In this repository I provide some basic examples of forecasting likelihoods for LiteBIRD. These are implemented to be used a [Cobaya](https://github.com/CobayaSampler/cobaya) context ([J. Torrado and A. Lewis, 2020](https://arxiv.org/abs/2005.05290)), which encapsulates [CosmoMC](https://github.com/cmbant/CosmoMC) in a Python framework. The idea of this repository is to ease the creation of common framework among different  LiteBIRDers, trying to homogenize the post-PTEP works as we recently discussed among the collaboration. The main product of this repository is the Likelihood for LiteBIRD (LiLit), which you can find [here](lilit/likelihood.py). Within LiLit, the most relevant study cases of LiteBIRD (T, E, B) are already tested and working. So, if you need to work with those, you should not need to look into the actual definition of the likelihood function, since you can proptly start running your MCMCs. Despite this, you should provide to the likelihood some file where to find the proper LiteBIRD noise power spectra, given that LiLit is implementing a simple inverse noise weighting just as a place-holder for something more realistic. As regards lensing, LiLit will need you to pass the reconstruction noise, since its computation is not coded, thus there is no place-holder for lensing.
+        
+        This repository should also give to new Cobaya-users a good starting point to build upon (see [this](examples/other_simple_likelihood.py)). 
+        
+        The repository can be found at [https://github.com/ggalloni/LiLit](https://github.com/ggalloni/LiLit).
+        
+        ## Installation
+        
+        To install the LiLit package it is sufficient to do:
+        
+        ```
+        pip install lilit
+        ```
+        
+        Then, to access the LiLit class, it is sufficient to import it as:
+        
+        ```
+        from lilit import LiLit
+        ```
+        
+        ## Some further details on LiLit
+        
+        If you want to start using LiLit, here are some further details on what you can do with it. Firstly, LiLit is independent of the number of fields considered and can be dynamically modified at declaration. Thus, it makes no difference if you want to use B-modes alone, or if you want to use CMB temperature, E-modes, lensing, etc. The only constraint is that the Boltzmann code you are using to provide the spectra should understand the fields you are asking to LiLit. Each of these fields may have their own $\ell_{\rm min}$, $\ell_{\rm max}$ and $f_{\rm sky}$. So, I implemented the possibility to pass all these quantities as lists to LiLit, which will then take case of the proper multipoles cuts and so on. The only requirement is that you should pass these lists following the order in which you passes the requested fields. For example:
+        
+        ```
+        fields = ["t", "e", "b"]
+        
+        # lmax = [lmaxTT, lmaxEE, lmaxBB]
+        lmax = [1500, 1200, 900]
+        
+        # lmin = [lminTT, lminEE, lminBB]
+        lmin = [20, 2, 2]
+        
+        # fsky = [fskyTT, fskyEE, fskyBB]
+        fsky = [1.0, 0.8, 0.6]
+        ```
+        
+        If you do not want to pass custom fiducial power spectra for the fields you requested, you can exploit the fact that LiLit will internally compute every spectra according to _Planck_ 2018 best-fit values of the cosmological parameters. Note that if you requested B-modes, you must provide the value you want to assign to the tensor-to-scalar ratio $r$ (be careful on what pivot scale you are using here). If you do not pass the spectral index $n_t$, it will follow the standard consistency relation. 
+        
+        As regards noise, as mentioned above you should pass realistic power spectra according to what you are working on. Just as a mere place-holder, LiLit will compute the inverse-weighted noise ([P. Campeti et al., 2020](https://arxiv.org/abs/2007.04241)) over each channel of LiteBIRD ([E. Allys et al., 2022](https://arxiv.org/abs/2202.02773)).
+        
+        Once you have fixed all these quantities, you are ready to define your likelihood. The only remaining things to decide are what approximation you want to use to compute the $\chi^2$ and the actual name of the likelihood. LiLit implements the exact likelihood ([S. Hamimeche and A. Lewis, 2008](https://arxiv.org/abs/0801.0554)) and the Gaussian one. Thus, you can define your likelihood with:
+        
+        ```
+        name = exampleTEB
+        
+        # using the exact likelihood approximation
+        exampleTEB = LiLit(name=name, fields=fields, like="exact", nl_file="/path/to/noise.pkl", lmax=lmax, fsky=fsky, debug=False)
+        
+        # using the Gaussian likelihood approximation
+        exampleTEB = LiLit(name=name, fields=fields, like="gaussian", nl_file="/path/to/noise.pkl", lmax=lmax, fsky=fsky, debug=False)
+        ```
+        
+        Note that you may want to set debug to True in order to check that everything is OK.
+        
+        I tried to be as modular as possible so that you can plug whatever existing function you have. Also, this should make parallelization easier if you need it.
+        
+        ## Other simple likelihood
+        
+        [Here](examples/other_simple_likelihood.py), you can find two very simple examples of the skeleton of a single-field likelihood and a two-field one. If you are new to Cobaya, you may want to have a look at these before jumping to LiLit. 
+        
+        As regards the single-field likelihood, what you can find there is a very basic example of how to run Cobaya on a generic field X. Some parts of this may require additional attention before running, however this should give you an idea of how to work with this package. For instance, here I am considering a very simple case in which I do not need to pass anything to the likelihood class but the spectra, and in which the likelihood does not provide any derived parameters.
+        
+        ## Examples
+        
+        I provide also few working examples of the usage of LiLit. Some particular attention should be given to the dictionaries defined in the sampling scripts. If you are not familiar with their structure, have a look at Cobaya's [documentation](https://cobaya.readthedocs.io/en/latest/). Then, I customized these to maximize accordance with the fiducial _Planck_ 2018 spectra. These also assume that you will be using [CAMB](https://github.com/cmbant/CAMB) ([A. Lewis et al., 2000](https://arxiv.org/abs/astro-ph/9911177)); for the [CLASS](https://github.com/lesgourg/class_public) ([D. Blas et al., 2011](https://arxiv.org/abs/1104.2933)) equivalent of this, refer again to documentiation, since some of the parameters are renamed. Note that Cobaya will understand whatever newly defined parameter you added to the Boltzmann code.
+        
+        In the parameters block of the sampling dictionary, parameters with a prior will be interpreted as open parameters, while all the others are essentially derived ones. Cobaya will figure out by itself whether it has to ask for some of them to the theory code (CAMB) or to other parameters. Also, it will figure out what parts of the routines need certain parameters. For example, you can pass $A_s$ to the likelihood function and do something with it, but at the same time it will pass it also to CAMB to compute the spectra.
+        
+        Once you have finished preparing your sampling.py file, you can run it simply by using: 
+        
+        `python sampling.py > log.txt`
+        
+        Sending the inline output to a text file might help in recovering information on how the run is going. If you want to run it parallely, you may want to use something like:
+        
+        `mpirun -np 4 --cpus-per-proc 4 python sampling.py > log.txt`
+        
+        The number of processess translates on the number of chains that will be runned simultaneously.
+        
+        ## Dependencies
+        * cobaya
+        * numpy
+        * healpy
+        * pyyaml
+        * matplotlib
+        * camb
+        
+        ## Documentation
+        
+        The documentation can be found at [https://ggalloni.github.io/LiLit](https://ggalloni.github.io/LiLit).
+        
+        ## Developing the code
+        
+        If you want to help developing the code, feel free to send a pull request. Also, feel free to write me so that we can discuss on eventual major developments.
+        
+        ## Support
+        
+        For additional details on how Cobaya works, I suggest to see the [documentation](https://cobaya.readthedocs.io/en/latest/), which is very good to find whatever is not working in you case. If you cannot find the problem there, feel free to open an issue.
+        
+Keywords: bayesian-statistics,markov-chain-mote-carlo,cosmic-microwave-background,cobaya
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `lilit-1.2.1/lilit/experiments.yaml` & `lilit-1.2.2/lilit/experiments.yaml`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/lilit/functions.py` & `lilit-1.2.2/lilit/functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 import numpy as np
 
+__all__ = [
+    "get_keys",
+    "get_Gauss_keys",
+    "cov_filling",
+    "find_spectrum",
+    "sigma",
+    "inv_sigma",
+    "CAMBres2dict",
+    "txt2dict",
+]
+
 
 def get_keys(fields: list, *, debug: bool = False):
-    """Extracts the keys that has to be used as a function of the requested fields. These will be the usual 2-points, e.g., tt, te, ee, etc."""
-    # List of all the possible combinations of the requested fields
+    """Extracts the keys that has to be used as a function of the requested fields. These will be the usual 2-points, e.g., tt, te, ee, etc.
+
+    Parameters:
+        fields (list):
+            List of fields
+        debug (bool, optional):
+            If True, print out the requested keys
+    """
     n = len(fields)
     res = [fields[i] + fields[j] for i in range(n) for j in range(i, n)]
-    # Print the requested keys
     if debug:
         print(f"\nThe requested keys are {res}")
     return res
 
 
 def get_Gauss_keys(n: int, keys: list, *, debug: bool = False):
     """Find the proper dictionary keys for the requested fields.
 
     Extracts the keys that has to be used as a function of the requested fields for the Gaussian likelihood. Indeed, the Gaussian likelihood is computed using 4-points, so the keys are different. E.g., there will be keys such as tttt, ttee, tete, etc.
+
+    Parameters:
+        n (int):
+            Number of fields.
+        keys (list):
+            List of keys to use for the computation.
+        debug (bool, optional):
+            If set, print the keys that are used, by default False.
     """
-    # Calculate the number of elements in the covariance matrix from the number of fields
     n = int(n * (n + 1) / 2)
-    # Initialize a 3-d array to store the keys
     res = np.zeros((n, n, 4), dtype=str)
-    # Loop over all the elements in the covariance matrix
     for i in range(n):
         for j in range(i, n):
-            # Generate a key for the i-th and j-th element
             elem = keys[i] + keys[j]
-            # Loop over all the characters in the key
             for k in range(4):
-                # Add the k-th character to the i-th, j-th, and k-th
-                # indices of the array
                 res[i, j, k] = np.asarray(list(elem)[k])
                 res[j, i, k] = res[i, j, k]
-    # Print the keys if the debug flag is set
-    # if debug:
-    #     print(f"\nThe requested keys are {res}")
-    # Return the keys
+    if debug:
+        print(f"\nThe requested keys are {res}")
     return res
 
 
 def cov_filling(
     fields: list,
     absolute_lmin: int,
     absolute_lmax: int,
@@ -48,86 +63,91 @@
     lmaxs: dict = {},
 ):
     """Fill covariance matrix with appropriate spectra.
 
     Computes the covariance matrix once given a dictionary. Returns the covariance matrix of the considered fields, in a shape equal to (num_fields x num_fields x lmax). Note that if more than one lmax, or lmin, is specified, there will be null values in the matrices, making them singular. This will be handled in another method.
 
     Parameters:
+        fields (list):
+            The list of fields to consider.
+        absolute_lmin (int):
+            The minimum multipole to consider.
+        absolute_lmax (int):
+            The maximum multipole to consider.
         cov_dict (dict):
             The input dictionary of spectra.
+        lmins (dict):
+            The dictionary of minimum multipole to consider for each field pair.
+        lmaxs (dict):
+            The dictionary of maximum multipole to consider for each field pair.
     """
-    # Initialize output array
     n = len(fields)
     res = np.zeros((n, n, absolute_lmax + 1))
 
-    # Loop over field1
     for i, field1 in enumerate(fields):
-        # Loop over field2
         for j, field2 in enumerate(fields[i:]):
-            # Get the index of field2
             j += i
 
-            # Get the key of the covariance matrix
             key = field1 + field2
 
-            # Get lmin and lmax for this field pair
             lmin = lmins.get(key, absolute_lmin)
             lmax = lmaxs.get(key, absolute_lmax)
 
-            # Get the covariance for this field pair
             cov = cov_dict.get(key, np.zeros(lmax + 1))
 
-            # Set the appropriate values in the covariance matrix
             res[i, j, lmin : lmax + 1] = cov[lmin : lmax + 1]
-            # Fill the covariance matrix symmetrically
             res[j, i] = res[i, j]
 
     return res
 
 
 def find_spectrum(lmin, lmax, input_dict, key):
     """Find a spectrum in a given dictionary.
 
     Returns the corresponding power sepctrum for a given key. If the key is not found, it will try to find the reverse key. Otherwise it will fill the array with zeros.
 
     Parameters:
+        lmin (int):
+            The minimum multipole to consider.
+        lmax (int):
+            The maximum multipole to consider.
         input_dict (dict):
             Dictionary where you want to search for keys.
-
         key (str):
             Key to search for.
     """
-    # create a zero array
     res = np.zeros(lmax + 1)
 
-    # try to find the key in the dictionary
     if key in input_dict:
         cov = input_dict[key]
-    # if the key is not found, try the reverse key
+    # if the key is not found, try the reverse key, otherwise fill with zeros
     else:
         cov = input_dict.get(key[::-1], np.zeros(lmax + 1))
 
-    # fill the array with the requested spectrum
     res[lmin : lmax + 1] = cov[lmin : lmax + 1]
 
     return res
 
 
 def sigma(n, lmin, lmax, keys, fiduDICT, noiseDICT, fsky=None, fskies=[]):
     """Define the covariance matrix for the Gaussian case.
 
     In case of Gaussian likelihood, this returns the covariance matrix needed for the computation of the chi2. Note that the inversion is done in a separate funciton.
 
     Parameters:
+        n (int):
+            Number of fields.
+        lmin (int):
+            The minimum multipole to consider.
+        lmax (int):
+            The maximum multipole to consider.
         keys (dict):
             Keys for the covariance elements.
-
         fiduDICT (dict):
             Dictionary with the fiducial spectra.
-
         noiseDICT (dict):
             Dictionary with the noise spectra.
     """
     # The covariance matrix has to be symmetric.
     # The number of parameters in the likelihood is n.
     # The covariance matrix is a (n x n x lmax+1) ndarray.
     # We will store the covariance matrix in a (n x n x lmax+1) ndarray,
@@ -167,92 +187,83 @@
 
 def inv_sigma(lmin, lmax, sigma):
     """Invert the covariance matrix of the Gaussian case.
 
     Inverts the previously calculated sigma ndarray. Note that some elements may be null, thus the covariance may be singular. If so, this also reduces the dimension of the matrix by deleting the corresponding row and column.
 
     Parameters:
-        ndarray (np.ndarray):
+        lmin (int):
+            The minimum multipole to consider.
+        lmax (int):
+            The maximum multipole to consider.
+        sigma (np.ndarray):
             (n x n x lmax+1) ndarray with the previously computed sigma (not inverted).
     """
-    # Initialize array to store the inverted covariance matrices
     res = np.zeros(sigma.shape)
 
-    # Loop over multipoles
     for ell in range(lmin, lmax + 1):
         # Check if matrix is singular
         COV = sigma[:, :, ell]
         if np.linalg.det(COV) == 0:
             # Get indices of null diagonal elements
             idx = np.where(np.diag(COV) == 0)[0]
             # Remove corresponding rows and columns
             COV = np.delete(COV, idx, axis=0)
             COV = np.delete(COV, idx, axis=1)
-        # Invert matrix
+
         res[:, :, ell] = np.linalg.inv(COV)
     return res[:, :, lmin:]
 
 
-def CAMBres2dict(camb_results, keys):
+def CAMBres2dict(camb_results, probes):
     """Takes the CAMB result product from get_cmb_power_spectra and convert it to a dictionary with the proper keys.
 
     Parameters:
         camb_results (CAMBdata):
             CAMB result product from the method get_cmb_power_spectra.
+        probes (dict):
+            Keys for the spectra dictionary we want to save.
     """
-    # Get the number of multipoles
     ls = np.arange(camb_results["total"].shape[0], dtype=np.int64)
     # Mapping between the CAMB keys and the ones we want
     mapping = {"tt": 0, "ee": 1, "bb": 2, "te": 3, "et": 3}
-    # Initialize the output dictionary
     res = {"ell": ls}
-    # Loop over the keys we want
-    for key, i in mapping.items():
-        # Save the results
-        res[key] = camb_results["total"][:, i]
-    # Check if we want the lensing potential
-    if "pp" in keys:
-        # Get the lensing potential
+    for probe, i in mapping.items():
+        res[probe] = camb_results["total"][:, i]
+    if "pp" in probes:
         cl_lens = camb_results.get("lens_potential")
-        # Check if it exists
         if cl_lens is not None:
             # Save it with the normalization to obtain phiphi
             array = cl_lens[:, 0].copy()
             array[2:] /= (res["ell"] * (res["ell"] + 1))[2:]
             res["pp"] = array
-            # Check if we want the cross terms
-            if "pt" in keys and "pe" in keys:
-                # Loop over the cross terms
+            if "pt" in probes and "pe" in probes:
+                # Loop over the cross terms correcting the normalization to phiX
                 for i, cross in enumerate(["pt", "pe"]):
-                    # Save the result
                     array = cl_lens[:, i + 1].copy()
                     array[2:] /= np.sqrt(res["ell"] * (res["ell"] + 1))[2:]
                     res[cross] = array
-                    # Save the symmetric term
                     res[cross[::-1]] = res[cross]
     return res
 
 
-def txt2dict(txt, mapping=None, apply_ellfactor=None):
+def txt2dict(txt, mapping_probe2colnum=None, apply_ellfactor=None):
     """Takes a txt file and convert it to a dictionary. This requires a way to map the columns to the keys. Also, it is possible to apply an ell factor to the Cls.
 
     Parameters:
         txt (str):
             Path to txt file containing the spectra as columns.
         mapping (dict):
             Dictionary containing the mapping. Keywords will become the new keywords and values represent the index of the corresponding column.
     """
-    # Define the ell values from the length of the txt file
     assert (
-        mapping is not None
+        mapping_probe2colnum is not None
     ), "You must provide a way to map the columns of your txt to the keys of a dictionary"
     res = {}
-    # Loop over the mapping and extract the corresponding column from the txt file
-    # and store it in the dictionary under the corresponding keyword
-    for key, i in mapping.items():
+    for probe, i in mapping_probe2colnum.items():
         ls = np.arange(len(txt[:, i]), dtype=np.int64)
         res["ell"] = ls
         if apply_ellfactor:
-            res[key] = txt[:, i] * ls * (ls + 1) / 2 / np.pi
+            res[probe] = txt[:, i] * ls * (ls + 1) / 2 / np.pi
         else:
-            res[key] = txt[:, i]
+            res[probe] = txt[:, i]
     return res
```

### Comparing `lilit-1.2.1/lilit/planck_2018.ini` & `lilit-1.2.2/lilit/planck_2018.ini`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/lilit.egg-info/SOURCES.txt` & `lilit-1.2.2/lilit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lilit-1.2.1/setup.py` & `lilit-1.2.2/setup.py`

 * *Files identical despite different names*

