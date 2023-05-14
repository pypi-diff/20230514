# Comparing `tmp/references_parser-0.2.3.tar.gz` & `tmp/references_parser-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "references_parser-0.2.3.tar", last modified: Thu Jan 12 18:53:10 2023, max compression
+gzip compressed data, was "references_parser-0.2.4.tar", last modified: Sun May 14 16:28:00 2023, max compression
```

## Comparing `references_parser-0.2.3.tar` & `references_parser-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:53:10.892678 references_parser-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-01-12 18:53:10.892678 references_parser-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-01-12 18:52:58.000000 references_parser-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-12 18:52:58.000000 references_parser-0.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:53:10.888678 references_parser-0.2.3/references_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 18:52:58.000000 references_parser-0.2.3/references_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-01-12 18:52:58.000000 references_parser-0.2.3/references_parser/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:53:10.892678 references_parser-0.2.3/references_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-01-12 18:52:58.000000 references_parser-0.2.3/references_parser/parsers/IeeeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-01-12 18:52:58.000000 references_parser-0.2.3/references_parser/parsers/SsauParser.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-12 18:52:58.000000 references_parser-0.2.3/references_parser/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:53:10.892678 references_parser-0.2.3/references_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-01-12 18:53:10.000000 references_parser-0.2.3/references_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-12 18:53:10.000000 references_parser-0.2.3/references_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 18:53:10.000000 references_parser-0.2.3/references_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-12 18:53:10.000000 references_parser-0.2.3/references_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-12 18:53:10.000000 references_parser-0.2.3/references_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 18:53:10.892678 references_parser-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-01-12 18:52:58.000000 references_parser-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:28:00.279685 references_parser-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-14 16:28:00.279685 references_parser-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-14 16:27:47.000000 references_parser-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-14 16:27:47.000000 references_parser-0.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:28:00.279685 references_parser-0.2.4/references_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:27:47.000000 references_parser-0.2.4/references_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-14 16:27:47.000000 references_parser-0.2.4/references_parser/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:28:00.279685 references_parser-0.2.4/references_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-14 16:27:47.000000 references_parser-0.2.4/references_parser/parsers/IeeeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-14 16:27:47.000000 references_parser-0.2.4/references_parser/parsers/SsauParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 16:27:47.000000 references_parser-0.2.4/references_parser/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:28:00.279685 references_parser-0.2.4/references_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-14 16:28:00.000000 references_parser-0.2.4/references_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-14 16:28:00.000000 references_parser-0.2.4/references_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:28:00.000000 references_parser-0.2.4/references_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 16:28:00.000000 references_parser-0.2.4/references_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 16:28:00.000000 references_parser-0.2.4/references_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:28:00.279685 references_parser-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-14 16:27:47.000000 references_parser-0.2.4/setup.py
```

### Comparing `references_parser-0.2.3/PKG-INFO` & `references_parser-0.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: references_parser
-Version: 0.2.3
+Version: 0.2.4
 Summary: Tool for parsing bibtex in ssau's format
 Home-page: https://github.com/Banayaki/ReferencesParser
 Author: Mukhin Artem
 Author-email: artemmukhinssau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `references_parser-0.2.3/README.md` & `references_parser-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `references_parser-0.2.3/references_parser/parse.py` & `references_parser-0.2.4/references_parser/parse.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                            help='Path to the file containing bibtext citations.')
     argparser.add_argument('-s', '--save', type=str,
                            help='Path to file where to save the result of parsing.', default='')
     argparser.add_argument('-p', '--parser', type=str,
                            help='Parser to use. Available parsers: ieee, ssau. Default: ssau.', default='ssau')
 
     args = argparser.parse_args()
-    with open(args.path, 'r') as f:
+    with open(args.path, 'r', encoding='utf-8') as f:
         citations = f.read()
 
     parser_type = args.parser.lower()
     parser = PARSER_MAPPING.get(parser_type)
     if parser is None:
         raise ValueError(f"Unknown parser type. Expect one of {list(PARSER_MAPPING.keys())}, but received"
                          f"{parser_type}")
```

### Comparing `references_parser-0.2.3/references_parser/parsers/IeeeParser.py` & `references_parser-0.2.4/references_parser/parsers/IeeeParser.py`

 * *Files identical despite different names*

### Comparing `references_parser-0.2.3/references_parser/parsers/SsauParser.py` & `references_parser-0.2.4/references_parser/parsers/SsauParser.py`

 * *Files identical despite different names*

### Comparing `references_parser-0.2.3/references_parser.egg-info/PKG-INFO` & `references_parser-0.2.4/references_parser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: references-parser
-Version: 0.2.3
+Version: 0.2.4
 Summary: Tool for parsing bibtex in ssau's format
 Home-page: https://github.com/Banayaki/ReferencesParser
 Author: Mukhin Artem
 Author-email: artemmukhinssau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `references_parser-0.2.3/setup.py` & `references_parser-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='references_parser',
     packages=setuptools.find_packages(),
-    version='0.2.3',
+    version='0.2.4',
     description="Tool for parsing bibtex in ssau's format",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mukhin Artem',
     author_email='artemmukhinssau@gmail.com',
     url='https://github.com/Banayaki/ReferencesParser',
     include_package_data=True,
```

