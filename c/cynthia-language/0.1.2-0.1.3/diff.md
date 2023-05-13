# Comparing `tmp/cynthia_language-0.1.2.tar.gz` & `tmp/cynthia_language-0.1.3.tar.gz`

## Comparing `cynthia_language-0.1.2.tar` & `cynthia_language-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/setup.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/__init__.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/__main__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/__init__.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/nodes.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/parser.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/shell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/interpreter/__init__.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/interpreter/exceptions.py
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/interpreter/interpreter.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/lexer/__init__.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/lexer/lexer.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/lexer/lexer_utils.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/lexer/logics.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/lexer/supported_tokens.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/cynthia/tools/lexer/tokens.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/examples/base_account.cynthia
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/examples/e_transaction_0,3%.cynthia
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/examples/e_transaction_100k.cynthia
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/examples/e_transaction_200k.cynthia
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/LICENSE
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 cynthia_language-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/setup.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/__init__.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/__main__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/__init__.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/nodes.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/parser.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/shell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/interpreter/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/interpreter/exceptions.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/interpreter/interpreter.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/lexer/__init__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/lexer/lexer.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/lexer/lexer_utils.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/lexer/logics.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/lexer/supported_tokens.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/cynthia/tools/lexer/tokens.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/examples/base_account.cynthia
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/examples/e_transaction_0,3%.cynthia
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/examples/e_transaction_100k.cynthia
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/examples/e_transaction_200k.cynthia
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cynthia_language-0.1.3/PKG-INFO
```

### Comparing `cynthia_language-0.1.2/setup.cfg` & `cynthia_language-0.1.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     __pycache__,
     __init__.py,
     README.md,
     LICENSE
 
 per-file-ignores =
     cynthia/tools/parser.py: WPS214
+    cynthia/tools/interpreter/interpreter.py: WPS214
 
 [isort]
 combine_as_imports = true
 include_trailing_comma = true
 known_first_party = tools
 line_length = 110
 multi_line_output = 5
```

### Comparing `cynthia_language-0.1.2/cynthia/__main__.py` & `cynthia_language-0.1.3/cynthia/__main__.py`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.2/cynthia/tools/nodes.py` & `cynthia_language-0.1.3/cynthia/tools/nodes.py`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.2/cynthia/tools/parser.py` & `cynthia_language-0.1.3/cynthia/tools/parser.py`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.2/cynthia/tools/interpreter/interpreter.py` & `cynthia_language-0.1.3/cynthia/tools/interpreter/interpreter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Cynthia language interpreter definition."""
 
 import re
+from decimal import Decimal
 from io import TextIOBase
 
 from cynthia.tools.interpreter.exceptions import (
-    FunctionDoesNotExistError, VariableDoesNotExitError, VisitorDoesNotExistError,
+    FunctionDoesNotExistError, InvalidGlobalVariableError, VariableDoesNotExitError, VisitorDoesNotExistError,
 )
 from cynthia.tools.lexer.supported_tokens import TokenType
 from cynthia.tools.nodes import (
     AssignmentNode, BinaryNode, FunctionNode, Node, NumberNode, ProgramNode, UnaryNode, VariableNode,
 )
 from cynthia.tools.parser import Parser
 
@@ -52,14 +53,15 @@
         'min': lambda *args: min(*args),
         'print': lambda *args: print(*args),
     }
 
     def __init__(self, parser: Parser = None, global_variables: dict = None):
         self.parser = parser if parser else Parser()
         self.global_variables = global_variables if global_variables else {}
+        self._cast_global_variables()
 
     def visit_program_node(self, node: ProgramNode):
         for statement in node.statements:
             self.visit(statement)
 
     def visit_binary_node(self, node: BinaryNode):
         if binary_logic := self.binary_logics.get(node.token.type):
@@ -111,7 +113,21 @@
     def _check_file_extension(self, input_file: TextIOBase):
         if input_file.name.split('.')[-1] not in self.supported_file_extensions:
             raise TypeError(
                 'Allowed file extensions are: {extensions}'.format(
                     extensions=self.supported_file_extensions,
                 ),
             )
+
+    def _cast_global_variables(self):
+        casted_global = {}
+        for variable_name, variable_value in self.global_variables.items():
+            try:
+                casted_global[variable_name] = Decimal(variable_value)
+            except Exception:
+                raise InvalidGlobalVariableError(
+                    'Global variable "{name}" has an invalid type "{type}"'.format(
+                        name=variable_name,
+                        type=type(variable_value).__name__,
+                    ),
+                )
+        self.global_variables = casted_global
```

### Comparing `cynthia_language-0.1.2/cynthia/tools/lexer/lexer.py` & `cynthia_language-0.1.3/cynthia/tools/lexer/lexer.py`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.2/cynthia/tools/lexer/logics.py` & `cynthia_language-0.1.3/cynthia/tools/lexer/logics.py`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.2/cynthia/tools/lexer/tokens.py` & `cynthia_language-0.1.3/cynthia/tools/lexer/tokens.py`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.2/examples/e_transaction_100k.cynthia` & `cynthia_language-0.1.3/examples/e_transaction_100k.cynthia`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.2/examples/e_transaction_200k.cynthia` & `cynthia_language-0.1.3/examples/e_transaction_200k.cynthia`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.2/LICENSE` & `cynthia_language-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.2/README.md` & `cynthia_language-0.1.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 ```
 
 # Use the language tools directly
 
 Language tools can be used directly.
 
 ```
-from cynthia.tools import Parser
+from cynthia.tools import Interpreter
 
-parser = Parser()
-parser.parse('x=1+2')
+interpreter = Interpreter()
+interpreter.interpret('x=1+2')
 
-parser['x']
+interpreter['x']
 # 3
 ```
```

### Comparing `cynthia_language-0.1.2/pyproject.toml` & `cynthia_language-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cynthia-language"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name="Krisztian Szenasi", email="szenasi999@gmail.com" },
 ]
 description = "Cynthia is a small interpreted script language for basic mathematical expressions."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `cynthia_language-0.1.2/PKG-INFO` & `cynthia_language-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cynthia-language
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cynthia is a small interpreted script language for basic mathematical expressions.
 Project-URL: Homepage, https://github.com/krisztianszenasi/cynthia
 Project-URL: Bug Tracker, https://github.com/krisztianszenasi/cynthia/issues
 Author-email: Krisztian Szenasi <szenasi999@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -135,15 +135,15 @@
 ```
 
 # Use the language tools directly
 
 Language tools can be used directly.
 
 ```
-from cynthia.tools import Parser
+from cynthia.tools import Interpreter
 
-parser = Parser()
-parser.parse('x=1+2')
+interpreter = Interpreter()
+interpreter.interpret('x=1+2')
 
-parser['x']
+interpreter['x']
 # 3
 ```
```

