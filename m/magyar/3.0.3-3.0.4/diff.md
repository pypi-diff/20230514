# Comparing `tmp/magyar-3.0.3.tar.gz` & `tmp/magyar-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-3.0.3.tar", last modified: Fri May 12 19:21:37 2023, max compression
+gzip compressed data, was "magyar-3.0.4.tar", last modified: Sun May 14 21:05:05 2023, max compression
```

## Comparing `magyar-3.0.3.tar` & `magyar-3.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-12 19:21:37.550600 magyar-3.0.3/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6429 2023-05-12 19:21:37.550600 magyar-3.0.3/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     6019 2023-05-12 19:20:36.000000 magyar-3.0.3/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-12 19:21:37.550600 magyar-3.0.3/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6429 2023-05-12 19:21:37.000000 magyar-3.0.3/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-12 19:21:37.000000 magyar-3.0.3/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-12 19:21:37.000000 magyar-3.0.3/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-12 19:21:37.000000 magyar-3.0.3/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    38936 2023-05-12 19:16:45.000000 magyar-3.0.3/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-12 19:21:37.550600 magyar-3.0.3/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-12 19:10:58.000000 magyar-3.0.3/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-14 21:05:05.572022 magyar-3.0.4/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6525 2023-05-14 21:05:05.572022 magyar-3.0.4/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6115 2023-05-14 21:00:00.000000 magyar-3.0.4/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-14 21:05:05.572022 magyar-3.0.4/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6525 2023-05-14 21:05:05.000000 magyar-3.0.4/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-14 21:05:05.000000 magyar-3.0.4/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-14 21:05:05.000000 magyar-3.0.4/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-14 21:05:05.000000 magyar-3.0.4/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    38936 2023-05-12 19:16:45.000000 magyar-3.0.4/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-14 21:05:05.572022 magyar-3.0.4/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-14 21:02:15.000000 magyar-3.0.4/setup.py
```

### Comparing `magyar-3.0.3/PKG-INFO` & `magyar-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.0.3
+Version: 3.0.4
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -151,22 +151,25 @@
 '  ' = a behúzás mértéke ami sztring. '\t' </br>
 Kimenetként listát ad vissza. </br></br>
 
 Hasznalat :</br>
 formazott_lista= magyar.ftordel(varosok,5,'\t')</br>
 print(formazott_lista) vagy f.write(formazott_lista)
 </br></br></br>
+Minta a használathoz: </br>
+![Példa kép](./abc_rendezes.png)
 5. kerekítés egész számra:  </br>
 
         magyar.fel_kerekit(szam)
         magyar.le_kerekit(szam)
 
 
 Tizedes számot kerekít egész számra fel vagy le.  </br>
  </br>
+![Példa kép](./kerekites.png)
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-3.0.3/README.md` & `magyar-3.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -139,22 +139,25 @@
 '  ' = a behúzás mértéke ami sztring. '\t' </br>
 Kimenetként listát ad vissza. </br></br>
 
 Hasznalat :</br>
 formazott_lista= magyar.ftordel(varosok,5,'\t')</br>
 print(formazott_lista) vagy f.write(formazott_lista)
 </br></br></br>
+Minta a használathoz: </br>
+![Példa kép](./abc_rendezes.png)
 5. kerekítés egész számra:  </br>
 
         magyar.fel_kerekit(szam)
         magyar.le_kerekit(szam)
 
 
 Tizedes számot kerekít egész számra fel vagy le.  </br>
  </br>
+![Példa kép](./kerekites.png)
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-3.0.3/magyar.egg-info/PKG-INFO` & `magyar-3.0.4/magyar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.0.3
+Version: 3.0.4
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -151,22 +151,25 @@
 '  ' = a behúzás mértéke ami sztring. '\t' </br>
 Kimenetként listát ad vissza. </br></br>
 
 Hasznalat :</br>
 formazott_lista= magyar.ftordel(varosok,5,'\t')</br>
 print(formazott_lista) vagy f.write(formazott_lista)
 </br></br></br>
+Minta a használathoz: </br>
+![Példa kép](./abc_rendezes.png)
 5. kerekítés egész számra:  </br>
 
         magyar.fel_kerekit(szam)
         magyar.le_kerekit(szam)
 
 
 Tizedes számot kerekít egész számra fel vagy le.  </br>
  </br>
+![Példa kép](./kerekites.png)
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-3.0.3/magyar.py` & `magyar-3.0.4/magyar.py`

 * *Files identical despite different names*

### Comparing `magyar-3.0.3/setup.py` & `magyar-3.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="3.0.3",
+    version="3.0.4",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian lists of names,animals,foods, fruits, rivers ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

