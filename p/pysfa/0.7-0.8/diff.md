# Comparing `tmp/pysfa-0.7.tar.gz` & `tmp/pysfa-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysfa-0.7.tar", last modified: Fri May 12 14:06:46 2023, max compression
+gzip compressed data, was "pysfa-0.8.tar", last modified: Sun May 14 17:36:55 2023, max compression
```

## Comparing `pysfa-0.7.tar` & `pysfa-0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:06:46.440327 pysfa-0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 14:06:35.000000 pysfa-0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-12 14:06:46.440327 pysfa-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-12 14:06:35.000000 pysfa-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:06:46.436327 pysfa-0.7/pysfa/
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-05-12 14:06:35.000000 pysfa-0.7/pysfa/SFA.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-12 14:06:35.000000 pysfa-0.7/pysfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-12 14:06:35.000000 pysfa-0.7/pysfa/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:06:46.440327 pysfa-0.7/pysfa/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-12 14:06:35.000000 pysfa-0.7/pysfa/data/41Firm.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-12 14:06:35.000000 pysfa-0.7/pysfa/data/electricityFirms.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-12 14:06:35.000000 pysfa-0.7/pysfa/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:06:46.440327 pysfa-0.7/pysfa/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 14:06:35.000000 pysfa-0.7/pysfa/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-12 14:06:35.000000 pysfa-0.7/pysfa/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:06:46.436327 pysfa-0.7/pysfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-12 14:06:46.000000 pysfa-0.7/pysfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-12 14:06:46.000000 pysfa-0.7/pysfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:06:46.000000 pysfa-0.7/pysfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:06:46.000000 pysfa-0.7/pysfa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 14:06:46.000000 pysfa-0.7/pysfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 14:06:46.000000 pysfa-0.7/pysfa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 14:06:46.440327 pysfa-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-12 14:06:35.000000 pysfa-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:36:55.314136 pysfa-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-14 17:36:41.000000 pysfa-0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-14 17:36:55.314136 pysfa-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-14 17:36:41.000000 pysfa-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:36:55.310136 pysfa-0.8/pysfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-14 17:36:41.000000 pysfa-0.8/pysfa/SFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-14 17:36:41.000000 pysfa-0.8/pysfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-14 17:36:41.000000 pysfa-0.8/pysfa/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:36:55.310136 pysfa-0.8/pysfa/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-14 17:36:41.000000 pysfa-0.8/pysfa/data/41Firm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-14 17:36:41.000000 pysfa-0.8/pysfa/data/electricityFirms.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-14 17:36:41.000000 pysfa-0.8/pysfa/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:36:55.314136 pysfa-0.8/pysfa/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 17:36:41.000000 pysfa-0.8/pysfa/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-14 17:36:41.000000 pysfa-0.8/pysfa/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:36:55.310136 pysfa-0.8/pysfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-14 17:36:55.000000 pysfa-0.8/pysfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-14 17:36:55.000000 pysfa-0.8/pysfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:36:55.000000 pysfa-0.8/pysfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:36:55.000000 pysfa-0.8/pysfa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-14 17:36:55.000000 pysfa-0.8/pysfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 17:36:55.000000 pysfa-0.8/pysfa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:36:55.314136 pysfa-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-14 17:36:41.000000 pysfa-0.8/setup.py
```

### Comparing `pysfa-0.7/LICENSE` & `pysfa-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pysfa-0.7/PKG-INFO` & `pysfa-0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pysfa
-Version: 0.7
+Version: 0.8
 Summary: A Python Package for Stochastic Frontier Analysis
 Home-page: https://github.com/gEAPA/pySFA
 Download-URL: https://pypi.org/project/pysfa/
 Author: Sheng Dai, Zhiqiang Liao
 Author-email: sheng.dai@utu.fi
 License: MIT
 Keywords: SFA,MLE,TE
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -48,15 +48,15 @@
 df = load_Tim_Coelli_frontier(x_select=['labour', 'capital'],
                               y_select=['output'])
 y = np.log(df.y)
 x = np.log(df.x)
 
 # Estimate SFA model
 res = SFA.SFA(y, x, fun=SFA.FUN_PROD, method=SFA.TE_teJ)
-
+res.optimize()
 # print estimates
 print(res.get_beta())
 print(res.get_residuals())
 
 # print estimated parameters
 print(res.get_lambda())
 print(res.get_sigma2())
@@ -64,10 +64,13 @@
 print(res.get_sigmav2())
 
 # print statistics
 print(res.get_pvalue())
 print(res.get_tvalue())
 print(res.get_std_err())
 
+# OR print summary
+print(res.summary())
+
 # print TE
 print(res.get_technical_efficiency())
 ```
```

### Comparing `pysfa-0.7/README.md` & `pysfa-0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 df = load_Tim_Coelli_frontier(x_select=['labour', 'capital'],
                               y_select=['output'])
 y = np.log(df.y)
 x = np.log(df.x)
 
 # Estimate SFA model
 res = SFA.SFA(y, x, fun=SFA.FUN_PROD, method=SFA.TE_teJ)
-
+res.optimize()
 # print estimates
 print(res.get_beta())
 print(res.get_residuals())
 
 # print estimated parameters
 print(res.get_lambda())
 print(res.get_sigma2())
@@ -46,10 +46,13 @@
 print(res.get_sigmav2())
 
 # print statistics
 print(res.get_pvalue())
 print(res.get_tvalue())
 print(res.get_std_err())
 
+# OR print summary
+print(res.summary())
+
 # print TE
 print(res.get_technical_efficiency())
 ```
```

### Comparing `pysfa-0.7/pysfa/SFA.py` & `pysfa-0.8/pysfa/SFA.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import pandas as pd
 from sklearn.linear_model import LinearRegression
 from math import sqrt, pi, log
 from scipy.stats import norm, t
 from scipy.optimize import minimize
 from .constant import FUN_PROD, FUN_COST, TE_teJ, TE_te, TE_teMod
 from .utils import tools
 
@@ -26,15 +27,15 @@
         self.y, self.x = tools.assert_valid_basic_data(y, x, self.fun)
 
         if self.fun == FUN_COST:
             self.sign = -1
         else:
             self.sign = 1
 
-    def __mle(self):
+    def optimize(self):
 
         # initial OLS regression
         if self.intercept == False:
             reg = LinearRegression(fit_intercept=False).fit(X=self.x, y=self.y)
             parm = np.concatenate((reg.coef_, [self.lamda0]), axis=0)
         elif self.intercept == True:
             reg = LinearRegression().fit(X=self.x, y=self.y)
@@ -52,119 +53,116 @@
             beta0, lamda0 = parm[0:K], parm[K]
             res = self.__resfun(beta0)
             sig2 = np.sum(res**2)/N
             z = -lamda0*res/sqrt(sig2)
             pz = np.maximum(norm.cdf(z), 1e-323)
             return N/2*log(pi/2) + N/2*log(sig2) - np.sum(np.log(pz)) + N/2.0
 
-        fit = minimize(__loglik, parm, method='BFGS')
-
-        # beta, residuals, lambda, sigma^2
-        if self.intercept == False:
-            K = len(self.x[0])
-        elif self.intercept == True:
-            K = len(self.x[0]) + 1
-        self.beta = fit.x[0:K]
-        self.residuals = self.__resfun(self.beta)
-        self.lamda = fit.x[K]
-        self.sigma2 = np.sum(self.residuals ** 2)/self.residuals.shape[0]
-
-        # sigma_u^2, sigma_v^2
-        self.s2u = self.lamda**2 / (1+self.lamda**2) * self.sigma2
-        self.s2v = self.sigma2 / (1+self.lamda**2)
-
-        # calculate standard error, t-value, and p-value
-        self.vcov = fit.hess_inv
-        self.std_err = np.sqrt(np.diag(self.vcov))
-        self.tvalue = fit.x / self.std_err
-        self.pvalue = np.around(
-            2 * t.sf(abs(self.tvalue), len(self.x) - K), decimals=3)
+        return minimize(__loglik, parm, method='BFGS')
 
     def __resfun(self, beta):
+        ''' Residual function'''
         if self.intercept == False:
             return self.y - np.dot(self.x, beta[0:])
         elif self.intercept == True:
             return self.y - beta[0] - np.dot(self.x, beta[1:])
 
+    def get_beta(self):
+        '''Return the estimated coefficients'''
+        return self.optimize().x[0:-1]
+
+    def get_lambda(self):
+        '''Return the estimated lambda'''
+        return self.optimize().x[-1]
+
+    def get_residuals(self):
+        '''Return the estimated residuals'''
+        return self.__resfun(self.optimize().x[0:-1])
+
+    def get_sigma2(self):
+        '''Return the estimated sigma2'''
+        return np.sum(self.get_residuals()**2)/len(self.x)
+
+    def get_sigmau2(self):
+        '''Return the estimated sigmau2'''
+        return self.get_lambda()**2 / (1 + self.get_lambda()**2) * self.get_sigma2()
+
+    def get_sigmav2(self):
+        '''Return the estimated sigmav2'''
+        return self.get_sigma2()/(1 + self.get_lambda()**2)
+
+    def get_std_err(self):
+        '''Return the standard errors'''
+        return np.sqrt(np.diag(self.optimize().hess_inv))
+
+    def get_tvalue(self):
+        '''Return the t-values'''
+        return self.optimize().x/self.get_std_err()
+
+    def get_pvalue(self):
+        '''Return the p-values'''
+        if self.intercept == False:
+            K = len(self.x[0])
+        elif self.intercept == True:
+            K = len(self.x[0]) + 1
+        return np.around(2*t.sf(np.abs(self.get_tvalue()), len(self.x) - K), decimals=3)
+
     def __teJ(self):
         '''Efficiencies estimates using the conditional mean approach 
             Jondrow et al. (1982, 235)'''
 
-        self.ustar = - self.sign * self.residuals * \
-            self.lamda**2/(1+self.lamda**2)
-        self.sstar = self.lamda/(1+self.lamda**2)*sqrt(self.sigma2)
+        self.ustar = - self.sign * self.get_residuals() * \
+            self.get_lambda()**2/(1+self.get_lambda()**2)
+        self.sstar = self.get_lambda()/(1+self.get_lambda()**2)*sqrt(self.get_sigma2())
         return np.exp(-self.ustar - self.sstar *
                       (norm.pdf(self.ustar/self.sstar)/norm.cdf(self.ustar/self.sstar)))
 
     def __te(self):
         '''Efficiencies estimated by minimizing the mean square error; 
             Eq. (7.21) in Bogetoft and Otto (2011, 219) and Battese and Coelli (1988, 392)'''
 
-        self.ustar = - self.sign * self.residuals * \
-            self.lamda**2/(1+self.lamda**2)
-        self.sstar = self.lamda/(1+self.lamda**2)*sqrt(self.sigma2)
+        self.ustar = - self.sign * self.get_residuals() * \
+            self.get_lambda()**2/(1+self.get_lambda()**2)
+        self.sstar = self.get_lambda()/(1+self.get_lambda()**2)*sqrt(self.get_sigma2())
         return norm.cdf(self.ustar/self.sstar - self.sstar) / \
             norm.cdf(self.ustar/self.sstar) * \
             np.exp(self.sstar**2/2 - self.ustar)
 
     def __teMod(self):
         '''Efficiencies estimates using the conditional mode approach;
             Bogetoft and Otto (2011, 219), Jondrow et al. (1982, 235)'''
 
-        self.ustar = - self.sign * self.residuals * \
-            self.lamda**2/(1+self.lamda**2)
+        self.ustar = - self.sign * self.get_residuals() * \
+            self.get_lambda()**2/(1+self.get_lambda()**2)
         return np.exp(np.minimum(0, -self.ustar))
 
-    def __model_estimation(self):
-        '''Model estimation'''
+    def get_technical_efficiency(self):
+        '''Return the technical efficiency estimates'''
 
-        self.__mle()
         if self.method == TE_teJ:
-            self.te = self.__teJ()
+            return self.__teJ()
         elif self.method == TE_te:
-            self.te = self.__te()
+            return self.__te()
         elif self.method == TE_teMod:
-            self.te = self.__teMod()
+            return self.__teMod()
         else:
             raise ValueError("Undefined decomposition technique.")
 
-        return self.beta, self.residuals, self.lamda, self.sigma2, self.s2u, self.s2v, self.std_err, self.tvalue, self.pvalue, self.te
-
-    def get_beta(self):
-        '''Return the estimated coefficients'''
-        return self.__model_estimation()[0]
-
-    def get_residuals(self):
-        '''Return the residuals'''
-        return self.__model_estimation()[1]
-
-    def get_lambda(self):
-        '''Return the lambda'''
-        return self.__model_estimation()[2]
-
-    def get_sigma2(self):
-        '''Return the sigma2'''
-        return self.__model_estimation()[3]
-
-    def get_sigmau2(self):
-        '''Return the sigma_u**2'''
-        return self.__model_estimation()[4]
+    def summary(self):
+        '''Print the summary of the estimation results'''
 
-    def get_sigmav2(self):
-        '''Return the sigma_v**2'''
-        return self.__model_estimation()[5]
-
-    def get_std_err(self):
-        '''Return the standard errors'''
-        return self.__model_estimation()[6]
-
-    def get_tvalue(self):
-        '''Return the standard errors'''
-        return self.__model_estimation()[7]
-
-    def get_pvalue(self):
-        '''Return the standard errors'''
-        return self.__model_estimation()[8]
+        if self.intercept == False:
+            self.names = ['x'+str(i+1)
+                          for i in range(len(self.x[0]))] + ['lambda']
+        elif self.intercept == True:
+            self.names = ['(Intercept)'] + ['x'+str(i+1)
+                                            for i in range(len(self.x[0]))] + ['lambda']
 
-    def get_technical_efficiency(self):
-        '''Return the technical efficiency'''
-        return self.__model_estimation()[9]
+        output = np.vstack(
+            (np.round(self.optimize().x, decimals=5), np.round(self.get_std_err(), decimals=6), np.round(self.get_tvalue(), decimals=3), self.get_pvalue()))
+        index = ['Parameters', 'Std.err', 't-value', 'Pr(>|t|)']
+        re = pd.DataFrame(output, index=index, columns=self.names).T
+        print(re)
+        print('sigma2: ', self.get_sigma2().round(5))
+        print('sigmav2: ', self.get_sigmav2().round(5),
+              '; sigmau2: ', self.get_sigmau2().round(5))
+        print('log likelihood: ', round(self.optimize().fun, 5))
```

### Comparing `pysfa-0.7/pysfa/constant.py` & `pysfa-0.8/pysfa/constant.py`

 * *Files identical despite different names*

### Comparing `pysfa-0.7/pysfa/data/41Firm.csv` & `pysfa-0.8/pysfa/data/41Firm.csv`

 * *Files identical despite different names*

### Comparing `pysfa-0.7/pysfa/data/electricityFirms.csv` & `pysfa-0.8/pysfa/data/electricityFirms.csv`

 * *Files identical despite different names*

### Comparing `pysfa-0.7/pysfa/dataset.py` & `pysfa-0.8/pysfa/dataset.py`

 * *Files identical despite different names*

### Comparing `pysfa-0.7/pysfa/utils/tools.py` & `pysfa-0.8/pysfa/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pysfa-0.7/pysfa.egg-info/PKG-INFO` & `pysfa-0.8/pysfa.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pysfa
-Version: 0.7
+Version: 0.8
 Summary: A Python Package for Stochastic Frontier Analysis
 Home-page: https://github.com/gEAPA/pySFA
 Download-URL: https://pypi.org/project/pysfa/
 Author: Sheng Dai, Zhiqiang Liao
 Author-email: sheng.dai@utu.fi
 License: MIT
 Keywords: SFA,MLE,TE
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -48,15 +48,15 @@
 df = load_Tim_Coelli_frontier(x_select=['labour', 'capital'],
                               y_select=['output'])
 y = np.log(df.y)
 x = np.log(df.x)
 
 # Estimate SFA model
 res = SFA.SFA(y, x, fun=SFA.FUN_PROD, method=SFA.TE_teJ)
-
+res.optimize()
 # print estimates
 print(res.get_beta())
 print(res.get_residuals())
 
 # print estimated parameters
 print(res.get_lambda())
 print(res.get_sigma2())
@@ -64,10 +64,13 @@
 print(res.get_sigmav2())
 
 # print statistics
 print(res.get_pvalue())
 print(res.get_tvalue())
 print(res.get_std_err())
 
+# OR print summary
+print(res.summary())
+
 # print TE
 print(res.get_technical_efficiency())
 ```
```

### Comparing `pysfa-0.7/setup.py` & `pysfa-0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='pysfa',
-    version='0.7',
+    version='0.8',
     description='A Python Package for Stochastic Frontier Analysis',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Sheng Dai, Zhiqiang Liao',
     author_email='sheng.dai@utu.fi',
     keywords=['SFA', 'MLE', 'TE'],
     url='https://github.com/gEAPA/pySFA',
     download_url='https://pypi.org/project/pysfa/',
     include_package_data=True,
     zip_safe=False,
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     package_data={'pysfa': ['data/*.csv']},
 )
```

