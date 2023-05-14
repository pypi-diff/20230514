# Comparing `tmp/solana-0.9.1.tar.gz` & `tmp/solana-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/solana-0.9.1.tar", last modified: Mon May 31 23:28:27 2021, max compression
+gzip compressed data, was "dist/solana-0.9.2.tar", last modified: Wed Jun  2 00:16:34 2021, max compression
```

## Comparing `solana-0.9.1.tar` & `solana-0.9.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-05-31 23:28:27.000000 solana-0.9.1/
--rw-r--r--   0 michaelhuang   (501) staff       (20)     3177 2021-05-31 23:28:27.000000 solana-0.9.1/PKG-INFO
--rw-r--r--   0 michaelhuang   (501) staff       (20)     1842 2020-09-09 21:29:06.000000 solana-0.9.1/README.md
-drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-05-31 23:28:27.000000 solana-0.9.1/docs/
--rw-r--r--   0 michaelhuang   (501) staff       (20)     2102 2021-05-31 23:28:06.000000 solana-0.9.1/docs/conf.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)       38 2021-05-31 23:28:27.000000 solana-0.9.1/setup.cfg
--rw-r--r--   0 michaelhuang   (501) staff       (20)     1661 2021-05-31 23:28:06.000000 solana-0.9.1/setup.py
-drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-05-31 23:28:27.000000 solana-0.9.1/solana/
--rw-r--r--   0 michaelhuang   (501) staff       (20)      550 2021-05-31 23:28:04.000000 solana-0.9.1/solana/__init__.py
-drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-05-31 23:28:27.000000 solana-0.9.1/solana/_layouts/
--rw-r--r--   0 michaelhuang   (501) staff       (20)        0 2020-09-09 21:29:06.000000 solana-0.9.1/solana/_layouts/__init__.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)      305 2020-09-09 21:29:06.000000 solana-0.9.1/solana/_layouts/shared.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)     2847 2021-05-27 01:40:04.000000 solana-0.9.1/solana/_layouts/system_instructions.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)     2749 2021-04-24 21:28:55.000000 solana-0.9.1/solana/account.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)      265 2020-08-29 21:55:00.000000 solana-0.9.1/solana/blockhash.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)     1539 2020-09-09 21:29:06.000000 solana-0.9.1/solana/instruction.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)     9590 2021-04-17 21:13:38.000000 solana-0.9.1/solana/message.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)     3863 2021-05-31 23:21:10.000000 solana-0.9.1/solana/publickey.py
-drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-05-31 23:28:27.000000 solana-0.9.1/solana/rpc/
--rw-r--r--   0 michaelhuang   (501) staff       (20)       44 2020-08-29 21:55:00.000000 solana-0.9.1/solana/rpc/__init__.py
-drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-05-31 23:28:27.000000 solana-0.9.1/solana/rpc/_utils/
--rw-r--r--   0 michaelhuang   (501) staff       (20)        0 2020-08-29 21:55:00.000000 solana-0.9.1/solana/rpc/_utils/__init__.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)     2982 2021-04-18 02:12:58.000000 solana-0.9.1/solana/rpc/_utils/encoding.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)    50223 2021-05-17 05:29:31.000000 solana-0.9.1/solana/rpc/api.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)     1066 2020-11-11 02:03:02.000000 solana-0.9.1/solana/rpc/commitment.py
-drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-05-31 23:28:27.000000 solana-0.9.1/solana/rpc/providers/
--rw-r--r--   0 michaelhuang   (501) staff       (20)       21 2020-08-29 21:55:00.000000 solana-0.9.1/solana/rpc/providers/__init__.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)      507 2020-08-29 21:55:00.000000 solana-0.9.1/solana/rpc/providers/base.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)     2247 2020-09-10 18:32:06.000000 solana-0.9.1/solana/rpc/providers/http.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)     2875 2020-10-04 23:24:45.000000 solana-0.9.1/solana/rpc/types.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)    13666 2021-05-31 23:24:57.000000 solana-0.9.1/solana/system_program.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)      989 2020-08-30 03:46:44.000000 solana-0.9.1/solana/sysvar.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)    18068 2021-05-31 23:24:57.000000 solana-0.9.1/solana/transaction.py
-drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-05-31 23:28:27.000000 solana-0.9.1/solana/utils/
--rw-r--r--   0 michaelhuang   (501) staff       (20)       40 2020-08-29 21:55:00.000000 solana-0.9.1/solana/utils/__init__.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)     1313 2021-05-27 01:40:04.000000 solana-0.9.1/solana/utils/ed25519_base.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)      293 2020-09-09 21:29:06.000000 solana-0.9.1/solana/utils/helpers.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)      759 2020-08-29 21:55:00.000000 solana-0.9.1/solana/utils/shortvec_encoding.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)     1162 2020-09-09 21:29:06.000000 solana-0.9.1/solana/utils/validate.py
-drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-05-31 23:28:27.000000 solana-0.9.1/solana.egg-info/
--rw-r--r--   0 michaelhuang   (501) staff       (20)     3177 2021-05-31 23:28:27.000000 solana-0.9.1/solana.egg-info/PKG-INFO
--rw-r--r--   0 michaelhuang   (501) staff       (20)      948 2021-05-31 23:28:27.000000 solana-0.9.1/solana.egg-info/SOURCES.txt
--rw-r--r--   0 michaelhuang   (501) staff       (20)        1 2021-05-31 23:28:27.000000 solana-0.9.1/solana.egg-info/dependency_links.txt
--rw-r--r--   0 michaelhuang   (501) staff       (20)        1 2021-05-31 23:28:27.000000 solana-0.9.1/solana.egg-info/not-zip-safe
--rw-r--r--   0 michaelhuang   (501) staff       (20)      234 2021-05-31 23:28:27.000000 solana-0.9.1/solana.egg-info/requires.txt
--rw-r--r--   0 michaelhuang   (501) staff       (20)       42 2021-05-31 23:28:27.000000 solana-0.9.1/solana.egg-info/top_level.txt
-drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-05-31 23:28:27.000000 solana-0.9.1/spl/
-drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-05-31 23:28:27.000000 solana-0.9.1/spl/token/
--rw-r--r--   0 michaelhuang   (501) staff       (20)     3338 2021-05-27 01:40:04.000000 solana-0.9.1/spl/token/_layouts.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)    22678 2021-05-31 23:24:57.000000 solana-0.9.1/spl/token/client.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)      952 2021-05-27 01:40:04.000000 solana-0.9.1/spl/token/constants.py
--rw-r--r--   0 michaelhuang   (501) staff       (20)    36986 2021-05-31 23:24:57.000000 solana-0.9.1/spl/token/instructions.py
+drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-06-02 00:16:34.000000 solana-0.9.2/
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     3177 2021-06-02 00:16:34.000000 solana-0.9.2/PKG-INFO
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     1842 2020-09-09 21:29:06.000000 solana-0.9.2/README.md
+drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-06-02 00:16:34.000000 solana-0.9.2/docs/
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     2102 2021-06-02 00:16:08.000000 solana-0.9.2/docs/conf.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)       38 2021-06-02 00:16:34.000000 solana-0.9.2/setup.cfg
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     1661 2021-06-02 00:16:08.000000 solana-0.9.2/setup.py
+drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-06-02 00:16:34.000000 solana-0.9.2/solana/
+-rw-r--r--   0 michaelhuang   (501) staff       (20)      610 2021-05-31 23:47:36.000000 solana-0.9.2/solana/__init__.py
+drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-06-02 00:16:34.000000 solana-0.9.2/solana/_layouts/
+-rw-r--r--   0 michaelhuang   (501) staff       (20)        0 2020-09-09 21:29:06.000000 solana-0.9.2/solana/_layouts/__init__.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)      305 2020-09-09 21:29:06.000000 solana-0.9.2/solana/_layouts/shared.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     2847 2021-05-27 01:40:04.000000 solana-0.9.2/solana/_layouts/system_instructions.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     2749 2021-04-24 21:28:55.000000 solana-0.9.2/solana/account.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)      265 2020-08-29 21:55:00.000000 solana-0.9.2/solana/blockhash.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     1539 2020-09-09 21:29:06.000000 solana-0.9.2/solana/instruction.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     9590 2021-04-17 21:13:38.000000 solana-0.9.2/solana/message.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     3863 2021-05-31 23:21:10.000000 solana-0.9.2/solana/publickey.py
+drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-06-02 00:16:34.000000 solana-0.9.2/solana/rpc/
+-rw-r--r--   0 michaelhuang   (501) staff       (20)       44 2020-08-29 21:55:00.000000 solana-0.9.2/solana/rpc/__init__.py
+drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-06-02 00:16:34.000000 solana-0.9.2/solana/rpc/_utils/
+-rw-r--r--   0 michaelhuang   (501) staff       (20)        0 2020-08-29 21:55:00.000000 solana-0.9.2/solana/rpc/_utils/__init__.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     2982 2021-04-18 02:12:58.000000 solana-0.9.2/solana/rpc/_utils/encoding.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)    50223 2021-05-17 05:29:31.000000 solana-0.9.2/solana/rpc/api.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     1066 2020-11-11 02:03:02.000000 solana-0.9.2/solana/rpc/commitment.py
+drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-06-02 00:16:34.000000 solana-0.9.2/solana/rpc/providers/
+-rw-r--r--   0 michaelhuang   (501) staff       (20)       21 2020-08-29 21:55:00.000000 solana-0.9.2/solana/rpc/providers/__init__.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)      507 2020-08-29 21:55:00.000000 solana-0.9.2/solana/rpc/providers/base.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     2247 2020-09-10 18:32:06.000000 solana-0.9.2/solana/rpc/providers/http.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     2875 2020-10-04 23:24:45.000000 solana-0.9.2/solana/rpc/types.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)    13666 2021-05-31 23:31:01.000000 solana-0.9.2/solana/system_program.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)      989 2020-08-30 03:46:44.000000 solana-0.9.2/solana/sysvar.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)    18050 2021-06-02 00:16:08.000000 solana-0.9.2/solana/transaction.py
+drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-06-02 00:16:34.000000 solana-0.9.2/solana/utils/
+-rw-r--r--   0 michaelhuang   (501) staff       (20)       40 2020-08-29 21:55:00.000000 solana-0.9.2/solana/utils/__init__.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     1313 2021-05-27 01:40:04.000000 solana-0.9.2/solana/utils/ed25519_base.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)      293 2020-09-09 21:29:06.000000 solana-0.9.2/solana/utils/helpers.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)      759 2020-08-29 21:55:00.000000 solana-0.9.2/solana/utils/shortvec_encoding.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     1162 2020-09-09 21:29:06.000000 solana-0.9.2/solana/utils/validate.py
+drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-06-02 00:16:34.000000 solana-0.9.2/solana.egg-info/
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     3177 2021-06-02 00:16:34.000000 solana-0.9.2/solana.egg-info/PKG-INFO
+-rw-r--r--   0 michaelhuang   (501) staff       (20)      948 2021-06-02 00:16:34.000000 solana-0.9.2/solana.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelhuang   (501) staff       (20)        1 2021-06-02 00:16:34.000000 solana-0.9.2/solana.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelhuang   (501) staff       (20)        1 2021-06-02 00:16:34.000000 solana-0.9.2/solana.egg-info/not-zip-safe
+-rw-r--r--   0 michaelhuang   (501) staff       (20)      234 2021-06-02 00:16:34.000000 solana-0.9.2/solana.egg-info/requires.txt
+-rw-r--r--   0 michaelhuang   (501) staff       (20)       42 2021-06-02 00:16:34.000000 solana-0.9.2/solana.egg-info/top_level.txt
+drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-06-02 00:16:34.000000 solana-0.9.2/spl/
+drwxr-xr-x   0 michaelhuang   (501) staff       (20)        0 2021-06-02 00:16:34.000000 solana-0.9.2/spl/token/
+-rw-r--r--   0 michaelhuang   (501) staff       (20)     3338 2021-05-27 01:40:04.000000 solana-0.9.2/spl/token/_layouts.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)    22678 2021-05-31 23:31:01.000000 solana-0.9.2/spl/token/client.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)      952 2021-05-27 01:40:04.000000 solana-0.9.2/spl/token/constants.py
+-rw-r--r--   0 michaelhuang   (501) staff       (20)    36986 2021-05-31 23:31:01.000000 solana-0.9.2/spl/token/instructions.py
```

### Comparing `solana-0.9.1/PKG-INFO` & `solana-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solana
-Version: 0.9.1
+Version: 0.9.2
 Summary: Solana.py
 Home-page: https://github.com/michaelhly/solanapy
 Author: Michael Huang
 License: MIT
 Description: [![Actions
         Status](https://github.com/michaelhly/solanapy/workflows/CI/badge.svg)](https://github.com/michaelhly/solanapy/actions?query=workflow%3ACI)
         [![PyPI version](https://badge.fury.io/py/solana.svg)](https://badge.fury.io/py/solana)
```

### Comparing `solana-0.9.1/README.md` & `solana-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/docs/conf.py` & `solana-0.9.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 # -- Project information -----------------------------------------------------
 
 project = "solana.py"
 copyright = "2020, Michael Huang"
 # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.4
-version = "0.9.1"
+version = "0.9.2"
 author = "Michael Huang"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `solana-0.9.1/setup.py` & `solana-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 with open("README.md", "r") as file_handle:
     README_MD = file_handle.read()
 
 setup(
     name="solana",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="0.9.1",
+    version="0.9.2",
     author="Michael Huang",
     author_mail="michaelhly@gmail.com",
     description="""Solana.py""",
     long_description=README_MD,
     long_description_content_type="text/markdown",
     include_package_data=True,
     install_requires=[
```

### Comparing `solana-0.9.1/solana/_layouts/system_instructions.py` & `solana-0.9.2/solana/_layouts/system_instructions.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/account.py` & `solana-0.9.2/solana/account.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/instruction.py` & `solana-0.9.2/solana/instruction.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/message.py` & `solana-0.9.2/solana/message.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/publickey.py` & `solana-0.9.2/solana/publickey.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/rpc/_utils/encoding.py` & `solana-0.9.2/solana/rpc/_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/rpc/api.py` & `solana-0.9.2/solana/rpc/api.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/rpc/commitment.py` & `solana-0.9.2/solana/rpc/commitment.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/rpc/providers/http.py` & `solana-0.9.2/solana/rpc/providers/http.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/rpc/types.py` & `solana-0.9.2/solana/rpc/types.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/system_program.py` & `solana-0.9.2/solana/system_program.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/sysvar.py` & `solana-0.9.2/solana/sysvar.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/transaction.py` & `solana-0.9.2/solana/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             fee_payer = self.signatures[0].pubkey
 
         if not fee_payer:
             raise AttributeError("transaction feePayer required")
 
         account_metas, program_ids = [], set()
         for instr in self.instructions:
-            if not instr.program_id or not instr.keys:
+            if not instr.program_id:
                 raise AttributeError("invalid instruction:", instr)
             account_metas.extend(instr.keys)
             program_ids.add(str(instr.program_id))
 
         # Append programID account metas.
         for pg_id in program_ids:
             account_metas.append(AccountMeta(PublicKey(pg_id), False, False))
```

### Comparing `solana-0.9.1/solana/utils/ed25519_base.py` & `solana-0.9.2/solana/utils/ed25519_base.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/utils/shortvec_encoding.py` & `solana-0.9.2/solana/utils/shortvec_encoding.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana/utils/validate.py` & `solana-0.9.2/solana/utils/validate.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/solana.egg-info/PKG-INFO` & `solana-0.9.2/solana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solana
-Version: 0.9.1
+Version: 0.9.2
 Summary: Solana.py
 Home-page: https://github.com/michaelhly/solanapy
 Author: Michael Huang
 License: MIT
 Description: [![Actions
         Status](https://github.com/michaelhly/solanapy/workflows/CI/badge.svg)](https://github.com/michaelhly/solanapy/actions?query=workflow%3ACI)
         [![PyPI version](https://badge.fury.io/py/solana.svg)](https://badge.fury.io/py/solana)
```

### Comparing `solana-0.9.1/solana.egg-info/SOURCES.txt` & `solana-0.9.2/solana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/spl/token/_layouts.py` & `solana-0.9.2/spl/token/_layouts.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/spl/token/client.py` & `solana-0.9.2/spl/token/client.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/spl/token/constants.py` & `solana-0.9.2/spl/token/constants.py`

 * *Files identical despite different names*

### Comparing `solana-0.9.1/spl/token/instructions.py` & `solana-0.9.2/spl/token/instructions.py`

 * *Files identical despite different names*

