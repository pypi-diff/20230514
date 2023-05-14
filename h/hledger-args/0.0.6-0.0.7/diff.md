# Comparing `tmp/hledger_args-0.0.6.tar.gz` & `tmp/hledger_args-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_args-0.0.6.tar", last modified: Sat May 13 15:27:11 2023, max compression
+gzip compressed data, was "hledger_args-0.0.7.tar", last modified: Sun May 14 02:16:08 2023, max compression
```

## Comparing `hledger_args-0.0.6.tar` & `hledger_args-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-13 15:27:11.354608 hledger_args-0.0.6/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4504 2023-05-13 15:27:11.354608 hledger_args-0.0.6/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4164 2023-05-11 02:06:47.000000 hledger_args-0.0.6/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-13 15:27:11.348608 hledger_args-0.0.6/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4164 2023-05-11 02:06:47.000000 hledger_args-0.0.6/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-13 15:27:11.350607 hledger_args-0.0.6/hledger_args/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:28.000000 hledger_args-0.0.6/hledger_args/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       84 2023-05-09 19:53:32.000000 hledger_args-0.0.6/hledger_args/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1288 2023-05-11 14:44:16.000000 hledger_args-0.0.6/hledger_args/base_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1396 2023-05-13 15:06:47.000000 hledger_args-0.0.6/hledger_args/batch_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3512 2023-05-13 15:27:04.000000 hledger_args-0.0.6/hledger_args/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4819 2023-05-13 15:05:41.000000 hledger_args-0.0.6/hledger_args/inter_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-09 16:55:37.000000 hledger_args-0.0.6/hledger_args/options.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1203 2023-05-13 15:16:12.000000 hledger_args-0.0.6/hledger_args/output_result.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-13 15:27:11.351608 hledger_args-0.0.6/hledger_args.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4504 2023-05-13 15:27:11.000000 hledger_args-0.0.6/hledger_args.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      748 2023-05-13 15:27:11.000000 hledger_args-0.0.6/hledger_args.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-13 15:27:11.000000 hledger_args-0.0.6/hledger_args.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-13 15:27:11.000000 hledger_args-0.0.6/hledger_args.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       29 2023-05-13 15:27:11.000000 hledger_args-0.0.6/hledger_args.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-05-13 15:27:11.000000 hledger_args-0.0.6/hledger_args.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1152 2023-05-13 15:26:02.000000 hledger_args-0.0.6/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-13 15:27:11.354608 hledger_args-0.0.6/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-13 15:27:11.351608 hledger_args-0.0.6/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:22.000000 hledger_args-0.0.6/tests/__init__.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-13 15:27:11.347607 hledger_args-0.0.6/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-13 15:27:11.353608 hledger_args-0.0.6/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-05-09 16:48:40.000000 hledger_args-0.0.6/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-05-09 16:48:40.000000 hledger_args-0.0.6/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-05-09 16:48:40.000000 hledger_args-0.0.6/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-05-09 16:48:40.000000 hledger_args-0.0.6/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-05-09 16:48:40.000000 hledger_args-0.0.6/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-05-09 16:48:40.000000 hledger_args-0.0.6/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-05-09 16:48:40.000000 hledger_args-0.0.6/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-05-09 16:48:40.000000 hledger_args-0.0.6/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-05-09 16:48:40.000000 hledger_args-0.0.6/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-05-09 16:48:40.000000 hledger_args-0.0.6/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-05-09 16:48:40.000000 hledger_args-0.0.6/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-05-09 16:48:40.000000 hledger_args-0.0.6/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.089698 hledger_args-0.0.7/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9493 2023-05-14 02:16:08.089698 hledger_args-0.0.7/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9153 2023-05-14 02:13:20.000000 hledger_args-0.0.7/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.081698 hledger_args-0.0.7/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9153 2023-05-14 02:13:20.000000 hledger_args-0.0.7/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.083698 hledger_args-0.0.7/hledger_args/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:28.000000 hledger_args-0.0.7/hledger_args/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       84 2023-05-09 19:53:32.000000 hledger_args-0.0.7/hledger_args/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1288 2023-05-11 14:44:16.000000 hledger_args-0.0.7/hledger_args/base_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1968 2023-05-14 02:09:23.000000 hledger_args-0.0.7/hledger_args/batch_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3766 2023-05-14 02:09:23.000000 hledger_args-0.0.7/hledger_args/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4819 2023-05-13 15:05:41.000000 hledger_args-0.0.7/hledger_args/inter_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-09 16:55:37.000000 hledger_args-0.0.7/hledger_args/options.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1173 2023-05-14 02:09:10.000000 hledger_args-0.0.7/hledger_args/output_result.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.084698 hledger_args-0.0.7/hledger_args.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9493 2023-05-14 02:16:08.000000 hledger_args-0.0.7/hledger_args.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      748 2023-05-14 02:16:08.000000 hledger_args-0.0.7/hledger_args.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-14 02:16:08.000000 hledger_args-0.0.7/hledger_args.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-14 02:16:08.000000 hledger_args-0.0.7/hledger_args.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       29 2023-05-14 02:16:08.000000 hledger_args-0.0.7/hledger_args.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-05-14 02:16:08.000000 hledger_args-0.0.7/hledger_args.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1152 2023-05-14 02:14:48.000000 hledger_args-0.0.7/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-14 02:16:08.089698 hledger_args-0.0.7/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.084698 hledger_args-0.0.7/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:22.000000 hledger_args-0.0.7/tests/__init__.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.081698 hledger_args-0.0.7/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.089698 hledger_args-0.0.7/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rstpep2html.py
```

### Comparing `hledger_args-0.0.6/hledger_args/base_args.py` & `hledger_args-0.0.7/hledger_args/base_args.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/hledger_args/cli.py` & `hledger_args-0.0.7/hledger_args/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,17 +44,22 @@
     "-d",
     "--pdf-dir",
     type=click.Path(
         file_okay=False,
         dir_okay=True,
     ),
     required=False,
+    help="Save the report to a folder named according to the current date under the specified directory",
 )
 @click.option(
-    "-o", "--pdf-file", type=click.Path(file_okay=True, dir_okay=False), required=False
+    "-o",
+    "--pdf-file",
+    type=click.Path(file_okay=True, dir_okay=False),
+    required=False,
+    help="output the report to the specified file in pdf",
 )
 @click.argument("name", type=click.STRING, required=False)
 @click.argument("extra_hledger_options", nargs=-1)
 def cli(
     file: str,
     interactive: bool,
     name: str,
@@ -63,15 +68,15 @@
     pdf_file: Optional[str],
 ):
     """
      ---
 
      **NAME**: Command name to run saved in the journal sub directives. Not available in Interactive mode
 
-    **EXTRA_HLEDGER_OPTIONS**: Extra options to send to hledger command. Not available in Interactive mode.
+    **EXTRA_HLEDGER_OPTIONS**: Extra options to send to hledger command. Not available in Interactive mode. The name **"all"** is special and output all the *no interactive* commands.
 
      ---
 
      In basic usage, this package is a replacement for [hledger argument file](https://hledger.org/1.29/hledger.html#command-arguments) using custom directives inside the journal file, instead of referencing to an argument file
 
      **Interactive Mode**: Instead of giving the desired command thru a command-line argument, choose it by selecting from a menu using the flag *--interactive*
```

### Comparing `hledger_args-0.0.6/hledger_args/inter_args.py` & `hledger_args-0.0.7/hledger_args/inter_args.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/hledger_args/options.py` & `hledger_args-0.0.7/hledger_args/options.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/hledger_args/output_result.py` & `hledger_args-0.0.7/hledger_args/output_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from typing import Optional, Union
 
 from fpdf import FPDF
 
 from .batch_args import BatchArgs
 from .inter_args import InteractiveArgs
 
-# TODO: name for interactive
-
 
 def create_pdf(header: str, text: str, output_path: Path):
     pdf = FPDF()
     pdf.add_page(orientation="L")
     pdf.set_font("Courier", "", 12)
 
     pdf.multi_cell(0, None, header, ln=True)
```

### Comparing `hledger_args-0.0.6/hledger_args.egg-info/SOURCES.txt` & `hledger_args-0.0.7/hledger_args.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/pyproject.toml` & `hledger_args-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 keyword = ["hledger","PTA", "investments", "accounting"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_args"
-version = "0.0.6"
+version = "0.0.7"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
 	     "questionary"
```

### Comparing `hledger_args-0.0.6/venv/bin/rst2html.py` & `hledger_args-0.0.7/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/venv/bin/rst2html4.py` & `hledger_args-0.0.7/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/venv/bin/rst2html5.py` & `hledger_args-0.0.7/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/venv/bin/rst2latex.py` & `hledger_args-0.0.7/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/venv/bin/rst2man.py` & `hledger_args-0.0.7/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/venv/bin/rst2odt.py` & `hledger_args-0.0.7/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/venv/bin/rst2odt_prepstyles.py` & `hledger_args-0.0.7/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/venv/bin/rst2pseudoxml.py` & `hledger_args-0.0.7/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/venv/bin/rst2s5.py` & `hledger_args-0.0.7/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/venv/bin/rst2xetex.py` & `hledger_args-0.0.7/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/venv/bin/rst2xml.py` & `hledger_args-0.0.7/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.6/venv/bin/rstpep2html.py` & `hledger_args-0.0.7/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

