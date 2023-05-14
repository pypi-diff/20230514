# Comparing `tmp/PySciMath-1.5.2.tar.gz` & `tmp/PySciMath-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.5.2.tar", last modified: Sun May 14 06:31:52 2023, max compression
+gzip compressed data, was "PySciMath-1.5.3.tar", last modified: Sun May 14 06:48:17 2023, max compression
```

## Comparing `PySciMath-1.5.2.tar` & `PySciMath-1.5.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 06:31:52.623158 PySciMath-1.5.2/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.5.2/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2023-05-14 06:30:09.000000 PySciMath-1.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2591 2023-05-14 06:31:52.621164 PySciMath-1.5.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-14 06:31:52.531414 PySciMath-1.5.2/PySciMath/
--rw-rw-rw-   0        0        0     2090 2023-05-12 06:15:13.000000 PySciMath-1.5.2/PySciMath/Arithmetic.py
--rw-rw-rw-   0        0        0    22383 2023-05-12 03:54:01.000000 PySciMath-1.5.2/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0      598 2023-05-12 03:54:25.000000 PySciMath-1.5.2/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1272 2023-05-11 15:14:07.000000 PySciMath-1.5.2/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      558 2023-05-12 06:07:57.000000 PySciMath-1.5.2/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.5.2/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 06:31:52.612187 PySciMath-1.5.2/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2591 2023-05-14 06:31:52.000000 PySciMath-1.5.2/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-14 06:31:52.000000 PySciMath-1.5.2/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 06:31:52.000000 PySciMath-1.5.2/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-14 06:31:52.000000 PySciMath-1.5.2/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2077 2023-05-14 06:31:09.000000 PySciMath-1.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-14 06:31:52.623158 PySciMath-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-05-14 06:31:05.000000 PySciMath-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:48:17.606293 PySciMath-1.5.3/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.5.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2023-05-14 06:30:09.000000 PySciMath-1.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2591 2023-05-14 06:48:17.605294 PySciMath-1.5.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-14 06:48:17.585351 PySciMath-1.5.3/PySciMath/
+-rw-rw-rw-   0        0        0     2090 2023-05-12 06:15:13.000000 PySciMath-1.5.3/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0    22383 2023-05-12 03:54:01.000000 PySciMath-1.5.3/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0      598 2023-05-12 03:54:25.000000 PySciMath-1.5.3/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1272 2023-05-11 15:14:07.000000 PySciMath-1.5.3/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      558 2023-05-12 06:07:57.000000 PySciMath-1.5.3/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.5.3/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:48:17.602304 PySciMath-1.5.3/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2591 2023-05-14 06:48:17.000000 PySciMath-1.5.3/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-14 06:48:17.000000 PySciMath-1.5.3/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 06:48:17.000000 PySciMath-1.5.3/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-14 06:48:17.000000 PySciMath-1.5.3/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2077 2023-05-14 06:47:22.000000 PySciMath-1.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-14 06:48:17.607289 PySciMath-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-05-14 06:47:18.000000 PySciMath-1.5.3/setup.py
```

### Comparing `PySciMath-1.5.2/LICENSE.txt` & `PySciMath-1.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.2/PKG-INFO` & `PySciMath-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.5.2
+Version: 1.5.3
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/PySciMath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
@@ -18,15 +18,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.2</br>
+**Version** - 1.5.3</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.5.2/PySciMath/Arithmetic.py` & `PySciMath-1.5.3/PySciMath/Arithmetic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.2/PySciMath/Geometry.py` & `PySciMath-1.5.3/PySciMath/Geometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.2/PySciMath/Quadratic.py` & `PySciMath-1.5.3/PySciMath/Quadratic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.2/PySciMath/Statistics.py` & `PySciMath-1.5.3/PySciMath/Statistics.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.2/PySciMath/Trigonometry.py` & `PySciMath-1.5.3/PySciMath/Trigonometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.2/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.5.3/PySciMath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.5.2
+Version: 1.5.3
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/PySciMath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
@@ -18,15 +18,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.2</br>
+**Version** - 1.5.3</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.5.2/README.md` & `PySciMath-1.5.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.2</br>
+**Version** - 1.5.3</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.5.2/setup.py` & `PySciMath-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PySciMath",
-    version="1.5.2",
+    version="1.5.3",
     description="PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

