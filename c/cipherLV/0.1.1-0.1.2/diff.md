# Comparing `tmp/cipherLV-0.1.1.tar.gz` & `tmp/cipherLV-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipherLV-0.1.1.tar", last modified: Sat May 13 18:32:55 2023, max compression
+gzip compressed data, was "cipherLV-0.1.2.tar", last modified: Sun May 14 18:15:19 2023, max compression
```

## Comparing `cipherLV-0.1.1.tar` & `cipherLV-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 18:32:55.607060 cipherLV-0.1.1/
--rw-rw-rw-   0        0        0      780 2023-05-13 18:32:55.605390 cipherLV-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-05-13 18:16:31.000000 cipherLV-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 18:32:55.577932 cipherLV-0.1.1/cipherLV/
--rw-rw-rw-   0        0        0      107 2023-05-13 18:32:07.000000 cipherLV-0.1.1/cipherLV/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-05-13 16:55:55.000000 cipherLV-0.1.1/cipherLV/cipherLV.py
-drwxrwxrwx   0        0        0        0 2023-05-13 18:32:55.598961 cipherLV-0.1.1/cipherLV.egg-info/
--rw-rw-rw-   0        0        0      780 2023-05-13 18:32:55.000000 cipherLV-0.1.1/cipherLV.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-05-13 18:32:55.000000 cipherLV-0.1.1/cipherLV.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 18:32:55.000000 cipherLV-0.1.1/cipherLV.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-13 18:32:55.000000 cipherLV-0.1.1/cipherLV.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 18:32:55.608056 cipherLV-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-05-13 18:31:51.000000 cipherLV-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 18:15:19.160126 cipherLV-0.1.2/
+-rw-rw-rw-   0        0        0      795 2023-05-14 18:15:19.159123 cipherLV-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       98 2023-05-13 18:16:31.000000 cipherLV-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 18:15:19.151455 cipherLV-0.1.2/cipherLV.egg-info/
+-rw-rw-rw-   0        0        0      795 2023-05-14 18:15:18.000000 cipherLV-0.1.2/cipherLV.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-05-14 18:15:18.000000 cipherLV-0.1.2/cipherLV.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 18:15:18.000000 cipherLV-0.1.2/cipherLV.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 18:15:18.000000 cipherLV-0.1.2/cipherLV.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1563 2023-05-14 06:41:30.000000 cipherLV-0.1.2/cipherLV.py
+-rw-rw-rw-   0        0        0       42 2023-05-14 18:15:19.162186 cipherLV-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-05-14 14:37:07.000000 cipherLV-0.1.2/setup.py
```

### Comparing `cipherLV-0.1.1/PKG-INFO` & `cipherLV-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cipherLV
-Version: 0.1.1
+Version: 0.1.2
 Summary: Description: LV cipher is used for encrypting and decrypting with symmetric key
 Home-page: UNKNOWN
 Author: sarath babu
-Author-email: babusarath05@gmail.com
+Author-email: sarathbabu.karunanithi@latentview.com
 License: UNKNOWN
 Description: 
         <h1> LV cipher </h1>
         <h2> LV cipher is used for encrypting and decrypting with symmetric key</h2>
         
 Keywords: python,encryption,decryption,cryptography
 Platform: UNKNOWN
```

### Comparing `cipherLV-0.1.1/cipherLV/cipherLV.py` & `cipherLV-0.1.2/cipherLV.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Mar 16 21:44:59 2022
 
 @author: sarathbabu
 """
 
-def decrypt(text,s):
+def encrypt(text,s=3):
+    """Performs Encryption of the text data with a symmetric key number s.
+    
+    Parameters:
+        text(string) : Input text to be encrypted
+        
+        s(int) : Default value = 3, Symmetric Key number to perform ciphering
+        
+    Returns:
+        string: Encrypted Input text 
+    """
     result = ""
     # transverse the plain text
     for i in range(len(text)):
         char = text[i]
         # Encrypt uppercase characters in plain text
-
+    
         if (char.isupper()):
-            result += chr((ord(char) - s-65) % 26 + 65)
+            result += chr((ord(char) + s-65) % 26 + 65)
         # Encrypt lowercase characters in plain text
         else:
-            result += chr((ord(char) - s - 97) % 26 + 97)
+            result += chr((ord(char) + s - 97) % 26 + 97)
     return result
 
-def encrypt(text,s):
-    """Performs Encryption of the text data with a key number s.
+def decrypt(text,s=3):
+    """Performs Decryption of the text data with a symmetric key number s.
     
     Parameters:
-        text(string) : Input text to be encrypted
+        text(string) : Input text to be decrypted
         
-        s(int) : Key Number to perform ciphering
+        s(int) : Default value = 3, Symmetric Key number to perform ciphering
         
     Returns:
-        string: Encrypted Input text
-        
+        string: Decrypted Input text 
     """
     result = ""
     # transverse the plain text
     for i in range(len(text)):
         char = text[i]
-        # Encrypt uppercase characters in plain text
-    
+        # Decrypt uppercase characters in plain text
+
         if (char.isupper()):
-            result += chr((ord(char) + s-65) % 26 + 65)
-        # Encrypt lowercase characters in plain text
+            result += chr((ord(char) - s-65) % 26 + 65)
+        # Decrypt lowercase characters in plain text
         else:
-            result += chr((ord(char) + s - 97) % 26 + 97)
-    return result
-
+            result += chr((ord(char) - s - 97) % 26 + 97)
+    return result
```

### Comparing `cipherLV-0.1.1/cipherLV.egg-info/PKG-INFO` & `cipherLV-0.1.2/cipherLV.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cipherLV
-Version: 0.1.1
+Version: 0.1.2
 Summary: Description: LV cipher is used for encrypting and decrypting with symmetric key
 Home-page: UNKNOWN
 Author: sarath babu
-Author-email: babusarath05@gmail.com
+Author-email: sarathbabu.karunanithi@latentview.com
 License: UNKNOWN
 Description: 
         <h1> LV cipher </h1>
         <h2> LV cipher is used for encrypting and decrypting with symmetric key</h2>
         
 Keywords: python,encryption,decryption,cryptography
 Platform: UNKNOWN
```

### Comparing `cipherLV-0.1.1/setup.py` & `cipherLV-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,28 +3,26 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.1'
-DESCRIPTION = 'Description: LV cipher is used for encrypting and decrypting with symmetric key'
-#LONG_DESCRIPTION = 'Long Description: LV Cipher is used for encrypting and decrypting with symmetric key'
 
 # Setting up
 setup(
     name="cipherLV",
-    version=VERSION,
+    version='0.1.2',
     author="sarath babu",
-    author_email="babusarath05@gmail.com",
-    description=DESCRIPTION,
+    author_email="sarathbabu.karunanithi@latentview.com",
+    description='Description: LV cipher is used for encrypting and decrypting with symmetric key',
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
+    py_modules=['cipherLV'],
     #install_requires=['sklearn','pandas'],
     keywords=['python', 'encryption','decryption','cryptography'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

