# Comparing `tmp/om_quant_fin-1.0.0.tar.gz` & `tmp/om_quant_fin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "om_quant_fin-1.0.0.tar", last modified: Sun May 14 10:28:47 2023, max compression
+gzip compressed data, was "om_quant_fin-1.0.1.tar", last modified: Sun May 14 10:34:51 2023, max compression
```

## Comparing `om_quant_fin-1.0.0.tar` & `om_quant_fin-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-14 10:28:47.528271 om_quant_fin-1.0.0/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     4103 2023-05-14 10:28:47.528107 om_quant_fin-1.0.0/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)     3461 2023-05-14 10:27:07.000000 om_quant_fin-1.0.0/README.md
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-14 10:28:47.527095 om_quant_fin-1.0.0/om_quant_fin/
--rw-r--r--   0 leandroguerra   (501) staff       (20)      201 2023-05-04 19:12:22.000000 om_quant_fin-1.0.0/om_quant_fin/__init__.py
--rw-r--r--   0 leandroguerra   (501) staff       (20)    11873 2023-05-14 10:27:36.000000 om_quant_fin-1.0.0/om_quant_fin/om_quant_fin.py
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-14 10:28:47.527920 om_quant_fin-1.0.0/om_quant_fin.egg-info/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     4103 2023-05-14 10:28:47.000000 om_quant_fin-1.0.0/om_quant_fin.egg-info/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-14 10:28:47.000000 om_quant_fin-1.0.0/om_quant_fin.egg-info/SOURCES.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-14 10:28:47.000000 om_quant_fin-1.0.0/om_quant_fin.egg-info/dependency_links.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       51 2023-05-14 10:28:47.000000 om_quant_fin-1.0.0/om_quant_fin.egg-info/requires.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-14 10:28:47.000000 om_quant_fin-1.0.0/om_quant_fin.egg-info/top_level.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-14 10:28:47.528329 om_quant_fin-1.0.0/setup.cfg
--rw-r--r--   0 leandroguerra   (501) staff       (20)     1181 2023-05-14 10:27:40.000000 om_quant_fin-1.0.0/setup.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-14 10:34:51.236713 om_quant_fin-1.0.1/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     4121 2023-05-14 10:34:51.236562 om_quant_fin-1.0.1/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     3479 2023-05-14 10:34:21.000000 om_quant_fin-1.0.1/README.md
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-14 10:34:51.235714 om_quant_fin-1.0.1/om_quant_fin/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      241 2023-05-14 10:34:27.000000 om_quant_fin-1.0.1/om_quant_fin/__init__.py
+-rw-r--r--   0 leandroguerra   (501) staff       (20)    11873 2023-05-14 10:34:31.000000 om_quant_fin-1.0.1/om_quant_fin/om_quant_fin.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-14 10:34:51.236372 om_quant_fin-1.0.1/om_quant_fin.egg-info/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     4121 2023-05-14 10:34:51.000000 om_quant_fin-1.0.1/om_quant_fin.egg-info/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-14 10:34:51.000000 om_quant_fin-1.0.1/om_quant_fin.egg-info/SOURCES.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-14 10:34:51.000000 om_quant_fin-1.0.1/om_quant_fin.egg-info/dependency_links.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       51 2023-05-14 10:34:51.000000 om_quant_fin-1.0.1/om_quant_fin.egg-info/requires.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-14 10:34:51.000000 om_quant_fin-1.0.1/om_quant_fin.egg-info/top_level.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-14 10:34:51.236768 om_quant_fin-1.0.1/setup.cfg
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     1181 2023-05-14 10:34:40.000000 om_quant_fin-1.0.1/setup.py
```

### Comparing `om_quant_fin-1.0.0/PKG-INFO` & `om_quant_fin-1.0.1/om_quant_fin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: om_quant_fin
-Version: 1.0.0
+Name: om-quant-fin
+Version: 1.0.1
 Summary: A modern Python library for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
 Home-page: UNKNOWN
 Author: Outspoken Market
 Author-email: info@outspokenmarket.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
 # OM Quant Fin
 
-OM Quant Fin is a modern Python library for quantitative trading analysis. Our mission is to make your quant life easier.
+OM Quant Fin is a modern Python library for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
 
 ## Project Structure
 
 ```python
 om_quant_fin/               # Root directory of the project
 ├── om_quant_fin/           # Python package containing the library's code
 │   ├── __init__.py         # Marks the directory as a package and can contain package-level code or imports
```

### Comparing `om_quant_fin-1.0.0/README.md` & `om_quant_fin-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # OM Quant Fin
 
-OM Quant Fin is a modern Python library for quantitative trading analysis. Our mission is to make your quant life easier.
+OM Quant Fin is a modern Python library for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
 
 ## Project Structure
 
 ```python
 om_quant_fin/               # Root directory of the project
 ├── om_quant_fin/           # Python package containing the library's code
 │   ├── __init__.py         # Marks the directory as a package and can contain package-level code or imports
```

### Comparing `om_quant_fin-1.0.0/om_quant_fin/om_quant_fin.py` & `om_quant_fin-1.0.1/om_quant_fin/om_quant_fin.py`

 * *Files identical despite different names*

### Comparing `om_quant_fin-1.0.0/om_quant_fin.egg-info/PKG-INFO` & `om_quant_fin-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: om-quant-fin
-Version: 1.0.0
+Name: om_quant_fin
+Version: 1.0.1
 Summary: A modern Python library for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
 Home-page: UNKNOWN
 Author: Outspoken Market
 Author-email: info@outspokenmarket.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
 # OM Quant Fin
 
-OM Quant Fin is a modern Python library for quantitative trading analysis. Our mission is to make your quant life easier.
+OM Quant Fin is a modern Python library for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
 
 ## Project Structure
 
 ```python
 om_quant_fin/               # Root directory of the project
 ├── om_quant_fin/           # Python package containing the library's code
 │   ├── __init__.py         # Marks the directory as a package and can contain package-level code or imports
```

### Comparing `om_quant_fin-1.0.0/setup.py` & `om_quant_fin-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name = "om_quant_fin",
-    version = "1.0.0",
+    version = "1.0.1",
     packages = find_packages(),
     install_requires = [
         "yfinance",
         "pandas",
         "scikit-learn",
         "numpy",
         "time",
```

