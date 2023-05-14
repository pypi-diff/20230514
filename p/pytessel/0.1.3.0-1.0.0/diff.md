# Comparing `tmp/pytessel-0.1.3.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/pytessel-1.0.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 479591 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 14:26 pytessel-0.1.3.0.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 14:26 pytessel.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 14:26 pytessel/
--rw-rw-r--  2.0 unx      691 b- defN 23-May-14 14:26 pytessel-0.1.3.0.dist-info/RECORD
--rw-r--r--  2.0 unx      148 b- defN 23-May-14 14:26 pytessel-0.1.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-14 14:26 pytessel-0.1.3.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx    35121 b- defN 23-May-14 14:26 pytessel-0.1.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1736 b- defN 23-May-14 14:26 pytessel-0.1.3.0.dist-info/METADATA
--rwxr-xr-x  2.0 unx   168193 b- defN 23-May-14 14:26 pytessel.libs/libgomp-a34b3233.so.1.0.0
--rwxr-xr-x  2.0 unx  1434409 b- defN 23-May-14 14:26 pytessel/pytessel.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx       31 b- defN 23-May-14 14:26 pytessel/__init__.py
-11 files, 1640338 bytes uncompressed, 478071 bytes compressed:  70.9%
+Zip file size: 479783 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 16:23 pytessel.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 16:23 pytessel-1.0.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-14 16:23 pytessel/
+-rwxr-xr-x  2.0 unx   168193 b- defN 23-May-14 16:23 pytessel.libs/libgomp-a34b3233.so.1.0.0
+-rw-rw-r--  2.0 unx      681 b- defN 23-May-14 16:23 pytessel-1.0.0.dist-info/RECORD
+-rw-r--r--  2.0 unx      148 b- defN 23-May-14 16:23 pytessel-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-14 16:23 pytessel-1.0.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    35121 b- defN 23-May-14 16:23 pytessel-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2830 b- defN 23-May-14 16:23 pytessel-1.0.0.dist-info/METADATA
+-rwxr-xr-x  2.0 unx  1434409 b- defN 23-May-14 16:23 pytessel/pytessel.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx       31 b- defN 23-May-14 16:23 pytessel/__init__.py
+11 files, 1641422 bytes uncompressed, 478287 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -1,32 +1,32 @@
-Filename: pytessel-0.1.3.0.dist-info/
+Filename: pytessel.libs/
 Comment: 
 
-Filename: pytessel.libs/
+Filename: pytessel-1.0.0.dist-info/
 Comment: 
 
 Filename: pytessel/
 Comment: 
 
-Filename: pytessel-0.1.3.0.dist-info/RECORD
+Filename: pytessel.libs/libgomp-a34b3233.so.1.0.0
 Comment: 
 
-Filename: pytessel-0.1.3.0.dist-info/WHEEL
+Filename: pytessel-1.0.0.dist-info/RECORD
 Comment: 
 
-Filename: pytessel-0.1.3.0.dist-info/top_level.txt
+Filename: pytessel-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytessel-0.1.3.0.dist-info/LICENSE
+Filename: pytessel-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytessel-0.1.3.0.dist-info/METADATA
+Filename: pytessel-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: pytessel.libs/libgomp-a34b3233.so.1.0.0
+Filename: pytessel-1.0.0.dist-info/METADATA
 Comment: 
 
 Filename: pytessel/pytessel.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
 Filename: pytessel/__init__.py
 Comment:
```

## Comparing `pytessel-0.1.3.0.dist-info/RECORD` & `pytessel-1.0.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pytessel-0.1.3.0.dist-info/RECORD,,
-pytessel-0.1.3.0.dist-info/WHEEL,sha256=gREe7-l-MJWbGZG46A7WHnwwUSxA3XJYHQvGGLzmBNU,148
-pytessel-0.1.3.0.dist-info/top_level.txt,sha256=QDauMEeJ6MuBmtCTV4HZAr1XodXsUesXTlcImp5LE54,9
-pytessel-0.1.3.0.dist-info/LICENSE,sha256=4cCtcomD2KVzNeUs8QZPGv_R1FQXPYzr0-2LSnK0hwQ,35121
-pytessel-0.1.3.0.dist-info/METADATA,sha256=mEgiwB2ZsIUMsqwQ9yRk2eoOE2_2QD9J2pVqG54mzk8,1736
 pytessel.libs/libgomp-a34b3233.so.1.0.0,sha256=On6uznIxkRvi-7Gz58tMtcLg-E4MK7c3OUcrWh_uyME,168193
+pytessel-1.0.0.dist-info/RECORD,,
+pytessel-1.0.0.dist-info/WHEEL,sha256=gREe7-l-MJWbGZG46A7WHnwwUSxA3XJYHQvGGLzmBNU,148
+pytessel-1.0.0.dist-info/top_level.txt,sha256=QDauMEeJ6MuBmtCTV4HZAr1XodXsUesXTlcImp5LE54,9
+pytessel-1.0.0.dist-info/LICENSE,sha256=4cCtcomD2KVzNeUs8QZPGv_R1FQXPYzr0-2LSnK0hwQ,35121
+pytessel-1.0.0.dist-info/METADATA,sha256=aM7N2iB_Yh5LCmNKLOUIwROsueLKVXAH3EpB1iqgKeI,2830
 pytessel/pytessel.cpython-39-x86_64-linux-gnu.so,sha256=1CerlvZcQaIkELCm4zaZhrk9_xcJrRSDZoio6r3Sd24,1434409
 pytessel/__init__.py,sha256=7ym0uZ1xaGvtwUnWh3wGESmpVFZttcK9i_JXWhiHBLI,31
```

## Comparing `pytessel-0.1.3.0.dist-info/LICENSE` & `pytessel-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

