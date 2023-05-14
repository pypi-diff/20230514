# Comparing `tmp/indecode-1.4.2-py3-none-any.whl.zip` & `tmp/indecode-1.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2803 bytes, number of entries: 5
--rw-r--r--  2.0 unx     2970 b- defN 23-May-14 10:42 indecode.py
--rw-r--r--  2.0 unx     3122 b- defN 23-May-14 10:42 indecode-1.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-14 10:42 indecode-1.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-14 10:42 indecode-1.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      369 b- defN 23-May-14 10:42 indecode-1.4.2.dist-info/RECORD
-5 files, 6562 bytes uncompressed, 2115 bytes compressed:  67.8%
+Zip file size: 2709 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     2970 b- defN 23-May-14 10:57 indecode.py
+-rw-r--r--  2.0 unx     3418 b- defN 23-May-14 10:57 indecode-1.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-14 10:57 indecode-1.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-14 10:57 indecode-1.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      369 b- defN 23-May-14 10:57 indecode-1.4.3.dist-info/RECORD
+5 files, 6858 bytes uncompressed, 2021 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: indecode.py
 Comment: 
 
-Filename: indecode-1.4.2.dist-info/METADATA
+Filename: indecode-1.4.3.dist-info/METADATA
 Comment: 
 
-Filename: indecode-1.4.2.dist-info/WHEEL
+Filename: indecode-1.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: indecode-1.4.2.dist-info/top_level.txt
+Filename: indecode-1.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: indecode-1.4.2.dist-info/RECORD
+Filename: indecode-1.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indecode.py

```diff
@@ -1,9 +1,9 @@
 import random
-__version__="1.4.2"
+__version__="1.4.3"
 text="hello world"
 carac=["a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z","A","B","C","D","E","F","G","H","I","J","K","L","M","N","O","P","Q","R","S","T","U","V","W","X","Y","Z","0","1","2","3","4","5","6","7","8","9","&","é","~",'"',"#","{","}","(",")","[","]","-","è","_","\\","ç","^","à","@","°","+","=","ê","ë","$","£","%","ù","µ","*",",","?",".",";",":","/","!","§"]
 class CodeError(Exception):
     pass
 class DecodeError(Exception):
     pass
 class KeyElementError(Exception):
```

## Comparing `indecode-1.4.2.dist-info/METADATA` & `indecode-1.4.3.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,128 @@
 Metadata-Version: 2.1
 Name: indecode
-Version: 1.4.2
+Version: 1.4.3
 Summary: Code and decode string
 Author: lolo859
 License: UNKNOWN
 Keywords: code,incode,indecode,decode,incode,indc
 Platform: UNKNOWN
 Classifier: Natural Language :: French
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Code Generators
-Description-Content-Type: For install indecode : 
+Description-Content-Type: indecode
 Requires-Dist: docutils (>=0.3)
 
-~~~shell
-pip install indecode
-~~~
+========
+*Code and decode string*
+
+Installation and import
+-----------------------
+
+For install indecode : 
+
+.. code-block:: bash
+
+    pip install indecode
 
 For import indecode :
 
-~~~python
-import indecode
-~~~
+.. code-block:: python
+
+    import indecode
+
+Functions
+---------
 
 This module contain three functions :
 
 - generate_key() - return string
 
-~~~python
-import indecode
-key=indecode.generate_key()
-~~~
+.. code-block:: python
+
+    import indecode
+    key=indecode.generate_key()
 
 - code(text to code in str, key return by the "generate_key()" function) - return string
 
-~~~python
-import indecode
-key=indecode.generate_key()
-text="hello world"
-incode=indecode.code(text,key)
-print(incode)
-~~~
+.. code-block:: python
+
+    import indecode
+    key=indecode.generate_key()
+    text="hello world"
+    incode=indecode.code(text,key)
+    print(incode)
 
 - decode(text return by the "code()" function, key return by the "generate_key()" function) - return string
 
-~~~python
-import indecode
-key=indecode.generate_key()
-text="hello world"
-incode=indecode.code(text,key)
-print(incode)
-uncode=indecode.decode(incode,key)
-print(uncode)
-~~~
+.. code-block:: python
+
+    import indecode
+    key=indecode.generate_key()
+    text="hello world"
+    incode=indecode.code(text,key)
+    print(incode)
+    uncode=indecode.decode(incode,key)
+    print(uncode)
+
+Errors
+------
 
 The indecode module can trigger the following errors :
 
 - TypeError : one of the arguments is not a string
 
-~~~
->>> indecode.code(1,key)
-Traceback (most recent call last):
-  File "<stdin>", line 1, in <module>
-  File "/home/pi/Documents/indecode/indecode.py", line 24, in code
-    raise TypeError("text argument must be a string")
-TypeError: text argument must be a string
-~~~
+.. code-block:: python
+
+    >>> indecode.code(1,key)
+    Traceback (most recent call last):
+    File "<stdin>", line 1, in <module>
+    File "/home/pi/Documents/indecode/indecode.py", line 24, in code
+        raise TypeError("text argument must be a string")
+    TypeError: text argument must be a string
 
 - CodeError : one of the caracters in the text argument is not encodable
 
-~~~
->>> indecode.code("<",key)
-Traceback (most recent call last):
-  File "<stdin>", line 1, in <module>
-  File "/home/pi/Documents/indecode/indecode.py", line 38, in code
-    raise CodeError("'"+text[i]+"' is not encodable.")
-indecode.CodeError: '<' is not encodable.
-~~~
+.. code-block:: python
+
+    >>> indecode.code("<",key)
+    Traceback (most recent call last):
+    File "<stdin>", line 1, in <module>
+    File "/home/pi/Documents/indecode/indecode.py", line 38, in code
+        raise CodeError("'"+text[i]+"' is not encodable.")
+    indecode.CodeError: '<' is not encodable.
 
 - DecodeError : one of the caracters in the text argument is not decodable
 
-~~~
->>> indecode.decode(">",key)
-Traceback (most recent call last):
-  File "<stdin>", line 1, in <module>
-  File "/home/pi/Documents/indecode/indecode.py", line 59, in decode
-    raise DecodeError("'"+text[i]+"' is not decodable.")
-indecode.DecodeError: '>' is not decodable.
-~~~
+.. code-block:: python
+
+    >>> indecode.decode(">",key)
+    Traceback (most recent call last):
+    File "<stdin>", line 1, in <module>
+    File "/home/pi/Documents/indecode/indecode.py", line 59, in decode
+        raise DecodeError("'"+text[i]+"' is not decodable.")
+    indecode.DecodeError: '>' is not decodable.
 
 - KeyElementError : one of the caracters in the key argument must not be in the key
 
-~~~
->>> print(key)
-KBm%z5oèëMUaEPY\ldxn@98Hyà:T;N2we)DGZ[°W{JF(s}r-çiS§*,4.b60µ!t&ùVvI3#C]?7Aê£hQ=gu~f+1_Xq^"$péOjLk/c<
->>> indecode.code("hello world",key)
-Traceback (most recent call last):
-  File "<stdin>", line 1, in <module>
-  File "/home/pi/Documents/indecode/indecode.py", line 32, in code
-    raise KeyElementError("'"+keylist[i]+"' must not be in the key.")
-indecode.KeyElementError: '<' must not be in the key.
-~~~
+.. code-block:: python
+
+    >>> indecode.code("hello world",key)
+    Traceback (most recent call last):
+    File "<stdin>", line 1, in <module>
+    File "/home/pi/Documents/indecode/indecode.py", line 32, in code
+        raise KeyElementError("'"+keylist[i]+"' must not be in the key.")
+    indecode.KeyElementError: '<' must not be in the key.
 
 - KeyLengthError : the key is not of the expected length.
 
-~~~
->>> indecode.code("hello world",key="a")
-Traceback (most recent call last):
-  File "<stdin>", line 1, in <module>
-  File "/home/pi/Documents/indecode/indecode.py", line 29, in code
-    raise KeyLengthError("the key is not of the expected length.")
-indecode.KeyLengthError: the key is not of the expected length.
-~~~
+.. code-block:: python
+
+    >>> indecode.code("hello world",key="a")
+    Traceback (most recent call last):
+    File "<stdin>", line 1, in <module>
+    File "/home/pi/Documents/indecode/indecode.py", line 29, in code
+        raise KeyLengthError("the key is not of the expected length.")
+    indecode.KeyLengthError: the key is not of the expected length.
 
 UNKNOWN
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

