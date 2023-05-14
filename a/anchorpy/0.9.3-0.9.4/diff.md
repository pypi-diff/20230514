# Comparing `tmp/anchorpy-0.9.3.tar.gz` & `tmp/anchorpy-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anchorpy-0.9.3.tar", max compression
+gzip compressed data, was "anchorpy-0.9.4.tar", max compression
```

## Comparing `anchorpy-0.9.3.tar` & `anchorpy-0.9.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1055 2022-07-06 18:22:02.460175 anchorpy-0.9.3/LICENSE
--rw-r--r--   0        0        0     1329 2022-07-06 18:22:02.460175 anchorpy-0.9.3/README.md
--rw-r--r--   0        0        0     1448 2022-07-06 18:22:02.468175 anchorpy-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     1344 2022-07-06 18:22:02.468175 anchorpy-0.9.3/src/anchorpy/__init__.py
--rw-r--r--   0        0        0     3921 2022-07-06 18:22:02.468175 anchorpy-0.9.3/src/anchorpy/borsh_extension.py
--rw-r--r--   0        0        0     4087 2022-07-06 18:22:02.468175 anchorpy-0.9.3/src/anchorpy/cli.py
--rw-r--r--   0        0        0        0 2022-07-06 18:22:02.468175 anchorpy-0.9.3/src/anchorpy/clientgen/__init__.py
--rw-r--r--   0        0        0     9183 2022-07-06 18:22:02.468175 anchorpy-0.9.3/src/anchorpy/clientgen/accounts.py
--rw-r--r--   0        0        0    20281 2022-07-06 18:22:02.468175 anchorpy-0.9.3/src/anchorpy/clientgen/common.py
--rw-r--r--   0        0        0     8186 2022-07-06 18:22:02.468175 anchorpy-0.9.3/src/anchorpy/clientgen/errors.py
--rw-r--r--   0        0        0     6499 2022-07-06 18:22:02.468175 anchorpy-0.9.3/src/anchorpy/clientgen/genpy_extension.py
--rw-r--r--   0        0        0     7605 2022-07-06 18:22:02.468175 anchorpy-0.9.3/src/anchorpy/clientgen/instructions.py
--rw-r--r--   0        0        0      617 2022-07-06 18:22:02.468175 anchorpy-0.9.3/src/anchorpy/clientgen/program_id.py
--rw-r--r--   0        0        0    22519 2022-07-06 18:22:02.468175 anchorpy-0.9.3/src/anchorpy/clientgen/types.py
--rw-r--r--   0        0        0       47 2022-07-06 18:22:02.468175 anchorpy-0.9.3/src/anchorpy/coder/__init__.py
--rw-r--r--   0        0        0     2346 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/coder/accounts.py
--rw-r--r--   0        0        0      621 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/coder/coder.py
--rw-r--r--   0        0        0     3483 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/coder/common.py
--rw-r--r--   0        0        0     2221 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/coder/event.py
--rw-r--r--   0        0        0     9992 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/coder/idl.py
--rw-r--r--   0        0        0     3027 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/coder/instruction.py
--rw-r--r--   0        0        0     9044 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/error.py
--rw-r--r--   0        0        0     6158 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/idl.py
--rw-r--r--   0        0        0       51 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/program/__init__.py
--rw-r--r--   0        0        0     2224 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/program/common.py
--rw-r--r--   0        0        0     2611 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/program/context.py
--rw-r--r--   0        0        0     7486 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/program/core.py
--rw-r--r--   0        0        0     5124 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/program/event.py
--rw-r--r--   0        0        0       73 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/program/namespace/__init__.py
--rw-r--r--   0        0        0     8055 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/program/namespace/account.py
--rw-r--r--   0        0        0     3792 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/program/namespace/instruction.py
--rw-r--r--   0        0        0     2123 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/program/namespace/rpc.py
--rw-r--r--   0        0        0     2991 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/program/namespace/simulate.py
--rw-r--r--   0        0        0     1586 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/program/namespace/transaction.py
--rw-r--r--   0        0        0      645 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/program/namespace/types.py
--rw-r--r--   0        0        0     8465 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/provider.py
--rw-r--r--   0        0        0        0 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/py.typed
--rw-r--r--   0        0        0     8423 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/pytest_plugin.py
--rw-r--r--   0        0        0      831 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/template.py
--rw-r--r--   0        0        0      125 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/utils/__init__.py
--rw-r--r--   0        0        0     5344 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/utils/rpc.py
--rw-r--r--   0        0        0     9281 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/utils/token.py
--rw-r--r--   0        0        0     1578 2022-07-06 18:22:02.472175 anchorpy-0.9.3/src/anchorpy/workspace.py
--rw-r--r--   0        0        0     2976 2022-07-06 18:22:29.695401 anchorpy-0.9.3/setup.py
--rw-r--r--   0        0        0     2784 2022-07-06 18:22:29.696143 anchorpy-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1055 2022-07-18 11:21:01.764528 anchorpy-0.9.4/LICENSE
+-rw-r--r--   0        0        0     1329 2022-07-18 11:21:01.764528 anchorpy-0.9.4/README.md
+-rw-r--r--   0        0        0     1448 2022-07-18 11:21:01.768528 anchorpy-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1344 2022-07-18 11:21:01.768528 anchorpy-0.9.4/src/anchorpy/__init__.py
+-rw-r--r--   0        0        0     3921 2022-07-18 11:21:01.768528 anchorpy-0.9.4/src/anchorpy/borsh_extension.py
+-rw-r--r--   0        0        0     4087 2022-07-18 11:21:01.768528 anchorpy-0.9.4/src/anchorpy/cli.py
+-rw-r--r--   0        0        0        0 2022-07-18 11:21:01.768528 anchorpy-0.9.4/src/anchorpy/clientgen/__init__.py
+-rw-r--r--   0        0        0     9183 2022-07-18 11:21:01.768528 anchorpy-0.9.4/src/anchorpy/clientgen/accounts.py
+-rw-r--r--   0        0        0    20281 2022-07-18 11:21:01.768528 anchorpy-0.9.4/src/anchorpy/clientgen/common.py
+-rw-r--r--   0        0        0     8186 2022-07-18 11:21:01.768528 anchorpy-0.9.4/src/anchorpy/clientgen/errors.py
+-rw-r--r--   0        0        0     6499 2022-07-18 11:21:01.768528 anchorpy-0.9.4/src/anchorpy/clientgen/genpy_extension.py
+-rw-r--r--   0        0        0     7605 2022-07-18 11:21:01.768528 anchorpy-0.9.4/src/anchorpy/clientgen/instructions.py
+-rw-r--r--   0        0        0      617 2022-07-18 11:21:01.768528 anchorpy-0.9.4/src/anchorpy/clientgen/program_id.py
+-rw-r--r--   0        0        0    22584 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/clientgen/types.py
+-rw-r--r--   0        0        0       47 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/coder/__init__.py
+-rw-r--r--   0        0        0     2346 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/coder/accounts.py
+-rw-r--r--   0        0        0      621 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/coder/coder.py
+-rw-r--r--   0        0        0     3483 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/coder/common.py
+-rw-r--r--   0        0        0     2221 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/coder/event.py
+-rw-r--r--   0        0        0     9992 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/coder/idl.py
+-rw-r--r--   0        0        0     3027 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/coder/instruction.py
+-rw-r--r--   0        0        0     9044 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/error.py
+-rw-r--r--   0        0        0     6158 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/idl.py
+-rw-r--r--   0        0        0       51 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/program/__init__.py
+-rw-r--r--   0        0        0     2224 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/program/common.py
+-rw-r--r--   0        0        0     2611 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/program/context.py
+-rw-r--r--   0        0        0     7486 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/program/core.py
+-rw-r--r--   0        0        0     5124 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/program/event.py
+-rw-r--r--   0        0        0       73 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/program/namespace/__init__.py
+-rw-r--r--   0        0        0     8055 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/program/namespace/account.py
+-rw-r--r--   0        0        0     3792 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/program/namespace/instruction.py
+-rw-r--r--   0        0        0     2123 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/program/namespace/rpc.py
+-rw-r--r--   0        0        0     2991 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/program/namespace/simulate.py
+-rw-r--r--   0        0        0     1586 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/program/namespace/transaction.py
+-rw-r--r--   0        0        0      645 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/program/namespace/types.py
+-rw-r--r--   0        0        0     8465 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/provider.py
+-rw-r--r--   0        0        0        0 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/py.typed
+-rw-r--r--   0        0        0     8423 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/pytest_plugin.py
+-rw-r--r--   0        0        0      831 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/template.py
+-rw-r--r--   0        0        0      125 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/utils/__init__.py
+-rw-r--r--   0        0        0     5344 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/utils/rpc.py
+-rw-r--r--   0        0        0     9281 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/utils/token.py
+-rw-r--r--   0        0        0     1578 2022-07-18 11:21:01.772529 anchorpy-0.9.4/src/anchorpy/workspace.py
+-rw-r--r--   0        0        0     2976 2022-07-18 11:21:20.482695 anchorpy-0.9.4/setup.py
+-rw-r--r--   0        0        0     2784 2022-07-18 11:21:20.483060 anchorpy-0.9.4/PKG-INFO
```

### Comparing `anchorpy-0.9.3/LICENSE` & `anchorpy-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/README.md` & `anchorpy-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/pyproject.toml` & `anchorpy-0.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anchorpy"
-version = "0.9.3"
+version = "0.9.4"
 description = "The Python Anchor client."
 readme = "README.md"
 repository = "https://github.com/kevinheavey/anchorpy"
 documentation = "https://kevinheavey.github.io/anchorpy/"
 authors = ["kevinheavey <kevinheavey123@gmail.com>"]
 
 [tool.poetry.dependencies]
```

### Comparing `anchorpy-0.9.3/src/anchorpy/__init__.py` & `anchorpy-0.9.4/src/anchorpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,8 @@
     "EventParser",
     "SimulateResponse",
     "error",
     "utils",
 ]
 
 
-__version__ = "0.9.3"
+__version__ = "0.9.4"
```

### Comparing `anchorpy-0.9.3/src/anchorpy/borsh_extension.py` & `anchorpy-0.9.4/src/anchorpy/borsh_extension.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/cli.py` & `anchorpy-0.9.4/src/anchorpy/cli.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/clientgen/accounts.py` & `anchorpy-0.9.4/src/anchorpy/clientgen/accounts.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/clientgen/common.py` & `anchorpy-0.9.4/src/anchorpy/clientgen/common.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/clientgen/errors.py` & `anchorpy-0.9.4/src/anchorpy/clientgen/errors.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/clientgen/genpy_extension.py` & `anchorpy-0.9.4/src/anchorpy/clientgen/genpy_extension.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/clientgen/instructions.py` & `anchorpy-0.9.4/src/anchorpy/clientgen/instructions.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/clientgen/program_id.py` & `anchorpy-0.9.4/src/anchorpy/clientgen/program_id.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/clientgen/types.py` & `anchorpy-0.9.4/src/anchorpy/clientgen/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
 
 def gen_struct(idl: Idl, name: str, fields: list[_IdlField]) -> Collection:
     imports = [
         Import("typing"),
         FromImport("dataclasses", ["dataclass"]),
         FromImport("construct", ["Container", "Construct"]),
         FromImport("solana.publickey", ["PublicKey"]),
+        FromImport("anchorpy.borsh_extension", ["BorshPubkey"]),
         ImportAs("borsh_construct", "borsh"),
     ]
     json_interface_name = _json_interface_name(name)
     field_params: list[TypedParam] = []
     json_interface_params: list[TypedParam] = []
     layout_items: list[str] = []
     from_decoded_items: list[str] = []
```

### Comparing `anchorpy-0.9.3/src/anchorpy/coder/accounts.py` & `anchorpy-0.9.4/src/anchorpy/coder/accounts.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/coder/coder.py` & `anchorpy-0.9.4/src/anchorpy/coder/coder.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/coder/common.py` & `anchorpy-0.9.4/src/anchorpy/coder/common.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/coder/event.py` & `anchorpy-0.9.4/src/anchorpy/coder/event.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/coder/idl.py` & `anchorpy-0.9.4/src/anchorpy/coder/idl.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/coder/instruction.py` & `anchorpy-0.9.4/src/anchorpy/coder/instruction.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/error.py` & `anchorpy-0.9.4/src/anchorpy/error.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/idl.py` & `anchorpy-0.9.4/src/anchorpy/idl.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/program/common.py` & `anchorpy-0.9.4/src/anchorpy/program/common.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/program/context.py` & `anchorpy-0.9.4/src/anchorpy/program/context.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/program/core.py` & `anchorpy-0.9.4/src/anchorpy/program/core.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/program/event.py` & `anchorpy-0.9.4/src/anchorpy/program/event.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/program/namespace/account.py` & `anchorpy-0.9.4/src/anchorpy/program/namespace/account.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/program/namespace/instruction.py` & `anchorpy-0.9.4/src/anchorpy/program/namespace/instruction.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/program/namespace/rpc.py` & `anchorpy-0.9.4/src/anchorpy/program/namespace/rpc.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/program/namespace/simulate.py` & `anchorpy-0.9.4/src/anchorpy/program/namespace/simulate.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/program/namespace/transaction.py` & `anchorpy-0.9.4/src/anchorpy/program/namespace/transaction.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/program/namespace/types.py` & `anchorpy-0.9.4/src/anchorpy/program/namespace/types.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/provider.py` & `anchorpy-0.9.4/src/anchorpy/provider.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/pytest_plugin.py` & `anchorpy-0.9.4/src/anchorpy/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/template.py` & `anchorpy-0.9.4/src/anchorpy/template.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/utils/rpc.py` & `anchorpy-0.9.4/src/anchorpy/utils/rpc.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/utils/token.py` & `anchorpy-0.9.4/src/anchorpy/utils/token.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/src/anchorpy/workspace.py` & `anchorpy-0.9.4/src/anchorpy/workspace.py`

 * *Files identical despite different names*

### Comparing `anchorpy-0.9.3/setup.py` & `anchorpy-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 entry_points = \
 {'console_scripts': ['anchorpy = anchorpy.cli:app'],
  'pytest11': ['pytest_anchorpy = anchorpy.pytest_plugin']}
 
 setup_kwargs = {
     'name': 'anchorpy',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'The Python Anchor client.',
     'long_description': '# AnchorPy\n<div align="center">\n    <img src="https://raw.githubusercontent.com/kevinheavey/anchorpy/main/docs/img/logo.png" width="40%" height="40%">\n</div>\n\n---\n\n[![Discord Chat](https://img.shields.io/discord/889577356681945098?color=blueviolet)](https://discord.gg/sxy4zxBckh)  \n\nAnchorPy is the gateway to interacting with [Anchor](https://github.com/project-serum/anchor) programs in Python.\nIt provides:\n\n- A static client generator\n- A dynamic client similar to `anchor-ts`\n- A Pytest plugin\n- A CLI with various utilities for Anchor Python development.\n\nRead the [Documentation](https://kevinheavey.github.io/anchorpy/).\n\n\n\n## Installation (requires Python >=3.9)\n\n```sh\npip install anchorpy[cli]\n\n```\nOr, if you\'re not using the CLI features of AnchorPy you can just run `pip install anchorpy`.\n\n### Development Setup\n\nIf you want to contribute to AnchorPy, follow these steps to get set up:\n\n1. Install [poetry](https://python-poetry.org/docs/#installation)\n2. Install dev dependencies:\n```sh\npoetry install\n\n```\n3. Install [nox-poetry](https://github.com/cjolowicz/nox-poetry) (note: do not use Poetry to install this, see [here](https://medium.com/@cjolowicz/nox-is-a-part-of-your-global-developer-environment-like-poetry-pre-commit-pyenv-or-pipx-1cdeba9198bd))\n4. Activate the poetry shell:\n```sh\npoetry shell\n\n```\n',
     'author': 'kevinheavey',
     'author_email': 'kevinheavey123@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/kevinheavey/anchorpy',
```

### Comparing `anchorpy-0.9.3/PKG-INFO` & `anchorpy-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchorpy
-Version: 0.9.3
+Version: 0.9.4
 Summary: The Python Anchor client.
 Home-page: https://github.com/kevinheavey/anchorpy
 Author: kevinheavey
 Author-email: kevinheavey123@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

