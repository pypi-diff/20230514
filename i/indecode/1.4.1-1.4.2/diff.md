# Comparing `tmp/indecode-1.4.1-py3-none-any.whl.zip` & `tmp/indecode-1.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2821 bytes, number of entries: 5
--rw-r--r--  2.0 unx     2970 b- defN 23-May-14 10:39 indecode.py
--rw-r--r--  2.0 unx     3163 b- defN 23-May-14 10:40 indecode-1.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-14 10:40 indecode-1.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-14 10:40 indecode-1.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      369 b- defN 23-May-14 10:40 indecode-1.4.1.dist-info/RECORD
-5 files, 6603 bytes uncompressed, 2133 bytes compressed:  67.7%
+Zip file size: 2803 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     2970 b- defN 23-May-14 10:42 indecode.py
+-rw-r--r--  2.0 unx     3122 b- defN 23-May-14 10:42 indecode-1.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 10:42 indecode-1.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-14 10:42 indecode-1.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      369 b- defN 23-May-14 10:42 indecode-1.4.2.dist-info/RECORD
+5 files, 6562 bytes uncompressed, 2115 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: indecode.py
 Comment: 
 
-Filename: indecode-1.4.1.dist-info/METADATA
+Filename: indecode-1.4.2.dist-info/METADATA
 Comment: 
 
-Filename: indecode-1.4.1.dist-info/WHEEL
+Filename: indecode-1.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: indecode-1.4.1.dist-info/top_level.txt
+Filename: indecode-1.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: indecode-1.4.1.dist-info/RECORD
+Filename: indecode-1.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indecode.py

```diff
@@ -1,9 +1,9 @@
 import random
-__version__="1.4.1"
+__version__="1.4.2"
 text="hello world"
 carac=["a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z","A","B","C","D","E","F","G","H","I","J","K","L","M","N","O","P","Q","R","S","T","U","V","W","X","Y","Z","0","1","2","3","4","5","6","7","8","9","&","é","~",'"',"#","{","}","(",")","[","]","-","è","_","\\","ç","^","à","@","°","+","=","ê","ë","$","£","%","ù","µ","*",",","?",".",";",":","/","!","§"]
 class CodeError(Exception):
     pass
 class DecodeError(Exception):
     pass
 class KeyElementError(Exception):
```

## Comparing `indecode-1.4.1.dist-info/METADATA` & `indecode-1.4.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 Metadata-Version: 2.1
 Name: indecode
-Version: 1.4.1
+Version: 1.4.2
 Summary: Code and decode string
 Author: lolo859
 License: UNKNOWN
 Keywords: code,incode,indecode,decode,incode,indc
 Platform: UNKNOWN
 Classifier: Natural Language :: French
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Code Generators
-Description-Content-Type: #Install and import
+Description-Content-Type: For install indecode : 
 Requires-Dist: docutils (>=0.3)
 
-For install indecode : 
-
 ~~~shell
 pip install indecode
 ~~~
 
 For import indecode :
 
 ~~~python
 import indecode
 ~~~
 
-#Functions
-
 This module contain three functions :
 
 - generate_key() - return string
 
 ~~~python
 import indecode
 key=indecode.generate_key()
@@ -53,16 +49,14 @@
 text="hello world"
 incode=indecode.code(text,key)
 print(incode)
 uncode=indecode.decode(incode,key)
 print(uncode)
 ~~~
 
-#Error
-
 The indecode module can trigger the following errors :
 
 - TypeError : one of the arguments is not a string
 
 ~~~
 >>> indecode.code(1,key)
 Traceback (most recent call last):
```

