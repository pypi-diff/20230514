# Comparing `tmp/html2notion-0.1.8.tar.gz` & `tmp/html2notion-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2notion-0.1.8.tar", last modified: Wed May 10 11:34:46 2023, max compression
+gzip compressed data, was "html2notion-0.1.9.tar", last modified: Sun May 14 05:53:25 2023, max compression
```

## Comparing `html2notion-0.1.8.tar` & `html2notion-0.1.9.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-10 11:34:46.060612 html2notion-0.1.8/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1064 2023-03-22 08:52:55.000000 html2notion-0.1.8/LICENSE
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-05-10 11:34:46.060863 html2notion-0.1.8/PKG-INFO
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4111 2023-04-23 03:24:11.000000 html2notion-0.1.8/README.md
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-10 11:34:46.039083 html2notion-0.1.8/html2notion/
--rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.8/html2notion/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     6037 2023-05-10 11:12:48.000000 html2notion-0.1.8/html2notion/main.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-10 11:34:46.050989 html2notion-0.1.8/html2notion/translate/
--rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.8/html2notion/translate/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3610 2023-05-10 11:11:53.000000 html2notion-0.1.8/html2notion/translate/batch_import.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2724 2023-04-19 01:44:49.000000 html2notion-0.1.8/html2notion/translate/cos_uploader.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4003 2023-05-10 11:13:13.000000 html2notion-0.1.8/html2notion/translate/html2json.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)    16287 2023-05-10 11:16:12.000000 html2notion-0.1.8/html2notion/translate/html2json_base.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     5812 2023-05-10 11:16:58.000000 html2notion-0.1.8/html2notion/translate/html2json_clipper.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      534 2023-05-10 11:11:53.000000 html2notion-0.1.8/html2notion/translate/html2json_default.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     7744 2023-05-10 11:17:48.000000 html2notion-0.1.8/html2notion/translate/html2json_yinxiang.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2331 2023-05-10 11:11:53.000000 html2notion-0.1.8/html2notion/translate/import_stats.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     7168 2023-04-23 11:21:17.000000 html2notion-0.1.8/html2notion/translate/notion_export.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3894 2023-05-10 11:11:53.000000 html2notion-0.1.8/html2notion/translate/notion_import.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-10 11:34:46.055179 html2notion-0.1.8/html2notion/utils/
--rw-r--r--   0 daemonzhao   (501) staff       (20)      453 2023-05-10 11:11:53.000000 html2notion-0.1.8/html2notion/utils/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      895 2023-05-10 11:11:53.000000 html2notion-0.1.8/html2notion/utils/load_config.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1579 2023-04-20 06:50:27.000000 html2notion-0.1.8/html2notion/utils/log.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      437 2023-04-21 02:46:15.000000 html2notion-0.1.8/html2notion/utils/timeutil.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-10 11:34:46.042275 html2notion-0.1.8/html2notion.egg-info/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-05-10 11:34:45.000000 html2notion-0.1.8/html2notion.egg-info/PKG-INFO
--rw-r--r--   0 daemonzhao   (501) staff       (20)      979 2023-05-10 11:34:45.000000 html2notion-0.1.8/html2notion.egg-info/SOURCES.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)        1 2023-05-10 11:34:45.000000 html2notion-0.1.8/html2notion.egg-info/dependency_links.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)       54 2023-05-10 11:34:45.000000 html2notion-0.1.8/html2notion.egg-info/entry_points.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)      188 2023-05-10 11:34:45.000000 html2notion-0.1.8/html2notion.egg-info/requires.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)       12 2023-05-10 11:34:45.000000 html2notion-0.1.8/html2notion.egg-info/top_level.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)      103 2023-03-20 01:38:35.000000 html2notion-0.1.8/pyproject.toml
--rw-r--r--   0 daemonzhao   (501) staff       (20)      871 2023-05-10 11:34:46.061940 html2notion-0.1.8/setup.cfg
--rw-r--r--   0 daemonzhao   (501) staff       (20)       38 2023-03-17 05:39:04.000000 html2notion-0.1.8/setup.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-10 11:34:46.059513 html2notion-0.1.8/tests/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3940 2023-05-10 11:11:53.000000 html2notion-0.1.8/tests/test_batchimport.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3038 2023-04-20 03:22:52.000000 html2notion-0.1.8/tests/test_cosupload.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2698 2023-04-13 05:01:24.000000 html2notion-0.1.8/tests/test_notionexport.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1801 2023-05-10 11:22:37.000000 html2notion-0.1.8/tests/test_reqlimit.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)    32686 2023-05-10 11:11:53.000000 html2notion-0.1.8/tests/test_yinxiang.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-05-14 05:53:25.051017 html2notion-0.1.9/
+-rw-r--r--   0 feizhao    (501) staff       (20)     1064 2023-03-22 13:58:21.000000 html2notion-0.1.9/LICENSE
+-rw-r--r--   0 feizhao    (501) staff       (20)     4600 2023-05-14 05:53:25.052676 html2notion-0.1.9/PKG-INFO
+-rw-r--r--   0 feizhao    (501) staff       (20)     4111 2023-04-22 07:11:47.000000 html2notion-0.1.9/README.md
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-05-14 05:53:25.001062 html2notion-0.1.9/html2notion/
+-rw-r--r--   0 feizhao    (501) staff       (20)        0 2023-03-18 15:41:01.000000 html2notion-0.1.9/html2notion/__init__.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     6037 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/main.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-05-14 05:53:25.037976 html2notion-0.1.9/html2notion/translate/
+-rw-r--r--   0 feizhao    (501) staff       (20)        0 2023-04-08 10:17:44.000000 html2notion-0.1.9/html2notion/translate/__init__.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     3610 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/batch_import.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     2724 2023-04-19 14:40:39.000000 html2notion-0.1.9/html2notion/translate/cos_uploader.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     4546 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/html2json.py
+-rw-r--r--   0 feizhao    (501) staff       (20)    17995 2023-05-14 05:46:27.000000 html2notion-0.1.9/html2notion/translate/html2json_base.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     5810 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/html2json_clipper.py
+-rw-r--r--   0 feizhao    (501) staff       (20)      534 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/html2json_default.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     8707 2023-05-14 05:22:26.000000 html2notion-0.1.9/html2notion/translate/html2json_markdown.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     7300 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/html2json_yinxiang.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     2331 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/import_stats.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     7168 2023-04-23 14:40:05.000000 html2notion-0.1.9/html2notion/translate/notion_export.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     3594 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/notion_import.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-05-14 05:53:25.042565 html2notion-0.1.9/html2notion/utils/
+-rw-r--r--   0 feizhao    (501) staff       (20)      453 2023-04-29 09:56:35.000000 html2notion-0.1.9/html2notion/utils/__init__.py
+-rw-r--r--   0 feizhao    (501) staff       (20)      895 2023-04-29 09:55:54.000000 html2notion-0.1.9/html2notion/utils/load_config.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     1579 2023-04-20 14:39:58.000000 html2notion-0.1.9/html2notion/utils/log.py
+-rw-r--r--   0 feizhao    (501) staff       (20)      437 2023-04-21 14:23:32.000000 html2notion-0.1.9/html2notion/utils/timeutil.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-05-14 05:53:25.008065 html2notion-0.1.9/html2notion.egg-info/
+-rw-r--r--   0 feizhao    (501) staff       (20)     4600 2023-05-14 05:53:24.000000 html2notion-0.1.9/html2notion.egg-info/PKG-INFO
+-rw-r--r--   0 feizhao    (501) staff       (20)     1023 2023-05-14 05:53:24.000000 html2notion-0.1.9/html2notion.egg-info/SOURCES.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)        1 2023-05-14 05:53:24.000000 html2notion-0.1.9/html2notion.egg-info/dependency_links.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)       54 2023-05-14 05:53:24.000000 html2notion-0.1.9/html2notion.egg-info/entry_points.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)      203 2023-05-14 05:53:24.000000 html2notion-0.1.9/html2notion.egg-info/requires.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)       12 2023-05-14 05:53:24.000000 html2notion-0.1.9/html2notion.egg-info/top_level.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)      103 2023-03-18 15:06:24.000000 html2notion-0.1.9/pyproject.toml
+-rw-r--r--   0 feizhao    (501) staff       (20)      887 2023-05-14 05:53:25.057687 html2notion-0.1.9/setup.cfg
+-rw-r--r--   0 feizhao    (501) staff       (20)       38 2023-03-18 07:34:12.000000 html2notion-0.1.9/setup.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-05-14 05:53:25.048173 html2notion-0.1.9/tests/
+-rw-r--r--   0 feizhao    (501) staff       (20)     3940 2023-04-29 10:35:21.000000 html2notion-0.1.9/tests/test_batchimport.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     3038 2023-04-20 14:39:58.000000 html2notion-0.1.9/tests/test_cosupload.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     2698 2023-04-13 14:42:38.000000 html2notion-0.1.9/tests/test_notionexport.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     1801 2023-05-13 08:31:32.000000 html2notion-0.1.9/tests/test_reqlimit.py
+-rw-r--r--   0 feizhao    (501) staff       (20)    32686 2023-05-13 08:31:32.000000 html2notion-0.1.9/tests/test_yinxiang.py
```

### Comparing `html2notion-0.1.8/LICENSE` & `html2notion-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/PKG-INFO` & `html2notion-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.8
+Version: 0.1.9
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.8/README.md` & `html2notion-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/html2notion/main.py` & `html2notion-0.1.9/html2notion/main.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/html2notion/translate/batch_import.py` & `html2notion-0.1.9/html2notion/translate/batch_import.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/html2notion/translate/cos_uploader.py` & `html2notion-0.1.9/html2notion/translate/cos_uploader.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/html2notion/translate/html2json.py` & `html2notion-0.1.9/html2notion/translate/html2json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,77 @@
-import sys
 import json
+import chardet
+import time
 from functools import singledispatch
 from pathlib import Path
 from bs4 import BeautifulSoup, Tag
 from ..utils import logger, test_prepare_conf
 from ..translate.html2json_base import Html2JsonBase
 from ..translate.html2json_default import Default_Type
 from ..translate.html2json_yinxiang import YinXiang_Type
 from ..translate.html2json_clipper import YinXiangClipper_Type
+from ..translate.html2json_markdown import YinXiangMarkdown_Type
 
 
 """
 <meta name="source" content="yinxiang.superNote"/>
 <meta name="source" content="desktop.mac"/>
 <meta name="source" content="mobile.android"/>
 """
 def _is_yinxiang_export_html(html_soup):
-    exporter_version_meta = html_soup.select_one('html > head > meta[name="exporter-version"]')
     meta_source = html_soup.select_one('html > head > meta[name="source"]')
-    exporter_version_content = exporter_version_meta.get( 'content', "") if isinstance(exporter_version_meta, Tag) else ""
-
     meta_source_content = meta_source.get('content', "") if isinstance(meta_source, Tag) else ""
-    if isinstance(exporter_version_content, str) and not exporter_version_content.startswith("Evernote"):
-        return False
-
     yinxiang_source_content = ["yinxiang", "desktop", "mobile"]
     for prefix in yinxiang_source_content:
         if isinstance(meta_source_content, str) and meta_source_content.startswith(prefix):
             return True
     return False
 
 
 """
 <meta name="source-application" content="webclipper.evernote" />
 <meta name="source-application" content="微信" />
 """
 def _is_yinxiang_clipper_html(html_soup):
-    exporter_version_meta = html_soup.select_one('html > head > meta[name="exporter-version"]')
-    exporter_version_content = exporter_version_meta.get(
-        'content', "") if isinstance(
-        exporter_version_meta, Tag) else ""
-
-    if isinstance(exporter_version_content, str) and not exporter_version_content.startswith("Evernote"):
-        return False
-    clipper_source_meta = html_soup.select_one('html > head > meta[name="source-application"]')
-    clipper_source_content = clipper_source_meta.get('content', "") if isinstance(clipper_source_meta, Tag) else ""
-    if isinstance(clipper_source_content, str) and clipper_source_content.endswith("evernote"):
+    meta_source_application = html_soup.select_one('html > head > meta[name="source-application"]')
+    source_application = meta_source_application.get('content', "") if isinstance(meta_source_application, Tag) else ""
+    if isinstance(source_application, str) and source_application.endswith("evernote"):
         return True
-    if isinstance(clipper_source_content, str) and clipper_source_content in ["微信",]:
+    if isinstance(source_application, str) and source_application in ["微信",]:
+        return True
+    return False
+
+
+"""
+<meta name="content-class" content="yinxiang.markdown" />
+"""
+def _is_yinxiang_markdown_html(html_soup):
+    meta_content_class = html_soup.select_one('html > head > meta[name="content-class"]')
+    content_class = meta_content_class.get('content', "") if isinstance(meta_content_class, Tag) else ""
+    if isinstance(content_class, str) and content_class.endswith("markdown"):
         return True
     return False
 
 
 def _infer_input_type(html_content):
     soup = BeautifulSoup(html_content, 'html.parser')
-    if _is_yinxiang_clipper_html(soup):
-        return YinXiangClipper_Type
-    elif _is_yinxiang_export_html(soup):
-        return YinXiang_Type
+    exporter_version_meta = soup.select_one('html > head > meta[name="exporter-version"]')
+    exporter_version_content = exporter_version_meta.get(
+        'content', "") if isinstance(
+        exporter_version_meta, Tag) else ""
+
+    # yinxiang export
+    if isinstance(exporter_version_content, str) and exporter_version_content.startswith("Evernote"):
+        if _is_yinxiang_markdown_html(soup):
+            return YinXiangMarkdown_Type
+        if _is_yinxiang_clipper_html(soup):
+            return YinXiangClipper_Type
+        elif _is_yinxiang_export_html(soup):
+            return YinXiang_Type
+
     return Default_Type
 
 
 def _get_converter(html_content, import_stat):
     html_type = _infer_input_type(html_content)
     logger.info(f"Input type: {html_type}")
     converter = Html2JsonBase.create(html_type, html_content, import_stat)
@@ -82,16 +92,24 @@
 
 @html2json_process.register
 def _(html_file: Path, import_stat):
     if not html_file.is_file():
         print(f"Load file: {html_file.resolve()} failed")
         raise FileNotFoundError
 
-    with open(html_file, "r") as file:
-        html_content = file.read()
+    html_content = ""
+    with html_file.open('rb') as f:
+        data = f.read()
+        result = chardet.detect(data)
+        encoding = result['encoding'] if result['encoding'] else 'utf-8'
+        html_content = data.decode(encoding)
+
+        if html_content == "main_hold":                  # just for local debug
+            time.sleep(1)
+            return "main_hold"
 
     converter = _get_converter(html_content, import_stat)
     result = converter.process()
     return converter.get_notion_data(), result
 
 
 if __name__ == "__main__":
```

### Comparing `html2notion-0.1.8/html2notion/translate/html2json_base.py` & `html2notion-0.1.9/html2notion/translate/html2json_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,26 +12,38 @@
     NUMBERED_LIST = "numbered_list_item"
     BULLETED_LIST = "bulleted_list_item"
     HEADING = "heading"
     CODE = "code"
     DIVIDER = "divider"
     TABLE = "table"
     TO_DO = "to_do"
+    EQUATION = "equation"
 
 class Html2JsonBase:
     _registry = {}
     _text_annotations = {
         "bold": bool,
         "italic": bool,
         "strikethrough": bool,
         "underline": bool,
         "code": bool,
         "color": str,
     }
 
+    _language = {"abap", "agda", "arduino",
+    "assembly", "bash", "basic", "bnf", "c", "c#", "c++", "clojure", "coffeescript", "coq", "css",
+    "dart", "dhall", "diff", "docker", "ebnf", "elixir", "elm", "erlang", "f#", "flow", "fortran",
+    "gherkin", "glsl", "go", "graphql", "groovy", "haskell", "html", "idris", "java", "javascript",
+    "json", "julia", "kotlin", "latex", "less", "lisp", "livescript", "llvm ir", "lua", "makefile",
+    "markdown", "markup", "matlab", "mathematica", "mermaid", "nix", "objective-c", "ocaml", "pascal",
+    "perl", "php", "plain text", "powershell", "prolog", "protobuf", "purescript", "python", "r",
+    "racket", "reason", "ruby", "rust", "sass", "scala", "scheme", "scss", "shell", "solidity", "sql",
+    "swift", "toml", "typescript", "vb.net", "verilog", "vhdl", "visual basic", "webassembly", "xml",
+    "yaml", "java/c/c++/c#"}
+    
     _color_tuple = namedtuple("Color", "name r g b")
     _notion_color = [
         _color_tuple("default", 0, 0, 0),
         _color_tuple("gray", 128, 128, 128),
         _color_tuple("brown", 165, 42, 42),
         _color_tuple("orange", 255, 165, 0),
         _color_tuple("yellow", 255, 255, 0),
@@ -88,19 +100,15 @@
                 else:
                     results.extend(Html2JsonBase.extract_text_and_parents(child, parents + [tag]))
         return results
 
     @staticmethod
     def parse_one_style(tag_soup: Tag, text_params: dict):
         tag_name = tag_soup.name.lower()
-        style = tag_soup.get('style', "")
-        styles = {}
-        if str and isinstance(style, str):
-            styles = {rule.split(':')[0].strip(): rule.split(':')[1].strip() for rule in style.split(';') if rule}
-
+        styles = Html2JsonBase.get_tag_style(tag_soup)
         if Html2JsonBase.is_bold(tag_name, styles):
             text_params["bold"] = True
         if Html2JsonBase.is_italic(tag_name, styles):
             text_params["italic"] = True
         if Html2JsonBase.is_strikethrough(tag_name, styles):
             text_params["strikethrough"] = True
         if Html2JsonBase.is_underline(tag_name, styles):
@@ -148,15 +156,14 @@
                 else:
                     text_obj = self.generate_text(**text_params)
                 if text_obj:
                     res_obj.append(text_obj)
         return res_obj
 
 
-    
     def generate_link(self, **kwargs):
         plain_text = kwargs.get("plain_text", "")
         if not plain_text:
             return
         
         self.import_stat.add_notion_text(plain_text)
         return {
@@ -413,31 +420,33 @@
             rich_text.extend(text_obj)
 
         return json_obj
 
     """
     <div>
     <div><br /></div>
-    <table> <tbody> <tr> <td> </td> </tr> </tbody>
+    <table> <thead> </thead><tbody> <tr> <td> </td> </tr> </tbody> </table>
     <div><br /></div>
     </div>
     """
     # ../examples/insert_table.ipynb
     def convert_table(self, soup):
         table_rows = []
         tr_tags = soup.find_all('tr')
         if not tr_tags:
             logger.error(f"No tr found in {soup}")
             return
         
         table_width = len(tr_tags[0].find_all('td'))
+        has_header = False
         for tr in tr_tags:
             td_tags = tr.find_all('td')
             if not td_tags:
-                continue
+                td_tags = tr.find_all('th')
+                has_header = True
             table_width = max(table_width, len(td_tags))
             one_row = {
                 "type": "table_row",
                 "table_row": {
                     "cells": []
                 }
             }
@@ -445,21 +454,44 @@
                 col = self.generate_inline_obj(td)
                 one_row["table_row"]["cells"].append(col)
             table_rows.append(one_row)
 
         table_obj = {
             "table": {
                 "has_row_header": False,
-                "has_column_header": False,
+                "has_column_header": has_header,
                 "table_width": table_width,
                 "children": table_rows,
             }
         }
         return table_obj
 
+    # Only if there is no ";" in the value of the attribute, you can use this method to get all attributes.
+    # Can't use this way like: background-image: url('data:image/png;base64...') 
+    @staticmethod
+    def get_tag_style(tag_soup):
+        styles = {}
+        if not isinstance(tag_soup, Tag):
+            return styles
+        style = tag_soup.get('style', "")
+        if str and isinstance(style, str):
+            # style = ''.join(style.split())
+            styles = {
+                rule.split(':')[0].strip(): rule.split(':')[1].strip().lower()
+                for rule in style.split(';')
+                if rule and len(rule.split(':')) > 1
+            }
+        return styles
+
+    @staticmethod
+    def get_valid_language(language):
+        if language in Html2JsonBase._language:
+            return language
+        return "plain text"
+    
     @classmethod
     def register(cls, input_type, subclass):
         cls._registry[input_type] = subclass
 
     @classmethod
     def create(cls, input_type, html_content, import_stat):
         subclass = cls._registry.get(input_type)
```

### Comparing `html2notion-0.1.8/html2notion/translate/html2json_clipper.py` & `html2notion-0.1.9/html2notion/translate/html2json_clipper.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ..utils import logger
 from ..translate.html2json_base import Html2JsonBase, Block
 from ..utils.timeutil import DateStrToISO8601
 
 YinXiangClipper_Type = "clipper.yinxiang"
 
 
-class Html2JsonYinXiang(Html2JsonBase):
+class Html2JsonClipper(Html2JsonBase):
     input_type = YinXiangClipper_Type
 
     def __init__(self, html_content, import_stat):
         super().__init__(html_content, import_stat)
 
     def process(self):
         soup = BeautifulSoup(self.html_content, 'html.parser')
@@ -154,8 +154,8 @@
         #     style_attrs = element.attrs['style'].lower()
         #     if 'border:' in style_attrs or 'padding:' in style_attrs:
         #         return True
 
         return False
 
     
-Html2JsonBase.register(YinXiangClipper_Type, Html2JsonYinXiang)
+Html2JsonBase.register(YinXiangClipper_Type, Html2JsonClipper)
```

### Comparing `html2notion-0.1.8/html2notion/translate/html2json_default.py` & `html2notion-0.1.9/html2notion/translate/html2json_default.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/html2notion/translate/html2json_yinxiang.py` & `html2notion-0.1.9/html2notion/translate/html2json_yinxiang.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,22 +75,17 @@
             is_last_child = index == len(children_list) - 1
             text_obj = self.generate_inline_obj(child)
             if text_obj:
                 rich_text.extend(text_obj)
             if not is_last_child:
                 rich_text.append(self.generate_text(plain_text='\n', stats_count=False))
         json_obj["code"]["rich_text"] = self.merge_rich_text(rich_text)
-
-        style = soup.get('style', "") if soup.name else ""
-        css_dict = {}
-        if isinstance(style, str):
-            style = ''.join(style.split())
-            css_dict = {rule.split(':')[0].strip(): rule.split(':')[1].strip() for rule in style.split(';') if rule}
-            language = css_dict.get('--en-codeblockLanguage', 'plain text')
-            json_obj["code"]["language"] = language
+        css_dict = Html2JsonBase.get_tag_style(soup)
+        language = css_dict.get('--en-codeblockLanguage', 'plain text')
+        json_obj["code"]["language"] = language
         
         return json_obj
 
     def convert_quote(self, soup):
         json_obj = {
             "object": "block",
             "type": "quote",
@@ -154,21 +149,16 @@
             return Block.BULLETED_LIST.value
         elif tag_name == 'p':
             return Block.PARAGRAPH.value
         elif tag_name in ('h1', 'h2', 'h3', 'h4', 'h5', 'h6'):
             return Block.HEADING.value
         elif tag_name == 'table' or self._check_is_table(single_tag):
             return Block.TABLE.value
-
-        css_dict = {}
-        if style:
-            # Remove all space such as \t \n in style
-            style = ''.join(style.split())
-            css_dict = {rule.split(':')[0].strip(): rule.split(
-                ':')[1].strip().lower() for rule in style.split(';') if rule}
+        
+        css_dict = Html2JsonBase.get_tag_style(single_tag)
         if css_dict.get('--en-blockquote', None) == 'true':
             return Block.QUOTE.value
         if css_dict.get('--en-codeblock', None) == 'true':
             return Block.CODE.value
         if css_dict.get('-en-codeblock', None) == 'true':
             return Block.CODE.value
```

### Comparing `html2notion-0.1.8/html2notion/translate/import_stats.py` & `html2notion-0.1.9/html2notion/translate/import_stats.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/html2notion/translate/notion_export.py` & `html2notion-0.1.9/html2notion/translate/notion_export.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/html2notion/translate/notion_import.py` & `html2notion-0.1.9/html2notion/translate/notion_import.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import os
+import traceback
 from aiohttp import ClientSession
 from pathlib import Path
 from notion_client import AsyncClient
 from notion_client.errors import RequestTimeoutError
 from tenacity import retry, stop_after_attempt, wait_exponential, retry_if_exception_type
 from ..utils import logger, test_prepare_conf, config, rate_limit
 from ..translate.html2json import html2json_process
@@ -14,41 +15,29 @@
     def __init__(self, session: ClientSession, notion_client):
         self.session = session
         self.notion_client = notion_client
         self.import_stats = ImportStats()
 
     async def process_file(self, file_path: Path):
         self.import_stats.set_filename(file_path)
-
-        if not file_path.is_file():
-            self.import_stats.set_exception(Exception(f"{file_path} is not file"))
-            logger.error(f"{file_path} is not a file.")
-            return "fail"
-
-        with file_path.open() as f:
-            content = f.read()
-
-        logger.info(f"Process file {file_path}")
-        if content == "main_hold":                  # local debug
-            await asyncio.sleep(1)
-            return "main_hold"
-
         try:
             notion_data, html_type = html2json_process(file_path, self.import_stats)
         except Exception as e:
+            error_message = traceback.format_exc()
             self.import_stats.set_exception(e)
-            logger.error(f"Error processing {file_path}: {str(e)}")
+            logger.error(f"Error processing {file_path}: {str(e)}, {error_message}")
             return "fail"
 
         logger.info(f"Process path: {file_path}, html type: {html_type}, {self.import_stats.get_detail()}")
         try:
             create_result = await self.create_new_page(notion_data)
         except Exception as e:
+            error_message = traceback.format_exc()
             self.import_stats.set_exception(e)
-            logger.error(f"Error create notion page {file_path}: {str(e)}")
+            logger.error(f"Error create notion page {file_path}: {str(e)}, {error_message}")
             return "fail"
         logger.info(f"Create notion page: {create_result}")
         return "succ"
 
     # https://developers.notion.com/reference/request-limits
     # The rate limit for incoming requests per integration is an average of three requests per second. 
     # Doc of create page: https://developers.notion.com/reference/post-page
```

### Comparing `html2notion-0.1.8/html2notion/utils/load_config.py` & `html2notion-0.1.9/html2notion/utils/load_config.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/html2notion/utils/log.py` & `html2notion-0.1.9/html2notion/utils/log.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/html2notion.egg-info/PKG-INFO` & `html2notion-0.1.9/html2notion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.8
+Version: 0.1.9
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.8/html2notion.egg-info/SOURCES.txt` & `html2notion-0.1.9/html2notion.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 html2notion/translate/__init__.py
 html2notion/translate/batch_import.py
 html2notion/translate/cos_uploader.py
 html2notion/translate/html2json.py
 html2notion/translate/html2json_base.py
 html2notion/translate/html2json_clipper.py
 html2notion/translate/html2json_default.py
+html2notion/translate/html2json_markdown.py
 html2notion/translate/html2json_yinxiang.py
 html2notion/translate/import_stats.py
 html2notion/translate/notion_export.py
 html2notion/translate/notion_import.py
 html2notion/utils/__init__.py
 html2notion/utils/load_config.py
 html2notion/utils/log.py
```

### Comparing `html2notion-0.1.8/setup.cfg` & `html2notion-0.1.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = html2notion
-version = 0.1.8
+version = 0.1.9
 author = selfboot
 author_email = xuezaigds@gmail.com
 description = This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/selfboot/html2notion
 license_files = LICENSE
@@ -19,18 +19,19 @@
 	beautifulsoup4>=4.11.2
 	httpcore>=0.16.3
 	httpx>=0.23.3
 	notion-client>=2.0.0
 	PyYAML>=6.0
 	aiohttp>=3.8.4
 	anyio>=3.6.2
-	rich>=13.3.4
 	cos-python-sdk-v5>=1.9.23
 	tenacity>=8.2.2
+	rich>=13.3.4
 	aiolimiter>=1.0.0
+	chardet>=5.1.0
 
 [options.entry_points]
 console_scripts = 
 	html2notion = html2notion.main:main
 
 [egg_info]
 tag_build =
```

### Comparing `html2notion-0.1.8/tests/test_batchimport.py` & `html2notion-0.1.9/tests/test_batchimport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/tests/test_cosupload.py` & `html2notion-0.1.9/tests/test_cosupload.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/tests/test_notionexport.py` & `html2notion-0.1.9/tests/test_notionexport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/tests/test_reqlimit.py` & `html2notion-0.1.9/tests/test_reqlimit.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.8/tests/test_yinxiang.py` & `html2notion-0.1.9/tests/test_yinxiang.py`

 * *Files identical despite different names*

