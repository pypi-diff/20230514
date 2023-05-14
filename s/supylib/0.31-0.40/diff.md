# Comparing `tmp/supylib-0.31.tar.gz` & `tmp/supylib-0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ak/projects/supylib/dist/tmp66_2pt52/supylib-0.31.tar", last modified: Wed May  3 17:06:52 2023, max compression
+gzip compressed data, was "/home/ak/projects/supylib/dist/tmpomaj5t0b/supylib-0.40.tar", last modified: Sun May 14 14:03:30 2023, max compression
```

## Comparing `supylib-0.31.tar` & `supylib-0.40.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 17:06:52.000000 supylib-0.31/
--rw-rw-r--   0 ak        (1000) ak        (1000)     1118 2022-03-09 09:38:11.000000 supylib-0.31/LICENSE
--rw-r--r--   0 ak        (1000) ak        (1000)     1211 2023-05-03 17:05:22.000000 supylib-0.31/README.md
-drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 17:06:52.000000 supylib-0.31/python/
-drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 17:06:52.000000 supylib-0.31/python/supylib.egg-info/
--rw-rw-r--   0 ak        (1000) ak        (1000)        5 2023-05-03 17:06:52.000000 supylib-0.31/python/supylib.egg-info/top_level.txt
--rw-rw-r--   0 ak        (1000) ak        (1000)        1 2023-05-03 17:06:52.000000 supylib-0.31/python/supylib.egg-info/dependency_links.txt
--rw-rw-r--   0 ak        (1000) ak        (1000)      671 2023-05-03 17:06:52.000000 supylib-0.31/python/supylib.egg-info/SOURCES.txt
--rw-rw-r--   0 ak        (1000) ak        (1000)     1825 2023-05-03 17:06:52.000000 supylib-0.31/python/supylib.egg-info/PKG-INFO
-drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-03 17:06:52.000000 supylib-0.31/python/supy/
--rw-r--r--   0 ak        (1000) ak        (1000)    12807 2019-02-28 09:55:09.000000 supylib-0.31/python/supy/forms.py
--rw-rw-r--   0 ak        (1000) ak        (1000)   170861 2023-05-03 16:18:00.000000 supylib-0.31/python/supy/signal.py
--rw-r--r--   0 ak        (1000) ak        (1000)     6868 2022-09-08 14:57:35.000000 supylib-0.31/python/supy/guimaker3.py
--rw-r--r--   0 ak        (1000) ak        (1000)    40317 2022-03-09 08:59:15.000000 supylib-0.31/python/supy/sqltableeditor.py
--rw-r--r--   0 ak        (1000) ak        (1000)     7965 2022-03-09 08:57:33.000000 supylib-0.31/python/supy/multibase.py
--rw-r--r--   0 ak        (1000) ak        (1000)     6871 2019-02-28 09:56:23.000000 supylib-0.31/python/supy/guimaker.py
--rw-r--r--   0 ak        (1000) ak        (1000)    17745 2022-03-09 08:58:19.000000 supylib-0.31/python/supy/sqldatabase_inputmask.py
--rw-r--r--   0 ak        (1000) ak        (1000)    20272 2022-03-09 08:54:20.000000 supylib-0.31/python/supy/database_inputmask3.py
--rw-r--r--   0 ak        (1000) ak        (1000)    20266 2022-03-09 08:55:21.000000 supylib-0.31/python/supy/database_inputmask.py
--rw-r--r--   0 ak        (1000) ak        (1000)    19500 2022-03-09 08:55:47.000000 supylib-0.31/python/supy/database.py
--rw-r--r--   0 ak        (1000) ak        (1000)    31946 2022-03-09 09:01:33.000000 supylib-0.31/python/supy/widgets.py
--rw-r--r--   0 ak        (1000) ak        (1000)     5419 2022-03-09 08:57:58.000000 supylib-0.31/python/supy/serialize.py
--rw-r--r--   0 ak        (1000) ak        (1000)   106175 2022-03-09 09:00:49.000000 supylib-0.31/python/supy/sqlforms.py
--rw-r--r--   0 ak        (1000) ak        (1000)    42485 2022-03-09 08:56:45.000000 supylib-0.31/python/supy/forms3.py
--rw-rw-r--   0 ak        (1000) ak        (1000)       22 2023-05-03 17:03:01.000000 supylib-0.31/python/supy/__init__.py
--rw-r--r--   0 ak        (1000) ak        (1000)    30059 2022-03-09 08:58:51.000000 supylib-0.31/python/supy/sqldatabase.py
--rw-r--r--   0 ak        (1000) ak        (1000)     5226 2022-03-09 09:01:13.000000 supylib-0.31/python/supy/utilities.py
--rw-r--r--   0 ak        (1000) ak        (1000)    76826 2023-04-14 09:28:16.000000 supylib-0.31/python/supy/computervision.py
--rw-rw-r--   0 ak        (1000) ak        (1000)      708 2023-05-03 17:06:52.000000 supylib-0.31/setup.cfg
--rw-rw-r--   0 ak        (1000) ak        (1000)      104 2022-03-09 09:36:04.000000 supylib-0.31/pyproject.toml
--rw-rw-r--   0 ak        (1000) ak        (1000)     1825 2023-05-03 17:06:52.000000 supylib-0.31/PKG-INFO
+drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-14 14:03:29.000000 supylib-0.40/
+-rw-rw-r--   0 ak        (1000) ak        (1000)     1118 2022-03-09 09:38:11.000000 supylib-0.40/LICENSE
+-rw-r--r--   0 ak        (1000) ak        (1000)     4473 2023-05-14 13:55:33.000000 supylib-0.40/README.md
+drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-14 14:03:29.000000 supylib-0.40/python/
+drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-14 14:03:29.000000 supylib-0.40/python/supylib.egg-info/
+-rw-rw-r--   0 ak        (1000) ak        (1000)        5 2023-05-14 14:03:29.000000 supylib-0.40/python/supylib.egg-info/top_level.txt
+-rw-rw-r--   0 ak        (1000) ak        (1000)        1 2023-05-14 14:03:29.000000 supylib-0.40/python/supylib.egg-info/dependency_links.txt
+-rw-rw-r--   0 ak        (1000) ak        (1000)      692 2023-05-14 14:03:29.000000 supylib-0.40/python/supylib.egg-info/SOURCES.txt
+-rw-rw-r--   0 ak        (1000) ak        (1000)     5087 2023-05-14 14:03:29.000000 supylib-0.40/python/supylib.egg-info/PKG-INFO
+drwxrwxr-x   0 ak        (1000) ak        (1000)        0 2023-05-14 14:03:29.000000 supylib-0.40/python/supy/
+-rw-r--r--   0 ak        (1000) ak        (1000)    12807 2019-02-28 09:55:09.000000 supylib-0.40/python/supy/forms.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     6868 2022-09-08 14:57:35.000000 supylib-0.40/python/supy/guimaker3.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    40317 2022-03-09 08:59:15.000000 supylib-0.40/python/supy/sqltableeditor.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     7965 2022-03-09 08:57:33.000000 supylib-0.40/python/supy/multibase.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     6871 2019-02-28 09:56:23.000000 supylib-0.40/python/supy/guimaker.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    17745 2022-03-09 08:58:19.000000 supylib-0.40/python/supy/sqldatabase_inputmask.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    20272 2022-03-09 08:54:20.000000 supylib-0.40/python/supy/database_inputmask3.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    20266 2022-03-09 08:55:21.000000 supylib-0.40/python/supy/database_inputmask.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    19500 2022-03-09 08:55:47.000000 supylib-0.40/python/supy/database.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    31946 2022-03-09 09:01:33.000000 supylib-0.40/python/supy/widgets.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     5419 2022-03-09 08:57:58.000000 supylib-0.40/python/supy/serialize.py
+-rw-rw-r--   0 ak        (1000) ak        (1000)   171599 2023-05-14 10:37:26.000000 supylib-0.40/python/supy/signals.py
+-rw-r--r--   0 ak        (1000) ak        (1000)   106175 2022-03-09 09:00:49.000000 supylib-0.40/python/supy/sqlforms.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    42485 2022-03-09 08:56:45.000000 supylib-0.40/python/supy/forms3.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    45710 2023-05-14 10:23:38.000000 supylib-0.40/python/supy/rgps.py
+-rw-rw-r--   0 ak        (1000) ak        (1000)       22 2023-05-14 13:16:01.000000 supylib-0.40/python/supy/__init__.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    30059 2022-03-09 08:58:51.000000 supylib-0.40/python/supy/sqldatabase.py
+-rw-r--r--   0 ak        (1000) ak        (1000)     5226 2022-03-09 09:01:13.000000 supylib-0.40/python/supy/utilities.py
+-rw-r--r--   0 ak        (1000) ak        (1000)    76826 2023-04-14 09:28:16.000000 supylib-0.40/python/supy/computervision.py
+-rw-rw-r--   0 ak        (1000) ak        (1000)      708 2023-05-14 14:03:29.000000 supylib-0.40/setup.cfg
+-rw-rw-r--   0 ak        (1000) ak        (1000)      104 2022-03-09 09:36:04.000000 supylib-0.40/pyproject.toml
+-rw-rw-r--   0 ak        (1000) ak        (1000)     5087 2023-05-14 14:03:29.000000 supylib-0.40/PKG-INFO
```

### Comparing `supylib-0.31/LICENSE` & `supylib-0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supylib.egg-info/SOURCES.txt` & `supylib-0.40/python/supylib.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 python/supy/database_inputmask.py
 python/supy/database_inputmask3.py
 python/supy/forms.py
 python/supy/forms3.py
 python/supy/guimaker.py
 python/supy/guimaker3.py
 python/supy/multibase.py
+python/supy/rgps.py
 python/supy/serialize.py
-python/supy/signal.py
+python/supy/signals.py
 python/supy/sqldatabase.py
 python/supy/sqldatabase_inputmask.py
 python/supy/sqlforms.py
 python/supy/sqltableeditor.py
 python/supy/utilities.py
 python/supy/widgets.py
 python/supylib.egg-info/PKG-INFO
```

### Comparing `supylib-0.31/python/supy/forms.py` & `supylib-0.40/python/supy/forms.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/signal.py` & `supylib-0.40/python/supy/signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
 import numpy as np
 from scipy.special import erf, erfcinv
 
 # ***************************************************************************************
 # ***************************************************************************************
 # ***************************************************************************************
-# SUPY_SIGNAL.PY
-# -------------------------
+# SUPY_SIGNSYS.PY    - TOOLBOX FOR SIGNAL AND SYSTEMS
+# ----------------------------------------------------
 # Version 16/04/2023, Andreas Knoblauch, HS Albstadt-Sigmaringen, Germany
 # EXPERIMENTAL SOFTWARE: NO WARRANTIES! REGULARLY BACKUP YOUR DATA!
+# former name: signal.py  (renamed on 14/5/2023) 
 #
 # CONTENTS:
 # -------------------------
 # Part I) Linear Algebra and Optimization Operations
 #  - def inv3(A,eps=1e-12)
 #  - def inv3_arr(A)
 #  - def inv3sym(A,eps=1e-12)
@@ -1059,15 +1060,15 @@
     """
     Unsupervised Signal Detection Algorithm employing Truncated Gaussian Moments to estimate background noise and set optimal threshold for extracting the signal (see NB36/17.4.2023 and cf., AB4/pp299-301, AB5/pp1-5)
     For earlier implementation of the algorithm see also: ~/hs-albsig/02-research/Borst_Fledermaeuse/python/OLD_ARCHIVE/ivisit_spekview_v1_3_20230427.py  
                                                           --> in step(), line 182, (iv) Unsupervised Signal Detection with Truncated Gaussians
                                                           --> to be started with: python ivisit_spekview_v1_3_20230427.py ivisit_spekview_v1_3_20230427.db
     :param x: the raw signal where the signal detection algorithm should be applied to (1D array); 
               it is assumed that x is composed of the signal plus additive stationary Gaussian noise (with some mean mu0_est, variance sig02_est and noise data number N0_est)
-    :param fac_p_decision: parameter determining threshold for signal detection; 
+    :param fac_p_decision: parameter determining threshold for signal detection; either float or list of floats (in the latter case resulting theta will also be a list)
                            set decision threshold to the smallest bin (see parameters p_binsize and max_binsize) larger than the mean and satisfying p(signal)>=fac_p_decision*p(noise)
                            e.g., fac_p_decision=1 corresponds to a maximum accuracy decision setting the threshold to the first bin where p(signal)>=p(noise) holds
                            e.g., fac_p_decision=5 corresponds to a larger threshold where p(signal)>=5*p(noise), where p(.) corresponds to estimated probability density within the bins of the data histogram
                            where it is assumed that signal is larger than noise on average (see also parameters list_ptrunc_a/b)
     :param nEstimates: number of parallel estimations of noise distribution parameters (mu0_est,sig02_est), each using different initialization parameters; 
                        as the convergence of the Newton algorithm depends on initial parameters, doing only a single estimation may give bad estimates or even diverge (to NaN);
                        therefore it is recommended using nEstimates>1, e.g., nEstimates=10
@@ -1092,15 +1093,14 @@
     :param p_binsize:   determines binsize=max(1,len(x)*p_binsize) (in data number per bin) of the histograms used for estimating the mode of the data distribution (as initial estimate for the noise mean mu0_est) 
                         and to determine the decision threshold (see parameter fac_p_decision); each bin of the histogram contains binsize data values (except possibly the last one)
                         The binsize should be much smaller than the data number len(x), e.g., binsize<len(x)/100 to have enough "resolution" to obtain mode estimate and decision threshold with sufficient precision
     :param max_binsize: Bound binsize to values smaller than max_binsize, that is, binsize=max(1,min(max_binsize,len(x)*p_binsize))
     :param p_cutoff_mode: for determining mode of data distribution, cut of fraction p_cutoff_mode/2 from both below and above to avoide extreme values of densities (which may occur, e.g., if the data range is bounded)
                           As the mode for Gaussian background noise and sparse signal data should be close to the median, we can safely cut off, for example,
                           10% from below and 10% from above (corresponding to default value p_cutoff_mode=0.2) 
-                          
     """
 
     # (i) prepare data and compute mode and histograms 
     binsize=max(1,min(max_binsize,int(len(x)*p_binsize)))                                                     # determine bin size for histogram analysis
     binsize=max_binsize #200 #!!!!
     x_sorted=np.sort(x)                                                                                       # sort data values for estimation of mode and density of data distribution from histograms
     mode,p_mode,dummy1,dummy2,dummy3 = getModeOfDensity(x,binsize=binsize,p_cutoff=p_cutoff_mode,x_sorted=x_sorted)       # get mode of data distribution (most frequent value of histogram values) 
@@ -1143,27 +1143,32 @@
         N0_est    = res['N_est_best'   ][idx_best]
         E         = res['E_best'       ][idx_best]
         nablaE    = res['DE_best'      ][:,idx_best]
         H_E       = res['DDE_best'     ][:,idx_best]
         tau       = res['tau'          ]
         np.seterr(**old_err_settings)               # reactivate warnings (set to previous state) 
 
-    # (v) determine decision threshold 
+    # (v) determine decision threshold
     minhist,maxhist=np.min(x),np.max(x)     # minimal and maximal data value
     yy0 = N0_est/np.sqrt(2*np.pi*sig02_est)*np.exp(-0.5*np.multiply(bin_centers-mu0_est,bin_centers-mu0_est)/sig02_est)   # theoretical class 0 histogram density (# expected data points per length) at histogram centers
     yy01_x=len(x)*bin_density                                                                                          # empirical histogram density for both class 0 and class 1
     yy1=yy01_x-yy0                          # histogram density of class 1  (whereas yy0 is estimated histogram density of class 0)
     min_theta=np.max(list_b)                # upper interval bounds b are assumed to belong to class 0
-    idx_theta=np.argmax(np.logical_and(yy1>fac_p_decision*yy0,\
-                                       bin_centers>min_theta))  # get index of lowest threshold (beyond min_theta), where class1 has a larger density (times fac_p_decision) than class 0 to maximize classification accuracy
-    if idx_theta==0:                   # no values available where class 1 has larger density than class 0 
-        #theta=maxhist*1.01            # previous choice: --> then set theta above maximum of histogram values
-        theta=mu0_est+np.sqrt(2*sig02_est)*erfcinv(2.0/(fac_p_decision*len(x)))   # maybe better choice: set threshold such that 1/fac_p_decision false class 1 sample occurs on average (see AB5/pp8-9/24.4.2023)
-    else:
-        theta=bin_centers[idx_theta]   # decision threshold
+    fac_p_dec_list=fac_p_decision                                              # list of decision factors
+    if not isinstance(fac_p_dec_list, list): fac_p_dec_list=[fac_p_dec_list]   # enforce list
+    theta,idx_theta=[],[]
+    for i in range(len(fac_p_dec_list)):    # iterate over all decision factors to compute a corresponding decision threshold
+        idx_theta+=[np.argmax(np.logical_and(yy1>fac_p_dec_list[i]*yy0,\
+                                             bin_centers>min_theta))] # get index of lowest threshold (beyond min_theta), where class1 has a larger density (times fac_p_decision) than class 0 to maximize classif. accuracy
+        if idx_theta[i]==0:                 # no values available where class 1 has larger density than class 0 
+            #theta=maxhist*1.01             # previous choice: --> then set theta above maximum of histogram values
+            theta+=[mu0_est+np.sqrt(2*sig02_est)*erfcinv(2.0/(fac_p_dec_list[i]*len(x)))]   # maybe better choice: set threshold such that 1/fac_p_decision false class 1 sample occurs on average (see AB5/pp8-9/24.4.2023)
+        else:
+            theta+=[bin_centers[idx_theta[i]]] # decision threshold
+    if not isinstance(fac_p_decision, list): theta,idx_theta=theta[0],idx_theta[0]  # enforce type for theta being same as for fac_p_decision
 
     # (vi) return results as data dict
     dd={}
     dd['res']=res
     dd['idx_best']=idx_best
     dd['mu0_est']=mu0_est
     dd['sig02_est']=sig02_est
@@ -1185,14 +1190,15 @@
     dd['binsize']=binsize
     dd['bin_centers']=bin_centers
     dd['bin_density']=bin_density
     dd['bin_widths' ]=bin_widths
     dd['yy0']=yy0
     dd['yy01_x']=yy01_x
     dd['yy1']=yy1
+    dd['min_theta']=min_theta
     return dd
 
 ##################################################################################################################################################################
 ##################################################################################################################################################################
 ##################################################################################################################################################################
 # Part XX: Module test
 ##################################################################################################################################################################
```

### Comparing `supylib-0.31/python/supy/guimaker3.py` & `supylib-0.40/python/supy/guimaker3.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/sqltableeditor.py` & `supylib-0.40/python/supy/sqltableeditor.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/multibase.py` & `supylib-0.40/python/supy/multibase.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/guimaker.py` & `supylib-0.40/python/supy/guimaker.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/sqldatabase_inputmask.py` & `supylib-0.40/python/supy/sqldatabase_inputmask.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/database_inputmask3.py` & `supylib-0.40/python/supy/database_inputmask3.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/database_inputmask.py` & `supylib-0.40/python/supy/database_inputmask.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/database.py` & `supylib-0.40/python/supy/database.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/widgets.py` & `supylib-0.40/python/supy/widgets.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/serialize.py` & `supylib-0.40/python/supy/serialize.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/sqlforms.py` & `supylib-0.40/python/supy/sqlforms.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/forms3.py` & `supylib-0.40/python/supy/forms3.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/sqldatabase.py` & `supylib-0.40/python/supy/sqldatabase.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/utilities.py` & `supylib-0.40/python/supy/utilities.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/python/supy/computervision.py` & `supylib-0.40/python/supy/computervision.py`

 * *Files identical despite different names*

### Comparing `supylib-0.31/setup.cfg` & `supylib-0.40/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = supylib
-version = 0.31
+version = 0.40
 author = Andreas Knoblauch
 author_email = knoblauch@hs-albsig.de
 description = A Python-based utility library for databases, computer vision, signal processing, and machine learning
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/aknoblauch/supylib
 project_urls =
```

