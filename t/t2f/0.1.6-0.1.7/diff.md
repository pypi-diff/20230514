# Comparing `tmp/t2f-0.1.6.tar.gz` & `tmp/t2f-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2f-0.1.6.tar", max compression
+gzip compressed data, was "t2f-0.1.7.tar", max compression
```

## Comparing `t2f-0.1.6.tar` & `t2f-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.6/README.md
--rw-r--r--   0        0        0      347 2023-05-14 07:34:21.335378 t2f-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.6/t2f/__init__.py
--rw-r--r--   0        0        0    43498 2023-05-14 07:08:34.228998 t2f-0.1.6/t2f/patched_asm.py
--rw-r--r--   0        0        0    33456 2023-05-14 06:38:45.515126 t2f-0.1.6/t2f/stdlib.py
--rw-r--r--   0        0        0    11887 2023-05-14 07:33:52.935655 t2f-0.1.6/t2f/t2f.py
--rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.6/t2f/utils.py
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.7/README.md
+-rw-r--r--   0        0        0      347 2023-05-14 20:34:41.459112 t2f-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.7/t2f/__init__.py
+-rw-r--r--   0        0        0    43498 2023-05-14 07:08:34.228998 t2f-0.1.7/t2f/patched_asm.py
+-rw-r--r--   0        0        0    33456 2023-05-14 06:38:45.515126 t2f-0.1.7/t2f/stdlib.py
+-rw-r--r--   0        0        0    11888 2023-05-14 20:34:19.176126 t2f-0.1.7/t2f/t2f.py
+-rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.7/t2f/utils.py
+-rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.7/PKG-INFO
```

### Comparing `t2f-0.1.6/t2f/patched_asm.py` & `t2f-0.1.7/t2f/patched_asm.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.6/t2f/stdlib.py` & `t2f-0.1.7/t2f/stdlib.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.6/t2f/t2f.py` & `t2f-0.1.7/t2f/t2f.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
     if args.asm:
         patched_asm_path = os.path.join(os.path.dirname(args.output), "PatchedAsm.fif")
         with open(patched_asm_path, 'w') as file:
             file.write(patched_asm)
         prog_code = '"PatchedAsm.fif" include\n\n' + prog_code
 
     if args.tvc:
-        prog_code += f'\n\n<b b{{0011}} s, swap ref, <b b> ref, b>\n' \
+        prog_code += f'\n\n<b b{{00110}} s, swap ref, <b b> ref, b>\n' \
                      f'2 boc+>B "{os.path.splitext(args.output)[0]}.tvc" B>file\n'
 
     with open(args.output, 'w') as file:
         file.write(prog_code)
 
 DEBUG = False
```

### Comparing `t2f-0.1.6/t2f/utils.py` & `t2f-0.1.7/t2f/utils.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.6/PKG-INFO` & `t2f-0.1.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2f
-Version: 0.1.6
+Version: 0.1.7
 Summary: TVM Assembly to Fift Assembly Translator
 Author: Andrew Gutarev
 Author-email: gutarev01@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

