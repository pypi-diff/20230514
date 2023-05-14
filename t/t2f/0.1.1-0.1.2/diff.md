# Comparing `tmp/t2f-0.1.1.tar.gz` & `tmp/t2f-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2f-0.1.1.tar", max compression
+gzip compressed data, was "t2f-0.1.2.tar", max compression
```

## Comparing `t2f-0.1.1.tar` & `t2f-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-14 00:37:13.546583 t2f-0.1.1/README.md
--rw-r--r--   0        0        0      347 2023-05-14 01:22:23.660887 t2f-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.1/t2f/__init__.py
--rw-r--r--   0        0        0     6616 2023-05-14 01:24:11.064232 t2f-0.1.1/t2f/t2f.py
--rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.1/t2f/utils.py
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 t2f-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.2/README.md
+-rw-r--r--   0        0        0      347 2023-05-14 04:31:11.802653 t2f-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.2/t2f/__init__.py
+-rw-r--r--   0        0        0    42601 2023-05-14 04:12:50.125106 t2f-0.1.2/t2f/patched_asm.py
+-rw-r--r--   0        0        0    33456 2023-05-14 03:52:36.916873 t2f-0.1.2/t2f/stdlib.py
+-rw-r--r--   0        0        0     9397 2023-05-14 04:30:38.782962 t2f-0.1.2/t2f/t2f.py
+-rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.2/t2f/utils.py
+-rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.2/PKG-INFO
```

### Comparing `t2f-0.1.1/t2f/t2f.py` & `t2f-0.1.2/t2f/t2f.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from collections import defaultdict
 from pprint import pprint
 import argparse
 from t2f.utils import topo_sort
+from t2f.stdlib import stdlib
+from t2f.patched_asm import patched_asm
 import os
 import re
 
 
 class Opcode(object):
 
     def __init__(self, opcode, params=None):
@@ -54,14 +56,16 @@
         self.name = code_lines[0]
         self.body = Procedure.process_code(code_lines[1:])
     
     def process_code(code_lines):
         result_list = [Continuation()]
         
         for line in code_lines:
+            if line == "":
+                continue
             if '<{' in line:
                 cont_type = re.findall(r'([\w\d]+):<{', line)[0]
                 if cont_type == "IFELSE":
                     cont_type = "ELSE"
                     result_list[-1].opcodes[-1].change_type("IF")
                 result_list.append(Continuation(cont_type))
             elif '}>' in line:
@@ -78,80 +82,129 @@
                 opcode_name = ll[-1]
                 params = None
                 if len(ll) > 1:
                     params = ll[0:-1]
                 if opcode_name == "IFELSE":
                      result_list[-1].opcodes[-1].change_type("ELSE")
                      result_list[-1].opcodes[-2].change_type("IF")
+                elif opcode_name in ["IF", "IFNOT", "REPEAT"]:
+                     result_list[-1].opcodes[-1].change_type(opcode_name)
+                elif opcode_name == "WHILE":
+                     result_list[-1].opcodes[-1].change_type("DO")
+                     result_list[-1].opcodes[-2].change_type("WHILE")
                 else:
                     cont_0 = result_list.pop()
                     cont_0.add_opcode(Opcode(opcode_name, params))
                     result_list.append(cont_0)
         cont_0 = result_list[0]
         proc_code = cont_0.build_body()
         proc_code = re.sub(r'}>\s*ELSE:<{', r'}>ELSE<{', proc_code)
+        proc_code = re.sub(r'}>\s*DO:<{', r'}>DO<{', proc_code)
         return proc_code
 
 
 class Program(object):   
 
     def __init__(self, procs, root=''):
         self.procs = procs
         self.root = root
     
-    def declar_proc(r, proc):
-        return f"{r}DECLPROC {proc.name}\n"
+    def declar_proc(r, proc_name):
+        return f"{r}DECLPROC {proc_name}\n"
     
     def add_proc_body(r, proc):
         return f"{r}{proc.name} PROCINLINE:<{'{'}{proc.body}\n{'}'}>\n\n"
     
     def build(self):
         r = "<{\n\n"
-        for proc in self.procs:
-            r = Program.declar_proc(r, proc)
+        for proc_name in self.procs.keys():
+            r = Program.declar_proc(r, proc_name)
         r += "\n"
         for proc in self.procs:
-            r = Program.add_proc_body(r, proc)
-        r += "IFNOT: recv_internal INLINECALL\n\n"
+            r = Program.add_proc_body(r, self.procs[proc])
+        internal = "recv_internal" in self.procs.keys()
+        external = "recv_external" in self.procs.keys()
+        if internal and external:
+            r += "0 EQINT IFJMP:<{\n" \
+                     "recv_internal INLINECALL\n" \
+                 "}>\n\n"
+            r += "-1 EQINT IFJMP:<{\n" \
+                     "recv_external INLINECALL\n" \
+                 "}>\n\n"
+        elif internal:
+            r += "IFNOT: recv_internal INLINECALL\n\n"
+        elif external:
+            r += "-1 EQINT IFJMP:<{\n" \
+                     "recv_external INLINECALL\n" \
+                 "}>\n\n"
+                  
         return r + self.root + "}>"
 
     def return_cell(self):
         return self.build() + "c"
     
     def return_slice(self):
         return self.build() + "s"
 
 
 def sort_procs(procedures):
-    procedures = {proc.name:proc for proc in procedures}
-
     proc_names = procedures.keys()
     proc_inlines = {procedures[proc].name:re.findall(r'([\w\d]+) INLINECALL', procedures[proc].body) for proc in procedures}
 
     graph = defaultdict(list)
     for func in proc_names:
         graph[func] = []
         if func in proc_inlines:
             for called_func in proc_inlines[func]:
                 graph[func].append(called_func)
-
-    sorted_functions = topo_sort(graph)
+    
+    # remove unused funcs
+    new_graph = defaultdict()
+    funcs = []
+    if "recv_internal" in graph:
+        funcs.append("recv_internal")
+    if "recv_external" in graph:
+        funcs.append("recv_external")
+    f_len = -1
+    while (f_len != len(funcs)):
+        f_len = len(funcs)
+        new_funcs = funcs
+        for f in funcs:
+            new_graph[f] = graph[f]
+            new_funcs = list(set(new_funcs + graph[f]))
+        funcs = new_funcs
+            
+    sorted_functions = topo_sort(new_graph)
+            
     sorted_functions.reverse()
     
-    return [procedures[proc] for proc in sorted_functions]
+    return {proc:procedures[proc] for proc in sorted_functions}
 
 
-def translate(in_path, out_path):
-    with open(in_path) as file:
+def translate(args):
+    with open(args.filename) as file:
         code: str = file.read()
     
+    code = stdlib + code
+    
     # REPLACES BLOCK
+    code = re.sub(r'\n\n[\n]*', r'\n\n', code)
+
+    code_l = list(filter(lambda block: (".macro" in block) or (".internal-alias" in block), code.split('\n\n')))
+
+    code = "\n\n".join(code_l)
+
+    code = re.sub(r'\.loc.+\n', r'', code)
+    code = re.sub(r'\.loc.+$', r'', code)
+
     code = code.replace(".internal-alias :main_internal, 0\n.internal :main_internal", "recv_internal")
+    code = code.replace(".internal-alias :main_external, -1\n.internal :main_external", "recv_external")
     code = re.sub(r'.macro (\w+)', r'\1', code)
 
+
     code = code.replace("\s$", "")
     code = code.replace("^\s", "")
     code = code.replace(" {", ":<{")
     code = code.replace(",", "")
     code = code.replace("}", "}>")
     code = code.replace("PUSHCONT:<{", "CONT:<{")
     code = code.replace("IFREF", "IF")
@@ -171,15 +224,15 @@
     code = re.sub(r'(\d+ MODPOW2)', r'\1#', code)
 
     code = re.sub(r'\t+', r'', code)
     code = re.sub(r'[ ]+', r' ', code)
     code = re.sub(r'[ ]*(\n+)[ ]*', r'\1', code)
 
     # BUILD
-    procs = [Procedure(proc_code) for proc_code in code.split("\n\n")[1:]]
+    procs = {proc.name:proc for proc in [Procedure(proc_code) for proc_code in code.split("\n\n")]}
 
     prog = Program(sort_procs(procs))
     prog_code = prog.return_cell()
 
 
     lvl = 0
     proc_rows = prog_code.split("\n")
@@ -189,30 +242,45 @@
         if lvl > 0:
             new_row = "    " * lvl + row
             proc_rows[idx] = new_row
         if "<{" in row:
             lvl += 1
     prog_code = "\n".join(proc_rows)
 
-    with open(out_path, 'w') as file:
+    prog_code = f"// Translated from TVM-asm: {os.path.basename(args.filename)}\n\n" + prog_code
+
+    if args.asm:
+        patched_asm_path = os.path.dirname(args.output) + "/PatchedAsm.fif"
+        with open(patched_asm_path, 'w') as file:
+            file.write(patched_asm)
+        prog_code = '"PatchedAsm.fif" include\n\n' + prog_code
+
+    if args.tvc:
+        prog_code += f'\n\n<b b{{0011}} s, swap ref, <b b> ref, b>\n' \
+                     f'2 boc+>B "{os.path.splitext(args.output)[0]}.tvc" B>file\n'
+
+    with open(args.output, 'w') as file:
         file.write(prog_code)
 
 
 def main():
 
     parser = argparse.ArgumentParser(
         prog='t2f',
         description='TVM Assembly to Fift Assembly Translator',
     )
 
     parser.add_argument('filename')
     parser.add_argument('-o', '--output', dest='output', default=None, help='output file name')
+    parser.add_argument('-t', '--tvc', dest='tvc', default=False, help='add tvc generation', action='store_true')
+    parser.add_argument('-a', '--asm-include', dest='asm', default=False, help='add PatchedAsm.fif', action='store_true')
+
     args = parser.parse_args()
 
     default_output = f'{os.path.splitext(args.filename)[0]}.fif'
     args.output = default_output if args.output is None else args.output
     
-    translate(args.filename, args.output)
+    translate(args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `t2f-0.1.1/t2f/utils.py` & `t2f-0.1.2/t2f/utils.py`

 * *Files identical despite different names*

