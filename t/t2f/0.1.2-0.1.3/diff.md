# Comparing `tmp/t2f-0.1.2.tar.gz` & `tmp/t2f-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2f-0.1.2.tar", max compression
+gzip compressed data, was "t2f-0.1.3.tar", max compression
```

## Comparing `t2f-0.1.2.tar` & `t2f-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.2/README.md
--rw-r--r--   0        0        0      347 2023-05-14 04:31:11.802653 t2f-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.2/t2f/__init__.py
--rw-r--r--   0        0        0    42601 2023-05-14 04:12:50.125106 t2f-0.1.2/t2f/patched_asm.py
--rw-r--r--   0        0        0    33456 2023-05-14 03:52:36.916873 t2f-0.1.2/t2f/stdlib.py
--rw-r--r--   0        0        0     9397 2023-05-14 04:30:38.782962 t2f-0.1.2/t2f/t2f.py
--rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.2/t2f/utils.py
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.3/README.md
+-rw-r--r--   0        0        0      347 2023-05-14 04:39:12.814994 t2f-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.3/t2f/__init__.py
+-rw-r--r--   0        0        0    42601 2023-05-14 04:12:50.125106 t2f-0.1.3/t2f/patched_asm.py
+-rw-r--r--   0        0        0    33456 2023-05-14 03:52:36.916873 t2f-0.1.3/t2f/stdlib.py
+-rw-r--r--   0        0        0     9409 2023-05-14 04:38:31.566693 t2f-0.1.3/t2f/t2f.py
+-rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.3/t2f/utils.py
+-rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.3/PKG-INFO
```

### Comparing `t2f-0.1.2/t2f/patched_asm.py` & `t2f-0.1.3/t2f/patched_asm.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.2/t2f/stdlib.py` & `t2f-0.1.3/t2f/stdlib.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.2/t2f/t2f.py` & `t2f-0.1.3/t2f/t2f.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
         if "<{" in row:
             lvl += 1
     prog_code = "\n".join(proc_rows)
 
     prog_code = f"// Translated from TVM-asm: {os.path.basename(args.filename)}\n\n" + prog_code
 
     if args.asm:
-        patched_asm_path = os.path.dirname(args.output) + "/PatchedAsm.fif"
+        patched_asm_path = os.path.join(os.path.dirname(args.output), "PatchedAsm.fif")
         with open(patched_asm_path, 'w') as file:
             file.write(patched_asm)
         prog_code = '"PatchedAsm.fif" include\n\n' + prog_code
 
     if args.tvc:
         prog_code += f'\n\n<b b{{0011}} s, swap ref, <b b> ref, b>\n' \
                      f'2 boc+>B "{os.path.splitext(args.output)[0]}.tvc" B>file\n'
```

### Comparing `t2f-0.1.2/t2f/utils.py` & `t2f-0.1.3/t2f/utils.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.2/PKG-INFO` & `t2f-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2f
-Version: 0.1.2
+Version: 0.1.3
 Summary: TVM Assembly to Fift Assembly Translator
 Author: Andrew Gutarev
 Author-email: gutarev01@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

