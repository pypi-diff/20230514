# Comparing `tmp/indecode-1.4.7-py3-none-any.whl.zip` & `tmp/indecode-1.4.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2637 bytes, number of entries: 5
--rw-r--r--  2.0 unx     2970 b- defN 23-May-14 11:18 indecode.py
--rw-r--r--  2.0 unx     2866 b- defN 23-May-14 11:19 indecode-1.4.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-14 11:19 indecode-1.4.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-14 11:19 indecode-1.4.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      369 b- defN 23-May-14 11:19 indecode-1.4.7.dist-info/RECORD
-5 files, 6306 bytes uncompressed, 1949 bytes compressed:  69.1%
+Zip file size: 2615 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     2970 b- defN 23-May-14 11:20 indecode.py
+-rw-r--r--  2.0 unx     2832 b- defN 23-May-14 11:21 indecode-1.4.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 11:21 indecode-1.4.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-14 11:21 indecode-1.4.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      369 b- defN 23-May-14 11:21 indecode-1.4.8.dist-info/RECORD
+5 files, 6272 bytes uncompressed, 1927 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: indecode.py
 Comment: 
 
-Filename: indecode-1.4.7.dist-info/METADATA
+Filename: indecode-1.4.8.dist-info/METADATA
 Comment: 
 
-Filename: indecode-1.4.7.dist-info/WHEEL
+Filename: indecode-1.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: indecode-1.4.7.dist-info/top_level.txt
+Filename: indecode-1.4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: indecode-1.4.7.dist-info/RECORD
+Filename: indecode-1.4.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indecode.py

```diff
@@ -1,9 +1,9 @@
 import random
-__version__="1.4.7"
+__version__="1.4.8"
 text="hello world"
 carac=["a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z","A","B","C","D","E","F","G","H","I","J","K","L","M","N","O","P","Q","R","S","T","U","V","W","X","Y","Z","0","1","2","3","4","5","6","7","8","9","&","é","~",'"',"#","{","}","(",")","[","]","-","è","_","\\","ç","^","à","@","°","+","=","ê","ë","$","£","%","ù","µ","*",",","?",".",";",":","/","!","§"]
 class CodeError(Exception):
     pass
 class DecodeError(Exception):
     pass
 class KeyElementError(Exception):
```

## Comparing `indecode-1.4.7.dist-info/METADATA` & `indecode-1.4.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: indecode
-Version: 1.4.7
+Version: 1.4.8
 Summary: Code and decode string
 Author: lolo859
 License: UNKNOWN
 Keywords: code,incode,indecode,decode,incode,indc
 Platform: UNKNOWN
 Classifier: Natural Language :: French
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Code Generators
-Description-Content-Type: For install indecode : 
 Requires-Dist: docutils (>=0.3)
 
+For install indecode : 
+
 pip install indecode
 
 For import indecode :
 
 import indecode
 
 This module contain three functions :
@@ -86,9 +87,7 @@
 >>> indecode.code("hello world",key="a")
 Traceback (most recent call last):
 File "<stdin>", line 1, in <module>
 File "/home/pi/Documents/indecode/indecode.py", line 29, in code
     raise KeyLengthError("the key is not of the expected length.")
 indecode.KeyLengthError: the key is not of the expected length.
 
-UNKNOWN
-
```

