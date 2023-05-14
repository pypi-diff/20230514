# Comparing `tmp/indecode-1.4.5-py3-none-any.whl.zip` & `tmp/indecode-1.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2639 bytes, number of entries: 5
--rw-r--r--  2.0 unx     2970 b- defN 23-May-14 11:07 indecode.py
--rw-r--r--  2.0 unx     2866 b- defN 23-May-14 11:07 indecode-1.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-14 11:07 indecode-1.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-14 11:07 indecode-1.4.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      369 b- defN 23-May-14 11:07 indecode-1.4.5.dist-info/RECORD
-5 files, 6306 bytes uncompressed, 1951 bytes compressed:  69.1%
+Zip file size: 2638 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     2970 b- defN 23-May-14 11:16 indecode.py
+-rw-r--r--  2.0 unx     2866 b- defN 23-May-14 11:17 indecode-1.4.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 11:17 indecode-1.4.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-14 11:17 indecode-1.4.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      369 b- defN 23-May-14 11:17 indecode-1.4.6.dist-info/RECORD
+5 files, 6306 bytes uncompressed, 1950 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: indecode.py
 Comment: 
 
-Filename: indecode-1.4.5.dist-info/METADATA
+Filename: indecode-1.4.6.dist-info/METADATA
 Comment: 
 
-Filename: indecode-1.4.5.dist-info/WHEEL
+Filename: indecode-1.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: indecode-1.4.5.dist-info/top_level.txt
+Filename: indecode-1.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: indecode-1.4.5.dist-info/RECORD
+Filename: indecode-1.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indecode.py

```diff
@@ -1,9 +1,9 @@
 import random
-__version__="1.4.5"
+__version__="1.4.6"
 text="hello world"
 carac=["a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z","A","B","C","D","E","F","G","H","I","J","K","L","M","N","O","P","Q","R","S","T","U","V","W","X","Y","Z","0","1","2","3","4","5","6","7","8","9","&","é","~",'"',"#","{","}","(",")","[","]","-","è","_","\\","ç","^","à","@","°","+","=","ê","ë","$","£","%","ù","µ","*",",","?",".",";",":","/","!","§"]
 class CodeError(Exception):
     pass
 class DecodeError(Exception):
     pass
 class KeyElementError(Exception):
```

## Comparing `indecode-1.4.5.dist-info/METADATA` & `indecode-1.4.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indecode
-Version: 1.4.5
+Version: 1.4.6
 Summary: Code and decode string
 Author: lolo859
 License: UNKNOWN
 Keywords: code,incode,indecode,decode,incode,indc
 Platform: UNKNOWN
 Classifier: Natural Language :: French
 Classifier: Topic :: Security :: Cryptography
```

