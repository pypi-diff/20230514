# Comparing `tmp/cipherLV-0.1.2.tar.gz` & `tmp/cipherLV-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipherLV-0.1.2.tar", last modified: Sun May 14 18:15:19 2023, max compression
+gzip compressed data, was "cipherLV-0.1.3.tar", last modified: Sun May 14 18:18:58 2023, max compression
```

## Comparing `cipherLV-0.1.2.tar` & `cipherLV-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 18:15:19.160126 cipherLV-0.1.2/
--rw-rw-rw-   0        0        0      795 2023-05-14 18:15:19.159123 cipherLV-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-05-13 18:16:31.000000 cipherLV-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 18:15:19.151455 cipherLV-0.1.2/cipherLV.egg-info/
--rw-rw-rw-   0        0        0      795 2023-05-14 18:15:18.000000 cipherLV-0.1.2/cipherLV.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-05-14 18:15:18.000000 cipherLV-0.1.2/cipherLV.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 18:15:18.000000 cipherLV-0.1.2/cipherLV.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 18:15:18.000000 cipherLV-0.1.2/cipherLV.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1563 2023-05-14 06:41:30.000000 cipherLV-0.1.2/cipherLV.py
--rw-rw-rw-   0        0        0       42 2023-05-14 18:15:19.162186 cipherLV-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-05-14 14:37:07.000000 cipherLV-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 18:18:58.919859 cipherLV-0.1.3/
+-rw-rw-rw-   0        0        0      919 2023-05-14 18:18:58.914860 cipherLV-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-05-14 18:18:38.000000 cipherLV-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 18:18:58.911042 cipherLV-0.1.3/cipherLV.egg-info/
+-rw-rw-rw-   0        0        0      919 2023-05-14 18:18:58.000000 cipherLV-0.1.3/cipherLV.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-05-14 18:18:58.000000 cipherLV-0.1.3/cipherLV.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 18:18:58.000000 cipherLV-0.1.3/cipherLV.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 18:18:58.000000 cipherLV-0.1.3/cipherLV.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1563 2023-05-14 06:41:30.000000 cipherLV-0.1.3/cipherLV.py
+-rw-rw-rw-   0        0        0       42 2023-05-14 18:18:58.920854 cipherLV-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-05-14 18:17:25.000000 cipherLV-0.1.3/setup.py
```

### Comparing `cipherLV-0.1.2/PKG-INFO` & `cipherLV-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: cipherLV
-Version: 0.1.2
+Version: 0.1.3
 Summary: Description: LV cipher is used for encrypting and decrypting with symmetric key
 Home-page: UNKNOWN
 Author: sarath babu
 Author-email: sarathbabu.karunanithi@latentview.com
 License: UNKNOWN
 Description: 
-        <h1> LV cipher </h1>
-        <h2> LV cipher is used for encrypting and decrypting with symmetric key</h2>
+        <h1> cipher LV</h1>
+        <h2> cipher LV is used for encrypting and decrypting with symmetric key</h2>
+        <p> cipher LV has two modules </p>
+        <ul>
+        <li>Encrypt</li>
+        <li>Decrypt</li>
+        </ul>
         
 Keywords: python,encryption,decryption,cryptography
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `cipherLV-0.1.2/cipherLV.egg-info/PKG-INFO` & `cipherLV-0.1.3/cipherLV.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: cipherLV
-Version: 0.1.2
+Version: 0.1.3
 Summary: Description: LV cipher is used for encrypting and decrypting with symmetric key
 Home-page: UNKNOWN
 Author: sarath babu
 Author-email: sarathbabu.karunanithi@latentview.com
 License: UNKNOWN
 Description: 
-        <h1> LV cipher </h1>
-        <h2> LV cipher is used for encrypting and decrypting with symmetric key</h2>
+        <h1> cipher LV</h1>
+        <h2> cipher LV is used for encrypting and decrypting with symmetric key</h2>
+        <p> cipher LV has two modules </p>
+        <ul>
+        <li>Encrypt</li>
+        <li>Decrypt</li>
+        </ul>
         
 Keywords: python,encryption,decryption,cryptography
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `cipherLV-0.1.2/cipherLV.py` & `cipherLV-0.1.3/cipherLV.py`

 * *Files identical despite different names*

### Comparing `cipherLV-0.1.2/setup.py` & `cipherLV-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
 # Setting up
 setup(
     name="cipherLV",
-    version='0.1.2',
+    version="0.1.3",
     author="sarath babu",
     author_email="sarathbabu.karunanithi@latentview.com",
     description='Description: LV cipher is used for encrypting and decrypting with symmetric key',
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     py_modules=['cipherLV'],
```

