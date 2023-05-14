# Comparing `tmp/Inputbetter-0.4.0-py3-none-any.whl.zip` & `tmp/Inputbetter-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 1594 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat       29 b- defN 23-May-14 08:59 Inputbetter/__init__.py
+-rw-rw-rw-  2.0 fat       30 b- defN 23-May-14 09:06 Inputbetter/__init__.py
 -rw-rw-rw-  2.0 fat      440 b- defN 23-May-14 07:32 Inputbetter/functions.py
--rw-rw-rw-  2.0 fat      151 b- defN 23-May-14 09:00 Inputbetter-0.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-14 09:00 Inputbetter-0.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-14 09:00 Inputbetter-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      471 b- defN 23-May-14 09:00 Inputbetter-0.4.0.dist-info/RECORD
-6 files, 1195 bytes uncompressed, 734 bytes compressed:  38.6%
+-rw-rw-rw-  2.0 fat      151 b- defN 23-May-14 09:06 Inputbetter-0.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-14 09:06 Inputbetter-0.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-14 09:06 Inputbetter-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      471 b- defN 23-May-14 09:06 Inputbetter-0.5.0.dist-info/RECORD
+6 files, 1196 bytes uncompressed, 734 bytes compressed:  38.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: Inputbetter/__init__.py
 Comment: 
 
 Filename: Inputbetter/functions.py
 Comment: 
 
-Filename: Inputbetter-0.4.0.dist-info/METADATA
+Filename: Inputbetter-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: Inputbetter-0.4.0.dist-info/WHEEL
+Filename: Inputbetter-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: Inputbetter-0.4.0.dist-info/top_level.txt
+Filename: Inputbetter-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Inputbetter-0.4.0.dist-info/RECORD
+Filename: Inputbetter-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Inputbetter/__init__.py

```diff
@@ -1 +1 @@
-from functions import btrinpt
+from .functions import btrinpt
```

