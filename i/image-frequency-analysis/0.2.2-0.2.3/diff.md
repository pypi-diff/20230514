# Comparing `tmp/image_frequency_analysis-0.2.2.tar.gz` & `tmp/image_frequency_analysis-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_frequency_analysis-0.2.2.tar", last modified: Wed May 10 13:03:57 2023, max compression
+gzip compressed data, was "image_frequency_analysis-0.2.3.tar", last modified: Sun May 14 14:03:07 2023, max compression
```

## Comparing `image_frequency_analysis-0.2.2.tar` & `image_frequency_analysis-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:03:57.778496 image_frequency_analysis-0.2.2/
--rw-rw-rw-   0        0        0     1086 2023-04-15 11:42:59.000000 image_frequency_analysis-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     1647 2023-05-10 13:03:57.777498 image_frequency_analysis-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1361 2023-05-10 13:03:27.000000 image_frequency_analysis-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 13:03:57.768498 image_frequency_analysis-0.2.2/image_frequency_analysis/
--rw-rw-rw-   0        0        0       92 2023-05-10 12:59:14.000000 image_frequency_analysis-0.2.2/image_frequency_analysis/__init__.py
--rw-rw-rw-   0        0        0     6507 2023-05-10 12:59:14.000000 image_frequency_analysis-0.2.2/image_frequency_analysis/frequency_analysis.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:03:57.775524 image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/
--rw-rw-rw-   0        0        0     1647 2023-05-10 13:03:57.000000 image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-05-10 13:03:57.000000 image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:03:57.000000 image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-10 13:03:57.000000 image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-05-10 13:03:57.000000 image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 13:03:57.778496 image_frequency_analysis-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      562 2023-05-10 12:59:14.000000 image_frequency_analysis-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:03:07.171125 image_frequency_analysis-0.2.3/
+-rw-rw-rw-   0        0        0     1086 2023-04-15 11:42:59.000000 image_frequency_analysis-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     1495 2023-05-14 14:03:07.170125 image_frequency_analysis-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1209 2023-05-14 13:59:53.000000 image_frequency_analysis-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 14:03:07.161119 image_frequency_analysis-0.2.3/image_frequency_analysis/
+-rw-rw-rw-   0        0        0       92 2023-05-10 12:59:14.000000 image_frequency_analysis-0.2.3/image_frequency_analysis/__init__.py
+-rw-rw-rw-   0        0        0     6507 2023-05-10 12:59:14.000000 image_frequency_analysis-0.2.3/image_frequency_analysis/frequency_analysis.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:03:07.169125 image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/
+-rw-rw-rw-   0        0        0     1495 2023-05-14 14:03:06.000000 image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-05-14 14:03:06.000000 image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:03:06.000000 image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-14 14:03:06.000000 image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-14 14:03:06.000000 image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 14:03:07.171125 image_frequency_analysis-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      562 2023-05-14 14:00:38.000000 image_frequency_analysis-0.2.3/setup.py
```

### Comparing `image_frequency_analysis-0.2.2/LICENSE` & `image_frequency_analysis-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `image_frequency_analysis-0.2.2/PKG-INFO` & `image_frequency_analysis-0.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_frequency_analysis
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package to perform image frequency analysis using the Fourier Transform method
 Author: M Thivagar
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -31,19 +31,14 @@
 You can then pass the image path to the function which is a required argument, to get the plot 
 of comparison between the original image and the filtered image
 
 **Example:**
 
 ` ifa.FrequencyAnalysis('sandstone.tif') `
 
-**Sample Output:**
-
-![image](https://github.com/thivagar-manickam/image_frequency_analysis/assets/51501788/e94cc29b-a7a5-4768-aebf-5e4a17a92517)
-
-
 By default the package uses the high pass filter to perform the filtering of the image. This option can be overridden using
 the optional parameters that can be sent to the function.
 
 You can find the various optional parameters and their usage in the package using the help command.
 
 ` help(ifa.FrequencyAnalysis) ` or looking through the docstring directly in the IDE
```

### Comparing `image_frequency_analysis-0.2.2/README.md` & `image_frequency_analysis-0.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -21,19 +21,14 @@
 You can then pass the image path to the function which is a required argument, to get the plot 
 of comparison between the original image and the filtered image
 
 **Example:**
 
 ` ifa.FrequencyAnalysis('sandstone.tif') `
 
-**Sample Output:**
-
-![image](https://github.com/thivagar-manickam/image_frequency_analysis/assets/51501788/e94cc29b-a7a5-4768-aebf-5e4a17a92517)
-
-
 By default the package uses the high pass filter to perform the filtering of the image. This option can be overridden using
 the optional parameters that can be sent to the function.
 
 You can find the various optional parameters and their usage in the package using the help command.
 
 ` help(ifa.FrequencyAnalysis) ` or looking through the docstring directly in the IDE
```

### Comparing `image_frequency_analysis-0.2.2/image_frequency_analysis/frequency_analysis.py` & `image_frequency_analysis-0.2.3/image_frequency_analysis/frequency_analysis.py`

 * *Files identical despite different names*

### Comparing `image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/PKG-INFO` & `image_frequency_analysis-0.2.3/image_frequency_analysis.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-frequency-analysis
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package to perform image frequency analysis using the Fourier Transform method
 Author: M Thivagar
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -31,19 +31,14 @@
 You can then pass the image path to the function which is a required argument, to get the plot 
 of comparison between the original image and the filtered image
 
 **Example:**
 
 ` ifa.FrequencyAnalysis('sandstone.tif') `
 
-**Sample Output:**
-
-![image](https://github.com/thivagar-manickam/image_frequency_analysis/assets/51501788/e94cc29b-a7a5-4768-aebf-5e4a17a92517)
-
-
 By default the package uses the high pass filter to perform the filtering of the image. This option can be overridden using
 the optional parameters that can be sent to the function.
 
 You can find the various optional parameters and their usage in the package using the help command.
 
 ` help(ifa.FrequencyAnalysis) ` or looking through the docstring directly in the IDE
```

### Comparing `image_frequency_analysis-0.2.2/setup.py` & `image_frequency_analysis-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="image_frequency_analysis",
-    version="0.2.2",
+    version="0.2.3",
     author="M Thivagar",
     packages=find_packages(),
     install_requires=["opencv-python", "numpy", "pandas", "matplotlib"],
     python_requires=">=3.6",
     description="A package to perform image frequency analysis using the Fourier Transform method",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

