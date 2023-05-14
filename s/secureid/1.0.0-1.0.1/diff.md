# Comparing `tmp/secureid-1.0.0-py3-none-any.whl.zip` & `tmp/secureid-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1789 bytes, number of entries: 5
--rw-r--r--  2.0 unx     2037 b- defN 22-Nov-27 15:07 secure_id.py
--rw-r--r--  2.0 unx      373 b- defN 22-Nov-27 15:10 secureid-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-27 15:10 secureid-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 22-Nov-27 15:10 secureid-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      370 b- defN 22-Nov-27 15:10 secureid-1.0.0.dist-info/RECORD
-5 files, 2882 bytes uncompressed, 1099 bytes compressed:  61.9%
+Zip file size: 2108 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     2037 b- defN 23-May-14 12:31 secure_id.py
+-rw-r--r--  2.0 unx     1110 b- defN 23-May-14 12:49 secureid-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 12:49 secureid-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-14 12:49 secureid-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      371 b- defN 23-May-14 12:49 secureid-1.0.1.dist-info/RECORD
+5 files, 3620 bytes uncompressed, 1418 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: secure_id.py
 Comment: 
 
-Filename: secureid-1.0.0.dist-info/METADATA
+Filename: secureid-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: secureid-1.0.0.dist-info/WHEEL
+Filename: secureid-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: secureid-1.0.0.dist-info/top_level.txt
+Filename: secureid-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: secureid-1.0.0.dist-info/RECORD
+Filename: secureid-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## secure_id.py

```diff
@@ -1,10 +1,10 @@
 import random
 from random import sample
-__version__="1.0.0"
+__version__="1.0.1"
 lettremin=["a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z"]
 lettremaj=["A","B","C","D","E","F","G","H","I","J","K","L","M","N","O","P","Q","R","S","T","U","V","W","X","Y","Z"]
 chiffre=["0","1","2","3","4","5","6","7","8","9"]
 def sid1():
     ensemble=lettremin+lettremaj+chiffre
     random.shuffle(ensemble)
     boucle=int(random.choice(chiffre))
```

