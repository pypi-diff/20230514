# Comparing `tmp/cynthia_language-0.1.0.tar.gz` & `tmp/cynthia_language-0.1.1.tar.gz`

## Comparing `cynthia_language-0.1.0.tar` & `cynthia_language-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/setup.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/__init__.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/__main__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/__init__.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/nodes.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/parser.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/shell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/interpreter/__init__.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/interpreter/exceptions.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/interpreter/interpreter.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/lexer/__init__.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/lexer/lexer.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/lexer/lexer_utils.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/lexer/logics.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/lexer/supported_tokens.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/cynthia/tools/lexer/tokens.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/examples/base_account.cynthia
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/examples/e_transaction_0,3%.cynthia
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/examples/e_transaction_100k.cynthia
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/examples/e_transaction_200k.cynthia
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/LICENSE
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 cynthia_language-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/.DS_Store
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/setup.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/__init__.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/__main__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/__init__.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/nodes.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/parser.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/shell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/interpreter/__init__.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/interpreter/exceptions.py
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/interpreter/interpreter.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/lexer/__init__.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/lexer/lexer.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/lexer/lexer_utils.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/lexer/logics.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/lexer/supported_tokens.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/cynthia/tools/lexer/tokens.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/examples/base_account.cynthia
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/examples/e_transaction_0,3%.cynthia
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/examples/e_transaction_100k.cynthia
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/examples/e_transaction_200k.cynthia
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 cynthia_language-0.1.1/PKG-INFO
```

### Comparing `cynthia_language-0.1.0/setup.cfg` & `cynthia_language-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.0/cynthia/__main__.py` & `cynthia_language-0.1.1/cynthia/__main__.py`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.0/cynthia/tools/nodes.py` & `cynthia_language-0.1.1/cynthia/tools/nodes.py`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.0/cynthia/tools/parser.py` & `cynthia_language-0.1.1/cynthia/tools/parser.py`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.0/cynthia/tools/interpreter/interpreter.py` & `cynthia_language-0.1.1/cynthia/tools/interpreter/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         method_name = 'visit_{node_name}'.format(
             node_name=self._pascal_to_snake(type(node).__name__),
         )
         visitor = getattr(self, method_name, self.generic_visit)
         return visitor(node)
 
     def generic_visit(self, node):
-        raise VisitorDoesNotExistError(node=node)
+        raise VisitorDoesNotExistError(f'Visitor does not exit for node {node}.')
 
     def _pascal_to_snake(self, pascal_name: str) -> str:
         return re.sub('(?<!^)(?=[A-Z])', '_', pascal_name).lower()
 
 
 class Interpreter(NodeVisitor):
     """Interpreter will evaluate a given AST."""
@@ -80,16 +80,16 @@
     def visit_variable_node(self, variable_node: VariableNode):
         try:
             return self.global_variables[variable_node.name]
         except KeyError:
             raise VariableDoesNotExitError(f' Variable {variable_node.name} does not exist.')
 
     def visit_function_node(self, function_node: FunctionNode):
-        args = [self.visit(arg) for arg in function_node.args]
         if core_function := self.core_functions.get(function_node.token.value):
+            args = [self.visit(arg) for arg in function_node.args]
             return core_function(*args)
         raise FunctionDoesNotExistError(f' Function {function_node.name} does not exist.')
 
     def interpret(self, to_interpret: str | Node | TextIOBase):
         if isinstance(to_interpret, TextIOBase):
             self._check_file_extension(to_interpret)
             to_interpret = to_interpret.read()
```

### Comparing `cynthia_language-0.1.0/cynthia/tools/lexer/lexer.py` & `cynthia_language-0.1.1/cynthia/tools/lexer/lexer.py`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.0/cynthia/tools/lexer/logics.py` & `cynthia_language-0.1.1/cynthia/tools/lexer/logics.py`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.0/cynthia/tools/lexer/tokens.py` & `cynthia_language-0.1.1/cynthia/tools/lexer/tokens.py`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.0/examples/e_transaction_100k.cynthia` & `cynthia_language-0.1.1/examples/e_transaction_100k.cynthia`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.0/examples/e_transaction_200k.cynthia` & `cynthia_language-0.1.1/examples/e_transaction_200k.cynthia`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.0/LICENSE` & `cynthia_language-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.0/README.md` & `cynthia_language-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cynthia_language-0.1.0/pyproject.toml` & `cynthia_language-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cynthia-language"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name="Krisztian Szenasi", email="szenasi999@gmail.com" },
 ]
 description = "Cynthia is a small interpreted script language for basic mathematical expressions."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `cynthia_language-0.1.0/PKG-INFO` & `cynthia_language-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cynthia-language
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cynthia is a small interpreted script language for basic mathematical expressions.
 Project-URL: Homepage, https://github.com/krisztianszenasi/cynthia
 Project-URL: Bug Tracker, https://github.com/krisztianszenasi/cynthia/issues
 Author-email: Krisztian Szenasi <szenasi999@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

