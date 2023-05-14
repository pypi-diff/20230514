# Comparing `tmp/t2f-0.1.0.tar.gz` & `tmp/t2f-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2f-0.1.0.tar", max compression
+gzip compressed data, was "t2f-0.1.1.tar", max compression
```

## Comparing `t2f-0.1.0.tar` & `t2f-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-14 00:37:13.546583 t2f-0.1.0/README.md
--rw-r--r--   0        0        0      347 2023-05-14 00:48:54.213702 t2f-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.0/t2f/__init__.py
--rw-r--r--   0        0        0     6621 2023-05-14 00:43:10.317512 t2f-0.1.0/t2f/t2f.py
--rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.0/t2f/utils.py
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 t2f-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-14 00:37:13.546583 t2f-0.1.1/README.md
+-rw-r--r--   0        0        0      347 2023-05-14 01:22:23.660887 t2f-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.1/t2f/__init__.py
+-rw-r--r--   0        0        0     6616 2023-05-14 01:24:11.064232 t2f-0.1.1/t2f/t2f.py
+-rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.1/t2f/utils.py
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 t2f-0.1.1/PKG-INFO
```

### Comparing `t2f-0.1.0/t2f/t2f.py` & `t2f-0.1.1/t2f/t2f.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,27 +56,27 @@
     
     def process_code(code_lines):
         result_list = [Continuation()]
         
         for line in code_lines:
             if '<{' in line:
                 cont_type = re.findall(r'([\w\d]+):<{', line)[0]
+                if cont_type == "IFELSE":
+                    cont_type = "ELSE"
+                    result_list[-1].opcodes[-1].change_type("IF")
                 result_list.append(Continuation(cont_type))
             elif '}>' in line:
                 cont_0 = result_list.pop()
-                cont_main = result_list.pop()
-                if cont_0.type == "IFELSE":
-                    cont_0.change_type("IF")
-                    cont_1 = cont_main.opcodes.pop()
-                    cont_1.change_type("ELSE")
-                    cont_main.add_opcode(cont_0)
-                    cont_main.add_opcode(cont_1)
+                cont_1 = result_list.pop()
+                if cont_0.type == "CALLREF":
+                    cont_1.opcodes += cont_0.opcodes
+                    result_list.append(cont_1)
                 else:
-                    cont_main.add_opcode(cont_0)
-                result_list.append(cont_main)
+                    cont_1.add_opcode(cont_0)
+                    result_list.append(cont_1)
             else:
                 ll = line.split(" ")
                 opcode_name = ll[-1]
                 params = None
                 if len(ll) > 1:
                     params = ll[0:-1]
                 if opcode_name == "IFELSE":
@@ -101,28 +101,28 @@
     def declar_proc(r, proc):
         return f"{r}DECLPROC {proc.name}\n"
     
     def add_proc_body(r, proc):
         return f"{r}{proc.name} PROCINLINE:<{'{'}{proc.body}\n{'}'}>\n\n"
     
     def build(self):
-        r = '"PatchedAsm.fif" include\n\n// Code translated from TVM-asm\n\n<{\n\n'
+        r = "<{\n\n"
         for proc in self.procs:
             r = Program.declar_proc(r, proc)
         r += "\n"
         for proc in self.procs:
             r = Program.add_proc_body(r, proc)
         r += "IFNOT: recv_internal INLINECALL\n\n"
         return r + self.root + "}>"
 
     def return_cell(self):
-        return self.build() + "c\n"
+        return self.build() + "c"
     
     def return_slice(self):
-        return self.build() + "s\n"
+        return self.build() + "s"
 
 
 def sort_procs(procedures):
     procedures = {proc.name:proc for proc in procedures}
 
     proc_names = procedures.keys()
     proc_inlines = {procedures[proc].name:re.findall(r'([\w\d]+) INLINECALL', procedures[proc].body) for proc in procedures}
@@ -144,39 +144,42 @@
     with open(in_path) as file:
         code: str = file.read()
     
     # REPLACES BLOCK
     code = code.replace(".internal-alias :main_internal, 0\n.internal :main_internal", "recv_internal")
     code = re.sub(r'.macro (\w+)', r'\1', code)
 
+    code = code.replace("\s$", "")
+    code = code.replace("^\s", "")
     code = code.replace(" {", ":<{")
+    code = code.replace(",", "")
     code = code.replace("}", "}>")
     code = code.replace("PUSHCONT:<{", "CONT:<{")
     code = code.replace("IFREF", "IF")
     code = code.replace("IFJMPREF", "IFJMP")
     code = code.replace("IFNOTJMPREF", "IFNOTJMP")
 
     code = re.sub(r'S(\d+)', r's\1', code)
+    code = re.sub(r'C(\d+)', r'c\1', code)
 
     code = re.sub(r'CALL \$(.*?)\$', r'INLINECALL \1', code)
-    
-    code = re.sub(r'STSLICECONST x(\w)', r'STSLICECONST x{\1}', code)
+
+    code = re.sub(r'(STSLICECONST|PUSHSLICE) x([\w_]+)', r'\1 x{\2}', code)
     code = re.sub(r';.+', r'', code)
 
     code = re.sub(r'( *)(\w+ )([\w \-{}]+)*', r'\1\3 \2', code)
-    code = re.sub(r'CALLREF:<{(?:\n|\r\n)?\t(.*?)\n?}>', r'\1', code, flags=re.DOTALL)
 
     code = re.sub(r'(\d+ MODPOW2)', r'\1#', code)
 
     code = re.sub(r'\t+', r'', code)
     code = re.sub(r'[ ]+', r' ', code)
     code = re.sub(r'[ ]*(\n+)[ ]*', r'\1', code)
 
     # BUILD
-    procs = [Procedure(proc_code) for proc_code in code.split("\n\n")[1:-1]]
+    procs = [Procedure(proc_code) for proc_code in code.split("\n\n")[1:]]
 
     prog = Program(sort_procs(procs))
     prog_code = prog.return_cell()
 
 
     lvl = 0
     proc_rows = prog_code.split("\n")
```

### Comparing `t2f-0.1.0/t2f/utils.py` & `t2f-0.1.1/t2f/utils.py`

 * *Files identical despite different names*

