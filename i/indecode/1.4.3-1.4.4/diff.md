# Comparing `tmp/indecode-1.4.3-py3-none-any.whl.zip` & `tmp/indecode-1.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2709 bytes, number of entries: 5
--rw-r--r--  2.0 unx     2970 b- defN 23-May-14 10:57 indecode.py
--rw-r--r--  2.0 unx     3418 b- defN 23-May-14 10:57 indecode-1.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-14 10:57 indecode-1.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-14 10:57 indecode-1.4.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      369 b- defN 23-May-14 10:57 indecode-1.4.3.dist-info/RECORD
-5 files, 6858 bytes uncompressed, 2021 bytes compressed:  70.5%
+Zip file size: 2697 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     2970 b- defN 23-May-14 11:02 indecode.py
+-rw-r--r--  2.0 unx     3374 b- defN 23-May-14 11:02 indecode-1.4.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 11:02 indecode-1.4.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-14 11:02 indecode-1.4.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      369 b- defN 23-May-14 11:02 indecode-1.4.4.dist-info/RECORD
+5 files, 6814 bytes uncompressed, 2009 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: indecode.py
 Comment: 
 
-Filename: indecode-1.4.3.dist-info/METADATA
+Filename: indecode-1.4.4.dist-info/METADATA
 Comment: 
 
-Filename: indecode-1.4.3.dist-info/WHEEL
+Filename: indecode-1.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: indecode-1.4.3.dist-info/top_level.txt
+Filename: indecode-1.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: indecode-1.4.3.dist-info/RECORD
+Filename: indecode-1.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indecode.py

```diff
@@ -1,9 +1,9 @@
 import random
-__version__="1.4.3"
+__version__="1.4.4"
 text="hello world"
 carac=["a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z","A","B","C","D","E","F","G","H","I","J","K","L","M","N","O","P","Q","R","S","T","U","V","W","X","Y","Z","0","1","2","3","4","5","6","7","8","9","&","é","~",'"',"#","{","}","(",")","[","]","-","è","_","\\","ç","^","à","@","°","+","=","ê","ë","$","£","%","ù","µ","*",",","?",".",";",":","/","!","§"]
 class CodeError(Exception):
     pass
 class DecodeError(Exception):
     pass
 class KeyElementError(Exception):
```

## Comparing `indecode-1.4.3.dist-info/METADATA` & `indecode-1.4.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: indecode
-Version: 1.4.3
+Version: 1.4.4
 Summary: Code and decode string
 Author: lolo859
 License: UNKNOWN
 Keywords: code,incode,indecode,decode,incode,indc
 Platform: UNKNOWN
 Classifier: Natural Language :: French
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Code Generators
-Description-Content-Type: indecode
+Description-Content-Type: Installation and import
 Requires-Dist: docutils (>=0.3)
 
-========
-*Code and decode string*
-
-Installation and import
 -----------------------
 
 For install indecode : 
 
 .. code-block:: bash
 
     pip install indecode
```

