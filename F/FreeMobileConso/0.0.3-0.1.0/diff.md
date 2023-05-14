# Comparing `tmp/FreeMobileConso-0.0.3.tar.gz` & `tmp/FreeMobileConso-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeMobileConso-0.0.3.tar", last modified: Mon May  8 18:53:49 2023, max compression
+gzip compressed data, was "FreeMobileConso-0.1.0.tar", last modified: Sun May 14 12:38:01 2023, max compression
```

## Comparing `FreeMobileConso-0.0.3.tar` & `FreeMobileConso-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-08 18:53:49.022197 FreeMobileConso-0.0.3/
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-08 18:53:49.021378 FreeMobileConso-0.0.3/FreeMobileConso/
--rw-r--r--   0 corentin   (501) staff       (20)     1396 2023-05-08 18:53:28.000000 FreeMobileConso-0.0.3/FreeMobileConso/__init__.py
--rw-r--r--   0 corentin   (501) staff       (20)     5894 2023-05-08 18:48:46.000000 FreeMobileConso-0.0.3/FreeMobileConso/client.py
--rw-r--r--   0 corentin   (501) staff       (20)     2000 2023-05-08 18:49:46.000000 FreeMobileConso-0.0.3/FreeMobileConso/dataClassification.py
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-08 18:53:49.021932 FreeMobileConso-0.0.3/FreeMobileConso.egg-info/
--rw-r--r--   0 corentin   (501) staff       (20)     6059 2023-05-08 18:53:49.000000 FreeMobileConso-0.0.3/FreeMobileConso.egg-info/PKG-INFO
--rw-r--r--   0 corentin   (501) staff       (20)      312 2023-05-08 18:53:49.000000 FreeMobileConso-0.0.3/FreeMobileConso.egg-info/SOURCES.txt
--rw-r--r--   0 corentin   (501) staff       (20)        1 2023-05-08 18:53:49.000000 FreeMobileConso-0.0.3/FreeMobileConso.egg-info/dependency_links.txt
--rw-r--r--   0 corentin   (501) staff       (20)       13 2023-05-08 18:53:49.000000 FreeMobileConso-0.0.3/FreeMobileConso.egg-info/requires.txt
--rw-r--r--   0 corentin   (501) staff       (20)       16 2023-05-08 18:53:49.000000 FreeMobileConso-0.0.3/FreeMobileConso.egg-info/top_level.txt
--rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 FreeMobileConso-0.0.3/LICENSE
--rw-r--r--   0 corentin   (501) staff       (20)     6059 2023-05-08 18:53:49.022089 FreeMobileConso-0.0.3/PKG-INFO
--rwxrwxrwx   0 corentin   (501) staff       (20)     5574 2023-05-08 18:53:17.000000 FreeMobileConso-0.0.3/README.md
--rw-r--r--   0 corentin   (501) staff       (20)       38 2023-05-08 18:53:49.022236 FreeMobileConso-0.0.3/setup.cfg
--rw-r--r--   0 corentin   (501) staff       (20)      864 2023-05-08 18:53:23.000000 FreeMobileConso-0.0.3/setup.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-14 12:38:01.417204 FreeMobileConso-0.1.0/
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-14 12:38:01.416085 FreeMobileConso-0.1.0/FreeMobileConso/
+-rw-r--r--   0 corentin   (501) staff       (20)     1396 2023-05-14 12:37:13.000000 FreeMobileConso-0.1.0/FreeMobileConso/__init__.py
+-rw-r--r--   0 corentin   (501) staff       (20)     6173 2023-05-14 12:36:03.000000 FreeMobileConso-0.1.0/FreeMobileConso/client.py
+-rw-r--r--   0 corentin   (501) staff       (20)     2033 2023-05-14 12:15:38.000000 FreeMobileConso-0.1.0/FreeMobileConso/dataClassification.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-14 12:38:01.416850 FreeMobileConso-0.1.0/FreeMobileConso.egg-info/
+-rw-r--r--   0 corentin   (501) staff       (20)     6059 2023-05-14 12:38:01.000000 FreeMobileConso-0.1.0/FreeMobileConso.egg-info/PKG-INFO
+-rw-r--r--   0 corentin   (501) staff       (20)      312 2023-05-14 12:38:01.000000 FreeMobileConso-0.1.0/FreeMobileConso.egg-info/SOURCES.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        1 2023-05-14 12:38:01.000000 FreeMobileConso-0.1.0/FreeMobileConso.egg-info/dependency_links.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       13 2023-05-14 12:38:01.000000 FreeMobileConso-0.1.0/FreeMobileConso.egg-info/requires.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       16 2023-05-14 12:38:01.000000 FreeMobileConso-0.1.0/FreeMobileConso.egg-info/top_level.txt
+-rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 FreeMobileConso-0.1.0/LICENSE
+-rw-r--r--   0 corentin   (501) staff       (20)     6059 2023-05-14 12:38:01.417033 FreeMobileConso-0.1.0/PKG-INFO
+-rwxrwxrwx   0 corentin   (501) staff       (20)     5574 2023-05-08 18:53:17.000000 FreeMobileConso-0.1.0/README.md
+-rw-r--r--   0 corentin   (501) staff       (20)       38 2023-05-14 12:38:01.417253 FreeMobileConso-0.1.0/setup.cfg
+-rw-r--r--   0 corentin   (501) staff       (20)      864 2023-05-14 12:37:01.000000 FreeMobileConso-0.1.0/setup.py
```

### Comparing `FreeMobileConso-0.0.3/FreeMobileConso/__init__.py` & `FreeMobileConso-0.1.0/FreeMobileConso/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 """
 
 
 __title__ = "FreeMobileConso"
 __author__ = "CorentinMre"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) CorentinMre"
-__version__ = "0.0.3"
+__version__ = "0.1.0"
 
 
 from .dataClassification import *
 from .client import *
```

### Comparing `FreeMobileConso-0.0.3/FreeMobileConso/client.py` & `FreeMobileConso-0.1.0/FreeMobileConso/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,45 +51,53 @@
         except:
             raise Exception("Identifiant or password is incorrect")
 
 
         nameAcount = userInfo.find("div", {"class": "identite_bis"}).text.strip()
         identifiant = userInfo.findAll("div", {"class": "smaller"})[0].text.strip()
         ligne = userInfo.findAll("div", {"class": "smaller"})[1].text.strip()
+        date = soup.find("div", {"class": "details"}).find("div", {"class": "sub-title"}).text.strip()
         
         
         result= {}
         
         for _ in range(2):
             
             place = soup.find("div", {"class": "conso-local"}) if _ == 0 else soup.find("div", {"class": "conso-roaming"})
         
             result[place["class"][1].split("-")[1]] = {}
             
             for key, value in self.dictOfAllInformation.items():
                 
                 if key == "internet": itteration = 0
-                elif key == "appel": itteration = 1
+                elif key == "call": itteration = 1
                 elif key == "SMS": itteration = 2
                 elif key == "MMS": itteration = 3
                 
                 result[place["class"][1].split("-")[1]][key] = {}
                 result[place["class"][1].split("-")[1]][key][value[0]] = place.findAll("div", {"class": "number-circle"})[itteration].find("span").text.strip().replace("*","")
-                result[place["class"][1].split("-")[1]][key][value[1]] = place.findAll("div", {"class": "number-circle"})[itteration].find("p").text.replace(result[place["class"][1].split("-")[1]][key][value[0]], "").replace("/", "").strip().replace("*","")
+    
+                dataSecondValue = place.findAll("div", {"class": "number-circle"})[itteration].find("p").text.strip().replace("*","")
+
+                if "/" in dataSecondValue:
+                    result[place["class"][1].split("-")[1]][key][value[1]] = dataSecondValue.split("/")[1]
+                else:
+                    result[place["class"][1].split("-")[1]][key][value[1]] = dataSecondValue
+
                 if result[place["class"][1].split("-")[1]][key][value[1]] == "": 
                     result[place["class"][1].split("-")[1]][key][value[1]] = result[place["class"][1].split("-")[1]][key][value[0]]
                 result[place["class"][1].split("-")[1]][key][value[2]] = place.findAll("div", {"class": "text-conso-content"})[itteration].findAll("p")[0].find("span").text.replace("/ ", "").strip().replace("*","")
                 thirdInformation = result[place["class"][1].split("-")[1]][key][value[3]] = place.findAll("div", {"class": "text-conso-content"})[itteration].findAll("p")
                 lastInternetAppelInformation = place.findAll("div", {"class": "text-conso-content"})[itteration].findAll("p")
                 lastSMSMMSInformation = place.findAll("div", {"class": "text-conso-content"})[itteration].findAll("p")[1].text.strip().split(": ")[1].replace("*","")
                 if key == "internet":
                     
                     result[place["class"][1].split("-")[1]][key][value[3]] = thirdInformation[1].text.strip().split(": ")[1].replace("*","")
                     
-                elif key == "appel":
+                elif key == "call":
                     result[place["class"][1].split("-")[1]][key][value[3]] = thirdInformation[1].text.strip().split(": ")[1].replace("*","")
                     result[place["class"][1].split("-")[1]][key][value[4]] = lastInternetAppelInformation[2].text.strip().split(": ")[1].replace("*","")
                     
                 else:
                     result[place["class"][1].split("-")[1]][key][value[3]] = thirdInformation[0].text.strip().split(" / ")[0].replace("*","")
                     result[place["class"][1].split("-")[1]][key][value[4]] = lastSMSMMSInformation
                 
@@ -104,13 +112,14 @@
                         if key3 == "excludingPackage":
                             result["totalExcludingPackage"] += float(value3.replace("€", ""))
         
         result["totalExcludingPackage"] = str(result["totalExcludingPackage"]) + "€"
         result["nameAcount"] = nameAcount
         result["identifier"] = identifiant.split(" : ")[1]
         result["number"] = ligne.split(" : ")[1].replace(" ", "")
+        result["date"] = date
         
         return result
     
     def consommation(self) -> dict:
         return dataClassification.Classification(self.getConsoDict())
```

### Comparing `FreeMobileConso-0.0.3/FreeMobileConso/dataClassification.py` & `FreeMobileConso-0.1.0/FreeMobileConso/dataClassification.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 class Classification:
     def __init__(self, data:dict):
         self.nameAcount = data["nameAcount"]
         self.identifier = data["identifier"]
         self.number = data["number"]
+        self.date = data["date"]
         self.totalExcludingPackage = data["totalExcludingPackage"]
         
         self.local = Local(data["local"])
         self.roaming = Roaming(data["roaming"])
```

### Comparing `FreeMobileConso-0.0.3/FreeMobileConso.egg-info/PKG-INFO` & `FreeMobileConso-0.1.0/FreeMobileConso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeMobileConso
-Version: 0.0.3
+Version: 0.1.0
 Summary: A python API for get your consommation of your Free mobile account
 Home-page: https://github.com/CorentinMre/FreeMobileConso
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FreeMobileConso-0.0.3/LICENSE` & `FreeMobileConso-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeMobileConso-0.0.3/PKG-INFO` & `FreeMobileConso-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeMobileConso
-Version: 0.0.3
+Version: 0.1.0
 Summary: A python API for get your consommation of your Free mobile account
 Home-page: https://github.com/CorentinMre/FreeMobileConso
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FreeMobileConso-0.0.3/README.md` & `FreeMobileConso-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `FreeMobileConso-0.0.3/setup.py` & `FreeMobileConso-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='FreeMobileConso',
-    version='0.0.3',    
+    version='0.1.0',    
     description='A python API for get your consommation of your Free mobile account',
     long_description_content_type = "text/markdown",
     long_description=long_description,
     url='https://github.com/CorentinMre/FreeMobileConso',
     author='CorentinMre',
     author_email='corentin.marie@isen-ouest.yncrea.fr',
     license='MIT',
```

