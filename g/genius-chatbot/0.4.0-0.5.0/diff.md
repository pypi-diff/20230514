# Comparing `tmp/genius_chatbot-0.4.0-py2.py3-none-any.whl.zip` & `tmp/genius_chatbot-0.5.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5986 bytes, number of entries: 9
--rw-r--r--  2.0 unx      352 b- defN 22-Dec-23 04:20 genius_chatbot/__init__.py
--rw-r--r--  2.0 unx    10029 b- defN 22-Dec-23 07:29 genius_chatbot/genius_chatbot.py
--rw-r--r--  2.0 unx      116 b- defN 22-Dec-23 19:04 genius_chatbot/version.py
--rw-r--r--  2.0 unx     1210 b- defN 22-Dec-23 19:04 genius_chatbot-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2294 b- defN 22-Dec-23 19:04 genius_chatbot-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Dec-23 19:04 genius_chatbot-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 22-Dec-23 19:04 genius_chatbot-0.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 22-Dec-23 19:04 genius_chatbot-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      777 b- defN 22-Dec-23 19:04 genius_chatbot-0.4.0.dist-info/RECORD
-9 files, 14974 bytes uncompressed, 4632 bytes compressed:  69.1%
+Zip file size: 5987 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      352 b- defN 23-May-14 05:52 genius_chatbot/__init__.py
+-rw-r--r--  2.0 unx    10029 b- defN 23-May-14 05:52 genius_chatbot/genius_chatbot.py
+-rw-r--r--  2.0 unx      116 b- defN 23-May-14 05:52 genius_chatbot/version.py
+-rw-r--r--  2.0 unx     1210 b- defN 23-May-14 05:52 genius_chatbot-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2294 b- defN 23-May-14 05:52 genius_chatbot-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-14 05:52 genius_chatbot-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 23-May-14 05:52 genius_chatbot-0.5.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-May-14 05:52 genius_chatbot-0.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      777 b- defN 23-May-14 05:52 genius_chatbot-0.5.0.dist-info/RECORD
+9 files, 14974 bytes uncompressed, 4633 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: genius_chatbot/genius_chatbot.py
 Comment: 
 
 Filename: genius_chatbot/version.py
 Comment: 
 
-Filename: genius_chatbot-0.4.0.dist-info/LICENSE
+Filename: genius_chatbot-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: genius_chatbot-0.4.0.dist-info/METADATA
+Filename: genius_chatbot-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: genius_chatbot-0.4.0.dist-info/WHEEL
+Filename: genius_chatbot-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: genius_chatbot-0.4.0.dist-info/entry_points.txt
+Filename: genius_chatbot-0.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: genius_chatbot-0.4.0.dist-info/top_level.txt
+Filename: genius_chatbot-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: genius_chatbot-0.4.0.dist-info/RECORD
+Filename: genius_chatbot-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genius_chatbot/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `genius_chatbot-0.4.0.dist-info/LICENSE` & `genius_chatbot-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `genius_chatbot-0.4.0.dist-info/METADATA` & `genius_chatbot-0.5.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genius-chatbot
-Version: 0.4.0
+Version: 0.5.0
 Summary: Use huggingface models to create an intelligent and scalable chatbot
 Home-page: https://github.com/Knuckles-Team/genius-chatbot
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: Unlicense
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,18 +16,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate (>=0.15.0)
 Requires-Dist: psutil (>=5.9.4)
 Requires-Dist: torch (>=1.13.1)
-Requires-Dist: transformers (>=4.25.1)
+Requires-Dist: transformers (>=4.29.1)
 
 # Genius Chatbot
-*Version: 0.4.0*
+*Version: 0.5.0*
 
 Chatbot that uses any desired hugging face model or allows for scalable 
 intelligence based on hardware limitations
 
 ### Usage:
 | Short Flag | Long Flag       | Description                                |
 |------------|-----------------|--------------------------------------------|
```

