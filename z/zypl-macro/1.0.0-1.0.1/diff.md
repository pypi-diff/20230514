# Comparing `tmp/zypl_macro-1.0.0.tar.gz` & `tmp/zypl_macro-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zypl_macro-1.0.0.tar", last modified: Sun May 14 08:59:39 2023, max compression
+gzip compressed data, was "zypl_macro-1.0.1.tar", last modified: Sun May 14 10:17:40 2023, max compression
```

## Comparing `zypl_macro-1.0.0.tar` & `zypl_macro-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 08:59:39.078552 zypl_macro-1.0.0/
--rw-rw-rw-   0        0        0     1099 2023-05-14 06:12:43.000000 zypl_macro-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4076 2023-05-14 08:59:39.071262 zypl_macro-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3713 2023-05-14 08:59:00.000000 zypl_macro-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-14 08:59:39.079523 zypl_macro-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-05-14 08:12:45.000000 zypl_macro-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:59:39.066292 zypl_macro-1.0.0/zypl_macro/
--rw-rw-rw-   0        0        0        2 2023-05-14 06:12:43.000000 zypl_macro-1.0.0/zypl_macro/__init__.py
--rw-rw-rw-   0        0        0     4302 2023-05-14 08:45:09.000000 zypl_macro-1.0.0/zypl_macro/library.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:59:39.070264 zypl_macro-1.0.0/zypl_macro.egg-info/
--rw-rw-rw-   0        0        0     4076 2023-05-14 08:59:39.000000 zypl_macro-1.0.0/zypl_macro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-05-14 08:59:39.000000 zypl_macro-1.0.0/zypl_macro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 08:59:39.000000 zypl_macro-1.0.0/zypl_macro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-14 08:59:39.000000 zypl_macro-1.0.0/zypl_macro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-14 08:59:39.000000 zypl_macro-1.0.0/zypl_macro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 10:17:40.801996 zypl_macro-1.0.1/
+-rw-rw-rw-   0        0        0     1099 2023-05-14 06:12:43.000000 zypl_macro-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4211 2023-05-14 10:17:40.793967 zypl_macro-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3848 2023-05-14 10:17:28.000000 zypl_macro-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-14 10:17:40.801996 zypl_macro-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-05-14 10:11:10.000000 zypl_macro-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 10:17:40.786986 zypl_macro-1.0.1/zypl_macro/
+-rw-rw-rw-   0        0        0        2 2023-05-14 06:12:43.000000 zypl_macro-1.0.1/zypl_macro/__init__.py
+-rw-rw-rw-   0        0        0     4302 2023-05-14 08:45:09.000000 zypl_macro-1.0.1/zypl_macro/library.py
+drwxrwxrwx   0        0        0        0 2023-05-14 10:17:40.791972 zypl_macro-1.0.1/zypl_macro.egg-info/
+-rw-rw-rw-   0        0        0     4211 2023-05-14 10:17:40.000000 zypl_macro-1.0.1/zypl_macro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-05-14 10:17:40.000000 zypl_macro-1.0.1/zypl_macro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 10:17:40.000000 zypl_macro-1.0.1/zypl_macro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-14 10:17:40.000000 zypl_macro-1.0.1/zypl_macro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-14 10:17:40.000000 zypl_macro-1.0.1/zypl_macro.egg-info/top_level.txt
```

### Comparing `zypl_macro-1.0.0/LICENSE` & `zypl_macro-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zypl_macro-1.0.0/PKG-INFO` & `zypl_macro-1.0.1/zypl_macro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zypl_macro
-Version: 1.0.0
+Name: zypl-macro
+Version: 1.0.1
 Summary: zypl.ai alternative data API interface lib
 Author: Me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
@@ -15,31 +15,30 @@
 This here is a Python interface module meant to streamline obtaining macroeconomic data from Zypl.ai's alternative data API macro endpoint. It offers a few simple methods to obtain the data from server and store it locally for future usage, whatever that may be.
 Please keep in mind that for succesfull usage of this module it is absolutely essential for you to be in a good mood and healthy disposition, otherwise it might not work. To be fair, it might not work either way, but if you meet the requirement stated above you, at the very least, won't get upset by this fact nearly as much.
 
 ## Usage
 
 This module is obtained from pip with the usual installation line:
 ```
-python pip install zypl_macro
+pip install zypl_macro
 ```
-If you're not running your machine under Windows or do not know how to use pip, please refer [here] (https://pip.pypa.io/en/stable/) for pointers. It is all very straightforward.
+If you're not running your machine under Windows or do not know how to use pip, please refer [here](https://pip.pypa.io/en/stable/) for pointers. It is all very straightforward.
 
 After installing the module first order of business is to import and instantiate its utility class, like so:
 ```
 from zypl_macro.library import DataGetter
 
 getter_instance = DataGetter()
 ```
 
 After this you're going to have to provide authorization token aka API key in order to be allowed to query data endpoint. It is done via a dedicated method:
 ```
 getter_instance.auth('your-very-very-secret-token')
 ```
 You can get an API key from zypl's alternative data API server administration, if they'll feel like providing you with one. Please don't lose it.
-
 Once you succesfully got an instance of the class in your code and provided it with the token, you can start querying data. For now there are three main methods you can utilize.
 
 ### get_countries
 
 You can obtain the list of all the countries supported in alt data system calling this method.
 ```
 getter_instance.get_countries()
@@ -48,25 +47,28 @@
 
 ### get_indicators
 
 Works similar to the previous one and provides you with a list of all the macroeconomic indicators in the database. You can call with a country specified in order to get only indicators pertaining to that country, otherwise you're gonna get them all.
 ```
 getter_instance.get_indicators(country='Uzbekistan')
 ```
-Results are also stored in a csv file near to your executing script.
+Results are also stored in a csv file near your executing script.
 
 ### get_data
 
 This is the main method that allows you to obtain the data itself. The only mandatory argument is the country you want your data on:
 ```
 getter_instance.get_data(country='Tajikistan')
 ```
+
 You can also provide it with `start` and `end` arguments to specify the date range you want to get your data in. Dates must be in iso format, e.g. YYYY-MM-DD.
 ```
 getter_instance.get_data(country='Tajikistan', start='2020-02-01', end='2022-02-01')
 ```
 You can provide either of these arguments or both of them or none, it'll be fine.
 
 ## Misc
-If alt data API endpoint gets changed or moved somewhere (it shouldn't, but weirder things has been known to happen), this module is not going to work properly. In this case, and if you happen to know it's new living address, you can call _set_url method to point the module there. Please don't touch this method otherwise, things will break.
+All the error messages, and there is quite a few, are ouput to console. So you should keep an eye it in case of something not working properly.
+
+If alt data API endpoint gets changed or moved somewhere (it shouldn't, but weirder things has been known to happen), this module is not going to work properly. In this case, and if you happen to know its new living address, you can call _set_url method to point the module there. Please don't touch this method otherwise, things will break.
 
 On the other note, every indicator in the has the `frequency` parameter associated with it specifying the period data is gathered at. These are typically associated with a certain group of indicators each and go like "Daily", "Monthly", "Quarterly" and "Yearly". It is entirely optional, but you can provide this parameter to get_data too (i.e. get_data(..., frequency="Monthly")) if you want to narrow down the dataset you get.
```

### Comparing `zypl_macro-1.0.0/README.md` & `zypl_macro-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,31 +3,30 @@
 This here is a Python interface module meant to streamline obtaining macroeconomic data from Zypl.ai's alternative data API macro endpoint. It offers a few simple methods to obtain the data from server and store it locally for future usage, whatever that may be.
 Please keep in mind that for succesfull usage of this module it is absolutely essential for you to be in a good mood and healthy disposition, otherwise it might not work. To be fair, it might not work either way, but if you meet the requirement stated above you, at the very least, won't get upset by this fact nearly as much.
 
 ## Usage
 
 This module is obtained from pip with the usual installation line:
 ```
-python pip install zypl_macro
+pip install zypl_macro
 ```
-If you're not running your machine under Windows or do not know how to use pip, please refer [here] (https://pip.pypa.io/en/stable/) for pointers. It is all very straightforward.
+If you're not running your machine under Windows or do not know how to use pip, please refer [here](https://pip.pypa.io/en/stable/) for pointers. It is all very straightforward.
 
 After installing the module first order of business is to import and instantiate its utility class, like so:
 ```
 from zypl_macro.library import DataGetter
 
 getter_instance = DataGetter()
 ```
 
 After this you're going to have to provide authorization token aka API key in order to be allowed to query data endpoint. It is done via a dedicated method:
 ```
 getter_instance.auth('your-very-very-secret-token')
 ```
 You can get an API key from zypl's alternative data API server administration, if they'll feel like providing you with one. Please don't lose it.
-
 Once you succesfully got an instance of the class in your code and provided it with the token, you can start querying data. For now there are three main methods you can utilize.
 
 ### get_countries
 
 You can obtain the list of all the countries supported in alt data system calling this method.
 ```
 getter_instance.get_countries()
@@ -36,25 +35,28 @@
 
 ### get_indicators
 
 Works similar to the previous one and provides you with a list of all the macroeconomic indicators in the database. You can call with a country specified in order to get only indicators pertaining to that country, otherwise you're gonna get them all.
 ```
 getter_instance.get_indicators(country='Uzbekistan')
 ```
-Results are also stored in a csv file near to your executing script.
+Results are also stored in a csv file near your executing script.
 
 ### get_data
 
 This is the main method that allows you to obtain the data itself. The only mandatory argument is the country you want your data on:
 ```
 getter_instance.get_data(country='Tajikistan')
 ```
+
 You can also provide it with `start` and `end` arguments to specify the date range you want to get your data in. Dates must be in iso format, e.g. YYYY-MM-DD.
 ```
 getter_instance.get_data(country='Tajikistan', start='2020-02-01', end='2022-02-01')
 ```
 You can provide either of these arguments or both of them or none, it'll be fine.
 
 ## Misc
-If alt data API endpoint gets changed or moved somewhere (it shouldn't, but weirder things has been known to happen), this module is not going to work properly. In this case, and if you happen to know it's new living address, you can call _set_url method to point the module there. Please don't touch this method otherwise, things will break.
+All the error messages, and there is quite a few, are ouput to console. So you should keep an eye it in case of something not working properly.
+
+If alt data API endpoint gets changed or moved somewhere (it shouldn't, but weirder things has been known to happen), this module is not going to work properly. In this case, and if you happen to know its new living address, you can call _set_url method to point the module there. Please don't touch this method otherwise, things will break.
 
 On the other note, every indicator in the has the `frequency` parameter associated with it specifying the period data is gathered at. These are typically associated with a certain group of indicators each and go like "Daily", "Monthly", "Quarterly" and "Yearly". It is entirely optional, but you can provide this parameter to get_data too (i.e. get_data(..., frequency="Monthly")) if you want to narrow down the dataset you get.
```

### Comparing `zypl_macro-1.0.0/setup.py` & `zypl_macro-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zypl_macro",
-    version="1.0.0",
+    version="1.0.1",
     author="Me",
     description="zypl.ai alternative data API interface lib",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `zypl_macro-1.0.0/zypl_macro/library.py` & `zypl_macro-1.0.1/zypl_macro/library.py`

 * *Files identical despite different names*

### Comparing `zypl_macro-1.0.0/zypl_macro.egg-info/PKG-INFO` & `zypl_macro-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zypl-macro
-Version: 1.0.0
+Name: zypl_macro
+Version: 1.0.1
 Summary: zypl.ai alternative data API interface lib
 Author: Me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
@@ -15,31 +15,30 @@
 This here is a Python interface module meant to streamline obtaining macroeconomic data from Zypl.ai's alternative data API macro endpoint. It offers a few simple methods to obtain the data from server and store it locally for future usage, whatever that may be.
 Please keep in mind that for succesfull usage of this module it is absolutely essential for you to be in a good mood and healthy disposition, otherwise it might not work. To be fair, it might not work either way, but if you meet the requirement stated above you, at the very least, won't get upset by this fact nearly as much.
 
 ## Usage
 
 This module is obtained from pip with the usual installation line:
 ```
-python pip install zypl_macro
+pip install zypl_macro
 ```
-If you're not running your machine under Windows or do not know how to use pip, please refer [here] (https://pip.pypa.io/en/stable/) for pointers. It is all very straightforward.
+If you're not running your machine under Windows or do not know how to use pip, please refer [here](https://pip.pypa.io/en/stable/) for pointers. It is all very straightforward.
 
 After installing the module first order of business is to import and instantiate its utility class, like so:
 ```
 from zypl_macro.library import DataGetter
 
 getter_instance = DataGetter()
 ```
 
 After this you're going to have to provide authorization token aka API key in order to be allowed to query data endpoint. It is done via a dedicated method:
 ```
 getter_instance.auth('your-very-very-secret-token')
 ```
 You can get an API key from zypl's alternative data API server administration, if they'll feel like providing you with one. Please don't lose it.
-
 Once you succesfully got an instance of the class in your code and provided it with the token, you can start querying data. For now there are three main methods you can utilize.
 
 ### get_countries
 
 You can obtain the list of all the countries supported in alt data system calling this method.
 ```
 getter_instance.get_countries()
@@ -48,25 +47,28 @@
 
 ### get_indicators
 
 Works similar to the previous one and provides you with a list of all the macroeconomic indicators in the database. You can call with a country specified in order to get only indicators pertaining to that country, otherwise you're gonna get them all.
 ```
 getter_instance.get_indicators(country='Uzbekistan')
 ```
-Results are also stored in a csv file near to your executing script.
+Results are also stored in a csv file near your executing script.
 
 ### get_data
 
 This is the main method that allows you to obtain the data itself. The only mandatory argument is the country you want your data on:
 ```
 getter_instance.get_data(country='Tajikistan')
 ```
+
 You can also provide it with `start` and `end` arguments to specify the date range you want to get your data in. Dates must be in iso format, e.g. YYYY-MM-DD.
 ```
 getter_instance.get_data(country='Tajikistan', start='2020-02-01', end='2022-02-01')
 ```
 You can provide either of these arguments or both of them or none, it'll be fine.
 
 ## Misc
-If alt data API endpoint gets changed or moved somewhere (it shouldn't, but weirder things has been known to happen), this module is not going to work properly. In this case, and if you happen to know it's new living address, you can call _set_url method to point the module there. Please don't touch this method otherwise, things will break.
+All the error messages, and there is quite a few, are ouput to console. So you should keep an eye it in case of something not working properly.
+
+If alt data API endpoint gets changed or moved somewhere (it shouldn't, but weirder things has been known to happen), this module is not going to work properly. In this case, and if you happen to know its new living address, you can call _set_url method to point the module there. Please don't touch this method otherwise, things will break.
 
 On the other note, every indicator in the has the `frequency` parameter associated with it specifying the period data is gathered at. These are typically associated with a certain group of indicators each and go like "Daily", "Monthly", "Quarterly" and "Yearly". It is entirely optional, but you can provide this parameter to get_data too (i.e. get_data(..., frequency="Monthly")) if you want to narrow down the dataset you get.
```

