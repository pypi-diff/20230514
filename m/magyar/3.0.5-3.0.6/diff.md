# Comparing `tmp/magyar-3.0.5.tar.gz` & `tmp/magyar-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-3.0.5.tar", last modified: Sun May 14 21:14:24 2023, max compression
+gzip compressed data, was "magyar-3.0.6.tar", last modified: Sun May 14 21:46:25 2023, max compression
```

## Comparing `magyar-3.0.5.tar` & `magyar-3.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-14 21:14:24.013403 magyar-3.0.5/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6635 2023-05-14 21:14:24.013403 magyar-3.0.5/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     6225 2023-05-14 21:13:25.000000 magyar-3.0.5/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-14 21:14:24.013403 magyar-3.0.5/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6635 2023-05-14 21:14:24.000000 magyar-3.0.5/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-14 21:14:24.000000 magyar-3.0.5/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-14 21:14:24.000000 magyar-3.0.5/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-14 21:14:24.000000 magyar-3.0.5/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    38936 2023-05-12 19:16:45.000000 magyar-3.0.5/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-14 21:14:24.013403 magyar-3.0.5/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-14 21:09:28.000000 magyar-3.0.5/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-14 21:46:25.523926 magyar-3.0.6/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6726 2023-05-14 21:46:25.523926 magyar-3.0.6/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6316 2023-05-14 21:42:14.000000 magyar-3.0.6/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-14 21:46:25.523926 magyar-3.0.6/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6726 2023-05-14 21:46:25.000000 magyar-3.0.6/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-14 21:46:25.000000 magyar-3.0.6/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-14 21:46:25.000000 magyar-3.0.6/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-14 21:46:25.000000 magyar-3.0.6/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    38936 2023-05-12 19:16:45.000000 magyar-3.0.6/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-14 21:46:25.523926 magyar-3.0.6/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-14 21:18:14.000000 magyar-3.0.6/setup.py
```

### Comparing `magyar-3.0.5/PKG-INFO` & `magyar-3.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.0.5
+Version: 3.0.6
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -87,15 +87,19 @@
  
 I recommend it mainly as a supplement to random number generators. 
        
             random.sample()
             utca = random.sample(magyar.utca, k=16) 
             random.choices()
             telepulesek = random.choice(magyar.telepules)
+<br>
 
+![Listák](https://raw.githubusercontent.com/kobanya/nevek/master/listak.png)
+
+</br>
 ## Szótárak:
 Több adatot tartalmaznak összekapcsolva.
 
     magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
     magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
     magyar.jaras :             {'megye' : (székhely, megye)}
     magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
@@ -151,15 +155,16 @@
 '  ' = a behúzás mértéke ami sztring. '\t' </br>
 Kimenetként listát ad vissza. </br></br>
 
 Hasznalat :</br>
 formazott_lista= magyar.ftordel(varosok,5,'\t')</br>
 print(formazott_lista) vagy f.write(formazott_lista)
 </br></br></br>
-Minta a használathoz: </br>
+Minta a használathoz: 
+</br>
 ![ABC rendezés](https://raw.githubusercontent.com/kobanya/nevek/master/abc_rendezes.png)
 
 5. kerekítés egész számra:  </br>
 
         magyar.fel_kerekit(szam)
         magyar.le_kerekit(szam)
```

### Comparing `magyar-3.0.5/README.md` & `magyar-3.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,19 @@
  
 I recommend it mainly as a supplement to random number generators. 
        
             random.sample()
             utca = random.sample(magyar.utca, k=16) 
             random.choices()
             telepulesek = random.choice(magyar.telepules)
+<br>
 
+![Listák](https://raw.githubusercontent.com/kobanya/nevek/master/listak.png)
+
+</br>
 ## Szótárak:
 Több adatot tartalmaznak összekapcsolva.
 
     magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
     magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
     magyar.jaras :             {'megye' : (székhely, megye)}
     magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
@@ -139,15 +143,16 @@
 '  ' = a behúzás mértéke ami sztring. '\t' </br>
 Kimenetként listát ad vissza. </br></br>
 
 Hasznalat :</br>
 formazott_lista= magyar.ftordel(varosok,5,'\t')</br>
 print(formazott_lista) vagy f.write(formazott_lista)
 </br></br></br>
-Minta a használathoz: </br>
+Minta a használathoz: 
+</br>
 ![ABC rendezés](https://raw.githubusercontent.com/kobanya/nevek/master/abc_rendezes.png)
 
 5. kerekítés egész számra:  </br>
 
         magyar.fel_kerekit(szam)
         magyar.le_kerekit(szam)
```

### Comparing `magyar-3.0.5/magyar.egg-info/PKG-INFO` & `magyar-3.0.6/magyar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.0.5
+Version: 3.0.6
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -87,15 +87,19 @@
  
 I recommend it mainly as a supplement to random number generators. 
        
             random.sample()
             utca = random.sample(magyar.utca, k=16) 
             random.choices()
             telepulesek = random.choice(magyar.telepules)
+<br>
 
+![Listák](https://raw.githubusercontent.com/kobanya/nevek/master/listak.png)
+
+</br>
 ## Szótárak:
 Több adatot tartalmaznak összekapcsolva.
 
     magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
     magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
     magyar.jaras :             {'megye' : (székhely, megye)}
     magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
@@ -151,15 +155,16 @@
 '  ' = a behúzás mértéke ami sztring. '\t' </br>
 Kimenetként listát ad vissza. </br></br>
 
 Hasznalat :</br>
 formazott_lista= magyar.ftordel(varosok,5,'\t')</br>
 print(formazott_lista) vagy f.write(formazott_lista)
 </br></br></br>
-Minta a használathoz: </br>
+Minta a használathoz: 
+</br>
 ![ABC rendezés](https://raw.githubusercontent.com/kobanya/nevek/master/abc_rendezes.png)
 
 5. kerekítés egész számra:  </br>
 
         magyar.fel_kerekit(szam)
         magyar.le_kerekit(szam)
```

### Comparing `magyar-3.0.5/magyar.py` & `magyar-3.0.6/magyar.py`

 * *Files identical despite different names*

### Comparing `magyar-3.0.5/setup.py` & `magyar-3.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="3.0.5",
+    version="3.0.6",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian lists of names,animals,foods, fruits, rivers ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

