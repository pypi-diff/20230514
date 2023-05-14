# Comparing `tmp/pybash-0.2.5.tar.gz` & `tmp/pybash-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybash-0.2.5.tar", max compression
+gzip compressed data, was "pybash-0.3.0.tar", max compression
```

## Comparing `pybash-0.2.5.tar` & `pybash-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     1060 2023-05-03 03:20:25.064041 pybash-0.2.5/LICENSE
--rw-r--r--   0        0        0     3794 2023-05-03 03:20:25.064041 pybash-0.2.5/README.md
--rw-r--r--   0        0        0    15950 2023-05-03 03:20:25.064041 pybash-0.2.5/pybash.py
--rw-r--r--   0        0        0      676 2023-05-03 03:20:25.064041 pybash-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4215 1970-01-01 00:00:00.000000 pybash-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-05-14 00:39:18.698108 pybash-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3912 2023-05-14 00:39:18.698108 pybash-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-14 00:39:18.698108 pybash-0.3.0/pybash/__init__.py
+-rw-r--r--   0        0        0      540 2023-05-14 00:39:18.698108 pybash-0.3.0/pybash/hook.py
+-rw-r--r--   0        0        0    15403 2023-05-14 00:39:18.698108 pybash-0.3.0/pybash/transformer.py
+-rw-r--r--   0        0        0      791 2023-05-14 00:39:18.698108 pybash-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4454 1970-01-01 00:00:00.000000 pybash-0.3.0/PKG-INFO
```

### Comparing `pybash-0.2.5/LICENSE` & `pybash-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybash-0.2.5/README.md` & `pybash-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,33 @@
 ![PyPI](https://img.shields.io/pypi/v/pybash)
 ![GitHub](https://img.shields.io/github/license/jaykv/pybash)
 
 Streamline bash-command execution from python with a new syntax. It combines the simplicity of writing bash scripts with the flexibility of python. Under the hood, any line or variable assignment starting with `>` or surrounded by parentheses is transformed to python `subprocess` calls and then injected into `sys.meta_path` as an import hook. All possible thanks to the wonderful [ideas](https://github.com/aroberge/ideas) project!
 
 For security and performance reasons, PyBash will NOT execute as shell, unless explicitly specified with a `$` instead of a single `>` before the command. While running commands as shell can be convenient, it can also spawn security risks if you're not too careful. If you're curious about the transformations, look at the [unit tests](test_pybash.py) for some quick examples.
 
-Note: this is a mainly experimental library. Consider the risks and test before using in prod.
+Note: this is a mainly experimental library.
 
-# Installation
+# Setup
+
+## As standalone transformer
 `pip install pybash`
 
-# Setup hook
+
 ```python
-import pybash
-pybash.add_hook()
+from pybash.transformer import transform
+
+transform(">echo hello world") # returns the python code for the bash command as string
 ```
 
+## As ideas hook
+`pip install "pybash[ideas]"`
+
+See [run.py](run.py) for an example.
+
 # Usage
 
 ### 1. Simple execution with output
 ```python
 >python --version
 >echo \\nthis is an echo
 ```
@@ -145,9 +153,9 @@
 ```
 
 # Dev
 
 #### Demo
 `python run.py`
 
-#### Debugging
-`python -m ideas demo -a pybash -s` to view the transformed source code
+#### Debug
+`make debug` to view the transformed source code
```

### Comparing `pybash-0.2.5/pybash.py` & `pybash-0.3.0/pybash/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,12 @@
 import re
 import shlex
 from typing import Callable, Union
 
 import token_utils
-from ideas import import_hook
-
-
-def source_init():
-    """Adds subprocess import"""
-    return "import subprocess"
-
-
-def add_hook(**_kwargs):
-    """Creates and automatically adds the import hook in sys.meta_path"""
-    return import_hook.create_hook(
-        hook_name=__name__,
-        transform_source=Transformer.transform_source,
-        source_init=source_init,
-    )
 
 
 class InvalidInterpolation(Exception):
     pass
 
 
 class Processor:
@@ -43,15 +28,16 @@
         self.token.string = Processor.fstring_interpolate(self.token_line, self.token.string)
         self.token.string = Processor.direct_interpolate(self.token.string)
 
     @staticmethod
     def fstring_interpolate(token_string: str, parsed_command: str) -> str:
         """Process f{ dynamic interpolations } and substitute.
             Dynamic interpolations are denotated by a f{ } with any expression inside.
-            Substitution in the parsed command string happens relative to the order of the interpolations in the original command string.
+            Substitution in the parsed command string happens relative to the order of the
+            interpolations in the original command string.
 
         Args:
             token_string (str): Original command string
             parsed_command (str): Parsed command string
 
         Returns:
             str: Interpolated parsed command string
@@ -67,15 +53,16 @@
 
         return parsed_command
 
     @staticmethod
     def direct_interpolate(string: str) -> str:
         """Process {{ static interpolations }} and substitute.
             Static interpolations are denotated by a {{ }} with a variable or a function call inside.
-            Substitution happens directly on the parsed command string. Therefore, certain characters cannot be interpolated as they get parsed out before substitution.
+            Substitution happens directly on the parsed command string. Therefore, certain characters
+            cannot be interpolated as they get parsed out before substitution.
 
         Args:
             string (str): String to interpolate
 
         Returns:
             str: Interpolated string
         """
@@ -148,50 +135,14 @@
             + self.raw_line[-1][self.raw_line[-1].index(')') :]
             + '\n'
         )
 
         return self.token
 
 
-class Transformer:
-    tokenizers = {"$": Shelled, ">": Execed}
-    greedy_tokenizers = {"= >": Variablized, "(>": Wrapped}
-
-    @staticmethod
-    def transform_source(source, **_kwargs):
-        """Convert >bash commands to subprocess calls"""
-        new_tokens = []
-        for line in token_utils.get_lines(source):
-            token = token_utils.get_first(line)
-            if not token:
-                new_tokens.extend(line)
-                continue
-
-            if token_match := [tokenizer for match, tokenizer in Transformer.tokenizers.items() if token == match]:
-                parser = token_match[0](token)
-                parser.transform()
-                parser.interpolate()
-                new_tokens.append(parser.token)
-                continue
-
-            if greedy_match := [
-                tokenizer for match, tokenizer in Transformer.greedy_tokenizers.items() if match in token.line
-            ]:
-                parser = greedy_match[0](token)
-                parser.transform()
-                parser.interpolate()
-                new_tokens.append(parser.token)
-                continue
-
-            # no match
-            new_tokens.extend(line)
-
-        return token_utils.untokenize(new_tokens)
-
-
 class Pipers:
     """Handles the logic of chaining operators"""
 
     OPS = ['|', '>', '>>', '<', '&&']
 
     @classmethod
     def get_piper(cls, op: str) -> Callable:
@@ -455,7 +406,40 @@
         command = command[:-1]
         command += ']'
         if kwargs:
             for k, v in kwargs.items():
                 command += f", {k}={v}"
         command += ")"
         return command
+
+
+TOKENIZERS = {"$": Shelled, ">": Execed}
+GREEDY_TOKENIZERS = {"= >": Variablized, "(>": Wrapped}
+
+
+def transform(source, **_kwargs):
+    """Convert >bash commands to subprocess calls"""
+    new_tokens = []
+    for line in token_utils.get_lines(source):
+        token = token_utils.get_first(line)
+        if not token:
+            new_tokens.extend(line)
+            continue
+
+        if token_match := [tokenizer for match, tokenizer in TOKENIZERS.items() if token == match]:
+            parser = token_match[0](token)
+            parser.transform()
+            parser.interpolate()
+            new_tokens.append(parser.token)
+            continue
+
+        if greedy_match := [tokenizer for match, tokenizer in GREEDY_TOKENIZERS.items() if match in token.line]:
+            parser = greedy_match[0](token)
+            parser.transform()
+            parser.interpolate()
+            new_tokens.append(parser.token)
+            continue
+
+        # no match
+        new_tokens.extend(line)
+
+    return token_utils.untokenize(new_tokens)
```

### Comparing `pybash-0.2.5/pyproject.toml` & `pybash-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 [tool.poetry]
 name = "PyBash"
-version = "0.2.5"
+version = "0.3.0"
 description = ">execute bash commands from python easily"
-authors = ["Jay"]
+authors = ["Jay <jay.github0@gmail.com>"]
 readme = "README.md"
-packages = [{include = "pybash.py"}]
+packages = [{include = "pybash"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-ideas = "^0.1.5"
+ideas = { version = "^0.1.5", optional = true }
+token-utils = "^0.1.8"
+
+[tool.poetry.extras]
+ideas = ["ideas"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 pytest = "^7.2.1"
 isort = "^5.11.4"
 flake8 = "^6.0.0"
 autoflake = "^2.0.0"
```

### Comparing `pybash-0.2.5/PKG-INFO` & `pybash-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 Metadata-Version: 2.1
 Name: pybash
-Version: 0.2.5
+Version: 0.3.0
 Summary: >execute bash commands from python easily
 Author: Jay
+Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ideas (>=0.1.5,<0.2.0)
+Provides-Extra: ideas
+Requires-Dist: ideas (>=0.1.5,<0.2.0) ; extra == "ideas"
+Requires-Dist: token-utils (>=0.1.8,<0.2.0)
 Description-Content-Type: text/markdown
 
 # PyBash
 
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jaykv/pybash/python-app.yml?branch=main)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pybash)
 ![PyPI](https://img.shields.io/pypi/v/pybash)
 ![GitHub](https://img.shields.io/github/license/jaykv/pybash)
 
 Streamline bash-command execution from python with a new syntax. It combines the simplicity of writing bash scripts with the flexibility of python. Under the hood, any line or variable assignment starting with `>` or surrounded by parentheses is transformed to python `subprocess` calls and then injected into `sys.meta_path` as an import hook. All possible thanks to the wonderful [ideas](https://github.com/aroberge/ideas) project!
 
 For security and performance reasons, PyBash will NOT execute as shell, unless explicitly specified with a `$` instead of a single `>` before the command. While running commands as shell can be convenient, it can also spawn security risks if you're not too careful. If you're curious about the transformations, look at the [unit tests](test_pybash.py) for some quick examples.
 
-Note: this is a mainly experimental library. Consider the risks and test before using in prod.
+Note: this is a mainly experimental library.
 
-# Installation
+# Setup
+
+## As standalone transformer
 `pip install pybash`
 
-# Setup hook
+
 ```python
-import pybash
-pybash.add_hook()
+from pybash.transformer import transform
+
+transform(">echo hello world") # returns the python code for the bash command as string
 ```
 
+## As ideas hook
+`pip install "pybash[ideas]"`
+
+See [run.py](run.py) for an example.
+
 # Usage
 
 ### 1. Simple execution with output
 ```python
 >python --version
 >echo \\nthis is an echo
 ```
@@ -158,10 +169,10 @@
 ```
 
 # Dev
 
 #### Demo
 `python run.py`
 
-#### Debugging
-`python -m ideas demo -a pybash -s` to view the transformed source code
+#### Debug
+`make debug` to view the transformed source code
```

