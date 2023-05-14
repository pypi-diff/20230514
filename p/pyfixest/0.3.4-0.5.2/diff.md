# Comparing `tmp/pyfixest-0.3.4.tar.gz` & `tmp/pyfixest-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfixest-0.3.4.tar", max compression
+gzip compressed data, was "pyfixest-0.5.2.tar", max compression
```

## Comparing `pyfixest-0.3.4.tar` & `pyfixest-0.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.3.4/LICENSE.md
--rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.3.4/pyfixest/__init__.py
--rw-r--r--   0        0        0     9613 2023-03-21 20:34:46.351334 pyfixest-0.3.4/pyfixest/feols.py
--rw-r--r--   0        0        0    22639 2023-04-01 14:20:37.440084 pyfixest-0.3.4/pyfixest/fixest.py
--rw-r--r--   0        0        0    14183 2023-03-28 21:31:50.654617 pyfixest-0.3.4/pyfixest/FormulaParser.py
--rw-r--r--   0        0        0     1089 2023-03-28 21:31:50.660731 pyfixest-0.3.4/pyfixest/utils.py
--rw-r--r--   0        0        0      516 2023-04-01 14:31:11.186077 pyfixest-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1763 2023-03-16 21:08:28.608240 pyfixest-0.3.4/readme.md
--rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 pyfixest-0.3.4/setup.py
--rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 pyfixest-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-11-19 12:53:04.921992 pyfixest-0.5.2/LICENSE.md
+-rw-r--r--   0        0        0       26 2023-03-16 21:51:51.234748 pyfixest-0.5.2/pyfixest/__init__.py
+-rw-r--r--   0        0        0    18071 2023-05-14 09:06:59.564643 pyfixest-0.5.2/pyfixest/feols.py
+-rw-r--r--   0        0        0    39786 2023-05-14 09:06:59.566819 pyfixest-0.5.2/pyfixest/fixest.py
+-rw-r--r--   0        0        0    17794 2023-05-13 20:24:52.625359 pyfixest-0.5.2/pyfixest/FormulaParser.py
+-rw-r--r--   0        0        0     3426 2023-04-27 19:03:35.062476 pyfixest-0.5.2/pyfixest/ssc_utils.py
+-rw-r--r--   0        0        0     1172 2023-05-13 20:24:52.632640 pyfixest-0.5.2/pyfixest/utils.py
+-rw-r--r--   0        0        0      863 2023-05-14 09:13:14.061103 pyfixest-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2684 2023-05-13 20:24:52.634902 pyfixest-0.5.2/readme.md
+-rw-r--r--   0        0        0     3535 1970-01-01 00:00:00.000000 pyfixest-0.5.2/PKG-INFO
```

### Comparing `pyfixest-0.3.4/LICENSE.md` & `pyfixest-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfixest-0.3.4/pyfixest/FormulaParser.py` & `pyfixest-0.5.2/pyfixest/FormulaParser.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,23 +47,58 @@
         # Clean up the formula string
         fml = "".join(fml.split())
 
         # Split the formula string into its components
         fml_split = fml.split('|')
         depvars, covars = fml_split[0].split("~")
 
-        if len(fml_split) > 1:
-            fevars = fml_split[1]
-        else:
+        if len(fml_split) == 1:
             fevars = "0"
+            endogvars = None
+            instruments = None
+        elif len(fml_split) == 2:
+            if "~" in fml_split[1]:
+                fevars = "0"
+                endogvars, instruments = fml_split[1].split("~")
+            else:
+                fevars = fml_split[1]
+                endogvars = None
+                instruments = None
+        elif len(fml_split) == 3:
+            fevars = fml_split[1]
+            endogvars, instruments = fml_split[2].split("~")
+
+        if endogvars is not None:
+            if len(endogvars) > len(instruments):
+                raise ValueError("The IV system is underdetermined. Only fully determined systems are allowed. Please provide as many instruments as endogenous variables.")
+            elif len(endogvars) < len(instruments):
+                raise ValueError("The IV system is overdetermined. Only fully determined systems are allowed. Please provide as many instruments as endogenous variables.")
+            else:
+                pass
 
         # Parse all individual formula components into lists
         self.depvars = depvars.split("+")
         self.covars = _unpack_fml(covars)
         self.fevars = _unpack_fml(fevars)
+        # no fancy syntax for endogvars, instruments allowed
+        self.endogvars = endogvars
+        self.instruments = instruments
+
+        if instruments is not None:
+            self.is_iv = True
+            # all rhs variables for the first stage (endog variable replaced with instrument)
+            first_stage_covars_list = covars.split("+")
+            first_stage_covars_list[first_stage_covars_list.index(endogvars)] = instruments
+            self.first_stage_covars_list = "+".join(first_stage_covars_list)
+            self.covars_first_stage = _unpack_fml(self.first_stage_covars_list)
+            self.depvars_first_stage = endogvars
+        else:
+            self.is_iv = False
+            self.covars_first_stage = None
+            self.depvars_first_stage = None
 
         if self.covars.get("i") is not None:
             self.ivars = dict()
             i_split = self.covars.get("i")[-1].split("=")
             if len(i_split) > 1:
                 ref = self.covars.get("i")[-1].split("=")[1]
                 ivar_list = self.covars.get("i")[:-1]
@@ -77,83 +112,128 @@
         else:
             self.ivars = None
 
 
         # Pack the formula components back into strings
         self.covars_fml = _pack_to_fml(self.covars)
         self.fevars_fml = _pack_to_fml(self.fevars)
-
+        if instruments is not None: 
+            self.covars_first_stage_fml = _pack_to_fml(self.covars_first_stage)
+        else: 
+            self.covars_first_stage_fml = None
         #if "^" in self.covars:
         #    raise CovariateInteractionError("Please use 'i()' or ':' syntax to interact covariates.")
 
         #for  x in ["i", ":"]:
         #    if x in self.fevars:
         #        raise FixedEffectInteractionError("Interacting fixed effects via", x, " is not allowed. Please use '^' to interact fixed effects.")
 
 
 
 
 
-    def get_fml_dict(self):
+    def get_fml_dict(self, iv = False):
 
         """
         Returns a dictionary of all fevars & formula without fevars. The keys are the fixed effect variable combinations.
         The values are lists of formula strings that do not include the fixed effect variables.
 
+        Args:
+            iv (bool): If True, the formula dictionary will be returned for the first stage of an IV regression.
+                       If False, the formula dictionary will be returned for the second stage of an IV regression / OLS regression.
         Returns:
             dict: A dictionary of the form {"fe1+fe2": ['Y1 ~ X', 'Y2~X'], "fe1+fe3": ['Y1 ~ X', 'Y2~X']} where
             the keys are the fixed effect variable combinations and the values are lists of formula strings
             that do not include the fixed effect variables.
+            If IV is True, creates an instance named fml_dict_iv. Otherwise, creates an instance named fml_dict.
         """
 
-        self.fml_dict = dict()
+
+        fml_dict = dict()
         for fevar in self.fevars_fml:
             res = []
             for depvar in self.depvars:
-               for covar in self.covars_fml:
-                   res.append(depvar + '~' + covar)
-            self.fml_dict[fevar] = res
+                if iv:
+                    for covar in self.covars_first_stage_fml:
+                        res.append(depvar + '~' + covar)
+                else:
+                    for covar in self.covars_fml:
+                        res.append(depvar + '~' + covar)
+            fml_dict[fevar] = res
 
+        if iv:
+            self.fml_dict_iv = fml_dict
+        else:
+            self.fml_dict = fml_dict
 
-    def _transform_fml_dict(self):
+    def _transform_fml_dict(self, iv = False):
 
         fml_dict2 = dict()
 
-        for fe in self.fml_dict.keys():
+        if iv:
 
-            fml_dict2[fe] = dict()
+            for fe in self.fml_dict_iv.keys():
 
-            for fml in self.fml_dict.get(fe):
-                depvars, covars = fml.split("~")
-                if fml_dict2[fe].get(depvars) is None:
-                    fml_dict2[fe][depvars] = [covars]
-                else:
-                    fml_dict2[fe][depvars].append(covars)
+                fml_dict2[fe] = dict()
 
-        self.fml_dict2 = fml_dict2
+                for fml in self.fml_dict_iv.get(fe):
+                    depvars, covars = fml.split("~")
+                    if fml_dict2[fe].get(depvars) is None:
+                        fml_dict2[fe][depvars] = [covars]
+                    else:
+                        fml_dict2[fe][depvars].append(covars)
+        else:
+
+          for fe in self.fml_dict.keys():
+
+              fml_dict2[fe] = dict()
+
+              for fml in self.fml_dict.get(fe):
+                  depvars, covars = fml.split("~")
+                  if fml_dict2[fe].get(depvars) is None:
+                      fml_dict2[fe][depvars] = [covars]
+                  else:
+                      fml_dict2[fe][depvars].append(covars)
+
+        if iv:
+            self.fml_dict2_iv = fml_dict2
+        else:
+            self.fml_dict2 = fml_dict2
 
 
 
-    def get_var_dict(self):
+    def get_var_dict(self, iv = False):
 
         """
         Create a dictionary of all fevars and list of covars and depvars used in regression with those fevars.
         The keys are the fixed effect variable combinations. The values are lists of variables (dependent variables and covariates) of
         the resespective regressions.
 
+        Args:
+            iv (bool): If True, the formula dictionary will be returned for the first stage of an IV regression.
+
         Returns:
             dict: A dictionary of the form {"fe1+fe2": ['Y1', 'X1', 'X2'], "fe1+fe3": ['Y1', 'X1', 'X2']} where
             the keys are the fixed effect variable combinations and the values are lists of variables
             (dependent variables and covariates) used in the regression with those fixed effect variables.
 
         """
-        self.var_dict = dict()
-        for fevar in self.fevars_fml:
-              self.var_dict[fevar] = _flatten_list(self.depvars) + _flatten_list(list(self.covars.values()))
+        var_dict = dict()
+        if iv:
+            for fevar in self.fevars_fml:
+                var_dict[fevar] = _flatten_list(self.depvars) + _flatten_list(list(self.covars_first_stage.values()))
 
+        else:
+            for fevar in self.fevars_fml:
+                var_dict[fevar] = _flatten_list(self.depvars) + _flatten_list(list(self.covars.values()))
+
+        if iv:
+            self.var_dict_iv = var_dict
+        else:
+            self.var_dict = var_dict
 
 
 def _unpack_fml(x):
 
     '''
     Given a formula string `x` - e.g. 'X1 + csw(X2, X3)' - , splits it into its constituent variables and their types (if any),
     and returns a dictionary containing the result. The dictionary has the following keys: 'constant', 'sw', 'sw0', 'csw'.
```

### Comparing `pyfixest-0.3.4/pyfixest/utils.py` & `pyfixest-0.5.2/pyfixest/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
 import pandas as pd
 
-def get_data():
+def get_data(seed = 1234):
 
     '''
     create a random example data set
     '''
 
     # create data
 
-    np.random.seed(1231)
+    np.random.seed(seed)
 
-    N = 6000
-    k = 5
+    N = 2000
+    k = 20
     G = 25
     X = np.random.normal(0, 1, N * k).reshape((N,k))
     X = pd.DataFrame(X)
     X[1] = np.random.choice(list(range(0, 5)), N, True)
     X[2] = np.random.choice(list(range(0, 10)), N, True)
     X[3] = np.random.choice(list(range(0, 10)), N, True)
     X[4] = np.random.normal(0, 1, N)
@@ -35,11 +35,13 @@
     data.rename(columns = {0:'X1', 1:'X2', 2:'X3', 3:'X4', 4:'X5'}, inplace = True)
 
     data['group_id'] = cluster
     data['Y2'] = data.Y + np.random.normal(0, 1, N)
 
     data['Y'][0] = np.nan
     data['X1'][1] = np.nan
+
+    data["Z1"] = data["X1"] + np.random.normal(0, 1, data.shape[0])
     #data['X2'][2] = np.nan
 
 
     return data
```

