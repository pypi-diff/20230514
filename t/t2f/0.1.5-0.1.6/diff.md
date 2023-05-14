# Comparing `tmp/t2f-0.1.5.tar.gz` & `tmp/t2f-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2f-0.1.5.tar", max compression
+gzip compressed data, was "t2f-0.1.6.tar", max compression
```

## Comparing `t2f-0.1.5.tar` & `t2f-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.5/README.md
--rw-r--r--   0        0        0      347 2023-05-14 07:13:25.871669 t2f-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.5/t2f/__init__.py
--rw-r--r--   0        0        0    43498 2023-05-14 07:08:34.228998 t2f-0.1.5/t2f/patched_asm.py
--rw-r--r--   0        0        0    33456 2023-05-14 06:38:45.515126 t2f-0.1.5/t2f/stdlib.py
--rw-r--r--   0        0        0    11839 2023-05-14 06:38:02.839076 t2f-0.1.5/t2f/t2f.py
--rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.5/t2f/utils.py
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.6/README.md
+-rw-r--r--   0        0        0      347 2023-05-14 07:34:21.335378 t2f-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.6/t2f/__init__.py
+-rw-r--r--   0        0        0    43498 2023-05-14 07:08:34.228998 t2f-0.1.6/t2f/patched_asm.py
+-rw-r--r--   0        0        0    33456 2023-05-14 06:38:45.515126 t2f-0.1.6/t2f/stdlib.py
+-rw-r--r--   0        0        0    11887 2023-05-14 07:33:52.935655 t2f-0.1.6/t2f/t2f.py
+-rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.6/t2f/utils.py
+-rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.6/PKG-INFO
```

### Comparing `t2f-0.1.5/t2f/patched_asm.py` & `t2f-0.1.6/t2f/patched_asm.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.5/t2f/stdlib.py` & `t2f-0.1.6/t2f/stdlib.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.5/t2f/t2f.py` & `t2f-0.1.6/t2f/t2f.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,17 @@
         
         for line in code_lines:
             if DEBUG: print(line)
             if line == "":
                 continue
             if '<{' in line:
                 cont_type = re.findall(r'([\w\d]+):<{', line)[0]
-                # if cont_type == "IFELSE":
-                #     result_list[-1].opcodes[-1].change_type("IF")
+                if cont_type == "IFELSE":
+                    cont_type = "ELSE"
+                    result_list[-1].opcodes[-1].change_type("IF")
                 
                 result_list.append(Continuation(cont_type))
             elif '}>' in line:
                 cont_0 = result_list.pop()
                 cont_1 = result_list.pop()
                 if cont_0.type == "CALLREF":
                     cont_1.opcodes += cont_0.opcodes
@@ -86,20 +87,20 @@
                     cont_1.opcodes.append(new_opcode)
                 elif cont_0.type == "PUSHREF":
                     new_opcode = Opcode("PUSHREF", ["<b b>"])
                     if len(cont_0.opcodes):
                         ref_bits = cont_0.opcodes[0].params[0]
                         new_opcode = Opcode("PUSHREF", [f"<b {ref_bits} s, b>"])
                     cont_1.opcodes.append(new_opcode)
-                elif cont_0.type == "IFELSE":
-                    cont_0.change_type("IF")
-                    cont_else = cont_1.opcodes.pop()
-                    cont_else.change_type("ELSE")
-                    cont_1.opcodes.append(cont_0)
-                    cont_1.opcodes.append(cont_else)
+                # elif cont_0.type == "IFELSE":
+                #     cont_0.change_type("IF")
+                #     cont_else = cont_1.opcodes.pop()
+                #     cont_else.change_type("ELSE")
+                #     cont_1.opcodes.append(cont_0)
+                #     cont_1.opcodes.append(cont_else)
                 elif cont_0.type == "SECOND_":
                     cont_1.opcodes[-1].change_type("IF")
                     cont_0.change_type("ELSE")
                     cont_1.opcodes.append(cont_0)
                 else:
                     cont_1.add_opcode(cont_0)
                 result_list.append(cont_1)
```

### Comparing `t2f-0.1.5/t2f/utils.py` & `t2f-0.1.6/t2f/utils.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.5/PKG-INFO` & `t2f-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2f
-Version: 0.1.5
+Version: 0.1.6
 Summary: TVM Assembly to Fift Assembly Translator
 Author: Andrew Gutarev
 Author-email: gutarev01@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

