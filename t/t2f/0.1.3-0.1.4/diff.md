# Comparing `tmp/t2f-0.1.3.tar.gz` & `tmp/t2f-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2f-0.1.3.tar", max compression
+gzip compressed data, was "t2f-0.1.4.tar", max compression
```

## Comparing `t2f-0.1.3.tar` & `t2f-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.3/README.md
--rw-r--r--   0        0        0      347 2023-05-14 04:39:12.814994 t2f-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.3/t2f/__init__.py
--rw-r--r--   0        0        0    42601 2023-05-14 04:12:50.125106 t2f-0.1.3/t2f/patched_asm.py
--rw-r--r--   0        0        0    33456 2023-05-14 03:52:36.916873 t2f-0.1.3/t2f/stdlib.py
--rw-r--r--   0        0        0     9409 2023-05-14 04:38:31.566693 t2f-0.1.3/t2f/t2f.py
--rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.3/t2f/utils.py
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-05-14 02:07:54.621007 t2f-0.1.4/README.md
+-rw-r--r--   0        0        0      347 2023-05-14 04:43:49.078125 t2f-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 00:37:13.545834 t2f-0.1.4/t2f/__init__.py
+-rw-r--r--   0        0        0    43498 2023-05-14 06:04:24.092256 t2f-0.1.4/t2f/patched_asm.py
+-rw-r--r--   0        0        0    33456 2023-05-14 06:38:45.515126 t2f-0.1.4/t2f/stdlib.py
+-rw-r--r--   0        0        0    11839 2023-05-14 06:38:02.839076 t2f-0.1.4/t2f/t2f.py
+-rw-r--r--   0        0        0      650 2023-05-13 23:17:17.630755 t2f-0.1.4/t2f/utils.py
+-rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 t2f-0.1.4/PKG-INFO
```

### Comparing `t2f-0.1.3/t2f/patched_asm.py` & `t2f-0.1.4/t2f/patched_asm.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,20 @@
 { <b 0xef 8 u, swap 12 i, b> } : si()
 // x mi ma -- ?
 { rot tuck >= -rot <= and } : @range
 { rot tuck < -rot > or } : @-range
 { @-range abort"Out of range" } : @rangechk
 { dup 0 < over 255 > or abort"Invalid stack register number" si() } : s()
 { si() constant } : @Sreg
+-8 @Sreg s(-8)
+-7 @Sreg s(-7)
+-6 @Sreg s(-6)
+-5 @Sreg s(-5)
+-4 @Sreg s(-4)
+-3 @Sreg s(-3)
 -2 @Sreg s(-2)
 -1 @Sreg s(-1)
 0 @Sreg s0
 1 @Sreg s1
 2 @Sreg s2
 3 @Sreg s3
 4 @Sreg s4
@@ -57,14 +63,49 @@
 9 @Sreg s9
 10 @Sreg s10
 11 @Sreg s11
 12 @Sreg s12
 13 @Sreg s13
 14 @Sreg s14
 15 @Sreg s15
+16 @Sreg s16
+17 @Sreg s17
+18 @Sreg s18
+19 @Sreg s19
+20 @Sreg s20
+21 @Sreg s21
+22 @Sreg s22
+23 @Sreg s23
+24 @Sreg s24
+25 @Sreg s25
+26 @Sreg s26
+27 @Sreg s27
+28 @Sreg s28
+29 @Sreg s29
+30 @Sreg s30
+31 @Sreg s31
+32 @Sreg s32
+33 @Sreg s33
+34 @Sreg s34
+35 @Sreg s35
+36 @Sreg s36
+37 @Sreg s37
+38 @Sreg s38
+39 @Sreg s39
+40 @Sreg s40
+41 @Sreg s41
+42 @Sreg s42
+43 @Sreg s43
+44 @Sreg s44
+45 @Sreg s45
+46 @Sreg s46
+47 @Sreg s47
+48 @Sreg s48
+49 @Sreg s49
+50 @Sreg s50
 { dup 0 < over 7 > or abort"Invalid control register number" <b 0xcc 8 u, swap 4 u, b> } : c()
 { c() constant } : @Creg
 0 @Creg c0
 1 @Creg c1
 2 @Creg c2
 3 @Creg c3
 4 @Creg c4
@@ -1207,14 +1248,27 @@
 x{FB00} @Defop SENDRAWMSG
 x{FB02} @Defop RAWRESERVE
 x{FB03} @Defop RAWRESERVEX
 x{FB04} @Defop SETCODE
 x{FB06} @Defop SETLIBCODE
 x{FB07} @Defop CHANGELIB
 
+// EVERSCALE OPCODES
+
+x{F82A} @Defop MYCODE
+x{F82B} @Defop INITCODEHASH
+x{6F90} @Defop ZEROSWAPIF 
+x{6F91} @Defop ZEROSWAPIFNOT
+x{6F92} @Defop ZEROROTRIF
+x{6F93} @Defop ZEROROTRIFNOT
+x{6F94} @Defop ZEROSWAPIF2
+x{6F95} @Defop ZEROSWAPIFNOT2
+x{6F96} @Defop ZEROROTRIF2
+x{6F97} @Defop ZEROROTRIFNOT2
+
 //
 // debug primitives
 
 { dup 0 239 @-range abort"debug selector out of range"
   <b x{FE} s, swap 8 u, @addopb
 } : DEBUG
 { dup $len 1- <b x{FEF} s, swap 4 u, swap $, @addopb
```

### Comparing `t2f-0.1.3/t2f/stdlib.py` & `t2f-0.1.4/t2f/stdlib.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.3/t2f/t2f.py` & `t2f-0.1.4/t2f/t2f.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 
 class Opcode(object):
 
     def __init__(self, opcode, params=None):
         self.opcode = opcode
         self.params = params
+
+        if opcode == "XCHG" and len(params) == 1:
+            self.opcode = "XCHG0"
     
     def build(self):
         if self.params is None:
             return self.opcode
         else:
             params_str = " ".join(self.params)
             return f"{params_str} {self.opcode}"
@@ -53,44 +56,67 @@
 
     def __init__(self, code):
         code_lines = code.split('\n')
         self.name = code_lines[0]
         self.body = Procedure.process_code(code_lines[1:])
     
     def process_code(code_lines):
+        global DEBUG
         result_list = [Continuation()]
         
         for line in code_lines:
+            if DEBUG: print(line)
             if line == "":
                 continue
             if '<{' in line:
                 cont_type = re.findall(r'([\w\d]+):<{', line)[0]
-                if cont_type == "IFELSE":
-                    cont_type = "ELSE"
-                    result_list[-1].opcodes[-1].change_type("IF")
+                # if cont_type == "IFELSE":
+                #     result_list[-1].opcodes[-1].change_type("IF")
+                
                 result_list.append(Continuation(cont_type))
             elif '}>' in line:
                 cont_0 = result_list.pop()
                 cont_1 = result_list.pop()
                 if cont_0.type == "CALLREF":
                     cont_1.opcodes += cont_0.opcodes
-                    result_list.append(cont_1)
+                elif cont_0.type == "PUSHSLICE":
+                    new_opcode = Opcode("PUSHSLICE", ["x{}"])
+                    if len(cont_0.opcodes):
+                        slice_bits = cont_0.opcodes[0].params
+                        new_opcode = Opcode("PUSHSLICE", slice_bits)
+                    cont_1.opcodes.append(new_opcode)
+                elif cont_0.type == "PUSHREF":
+                    new_opcode = Opcode("PUSHREF", ["<b b>"])
+                    if len(cont_0.opcodes):
+                        ref_bits = cont_0.opcodes[0].params[0]
+                        new_opcode = Opcode("PUSHREF", [f"<b {ref_bits} s, b>"])
+                    cont_1.opcodes.append(new_opcode)
+                elif cont_0.type == "IFELSE":
+                    cont_0.change_type("IF")
+                    cont_else = cont_1.opcodes.pop()
+                    cont_else.change_type("ELSE")
+                    cont_1.opcodes.append(cont_0)
+                    cont_1.opcodes.append(cont_else)
+                elif cont_0.type == "SECOND_":
+                    cont_1.opcodes[-1].change_type("IF")
+                    cont_0.change_type("ELSE")
+                    cont_1.opcodes.append(cont_0)
                 else:
                     cont_1.add_opcode(cont_0)
-                    result_list.append(cont_1)
+                result_list.append(cont_1)
             else:
                 ll = line.split(" ")
                 opcode_name = ll[-1]
                 params = None
                 if len(ll) > 1:
                     params = ll[0:-1]
                 if opcode_name == "IFELSE":
                      result_list[-1].opcodes[-1].change_type("ELSE")
                      result_list[-1].opcodes[-2].change_type("IF")
-                elif opcode_name in ["IF", "IFNOT", "REPEAT"]:
+                elif opcode_name in ["IF", "IFNOT", "REPEAT", "IFJMP", "IFNOTJMP"]:
                      result_list[-1].opcodes[-1].change_type(opcode_name)
                 elif opcode_name == "WHILE":
                      result_list[-1].opcodes[-1].change_type("DO")
                      result_list[-1].opcodes[-2].change_type("WHILE")
                 else:
                     cont_0 = result_list.pop()
                     cont_0.add_opcode(Opcode(opcode_name, params))
@@ -119,27 +145,30 @@
         for proc_name in self.procs.keys():
             r = Program.declar_proc(r, proc_name)
         r += "\n"
         for proc in self.procs:
             r = Program.add_proc_body(r, self.procs[proc])
         internal = "recv_internal" in self.procs.keys()
         external = "recv_external" in self.procs.keys()
-        if internal and external:
-            r += "0 EQINT IFJMP:<{\n" \
-                     "recv_internal INLINECALL\n" \
-                 "}>\n\n"
-            r += "-1 EQINT IFJMP:<{\n" \
-                     "recv_external INLINECALL\n" \
-                 "}>\n\n"
-        elif internal:
+        ticktock = "run_ticktock" in self.procs.keys()
+        if internal and not external and not ticktock:
             r += "IFNOT: recv_internal INLINECALL\n\n"
-        elif external:
-            r += "-1 EQINT IFJMP:<{\n" \
-                     "recv_external INLINECALL\n" \
-                 "}>\n\n"
+        else:
+            if ticktock:
+                r += "DUP -2 EQINT IFJMP:<{\n" \
+                        "DROP run_ticktock INLINECALL\n" \
+                    "}>\n\n"
+            if internal:
+                r += "DUP 0 EQINT IFJMP:<{\n" \
+                        "DROP recv_internal INLINECALL\n" \
+                    "}>\n\n"
+            if external:
+                r += "-1 EQINT IFJMP:<{\n" \
+                        "recv_external INLINECALL\n" \
+                    "}>\n\n"
                   
         return r + self.root + "}>"
 
     def return_cell(self):
         return self.build() + "c"
     
     def return_slice(self):
@@ -160,14 +189,16 @@
     # remove unused funcs
     new_graph = defaultdict()
     funcs = []
     if "recv_internal" in graph:
         funcs.append("recv_internal")
     if "recv_external" in graph:
         funcs.append("recv_external")
+    if "run_ticktock" in graph:
+        funcs.append("run_ticktock")
     f_len = -1
     while (f_len != len(funcs)):
         f_len = len(funcs)
         new_funcs = funcs
         for f in funcs:
             new_graph[f] = graph[f]
             new_funcs = list(set(new_funcs + graph[f]))
@@ -194,43 +225,60 @@
     code = "\n\n".join(code_l)
 
     code = re.sub(r'\.loc.+\n', r'', code)
     code = re.sub(r'\.loc.+$', r'', code)
 
     code = code.replace(".internal-alias :main_internal, 0\n.internal :main_internal", "recv_internal")
     code = code.replace(".internal-alias :main_external, -1\n.internal :main_external", "recv_external")
+    code = code.replace(".internal-alias :onTickTock, -2\n.internal :onTickTock", "run_ticktock")
     code = re.sub(r'.macro (\w+)', r'\1', code)
 
-
+    if len(re.findall(r'onCodeUpgrade', code)):
+        print("ERROR: onCodeUpgrade currently is not supported")
+        exit(1)
+        
     code = code.replace("\s$", "")
     code = code.replace("^\s", "")
     code = code.replace(" {", ":<{")
     code = code.replace(",", "")
+    code = code.replace(".", "")
     code = code.replace("}", "}>")
     code = code.replace("PUSHCONT:<{", "CONT:<{")
+    
     code = code.replace("IFREF", "IF")
+    code = code.replace("ELSEREF", "ELSE")
     code = code.replace("IFJMPREF", "IFJMP")
     code = code.replace("IFNOTJMPREF", "IFNOTJMP")
+    code = code.replace("PUSHREFSLICE", "PUSHSLICE")
 
     code = re.sub(r'S(\d+)', r's\1', code)
-    code = re.sub(r'C(\d+)', r'c\1', code)
+    code = re.sub(r'S(-\d+)', r's(\1)', code)
+    code = re.sub(r'C([-]?\d+)', r'c\1', code)
 
     code = re.sub(r'CALL \$(.*?)\$', r'INLINECALL \1', code)
 
-    code = re.sub(r'(STSLICECONST|PUSHSLICE) x([\w_]+)', r'\1 x{\2}', code)
+    code = re.sub(r'(STSLICECONST|PUSHSLICE|blob) x([\w_]*)', r'\1 x{\2}', code)
+    code = re.sub(r'STSLICECONST 0', r'STZERO', code)
+    code = re.sub(r'STSLICECONST 1', r'STONE', code)
+
     code = re.sub(r';.+', r'', code)
 
-    code = re.sub(r'( *)(\w+ )([\w \-{}]+)*', r'\1\3 \2', code)
+    code = re.sub(r'( *)(\w+ )([\w \-{}()]+)*', r'\1\3 \2', code)
 
     code = re.sub(r'(\d+ MODPOW2)', r'\1#', code)
+    code = re.sub(r'(\d+ RSHIFT)', r'\1#', code)
+    code = re.sub(r'(\d+ LSHIFT)', r'\1#', code)
 
     code = re.sub(r'\t+', r'', code)
     code = re.sub(r'[ ]+', r' ', code)
     code = re.sub(r'[ ]*(\n+)[ ]*', r'\1', code)
 
+    code = code.replace("IFELSE\n{", "IFELSE_:<{")
+    code = code.replace("\n{", "\nSECOND_:<{")
+
     # BUILD
     procs = {proc.name:proc for proc in [Procedure(proc_code) for proc_code in code.split("\n\n")]}
 
     prog = Program(sort_procs(procs))
     prog_code = prog.return_cell()
 
 
@@ -257,30 +305,32 @@
     if args.tvc:
         prog_code += f'\n\n<b b{{0011}} s, swap ref, <b b> ref, b>\n' \
                      f'2 boc+>B "{os.path.splitext(args.output)[0]}.tvc" B>file\n'
 
     with open(args.output, 'w') as file:
         file.write(prog_code)
 
+DEBUG = False
 
 def main():
-
+    global DEBUG
     parser = argparse.ArgumentParser(
         prog='t2f',
         description='TVM Assembly to Fift Assembly Translator',
     )
 
     parser.add_argument('filename')
     parser.add_argument('-o', '--output', dest='output', default=None, help='output file name')
     parser.add_argument('-t', '--tvc', dest='tvc', default=False, help='add tvc generation', action='store_true')
     parser.add_argument('-a', '--asm-include', dest='asm', default=False, help='add PatchedAsm.fif', action='store_true')
+    parser.add_argument('--debug', dest='debug', default=False, action='store_true')
 
     args = parser.parse_args()
 
     default_output = f'{os.path.splitext(args.filename)[0]}.fif'
     args.output = default_output if args.output is None else args.output
-    
+    DEBUG = args.debug
     translate(args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `t2f-0.1.3/t2f/utils.py` & `t2f-0.1.4/t2f/utils.py`

 * *Files identical despite different names*

### Comparing `t2f-0.1.3/PKG-INFO` & `t2f-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2f
-Version: 0.1.3
+Version: 0.1.4
 Summary: TVM Assembly to Fift Assembly Translator
 Author: Andrew Gutarev
 Author-email: gutarev01@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

