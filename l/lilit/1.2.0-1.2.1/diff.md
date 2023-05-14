# Comparing `tmp/lilit-1.2.0.tar.gz` & `tmp/lilit-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lilit-1.2.0.tar", last modified: Sun May 14 10:47:35 2023, max compression
+gzip compressed data, was "lilit-1.2.1.tar", last modified: Sun May 14 13:44:23 2023, max compression
```

## Comparing `lilit-1.2.0.tar` & `lilit-1.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 10:47:35.644811 lilit-1.2.0/
--rw-rw-r--   0 jack      (1000) jack      (1000)       99 2023-03-31 14:41:42.000000 lilit-1.2.0/.gitignore
--rw-rw-r--   0 jack      (1000) jack      (1000)    35149 2023-03-30 14:20:30.000000 lilit-1.2.0/LICENSE
--rw-rw-r--   0 jack      (1000) jack      (1000)     9231 2023-05-14 10:47:35.644811 lilit-1.2.0/PKG-INFO
--rw-rw-r--   0 jack      (1000) jack      (1000)     7972 2023-05-14 10:01:30.000000 lilit-1.2.0/README.md
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 10:47:35.640811 lilit-1.2.0/docs/
--rw-rw-r--   0 jack      (1000) jack      (1000)      136 2023-04-04 10:36:24.000000 lilit-1.2.0/docs/index.html
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 10:47:35.640811 lilit-1.2.0/docs/lilit/
--rw-rw-r--   0 jack      (1000) jack      (1000)   701863 2023-04-04 10:36:24.000000 lilit-1.2.0/docs/lilit/likelihood.html
--rw-rw-r--   0 jack      (1000) jack      (1000)    62222 2023-04-04 10:36:23.000000 lilit-1.2.0/docs/lilit.html
--rw-rw-r--   0 jack      (1000) jack      (1000)   196905 2023-04-04 10:36:24.000000 lilit-1.2.0/docs/search.js
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 10:47:35.644811 lilit-1.2.0/examples/
--rw-rw-r--   0 jack      (1000) jack      (1000)    10552 2023-03-13 10:51:04.000000 lilit-1.2.0/examples/experiments.yaml
--rw-rw-r--   0 jack      (1000) jack      (1000)     3863 2023-03-10 18:35:00.000000 lilit-1.2.0/examples/logBB.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)     4660 2023-03-10 19:11:31.000000 lilit-1.2.0/examples/logTTTEEE.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)     5102 2023-03-13 10:12:49.000000 lilit-1.2.0/examples/logTTTEEEBB.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)    13218 2023-03-25 19:08:04.000000 lilit-1.2.0/examples/other_simple_likelihood.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    11698 2023-03-03 18:27:08.000000 lilit-1.2.0/examples/planck_2018.ini
--rw-rw-r--   0 jack      (1000) jack      (1000)     3259 2023-04-20 15:07:20.000000 lilit-1.2.0/examples/samplingBB.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     5041 2023-03-25 19:13:19.000000 lilit-1.2.0/examples/samplingFULL.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     4380 2023-05-14 10:21:10.000000 lilit-1.2.0/examples/samplingTTTEEE.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 10:47:35.644811 lilit-1.2.0/lilit/
--rw-rw-r--   0 jack      (1000) jack      (1000)     8093 2023-05-14 10:44:10.000000 lilit-1.2.0/lilit/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    10552 2023-04-28 08:54:33.000000 lilit-1.2.0/lilit/experiments.yaml
--rw-rw-r--   0 jack      (1000) jack      (1000)     7692 2023-05-14 09:56:37.000000 lilit-1.2.0/lilit/functions.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    39256 2023-05-14 10:33:29.000000 lilit-1.2.0/lilit/likelihood.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    11698 2023-03-03 18:27:08.000000 lilit-1.2.0/lilit/planck_2018.ini
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 10:47:35.644811 lilit-1.2.0/lilit.egg-info/
--rw-rw-r--   0 jack      (1000) jack      (1000)     9231 2023-05-14 10:47:35.000000 lilit-1.2.0/lilit.egg-info/PKG-INFO
--rw-rw-r--   0 jack      (1000) jack      (1000)      586 2023-05-14 10:47:35.000000 lilit-1.2.0/lilit.egg-info/SOURCES.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-05-14 10:47:35.000000 lilit-1.2.0/lilit.egg-info/dependency_links.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)       43 2023-05-14 10:47:35.000000 lilit-1.2.0/lilit.egg-info/requires.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)        6 2023-05-14 10:47:35.000000 lilit-1.2.0/lilit.egg-info/top_level.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)       38 2023-05-14 10:47:35.644811 lilit-1.2.0/setup.cfg
--rw-rw-r--   0 jack      (1000) jack      (1000)     1005 2023-04-04 09:43:31.000000 lilit-1.2.0/setup.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 13:44:23.921509 lilit-1.2.1/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      107 2023-05-14 10:52:53.000000 lilit-1.2.1/.gitignore
+-rw-rw-r--   0 jack      (1000) jack      (1000)    35149 2023-03-30 14:20:30.000000 lilit-1.2.1/LICENSE
+-rw-rw-r--   0 jack      (1000) jack      (1000)     9231 2023-05-14 13:44:23.921509 lilit-1.2.1/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)     7972 2023-05-14 10:01:30.000000 lilit-1.2.1/README.md
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 13:44:23.921509 lilit-1.2.1/docs/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      136 2023-04-04 10:36:24.000000 lilit-1.2.1/docs/index.html
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 13:44:23.921509 lilit-1.2.1/docs/lilit/
+-rw-rw-r--   0 jack      (1000) jack      (1000)   701863 2023-04-04 10:36:24.000000 lilit-1.2.1/docs/lilit/likelihood.html
+-rw-rw-r--   0 jack      (1000) jack      (1000)    62222 2023-04-04 10:36:23.000000 lilit-1.2.1/docs/lilit.html
+-rw-rw-r--   0 jack      (1000) jack      (1000)   196905 2023-04-04 10:36:24.000000 lilit-1.2.1/docs/search.js
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 13:44:23.921509 lilit-1.2.1/examples/
+-rw-rw-r--   0 jack      (1000) jack      (1000)    10552 2023-03-13 10:51:04.000000 lilit-1.2.1/examples/experiments.yaml
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3863 2023-03-10 18:35:00.000000 lilit-1.2.1/examples/logBB.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4660 2023-03-10 19:11:31.000000 lilit-1.2.1/examples/logTTTEEE.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5102 2023-03-13 10:12:49.000000 lilit-1.2.1/examples/logTTTEEEBB.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)    13218 2023-03-25 19:08:04.000000 lilit-1.2.1/examples/other_simple_likelihood.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    11698 2023-03-03 18:27:08.000000 lilit-1.2.1/examples/planck_2018.ini
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3124 2023-05-14 12:34:24.000000 lilit-1.2.1/examples/samplingBB.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5041 2023-03-25 19:13:19.000000 lilit-1.2.1/examples/samplingFULL.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4797 2023-05-14 12:30:17.000000 lilit-1.2.1/examples/samplingTTTEEE.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 13:44:23.921509 lilit-1.2.1/lilit/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     8129 2023-05-14 13:41:06.000000 lilit-1.2.1/lilit/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    10552 2023-04-28 08:54:33.000000 lilit-1.2.1/lilit/experiments.yaml
+-rw-rw-r--   0 jack      (1000) jack      (1000)    10441 2023-05-14 13:38:08.000000 lilit-1.2.1/lilit/functions.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    39823 2023-05-14 12:38:14.000000 lilit-1.2.1/lilit/likelihood.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    11698 2023-03-03 18:27:08.000000 lilit-1.2.1/lilit/planck_2018.ini
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-05-14 13:44:23.921509 lilit-1.2.1/lilit.egg-info/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     9231 2023-05-14 13:44:23.000000 lilit-1.2.1/lilit.egg-info/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)      586 2023-05-14 13:44:23.000000 lilit-1.2.1/lilit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-05-14 13:44:23.000000 lilit-1.2.1/lilit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       43 2023-05-14 13:44:23.000000 lilit-1.2.1/lilit.egg-info/requires.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)        6 2023-05-14 13:44:23.000000 lilit-1.2.1/lilit.egg-info/top_level.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       38 2023-05-14 13:44:23.921509 lilit-1.2.1/setup.cfg
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1005 2023-04-04 09:43:31.000000 lilit-1.2.1/setup.py
```

### Comparing `lilit-1.2.0/LICENSE` & `lilit-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/PKG-INFO` & `lilit-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilit
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python package encoding a likelihood for LiteBIRD.
 Home-page: https://github.com/ggalloni/LiLit
 Author: Galloni, Giacomo
 Author-email: giacomo.galloni@roma2.infn.it
 License: GNU General Public License v3.0
 Description: # LiLit: Likelihood for LiteBIRD
```

### Comparing `lilit-1.2.0/README.md` & `lilit-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/docs/lilit/likelihood.html` & `lilit-1.2.1/docs/lilit/likelihood.html`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/docs/lilit.html` & `lilit-1.2.1/docs/lilit.html`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/docs/search.js` & `lilit-1.2.1/docs/search.js`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/examples/experiments.yaml` & `lilit-1.2.1/examples/experiments.yaml`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/examples/logBB.txt` & `lilit-1.2.1/examples/logBB.txt`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/examples/logTTTEEE.txt` & `lilit-1.2.1/examples/logTTTEEE.txt`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/examples/logTTTEEEBB.txt` & `lilit-1.2.1/examples/logTTTEEEBB.txt`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/examples/other_simple_likelihood.py` & `lilit-1.2.1/examples/other_simple_likelihood.py`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/examples/planck_2018.ini` & `lilit-1.2.1/examples/planck_2018.ini`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/examples/samplingBB.py` & `lilit-1.2.1/examples/samplingBB.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Sample on B-modes."""
 import time
 from mpi4py import MPI
 from cobaya.run import run
 from cobaya.log import LoggedError
 from lilit import LiLit
 
-debug = False
+debug = True
 name = "BB"
 lmax = 500
 
 r = 0.02
 nt = 0.1
 
 exactBB = LiLit(
@@ -90,15 +90,14 @@
                 "parameterization": 2,
                 "num_nu_massless": 2.046,
                 "share_delta_neff": True,
                 "YHe": 0.2454006,
                 "pivot_tensor": 0.01,
                 "num_massive_neutrinos": 1,
                 "theta_H0_range": [20, 100],
-                # "Accuracy.AccuracyBoost": 2, # This helps getting an extra squeeze on the accordance of Cobaya and Fiducial spectra
             },
         },
     },
 }
 
 comm = MPI.COMM_WORLD
 rank = comm.Get_rank()
```

### Comparing `lilit-1.2.0/examples/samplingFULL.py` & `lilit-1.2.1/examples/samplingFULL.py`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/examples/samplingTTTEEE.py` & `lilit-1.2.1/examples/samplingTTTEEE.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 """Sample on CMB temperature and E-modes."""
 import time
 from mpi4py import MPI
 from cobaya.run import run
 from cobaya.log import LoggedError
+import lilit
 from lilit import LiLit
 
+from lilit import functions as func
+
+print(func.get_keys(["t", "e"]))
+
+print(lilit.__version__)
+
 debug = True
 name = "TTTEEE"
 
 # Note that the order of these list has to be the same of the fields keyword
 lmin = [2, 20]
 lmax = [1500, 1200]
 fsky = [0.8, 0.5]
@@ -21,73 +28,80 @@
     nside=256,
     lmin=lmin,
     lmax=lmax,
     fsky=fsky,
     debug=debug,
 )
 
-gaussTTTEEE = LiLit(
-    name=name,
-    fields=["t", "e"],
-    like="gaussian",
-    experiment="PTEPLiteBIRD",
-    nside=256,
-    lmin=lmin,
-    lmax=lmax,
-    fsky=fsky,
-    debug=debug,
-)
+# gaussTTTEEE = LiLit(
+#     name=name,
+#     fields=["t", "e"],
+#     like="gaussian",
+#     experiment="PTEPLiteBIRD",
+#     nside=256,
+#     lmin=lmin,
+#     lmax=lmax,
+#     fsky=fsky,
+#     debug=debug,
+# )
 
 info = {
     "likelihood": {name: exactTTTEEE},
     "params": {
         "As": {"latex": "A_\\mathrm{s}", "value": "lambda logA: 1e-10*np.exp(logA)"},
         "H0": {"latex": "H_0", "max": 100, "min": 20},
+        # "H0": 67.32117,
         "cosmomc_theta": {
             "derived": False,
             "value": "lambda theta_MC_100: 1.e-2*theta_MC_100",
         },
         "logA": {
             "drop": True,
             "latex": "\\log(10^{10} A_\\mathrm{s})",
             "prior": {"max": 3.91, "min": 1.61},
             "proposal": 0.001,
-            "ref": {"dist": "norm", "loc": 3.044, "scale": 0.0001},
+            # "ref": {"dist": "norm", "loc": 3.04478383213, "scale": 0.0001},
+            "ref": 3.04478383213,
         },
         "mnu": 0.06,
         "ns": {
             "latex": "n_\\mathrm{s}",
             "prior": {"max": 1.2, "min": 0.8},
             "proposal": 0.002,
-            "ref": {"dist": "norm", "loc": 0.9660499, "scale": 0.0004},
+            # "ref": {"dist": "norm", "loc": 0.9660499, "scale": 0.0004},
+            "ref": 0.9660499,
         },
         "ombh2": {
             "latex": "\\Omega_\\mathrm{b} h^2",
             "prior": {"max": 0.1, "min": 0.005},
             "proposal": 0.0001,
-            "ref": {"dist": "norm", "loc": 0.0223828, "scale": 0.00001},
+            # "ref": {"dist": "norm", "loc": 0.0223828, "scale": 0.00001},
+            "ref": 0.0223828,
         },
         "omch2": {
             "latex": "\\Omega_\\mathrm{c} h^2",
             "prior": {"max": 0.99, "min": 0.001},
             "proposal": 0.0005,
-            "ref": {"dist": "norm", "loc": 0.1201075, "scale": 0.0001},
+            # "ref": {"dist": "norm", "loc": 0.1201075, "scale": 0.0001},
+            "ref": 0.1201075,
         },
         "tau": {
             "latex": "\\tau_\\mathrm{reio}",
             "prior": {"max": 0.8, "min": 0.01},
             "proposal": 0.003,
-            "ref": {"dist": "norm", "loc": 0.05430842, "scale": 0.0006},
+            # "ref": {"dist": "norm", "loc": 0.05430842, "scale": 0.0006},
+            "ref": 0.05430842,
         },
         "theta_MC_100": {
             "drop": True,
             "latex": "100\\theta_\\mathrm{MC}",
             "prior": {"max": 10, "min": 0.5},
             "proposal": 0.0002,
-            "ref": {"dist": "norm", "loc": 1.04109, "scale": 0.00004},
+            # "ref": {"dist": "norm", "loc": 1.04109, "scale": 0.00004},
+            "ref": 1.041456798,
             "renames": "theta",
         },
     },
     "output": f"chains/exact{name}_lmax{lmax}",
     "force": True,
     "resume": False,
     # "debug": True,
@@ -104,22 +118,25 @@
                 "bbn_predictor": "PArthENoPE_880.2_standard.dat",
                 "halofit_version": "mead",
                 "lens_potential_accuracy": 1,
                 "NonLinear": "NonLinear_both",  # This is necessary to be concordant with Planck2018 fiducial spectra
                 "max_l": 2700,  # This is necessary to get accurate lensing B-modes
                 "WantTransfer": True,  # This is necessary to be concordant with Planck2018 fiducial spectra
                 "Transfer.high_precision": True,  # This is necessary to be concordant with Planck2018 fiducial spectra (this will impact negatively on the performance, so you might want to switch it off. However, remember to chanfe the fiducial accordingly.)
+                "Reion.helium_delta_redshift": 0.4,
+                "Reion.helium_redshiftstart": 6.0,
+                "Reion.fraction": -1,
                 "parameterization": 2,
                 "num_nu_massless": 2.046,
                 "share_delta_neff": True,
                 "YHe": 0.2454006,
-                "pivot_tensor": 0.01,
+                "nu_mass_degeneracies": [0],
+                "pivot_tensor": 0.05,
                 "num_massive_neutrinos": 1,
                 "theta_H0_range": [20, 100],
-                # "Accuracy.AccuracyBoost": 2, # This helps getting an extra squeeze on the accordance of Cobaya and Fiducial spectra
             },
         },
     },
 }
 
 
 comm = MPI.COMM_WORLD
```

### Comparing `lilit-1.2.0/lilit/__init__.py` & `lilit-1.2.1/lilit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,11 +99,12 @@
 
 ## Support
 
 For additional details on how Cobaya works, I suggest to see the [documentation](https://cobaya.readthedocs.io/en/latest/), which is very good to find whatever is not working in you case. If you cannot find the problem there, feel free to open an issue.
 """
 
 from .likelihood import LiLit
+from .functions import CAMBres2dict
 
 __author__ = "Giacomo Galloni"
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __docformat__ = "numpy"
```

### Comparing `lilit-1.2.0/lilit/experiments.yaml` & `lilit-1.2.1/lilit/experiments.yaml`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/lilit/likelihood.py` & `lilit-1.2.1/lilit/likelihood.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from .functions import (
     get_keys,
     get_Gauss_keys,
     cov_filling,
     sigma,
     inv_sigma,
+    CAMBres2dict,
+    txt2dict,
 )
 
 
 class LiLit(Likelihood):
 
     """Class defining the Likelihood for LiteBIRD (LiLit).
 
@@ -152,15 +154,15 @@
         self.fields = fields
         self.n = len(fields)
         self.lmin = lmin
         self.like = like
         self.sep = sep
         self.cl_file = cl_file
         self.nl_file = nl_file
-        if self.nl_file.endswith(".txt"):
+        if self.nl_file is not None and self.nl_file.endswith(".txt"):
             self.mapping = mapping
         self.experiment = experiment
         if self.experiment is not None:
             # Check that the user has provided the nside if an experiment is used
             assert nside is not None, "You must provide an nside to compute the noise"
             self.nside = nside
         self.debug = debug
@@ -445,77 +447,77 @@
                 A ndarray containing the covariance matrices, with some singular ones.
         """
         # Select the indices corresponding to the zero diagonal
         idx = np.where(np.diag(mat) == 0)[0]
         # Delete the rows and columns from the matrix
         return np.delete(np.delete(mat, idx, axis=0), idx, axis=1)
 
-    def CAMBres2dict(self, camb_results):
-        """Takes the CAMB result product from get_cmb_power_spectra and convert it to a dictionary with the proper keys.
+    # def CAMBres2dict(self, camb_results):
+    #     """Takes the CAMB result product from get_cmb_power_spectra and convert it to a dictionary with the proper keys.
 
-        Parameters:
-            camb_results (CAMBdata):
-                CAMB result product from the method get_cmb_power_spectra.
-        """
-        # Get the number of multipoles
-        ls = np.arange(camb_results["total"].shape[0], dtype=np.int64)
-        # Mapping between the CAMB keys and the ones we want
-        mapping = {"tt": 0, "ee": 1, "bb": 2, "te": 3, "et": 3}
-        # Initialize the output dictionary
-        res = {"ell": ls}
-        # Loop over the keys we want
-        for key, i in mapping.items():
-            # Save the results
-            res[key] = camb_results["total"][:, i]
-        # Check if we want the lensing potential
-        if "pp" in self.keys:
-            # Get the lensing potential
-            cl_lens = camb_results.get("lens_potential")
-            # Check if it exists
-            if cl_lens is not None:
-                # Save it with the normalization to obtain phiphi
-                array = cl_lens[:, 0].copy()
-                array[2:] /= (res["ell"] * (res["ell"] + 1))[2:]
-                res["pp"] = array
-                # Check if we want the cross terms
-                if "pt" in self.keys and "pe" in self.keys:
-                    # Loop over the cross terms
-                    for i, cross in enumerate(["pt", "pe"]):
-                        # Save the result
-                        array = cl_lens[:, i + 1].copy()
-                        array[2:] /= np.sqrt(res["ell"] * (res["ell"] + 1))[2:]
-                        res[cross] = array
-                        # Save the symmetric term
-                        res[cross[::-1]] = res[cross]
-        return res
+    #     Parameters:
+    #         camb_results (CAMBdata):
+    #             CAMB result product from the method get_cmb_power_spectra.
+    #     """
+    #     # Get the number of multipoles
+    #     ls = np.arange(camb_results["total"].shape[0], dtype=np.int64)
+    #     # Mapping between the CAMB keys and the ones we want
+    #     mapping = {"tt": 0, "ee": 1, "bb": 2, "te": 3, "et": 3}
+    #     # Initialize the output dictionary
+    #     res = {"ell": ls}
+    #     # Loop over the keys we want
+    #     for key, i in mapping.items():
+    #         # Save the results
+    #         res[key] = camb_results["total"][:, i]
+    #     # Check if we want the lensing potential
+    #     if "pp" in self.keys:
+    #         # Get the lensing potential
+    #         cl_lens = camb_results.get("lens_potential")
+    #         # Check if it exists
+    #         if cl_lens is not None:
+    #             # Save it with the normalization to obtain phiphi
+    #             array = cl_lens[:, 0].copy()
+    #             array[2:] /= (res["ell"] * (res["ell"] + 1))[2:]
+    #             res["pp"] = array
+    #             # Check if we want the cross terms
+    #             if "pt" in self.keys and "pe" in self.keys:
+    #                 # Loop over the cross terms
+    #                 for i, cross in enumerate(["pt", "pe"]):
+    #                     # Save the result
+    #                     array = cl_lens[:, i + 1].copy()
+    #                     array[2:] /= np.sqrt(res["ell"] * (res["ell"] + 1))[2:]
+    #                     res[cross] = array
+    #                     # Save the symmetric term
+    #                     res[cross[::-1]] = res[cross]
+    #     return res
 
-    def txt2dict(self, txt, mapping=None, apply_ellfactor=None):
-        """Takes a txt file and convert it to a dictionary. This requires a way to map the columns to the keys. Also, it is possible to apply an ell factor to the Cls.
+    # def txt2dict(self, txt, mapping=None, apply_ellfactor=None):
+    #     """Takes a txt file and convert it to a dictionary. This requires a way to map the columns to the keys. Also, it is possible to apply an ell factor to the Cls.
 
-        Parameters:
-            txt (str):
-                Path to txt file containing the spectra as columns.
-            mapping (dict):
-                Dictionary containing the mapping. Keywords will become the new keywords and values represent the index of the corresponding column.
-        """
-        # Define the ell values from the length of the txt file
-        assert (
-            mapping is not None
-        ), "You must provide a way to map the columns of your txt to the keys of a dictionary"
-        res = {}
-        # Loop over the mapping and extract the corresponding column from the txt file
-        # and store it in the dictionary under the corresponding keyword
-        for key, i in mapping.items():
-            ls = np.arange(len(txt[:, i]), dtype=np.int64)
-            res["ell"] = ls
-            if apply_ellfactor:
-                res[key] = txt[:, i] * ls * (ls + 1) / 2 / np.pi
-            else:
-                res[key] = txt[:, i]
-        return res
+    #     Parameters:
+    #         txt (str):
+    #             Path to txt file containing the spectra as columns.
+    #         mapping (dict):
+    #             Dictionary containing the mapping. Keywords will become the new keywords and values represent the index of the corresponding column.
+    #     """
+    #     # Define the ell values from the length of the txt file
+    #     assert (
+    #         mapping is not None
+    #     ), "You must provide a way to map the columns of your txt to the keys of a dictionary"
+    #     res = {}
+    #     # Loop over the mapping and extract the corresponding column from the txt file
+    #     # and store it in the dictionary under the corresponding keyword
+    #     for key, i in mapping.items():
+    #         ls = np.arange(len(txt[:, i]), dtype=np.int64)
+    #         res["ell"] = ls
+    #         if apply_ellfactor:
+    #             res[key] = txt[:, i] * ls * (ls + 1) / 2 / np.pi
+    #         else:
+    #             res[key] = txt[:, i]
+    #     return res
 
     def prod_fidu(self):
         """Produce fiducial spectra or read the input ones.
 
         If the user has not provided a Cl file, this function will produce the fiducial power spectra starting from the CAMB inifile for Planck2018. The extra keywords defined will maximize the accordance between the fiducial Cls and the ones obtained from Cobaya. If B-modes are requested, the tensor-to-scalar ratio and the spectral tilt will be set to the requested values. Note that if you do not provide a tilt, this will follow the standard single-field consistency relation. If instead you provide a custom file, stores that.
         """
         # If a custom file is provided, use that
@@ -524,15 +526,15 @@
             if self.cl_file.endswith(".pkl"):
                 with open(self.cl_file, "rb") as pickle_file:
                     res = pickle.load(pickle_file)
             # Otherwise, load it as text file
             else:
                 txt = np.loadtxt(self.cl_file)
                 mapping = {"tt": 0, "ee": 1, "bb": 2, "te": 3, "et": 3}
-                res = self.txt2dict(txt, mapping)
+                res = txt2dict(txt, mapping)
             return res
 
         try:
             import camb
         except ImportError:
             print("CAMB seems to be not installed. Check the requirements.")
 
@@ -562,15 +564,15 @@
 
         results = camb.get_results(pars)
         res = results.get_cmb_power_spectra(
             CMB_unit="muK",
             lmax=self.lmax,
             raw_cl=False,
         )
-        return self.CAMBres2dict(res)
+        return CAMBres2dict(res, self.keys)
 
     def prod_noise(self):
         """Produce noise power spectra or read the input ones.
 
         If the user has not provided a noise file, this function will produce the noise power spectra for a given experiment with inverse noise weighting of white noise in each channel (TT, EE, BB). Note that you may want to have a look at the procedure since it is merely a place-holder. Indeed, you should provide a more realistic file from which to read the noise spectra, given that inverse noise weighting severely underestimates the amount of noise. If instead you provide the proper custom file, this method stores that.
         """
         # If the input noise file is a pickle file, load it.
@@ -579,15 +581,17 @@
             if self.nl_file.endswith(".pkl"):
                 with open(self.nl_file, "rb") as pickle_file:
                     res = pickle.load(pickle_file)
             # If not, load the file as a text file
             else:
                 _txt = np.loadtxt(self.nl_file)
                 # Convert the text file to a dictionary
-                res = self.txt2dict(_txt, self.mapping, apply_ellfactor=True)
+                res = txt2dict(
+                    _txt, self.mapping, apply_ellfactor=True
+                )  # eliminate this part, conversion can be done outside likelihood
             return res
 
         print(
             "***WARNING***: the inverse noise weighting performed here severely underestimates \
             the actual noise level of LiteBIRD. You should provide an input \
             noise power spectrum with a more realistic noise."
         )
@@ -683,16 +687,20 @@
     def initialize(self):
         """Initializes the fiducial spectra and the noise power spectra."""
         # Compute the fiducial and noise power spectra
         self.fiduCLS = self.prod_fidu()
         self.noiseCLS = self.prod_noise()
 
         # Compute the covariance matrices
-        self.fiduCOV = self.cov_filling(self.fiduCLS)
-        self.noiseCOV = self.cov_filling(self.noiseCLS)
+        self.fiduCOV = cov_filling(
+            self.fields, self.lmin, self.lmax, self.fiduCLS, self.lmins, self.lmaxs
+        )
+        self.noiseCOV = cov_filling(
+            self.fields, self.lmin, self.lmax, self.noiseCLS, self.lmins, self.lmaxs
+        )
 
         # Print some information for debugging
         if self.debug:
             print(f"Keys of fiducial CLs ---> {self.fiduCLS.keys()}")
             print(f"Keys of noise CLs ---> {self.noiseCLS.keys()}")
 
             print("\nPrinting the first few values to check that it starts from 0...")
@@ -759,16 +767,16 @@
         Parameters:
             i (int, optional):
                 ell index if needed. Defaults to 0.
         """
         # If the number of datasets is not equal to 1, then we have a
         # multi-dataset case, in which case we need to compute the
         # covariance matrix for each dataset.
-        ell = np.arange(0, self.lmax + 1, 1)
         if self.n != 1:
+            ell = np.arange(0, self.lmax + 1, 1)
             # We extract the covariance matrix and data for the ith
             # dataset.
             coba = self.coba[:, :, i]
             data = self.data[:, :, i]
             # If the determinant is equal to 0, then we need to reduce
             # the dimensionality of the data and covariance matrix.
             if np.linalg.det(coba) == 0:
@@ -782,14 +790,15 @@
             return (2 * ell[i] + 1) * (
                 np.trace(M) - np.linalg.slogdet(M)[1] - data.shape[0]
             )
         # If the number of datasets is equal to 1, then we have a single
         # dataset case, in which case we do not need to loop over the
         # datasets.
         else:
+            ell = np.arange(2, self.lmax + 1, 1)
             # We compute the matrix M using the covariance matrix and
             # the data.
             M = self.data / self.coba
             # We compute the chi-square term using M, the log of M, and
             # a constant value.
             return (2 * ell + 1) * (M - np.log(np.abs(M)) - 1)
 
@@ -852,44 +861,47 @@
         """Gets the log likelihood and pass it to Cobaya to carry on the MCMC process."""
         if self.debug:
             CAMBdata = self.provider.get_CAMBdata()
             pars = CAMBdata.Params
             print(pars)
 
         # Get the Cls from Cobaya
-        self.cobaCLs = self.provider.get_Cl(ell_factor=True)
+        self.cobaCLS = self.provider.get_Cl(ell_factor=True)
         ell = np.arange(0, self.lmax + 1, 1)
         for key, value in self.cobaCLS.items():
             if key == "pp":
                 value[2 : self.lmax + 1] = (
                     value[2 : self.lmax + 1] / (ell * (ell + 1))[2:]
                 )
             elif "p" in key:
                 value[2 : self.lmax + 1] = (
                     value[2 : self.lmax + 1] / np.sqrt(ell * (ell + 1))[2:]
                 )
             self.cobaCLS[key] = value[: self.lmax + 1]
 
         if self.debug:
-            print(f"Keys of Cobaya CLs ---> {self.cobaCLs.keys()}")
+            print(f"Keys of Cobaya CLs ---> {self.cobaCLS.keys()}")
 
-            field = list(self.cobaCLs.keys())[1]
+            field = list(self.cobaCLS.keys())[1]
             print("\nPrinting the first few values to check that it starts from 0...")
-            print(f"Cobaya CLs for {field.upper()} ---> {self.cobaCLs[field][0:5]}")
+            print(f"Cobaya CLs for {field.upper()} ---> {self.cobaCLS[field][0:5]}")
 
         # Fill the covariance matrix with the Cls from Cobaya
         self.cobaCOV = cov_filling(
             self.fields, self.lmin, self.lmax, self.cobaCLS, self.lmins, self.lmaxs
         )
 
         if self.debug:
             ell = np.arange(0, self.lmax + 1, 1)
-            plt.loglog(ell, self.fiduCOV[0, 0, :], label="Fiducial CLs")
-            plt.loglog(ell, self.cobaCOV[0, 0, :], label="Cobaya CLs", ls="--")
-            plt.loglog(ell, self.noiseCOV[0, 0, :], label="Noise CLs")
+            obs1 = 0
+            obs2 = 0
+            plt.plot(ell, self.fiduCOV[obs1, obs2, :], label="Fiducial CLs")
+            plt.plot(ell, self.cobaCOV[obs1, obs2, :], label="Cobaya CLs", ls="--")
+            plt.plot(ell, self.noiseCOV[obs1, obs2, :], label="Noise CLs")
+            plt.semilogx()
             plt.xlim(2, None)
             plt.legend()
             plt.show()
 
         # Add the noise covariance to the covariance matrix filled with the Cls from Cobaya
         self.coba = (
             self.cobaCOV[:, :, self.lmin : self.lmax + 1]
```

### Comparing `lilit-1.2.0/lilit/planck_2018.ini` & `lilit-1.2.1/lilit/planck_2018.ini`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/lilit.egg-info/PKG-INFO` & `lilit-1.2.1/lilit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilit
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python package encoding a likelihood for LiteBIRD.
 Home-page: https://github.com/ggalloni/LiLit
 Author: Galloni, Giacomo
 Author-email: giacomo.galloni@roma2.infn.it
 License: GNU General Public License v3.0
 Description: # LiLit: Likelihood for LiteBIRD
```

### Comparing `lilit-1.2.0/lilit.egg-info/SOURCES.txt` & `lilit-1.2.1/lilit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lilit-1.2.0/setup.py` & `lilit-1.2.1/setup.py`

 * *Files identical despite different names*

