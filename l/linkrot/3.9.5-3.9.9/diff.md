# Comparing `tmp/linkrot-3.9.5.tar.gz` & `tmp/linkrot-3.9.9.tar.gz`

## Comparing `linkrot-3.9.5.tar` & `linkrot-3.9.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 linkrot-3.9.5/linkrot/__init__.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 linkrot-3.9.5/linkrot/archive.py
--rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 linkrot-3.9.5/linkrot/backends.py
--rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 linkrot-3.9.5/linkrot/cli.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 linkrot-3.9.5/linkrot/colorprint.py
--rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 linkrot-3.9.5/linkrot/downloader.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 linkrot-3.9.5/linkrot/exceptions.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 linkrot-3.9.5/linkrot/extractor.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 linkrot-3.9.5/linkrot/threadpool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linkrot-3.9.5/linkrot/libs/__init__.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 linkrot-3.9.5/linkrot/libs/xmp.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 linkrot-3.9.5/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 linkrot-3.9.5/LICENSE
--rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 linkrot-3.9.5/README.md
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 linkrot-3.9.5/pyproject.toml
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 linkrot-3.9.5/PKG-INFO
+-rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 linkrot-3.9.9/linkrot/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 linkrot-3.9.9/linkrot/archive.py
+-rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 linkrot-3.9.9/linkrot/backends.py
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 linkrot-3.9.9/linkrot/cli.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 linkrot-3.9.9/linkrot/colorprint.py
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 linkrot-3.9.9/linkrot/downloader.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 linkrot-3.9.9/linkrot/exceptions.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 linkrot-3.9.9/linkrot/extractor.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 linkrot-3.9.9/linkrot/threadpool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linkrot-3.9.9/linkrot/libs/__init__.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 linkrot-3.9.9/linkrot/libs/xmp.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 linkrot-3.9.9/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 linkrot-3.9.9/LICENSE
+-rw-r--r--   0        0        0     7641 2020-02-02 00:00:00.000000 linkrot-3.9.9/README.md
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 linkrot-3.9.9/pyproject.toml
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 linkrot-3.9.9/PKG-INFO
```

### Comparing `linkrot-3.9.5/linkrot/__init__.py` & `linkrot-3.9.9/linkrot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,27 @@
 >>> import linkrot
 >>> pdf = linkrot.linkrot("filename-or-url.pdf")
 >>> metadata = pdf.get_metadata()
 >>> references_list = pdf.get_references()
 >>> references_dict = pdf.get_references_as_dict()
 >>> pdf.download_pdfs("target-directory")
 
-https://github.com/marshalmiller/linkrot
+https://github.com/rottingresearch/linkrot
 
-Copyright (c) 2021, Marshal Miller <marshal@marshalmiller.com>
-License: GPLv3
+Copyright (c) 2023, Marshal Miller <marshal@rottingresearch.org>
+License: MIT (see LICENSE for details)
 """
 
 __title__ = "linkrot"
-__version__ = "3.9.5"
+__version__ = "3.9.9"
 __author__ = "Marshal Miller"
 __license__ = "MIT"
-__copyright__ = "Copyright 2022 Marshal Miller"
+__copyright__ = "Copyright 2023, Marshal Miller"
 
 import os
-import sys
 import json
 import shutil
 import logging
 
 
 from .extractor import extract_urls
 from .backends import PDFMinerBackend, TextBackend
```

### Comparing `linkrot-3.9.5/linkrot/archive.py` & `linkrot-3.9.9/linkrot/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # Adds links to Wayback Machine from the Internet Archive
-import time
-from .threadpool import ThreadPool
-import re
 import requests
+from .threadpool import ThreadPool
 
 
 def archive_links(refs):
     """archive  urls """
 
     def web_archive(ref):
         url = ref.ref
         if 'web.archive' in url:
             return url, url
         try:
-            headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 6.2; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.100 Safari/537.36'}
+            headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 6.2; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/75.0.3770.100 Safari/537.36'}  # noqa: E501
             r = requests.get('https://web.archive.org/save/' +
                              url,  headers=headers)
             if r.status_code == 200:
                 result = r.headers['Content-Location']
                 internet_archive_url = "https://web.archive.org%s" % result
                 return internet_archive_url
             else:
```

### Comparing `linkrot-3.9.5/linkrot/backends.py` & `linkrot-3.9.9/linkrot/backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 PDF Backend: pdfMiner
 """
 
-import sys
 import logging
 from io import BytesIO
 from re import compile
 
 # Character Detection Helper
 import chardet
 
@@ -48,15 +47,15 @@
 
     # Detect the encoding now
     enc = chardet.detect(in_str)
 
     # Decode the object into a string object
     try:
         out_str = in_str.decode(enc["encoding"])
-    except UnicodeDecodeError as err:
+    except UnicodeDecodeError as err:  # noqa: F841
         out_str = ""
 
     # Cleanup
     if enc["encoding"] == "UTF-16BE":
         # Remove byte order marks (BOM)
         if out_str.startswith("\\ufeff"):
             out_str = out_str[1:]
```

### Comparing `linkrot-3.9.5/linkrot/cli.py` & `linkrot-3.9.9/linkrot/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     parser.add_argument(
         "-t",
         "--text",
         action="store_true",
         help="Only extract text (no metadata or references)",
     )
-    
+
     parser.add_argument(
         "-a",
         "--archive",
         action="store_true",
         help="Archive active links",
     )
 
@@ -120,16 +120,16 @@
     """ Normal output of infos of linkrot instance """
     # Metadata
     ret = ""
     ret += "Document info:\n"
     metadata = pdf.get_metadata()
     metadata.pop(None, None)
     for k, v in sorted(pdf.get_metadata().items()):
-         if v:
-             ret += "- {} = {}\n".format(k, str(v).strip("/"))
+        if v:
+            ret += "- {} = {}\n".format(k, str(v).strip("/"))
 
     # References
     ref_cnt = pdf.get_references_count()
     ret += "\nReferences: %s\n" % ref_cnt
     refs = pdf.get_references_as_dict()
     for k in refs:
         ret += "- {}: {}\n".format(k.upper(), len(refs[k]))
@@ -232,16 +232,16 @@
 
     # Checking for broken links
     if args.check_links:
         refs_all = pdf.get_references()
         refs = [ref for ref in refs_all if ref.reftype in ["url", "pdf"]]
         print("\nChecking %s URLs for broken links..." % len(refs))
         check_refs(refs)
-    
-    # Archive active links 
+
+    # Archive active links
     if args.archive:
         refs_all = pdf.get_references()
         refs = [ref for ref in refs_all if ref.reftype in ["url"]]
         print("\nArchieve %s URLs..." % len(refs))
         archive_links(refs)
 
     # Check for errors in downloading and then produce the output
```

### Comparing `linkrot-3.9.5/linkrot/colorprint.py` & `linkrot-3.9.9/linkrot/colorprint.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 UNDERLINE = "\033[4m"
 BLINK = "\033[5m"
 REVERSE = "\033[7m"
 
 # Nothing (Standard)
 ENDC = "\033[0m"
 
+
 def colorprint(color, s):
     '''Formates the string 's' with the ANSI octal escape sequence(s) 'color'
        and then makes sure that all the following print statements are of the of standard formatting.
 
     Args:
         color: ANSI octal escape sequence(s) to be used for formatting.
         s: The string to be formatted.
 
     Returns:
         None  
 
-    '''
+    '''  # noqa: E501
     output = "{}{}{}".format(color, s, ENDC)
     print(output)
     return output
```

### Comparing `linkrot-3.9.5/linkrot/downloader.py` & `linkrot-3.9.9/linkrot/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # importing modules
 from .colorprint import colorprint, OKGREEN, FAIL
 from .threadpool import ThreadPool
 from collections import defaultdict
 import ssl
 import os
-import sys
 import re
 
 
 from urllib.request import Request, urlopen, HTTPError, URLError
 
 unicode = str
 
@@ -79,18 +78,18 @@
     except KeyboardInterrupt:
         pass
 
     # Print summary
     output = "\nSummary of link checker:" 
     print(output)
     if "200" in codes:
-        output +="\n" +colorprint(OKGREEN, "%s working" % len(codes["200"]))
+        output += "\n" + colorprint(OKGREEN, "%s working" % len(codes["200"]))
     for c in sorted(codes):
         if c != "200":
-            output +="\n" + colorprint(FAIL, "{} broken (reason: {})".format(len(codes[c]), c))
+            output += "\n" + colorprint(FAIL, "{} broken (reason: {})".format(len(codes[c]), c))  # noqa: E501
             for ref in codes[c]:                
                 o = "  - %s" % ref.ref
                 if ref.page > 0:
                     o += " (page %s)" % ref.page
                 print(o)
                 output += "\n" + o
```

### Comparing `linkrot-3.9.5/linkrot/extractor.py` & `linkrot-3.9.9/linkrot/extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,24 +41,26 @@
 kh|ki|km|kn|kp|kr|kw|ky|kz|la|lb|lc|li|lk|lr|ls|lt|lu|lv|ly|ma|mc|md|me|mg|mh|\
 mk|ml|mm|mn|mo|mp|mq|mr|ms|mt|mu|mv|mw|mx|my|mz|na|nc|ne|nf|ng|ni|nl|no|np|nr|\
 nu|nz|om|pa|pe|pf|pg|ph|pk|pl|pm|pn|pr|ps|pt|pw|py|qa|re|ro|rs|ru|rw|sa|sb|sc|\
 sd|se|sg|sh|si|sj|Ja|sk|sl|sm|sn|so|sr|ss|st|su|sv|sx|sy|sz|tc|td|tf|tg|th|tj|\
 tk|tl|tm|tn|to|tp|tr|tt|tv|tw|tz|ua|ug|uk|us|uy|uz|va|vc|ve|vg|vi|vn|vu|wf|ws|\
 ye|yt|yu|za|zm|zw)\b/?(?!@)))"""
 
+
 def extract_urls(text):
     """
     This function will return all the unique URLs found in the `text` argument.
 
     - First we use the regex to find all matches for URLs
     - Finally we turn the list into a set, so we only end up with unique URLs\
      (no duplicates)
     """
     return set(re.findall(URL_REGEX, text, re.MULTILINE))
 
+
 def extract_arxiv(text):
     """
     This function will return all the unique occurences of `arvix.org/abs/` or\
      `arvix:`.
 
     - First we find all matches of the form `arvix:`
     - Then we find all matches of the form `arvic.org/abs/`
```

### Comparing `linkrot-3.9.5/linkrot/threadpool.py` & `linkrot-3.9.9/linkrot/threadpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Inspired by http://stackoverflow.com/a/7257510
 """
 
 from threading import Thread
-import sys
 
 from queue import Queue
 
 
 class Worker(Thread):
     """ Thread executing tasks from a given tasks queue """
```

### Comparing `linkrot-3.9.5/linkrot/libs/xmp.py` & `linkrot-3.9.9/linkrot/libs/xmp.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         Usage:
 
             parser = XmpParser(xmpstring)
             meta = parser.meta
     """
 
     def __init__(self, xmp):
-        self.tree = ET.XML(xmp, parser=etree.XMLParser(recover=True,encoding='utf-8'))
+        self.tree = ET.XML(xmp, parser=etree.XMLParser(recover=True, encoding='utf-8'))
         self.rdftree = self.tree.find(RDF_NS + "RDF")
 
     @property
     def meta(self):
         """ A dictionary of all the parsed metadata. """
         meta = defaultdict(dict)
         if self.rdftree is not None:
```

### Comparing `linkrot-3.9.5/.gitignore` & `linkrot-3.9.9/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -101,7 +101,9 @@
 /site
 
 # mypy
 .mypy_cache/
 
 # IDE settings
 .vscode/
+.DS_Store
+*.vsidx
```

### Comparing `linkrot-3.9.5/LICENSE` & `linkrot-3.9.9/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Marshal A. Miller
+Copyright (c) 2023 Marshal A. Miller
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `linkrot-3.9.5/README.md` & `linkrot-3.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 Check out our sister project, [Rotting Research](https://github.com/marshalmiller/rottingresearch), for a web app implementation of this project.
 
 # Features
 
 - Extract references and metadata from a given PDF.  
 - Detects pdf, url, arxiv and doi references.
-- Archives valid links using Internet Archive's Wayback Machine.
+- Archives valid links using Internet Archive's Wayback Machine (using the -a flag).
 - Checks for valid SSL certificate.  
 - Find broken hyperlinks (using the -c flag).  
 - Output as text or JSON (using the -j flag).  
 - Extract the PDF text (using the --text flag).  
 - Use as command-line tool or Python package.  
 - Works with local and online pdfs.
```

### Comparing `linkrot-3.9.5/pyproject.toml` & `linkrot-3.9.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,70 +4,70 @@
 
 [project]
 name = "linkrot"
 dynamic = ["version"]
 description = "Extract metadata and URLs from PDF files"
 readme = "README.md"
 license = "MIT"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
-    { name = "Marshal Miller", email = "marshal@marshalmiller.com" },
+    { name = "Marshal Miller", email = "marshal@rottingresearch.org" },
 ]
 keywords = [
     "pdf",
     "reference",
     "linkrot",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
 dependencies = [
-    "pdfminer.six==20220524",
-    "chardet==5.0.0",
-    "lxml==4.9.1",
+    "pdfminer.six==20221105",
+    "chardet==5.1.0",
+    "lxml==4.9.2",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "black==22.8.0",
-    "coverage==6.5.0",
-    "flake8==5.0.4",
+    "black==23.3.0",
+    "coverage==7.2.5",
+    "flake8==6.0.0",
     "mccabe<=0.7.0",
-    "mypy==0.981",
-    "pylint==2.15.3",
-    "pytest==7.1.3",
-    "build==0.8.0",
+    "mypy==1.3.0",
+    "pylint==2.17.4",
+    "pytest==7.3.1",
+    "build==0.10.0",
     "mega.py==1.0.8",
 ]
 test = [
-    "pytest==7.1.3",
+    "pytest==7.3.1",
     "mega.py==1.0.8",
 ]
 
 [project.urls]
-Homepage = "https://github.com/marshalmiller/linkrot"
+Homepage = "https://github.com/rottingresearch/linkrot"
 
 [tool.hatch.version]
 path = "linkrot/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/linkrot",
 ]
 
 [tool.hatch.build.targets.wheel]
-include = [
+packages = [
     "/linkrot",
 ]
 
 [project.scripts]
 linkrot= "linkrot.cli:main"
```

### Comparing `linkrot-3.9.5/PKG-INFO` & `linkrot-3.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 Metadata-Version: 2.1
 Name: linkrot
-Version: 3.9.5
+Version: 3.9.9
 Summary: Extract metadata and URLs from PDF files
-Project-URL: Homepage, https://github.com/marshalmiller/linkrot
-Author-email: Marshal Miller <marshal@marshalmiller.com>
+Project-URL: Homepage, https://github.com/rottingresearch/linkrot
+Author-email: Marshal Miller <marshal@rottingresearch.org>
+License-Expression: MIT
 License-File: LICENSE
 Keywords: linkrot,pdf,reference
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Requires-Dist: chardet==5.0.0
-Requires-Dist: lxml==4.9.1
-Requires-Dist: pdfminer-six==20220524
+Requires-Python: >=3.8
+Requires-Dist: chardet==5.1.0
+Requires-Dist: lxml==4.9.2
+Requires-Dist: pdfminer-six==20221105
 Provides-Extra: dev
-Requires-Dist: black==22.8.0; extra == 'dev'
-Requires-Dist: build==0.8.0; extra == 'dev'
-Requires-Dist: coverage==6.5.0; extra == 'dev'
-Requires-Dist: flake8==5.0.4; extra == 'dev'
+Requires-Dist: black==23.3.0; extra == 'dev'
+Requires-Dist: build==0.10.0; extra == 'dev'
+Requires-Dist: coverage==7.2.5; extra == 'dev'
+Requires-Dist: flake8==6.0.0; extra == 'dev'
 Requires-Dist: mccabe<=0.7.0; extra == 'dev'
 Requires-Dist: mega-py==1.0.8; extra == 'dev'
-Requires-Dist: mypy==0.981; extra == 'dev'
-Requires-Dist: pylint==2.15.3; extra == 'dev'
-Requires-Dist: pytest==7.1.3; extra == 'dev'
+Requires-Dist: mypy==1.3.0; extra == 'dev'
+Requires-Dist: pylint==2.17.4; extra == 'dev'
+Requires-Dist: pytest==7.3.1; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: mega-py==1.0.8; extra == 'test'
-Requires-Dist: pytest==7.1.3; extra == 'test'
+Requires-Dist: pytest==7.3.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 ![linkrot logo](https://github.com/marshalmiller/linkrot/blob/6e6fb45239f8d06e89671e2ec68a11629747355d/branding/Asset%207@4x.png)
 # Introduction
 
 Scans pdfs for links written in plaintext and checks if they are active or returns an error code. It then generates a report of its findings. Extract references (pdf, url, doi, arxiv) and metadata from a PDF.
 
 Check out our sister project, [Rotting Research](https://github.com/marshalmiller/rottingresearch), for a web app implementation of this project.
 
 # Features
 
 - Extract references and metadata from a given PDF.  
 - Detects pdf, url, arxiv and doi references.
-- Archives valid links using Internet Archive's Wayback Machine.
+- Archives valid links using Internet Archive's Wayback Machine (using the -a flag).
 - Checks for valid SSL certificate.  
 - Find broken hyperlinks (using the -c flag).  
 - Output as text or JSON (using the -j flag).  
 - Extract the PDF text (using the --text flag).  
 - Use as command-line tool or Python package.  
 - Works with local and online pdfs.
```

