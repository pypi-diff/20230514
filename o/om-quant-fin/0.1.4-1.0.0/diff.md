# Comparing `tmp/om_quant_fin-0.1.4.tar.gz` & `tmp/om_quant_fin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "om_quant_fin-0.1.4.tar", last modified: Thu May  4 19:59:08 2023, max compression
+gzip compressed data, was "om_quant_fin-1.0.0.tar", last modified: Sun May 14 10:28:47 2023, max compression
```

## Comparing `om_quant_fin-0.1.4.tar` & `om_quant_fin-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:59:08.141865 om_quant_fin-0.1.4/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2588 2023-05-04 19:59:08.141684 om_quant_fin-0.1.4/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2012 2023-05-04 19:58:47.000000 om_quant_fin-0.1.4/README.md
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:59:08.140711 om_quant_fin-0.1.4/om_quant_fin/
--rw-r--r--   0 leandroguerra   (501) staff       (20)      201 2023-05-04 19:12:22.000000 om_quant_fin-0.1.4/om_quant_fin/__init__.py
--rw-r--r--   0 leandroguerra   (501) staff       (20)     3999 2023-05-04 18:28:26.000000 om_quant_fin-0.1.4/om_quant_fin/om_quant_fin.py
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-04 19:59:08.141487 om_quant_fin-0.1.4/om_quant_fin.egg-info/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     2588 2023-05-04 19:59:08.000000 om_quant_fin-0.1.4/om_quant_fin.egg-info/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-04 19:59:08.000000 om_quant_fin-0.1.4/om_quant_fin.egg-info/SOURCES.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-04 19:59:08.000000 om_quant_fin-0.1.4/om_quant_fin.egg-info/dependency_links.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       35 2023-05-04 19:59:08.000000 om_quant_fin-0.1.4/om_quant_fin.egg-info/requires.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-04 19:59:08.000000 om_quant_fin-0.1.4/om_quant_fin.egg-info/top_level.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-04 19:59:08.141924 om_quant_fin-0.1.4/setup.cfg
--rw-r--r--   0 leandroguerra   (501) staff       (20)     1066 2023-05-04 19:58:56.000000 om_quant_fin-0.1.4/setup.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-14 10:28:47.528271 om_quant_fin-1.0.0/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     4103 2023-05-14 10:28:47.528107 om_quant_fin-1.0.0/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     3461 2023-05-14 10:27:07.000000 om_quant_fin-1.0.0/README.md
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-14 10:28:47.527095 om_quant_fin-1.0.0/om_quant_fin/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      201 2023-05-04 19:12:22.000000 om_quant_fin-1.0.0/om_quant_fin/__init__.py
+-rw-r--r--   0 leandroguerra   (501) staff       (20)    11873 2023-05-14 10:27:36.000000 om_quant_fin-1.0.0/om_quant_fin/om_quant_fin.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-14 10:28:47.527920 om_quant_fin-1.0.0/om_quant_fin.egg-info/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     4103 2023-05-14 10:28:47.000000 om_quant_fin-1.0.0/om_quant_fin.egg-info/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-14 10:28:47.000000 om_quant_fin-1.0.0/om_quant_fin.egg-info/SOURCES.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-14 10:28:47.000000 om_quant_fin-1.0.0/om_quant_fin.egg-info/dependency_links.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       51 2023-05-14 10:28:47.000000 om_quant_fin-1.0.0/om_quant_fin.egg-info/requires.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-14 10:28:47.000000 om_quant_fin-1.0.0/om_quant_fin.egg-info/top_level.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-14 10:28:47.528329 om_quant_fin-1.0.0/setup.cfg
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     1181 2023-05-14 10:27:40.000000 om_quant_fin-1.0.0/setup.py
```

### Comparing `om_quant_fin-0.1.4/setup.py` & `om_quant_fin-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,29 +6,32 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name = "om_quant_fin",
-    version = "0.1.4",
+    version = "1.0.0",
     packages = find_packages(),
     install_requires = [
         "yfinance",
         "pandas",
         "scikit-learn",
-        "numpy"
+        "numpy",
+        "time",
+        "sys",
+        "plotly"
     ],
     author = "Outspoken Market",
     author_email = "info@outspokenmarket.com",
-    description = "A simple quantitative trading library for the OMNP Class",
+    description = "A modern Python library for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.",
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     classifiers = [
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
 )
```

