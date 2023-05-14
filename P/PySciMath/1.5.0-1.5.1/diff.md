# Comparing `tmp/PySciMath-1.5.0.tar.gz` & `tmp/PySciMath-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.5.0.tar", last modified: Fri May 12 03:58:02 2023, max compression
+gzip compressed data, was "PySciMath-1.5.1.tar", last modified: Sun May 14 06:26:25 2023, max compression
```

## Comparing `PySciMath-1.5.0.tar` & `PySciMath-1.5.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 03:58:02.096891 PySciMath-1.5.0/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.5.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2591 2023-05-12 03:58:02.095880 PySciMath-1.5.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-12 03:58:02.080920 PySciMath-1.5.0/PySciMath/
--rw-rw-rw-   0        0        0     2090 2023-05-11 16:14:33.000000 PySciMath-1.5.0/PySciMath/Arithmetic.py
--rw-rw-rw-   0        0        0    22383 2023-05-12 03:54:01.000000 PySciMath-1.5.0/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0      598 2023-05-12 03:54:25.000000 PySciMath-1.5.0/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1272 2023-05-11 15:14:07.000000 PySciMath-1.5.0/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      558 2023-05-10 09:51:46.000000 PySciMath-1.5.0/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.5.0/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 03:58:02.092080 PySciMath-1.5.0/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2591 2023-05-12 03:58:01.000000 PySciMath-1.5.0/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-05-12 03:58:01.000000 PySciMath-1.5.0/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 03:58:01.000000 PySciMath-1.5.0/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-12 03:58:01.000000 PySciMath-1.5.0/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2077 2023-05-12 03:37:02.000000 PySciMath-1.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 03:58:02.097877 PySciMath-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-05-12 03:36:57.000000 PySciMath-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:26:25.419918 PySciMath-1.5.1/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2023-05-14 06:25:05.000000 PySciMath-1.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2591 2023-05-14 06:26:25.418921 PySciMath-1.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-14 06:26:25.388004 PySciMath-1.5.1/PySciMath/
+-rw-rw-rw-   0        0        0     2090 2023-05-12 06:15:13.000000 PySciMath-1.5.1/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0    22383 2023-05-12 03:54:01.000000 PySciMath-1.5.1/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0      598 2023-05-12 03:54:25.000000 PySciMath-1.5.1/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1272 2023-05-11 15:14:07.000000 PySciMath-1.5.1/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      558 2023-05-12 06:07:57.000000 PySciMath-1.5.1/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.5.1/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 06:26:25.414968 PySciMath-1.5.1/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2591 2023-05-14 06:26:24.000000 PySciMath-1.5.1/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-14 06:26:24.000000 PySciMath-1.5.1/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 06:26:24.000000 PySciMath-1.5.1/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-14 06:26:24.000000 PySciMath-1.5.1/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2077 2023-05-14 06:24:56.000000 PySciMath-1.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-14 06:26:25.420916 PySciMath-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-05-14 06:24:53.000000 PySciMath-1.5.1/setup.py
```

### Comparing `PySciMath-1.5.0/LICENSE.txt` & `PySciMath-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.0/PKG-INFO` & `PySciMath-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.5.0
+Version: 1.5.1
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
-Download-URL: https://pypi.org/project/pyscimath
+Download-URL: https://pypi.org/project/PySciMath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -18,15 +18,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.0</br>
+**Version** - 1.5.1</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.5.0/PySciMath/Arithmetic.py` & `PySciMath-1.5.1/PySciMath/Arithmetic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.0/PySciMath/Geometry.py` & `PySciMath-1.5.1/PySciMath/Geometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.0/PySciMath/Quadratic.py` & `PySciMath-1.5.1/PySciMath/Quadratic.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.0/PySciMath/Statistics.py` & `PySciMath-1.5.1/PySciMath/Statistics.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.0/PySciMath/Trigonometry.py` & `PySciMath-1.5.1/PySciMath/Trigonometry.py`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.0/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.5.1/PySciMath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.5.0
+Version: 1.5.1
 Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
-Download-URL: https://pypi.org/project/pyscimath
+Download-URL: https://pypi.org/project/PySciMath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Calculations
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -18,15 +18,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.0</br>
+**Version** - 1.5.1</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.5.0/README.md` & `PySciMath-1.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
 ## Module Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.0</br>
+**Version** - 1.5.1</br>
 **Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
```

### Comparing `PySciMath-1.5.0/setup.py` & `PySciMath-1.5.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PySciMath",
-    version="1.5.0",
+    version="1.5.1",
     description="PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
     author_email="anikethchavare@outlook.com",
     keywords=["Math", "Calculations"],
     url="https://github.com/Anikethc/PySciMath",
-    download_url="https://pypi.org/project/pyscimath"
+    download_url="https://pypi.org/project/PySciMath"
 )
 
 # Run the Setup File
 if __name__ == "__main__":
     setup(**setup_args)
```

