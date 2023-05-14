# Comparing `tmp/emi_calculator-1.0.1.tar.gz` & `tmp/emi_calculator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emi_calculator-1.0.1.tar", last modified: Sun May 14 16:13:23 2023, max compression
+gzip compressed data, was "emi_calculator-1.0.2.tar", last modified: Sun May 14 17:12:52 2023, max compression
```

## Comparing `emi_calculator-1.0.1.tar` & `emi_calculator-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 16:13:23.870902 emi_calculator-1.0.1/
--rw-rw-rw-   0        0        0     3395 2023-05-14 16:13:23.869462 emi_calculator-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 16:13:23.866391 emi_calculator-1.0.1/emi_calculator.egg-info/
--rw-rw-rw-   0        0        0     3395 2023-05-14 16:13:23.000000 emi_calculator-1.0.1/emi_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-05-14 16:13:23.000000 emi_calculator-1.0.1/emi_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 16:13:23.000000 emi_calculator-1.0.1/emi_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 16:13:23.000000 emi_calculator-1.0.1/emi_calculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 16:13:23.871894 emi_calculator-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3557 2023-05-14 16:09:21.000000 emi_calculator-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:12:52.611766 emi_calculator-1.0.2/
+-rw-rw-rw-   0        0        0     3395 2023-05-14 17:12:52.609610 emi_calculator-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-14 17:12:52.607036 emi_calculator-1.0.2/emi_calculator.egg-info/
+-rw-rw-rw-   0        0        0     3395 2023-05-14 17:12:50.000000 emi_calculator-1.0.2/emi_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-05-14 17:12:50.000000 emi_calculator-1.0.2/emi_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 17:12:50.000000 emi_calculator-1.0.2/emi_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 17:12:50.000000 emi_calculator-1.0.2/emi_calculator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 17:12:52.612768 emi_calculator-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3557 2023-05-14 17:12:28.000000 emi_calculator-1.0.2/setup.py
```

### Comparing `emi_calculator-1.0.1/PKG-INFO` & `emi_calculator-1.0.2/emi_calculator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: emi_calculator
-Version: 1.0.1
+Name: emi-calculator
+Version: 1.0.2
 Summary: The EMI Library is a Python library that provides a convenient way to calculate the Equated Monthly Installment (EMI) for loans. The library implements the EMI formula, which takes into account the principal loan amount, interest rate, and tenure in months.
 Home-page: https://github.com/Zack1o1/emi-calculator
 Author: Lalit Rajbanshi
 Author-email: lalitrajbanshi45@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `emi_calculator-1.0.1/emi_calculator.egg-info/PKG-INFO` & `emi_calculator-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: emi-calculator
-Version: 1.0.1
+Name: emi_calculator
+Version: 1.0.2
 Summary: The EMI Library is a Python library that provides a convenient way to calculate the Equated Monthly Installment (EMI) for loans. The library implements the EMI formula, which takes into account the principal loan amount, interest rate, and tenure in months.
 Home-page: https://github.com/Zack1o1/emi-calculator
 Author: Lalit Rajbanshi
 Author-email: lalitrajbanshi45@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `emi_calculator-1.0.1/setup.py` & `emi_calculator-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='emi_calculator',
-    version='1.0.1',
+    version='1.0.2',
     author='Lalit Rajbanshi',
     author_email='lalitrajbanshi45@gmail.com',
     description='The EMI Library is a Python library that provides a convenient way to calculate the Equated Monthly Installment (EMI) for loans. The library implements the EMI formula, which takes into account the principal loan amount, interest rate, and tenure in months.',
     long_description="""
             EMI Calculator Library
             =====================
```

