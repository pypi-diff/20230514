# Comparing `tmp/t2f-0.1.4.tar.gz` & `tmp/t2f-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2f-0.1.4.tar", max compression
+gzip compressed data, was "t2f-0.1.5.tar", max compression
```

## Comparing `t2f-0.1.4.tar` & `t2f-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.4/README.md
--rw-r--r--   0        0        0      347 2023-05-14 04:43:49.078125 t2f-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.4/t2f/__init__.py
--rw-r--r--   0        0        0    43498 2023-05-14 06:04:24.092256 t2f-0.1.4/t2f/patched_asm.py
--rw-r--r--   0        0        0    33456 2023-05-14 06:38:45.515126 t2f-0.1.4/t2f/stdlib.py
--rw-r--r--   0        0        0    11839 2023-05-14 06:38:02.839076 t2f-0.1.4/t2f/t2f.py
--rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.4/t2f/utils.py
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.5/README.md
+-rw-r--r--   0        0        0      347 2023-05-14 07:13:25.871669 t2f-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.5/t2f/__init__.py
+-rw-r--r--   0        0        0    43498 2023-05-14 07:08:34.228998 t2f-0.1.5/t2f/patched_asm.py
+-rw-r--r--   0        0        0    33456 2023-05-14 06:38:45.515126 t2f-0.1.5/t2f/stdlib.py
+-rw-r--r--   0        0        0    11839 2023-05-14 06:38:02.839076 t2f-0.1.5/t2f/t2f.py
+-rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.5/t2f/utils.py
+-rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.5/PKG-INFO
```

### Comparing `t2f-0.1.4/t2f/patched_asm.py` & `t2f-0.1.5/t2f/patched_asm.py`

 * *Files 0% similar despite different names*

```diff
@@ -616,15 +616,15 @@
 x{CF3C} @Defop(8u+1) BCHKBITSQ#
 x{CF3D} @Defop BCHKBITSQ
 x{CF3E} @Defop BCHKREFSQ
 x{CF3F} @Defop BCHKBITREFSQ
 x{CF40} @Defop STZEROES
 x{CF41} @Defop STONES
 x{CF42} @Defop STSAME
-{ tuck sbitrefs swap 15 + swap @havebitrefs not
+{ tuck sbitrefs swap 23 + swap @havebitrefs not
   { swap PUSHSLICE STSLICER }
   { over sbitrefs 2dup 57 3 2x<=
     { rot x{CFC_} s, swap 2 u, over 6 + 3 >> tuck 3 u, 3 roll s,
       -rot 3 << 2 + swap - @scomplete }
     { 2drop swap PUSHSLICE STSLICER } cond
   } cond
 } : STSLICECONST
```

### Comparing `t2f-0.1.4/t2f/stdlib.py` & `t2f-0.1.5/t2f/stdlib.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.4/t2f/t2f.py` & `t2f-0.1.5/t2f/t2f.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.4/t2f/utils.py` & `t2f-0.1.5/t2f/utils.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.4/PKG-INFO` & `t2f-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2f
-Version: 0.1.4
+Version: 0.1.5
 Summary: TVM Assembly to Fift Assembly Translator
 Author: Andrew Gutarev
 Author-email: gutarev01@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

