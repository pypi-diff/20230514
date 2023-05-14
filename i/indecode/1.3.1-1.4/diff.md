# Comparing `tmp/indecode-1.3.1-py3-none-any.whl.zip` & `tmp/indecode-1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2263 bytes, number of entries: 5
--rw-r--r--  2.0 unx     2912 b- defN 23-May-13 17:34 indecode.py
--rw-r--r--  2.0 unx     1025 b- defN 23-May-13 17:35 indecode-1.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-13 17:35 indecode-1.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-13 17:35 indecode-1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      369 b- defN 23-May-13 17:35 indecode-1.3.1.dist-info/RECORD
-5 files, 4407 bytes uncompressed, 1575 bytes compressed:  64.3%
+Zip file size: 2802 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     2968 b- defN 23-May-14 10:19 indecode.py
+-rw-r--r--  2.0 unx     3337 b- defN 23-May-14 10:35 indecode-1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 10:35 indecode-1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-14 10:35 indecode-1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      361 b- defN 23-May-14 10:35 indecode-1.4.dist-info/RECORD
+5 files, 6767 bytes uncompressed, 2130 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: indecode.py
 Comment: 
 
-Filename: indecode-1.3.1.dist-info/METADATA
+Filename: indecode-1.4.dist-info/METADATA
 Comment: 
 
-Filename: indecode-1.3.1.dist-info/WHEEL
+Filename: indecode-1.4.dist-info/WHEEL
 Comment: 
 
-Filename: indecode-1.3.1.dist-info/top_level.txt
+Filename: indecode-1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: indecode-1.3.1.dist-info/RECORD
+Filename: indecode-1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indecode.py

```diff
@@ -1,9 +1,9 @@
 import random
-__version__="1.3.1"
+__version__="1.4"
 text="hello world"
 carac=["a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z","A","B","C","D","E","F","G","H","I","J","K","L","M","N","O","P","Q","R","S","T","U","V","W","X","Y","Z","0","1","2","3","4","5","6","7","8","9","&","é","~",'"',"#","{","}","(",")","[","]","-","è","_","\\","ç","^","à","@","°","+","=","ê","ë","$","£","%","ù","µ","*",",","?",".",";",":","/","!","§"]
 class CodeError(Exception):
     pass
 class DecodeError(Exception):
     pass
 class KeyElementError(Exception):
@@ -29,14 +29,15 @@
         raise KeyLengthError("the key is not of the expected length.")
     for i in range(len(keylist)):
         if not keylist[i] in carac:
             raise KeyElementError("'"+keylist[i]+"' must not be in the key.")
     for i in range(len(key)):
         incode.update({carac[i]:key[i]})
     incode.update({" ":" "})
+    incode.update({"'":"'"})
     for i in range(len(text)):
         if not text[i] in incode:
             raise CodeError("'"+text[i]+"' is not encodable.")
         newtext=newtext+incode[text[i]]
     return newtext
 def decode(text,key):
     newtext=""
@@ -50,14 +51,15 @@
         raise KeyLengthError("the key is not of the expected length.")
     for i in range(len(keylist)):
         if not keylist[i] in carac:
             raise KeyElementError("'"+keylist[i]+"' must not be in the key.")
     for i in range(len(key)):
         uncode.update({key[i]:carac[i]})
     uncode.update({" ":" "})
+    uncode.update({"'":"'"})
     for i in range(len(text)):
         if not text[i] in uncode:
             raise DecodeError("'"+text[i]+"' is not decodable.")
         newtext=newtext+uncode[text[i]]
     return newtext
 if __name__=="__main__":
     keya=generate_key()
```

