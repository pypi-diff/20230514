# Comparing `tmp/chatcmd-1.0.1-py3-none-any.whl.zip` & `tmp/chatcmd-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6667 bytes, number of entries: 11
+Zip file size: 6668 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-26 12:02 chatcmd/__init__.py
 -rw-r--r--  2.0 unx     1644 b- defN 23-May-13 16:35 chatcmd/api.py
 -rw-r--r--  2.0 unx     3355 b- defN 23-May-13 20:46 chatcmd/chatcmd.py
 -rw-r--r--  2.0 unx     3770 b- defN 23-May-02 11:20 chatcmd/commands.py
 -rw-r--r--  2.0 unx     2147 b- defN 23-May-13 16:29 chatcmd/helpers.py
 -rw-r--r--  2.0 unx     2615 b- defN 23-May-11 23:45 chatcmd/lookup.py
--rw-r--r--  2.0 unx      594 b- defN 23-May-13 22:58 chatcmd-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-13 22:58 chatcmd-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-May-13 22:58 chatcmd-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-May-13 22:58 chatcmd-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      835 b- defN 23-May-13 22:58 chatcmd-1.0.1.dist-info/RECORD
-11 files, 15109 bytes uncompressed, 5263 bytes compressed:  65.2%
+-rw-r--r--  2.0 unx      594 b- defN 23-May-13 23:00 chatcmd-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-13 23:00 chatcmd-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-May-13 23:00 chatcmd-1.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-13 23:00 chatcmd-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      835 b- defN 23-May-13 23:00 chatcmd-1.0.2.dist-info/RECORD
+11 files, 15109 bytes uncompressed, 5264 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: chatcmd/helpers.py
 Comment: 
 
 Filename: chatcmd/lookup.py
 Comment: 
 
-Filename: chatcmd-1.0.1.dist-info/METADATA
+Filename: chatcmd-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: chatcmd-1.0.1.dist-info/WHEEL
+Filename: chatcmd-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: chatcmd-1.0.1.dist-info/entry_points.txt
+Filename: chatcmd-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: chatcmd-1.0.1.dist-info/top_level.txt
+Filename: chatcmd-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: chatcmd-1.0.1.dist-info/RECORD
+Filename: chatcmd-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `chatcmd-1.0.1.dist-info/METADATA` & `chatcmd-1.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.1
+Version: 1.0.2
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
```

## Comparing `chatcmd-1.0.1.dist-info/RECORD` & `chatcmd-1.0.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 chatcmd/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chatcmd/api.py,sha256=ak7hgCREYNeMEW0dB7efwnY8LUoCSMt5j2ZicHD02xk,1644
 chatcmd/chatcmd.py,sha256=AuoowrXe7-p-WDSOGDweMxM3KTBrBomNZCDDnbehKLM,3355
 chatcmd/commands.py,sha256=IbSIg-91ehT9Y9cz4gMCR15nf0zgTMK3oHXGYh5hWJU,3770
 chatcmd/helpers.py,sha256=_0543WTFqITsWCSG0A8i0JeNnpZswnuW4nLTMD21H90,2147
 chatcmd/lookup.py,sha256=UYOXnlRGaQTsxoFleUQtS1C12OgNY4guIokd11dgHVQ,2615
-chatcmd-1.0.1.dist-info/METADATA,sha256=5U-BL5-l611H2W5YTk0jZjZNaO-Xb_qPuwagTlAKwy4,594
-chatcmd-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-chatcmd-1.0.1.dist-info/entry_points.txt,sha256=SHisZXK06nIcJH7cI0-lPRPeT0aiyOUVS1-K_5EsLS8,49
-chatcmd-1.0.1.dist-info/top_level.txt,sha256=qLr2vX8BWYFHYfgwuOmgkw0PGTyTUEqT9k_S69YU0nE,8
-chatcmd-1.0.1.dist-info/RECORD,,
+chatcmd-1.0.2.dist-info/METADATA,sha256=XFlbdGprga766zGiK0_vUmcBLO8prBMoGujcvYVICj8,594
+chatcmd-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+chatcmd-1.0.2.dist-info/entry_points.txt,sha256=SHisZXK06nIcJH7cI0-lPRPeT0aiyOUVS1-K_5EsLS8,49
+chatcmd-1.0.2.dist-info/top_level.txt,sha256=qLr2vX8BWYFHYfgwuOmgkw0PGTyTUEqT9k_S69YU0nE,8
+chatcmd-1.0.2.dist-info/RECORD,,
```

