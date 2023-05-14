# Comparing `tmp/beancount-parser-0.1.8.tar.gz` & `tmp/beancount-parser-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount-parser-0.1.8.tar", max compression
+gzip compressed data, was "beancount-parser-0.1.9.tar", max compression
```

## Comparing `beancount-parser-0.1.8.tar` & `beancount-parser-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1076 2022-04-05 04:56:42.962435 beancount-parser-0.1.8/LICENSE
--rw-r--r--   0        0        0        0 2022-04-05 04:56:42.962435 beancount-parser-0.1.8/beancount_parser/__init__.py
--rw-r--r--   0        0        0      292 2022-04-05 04:56:42.962435 beancount-parser-0.1.8/beancount_parser/grammar/account.lark
--rw-r--r--   0        0        0     2543 2022-04-05 04:56:42.962435 beancount-parser-0.1.8/beancount_parser/grammar/beancount.lark
--rw-r--r--   0        0        0       22 2022-04-05 04:56:42.962435 beancount-parser-0.1.8/beancount_parser/grammar/comment.lark
--rw-r--r--   0        0        0      174 2022-04-05 04:56:42.966435 beancount-parser-0.1.8/beancount_parser/grammar/currency.lark
--rw-r--r--   0        0        0      247 2022-04-05 04:56:42.966435 beancount-parser-0.1.8/beancount_parser/grammar/date.lark
--rw-r--r--   0        0        0       60 2022-04-05 04:56:42.966435 beancount-parser-0.1.8/beancount_parser/grammar/flag.lark
--rw-r--r--   0        0        0       84 2022-04-05 04:56:42.966435 beancount-parser-0.1.8/beancount_parser/grammar/link.lark
--rw-r--r--   0        0        0      627 2022-04-05 04:56:42.966435 beancount-parser-0.1.8/beancount_parser/grammar/metadata.lark
--rw-r--r--   0        0        0      198 2022-04-05 04:56:42.966435 beancount-parser-0.1.8/beancount_parser/grammar/numbers.lark
--rw-r--r--   0        0        0       29 2022-04-05 04:56:42.966435 beancount-parser-0.1.8/beancount_parser/grammar/section_header.lark
--rw-r--r--   0        0        0      150 2022-04-05 04:56:42.966435 beancount-parser-0.1.8/beancount_parser/grammar/tag.lark
--rw-r--r--   0        0        0      403 2022-04-05 04:56:42.966435 beancount-parser-0.1.8/beancount_parser/parser.py
--rw-r--r--   0        0        0      508 2022-04-05 04:56:42.966435 beancount-parser-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      782 2022-04-05 04:56:46.658671 beancount-parser-0.1.8/setup.py
--rw-r--r--   0        0        0      641 2022-04-05 04:56:46.658896 beancount-parser-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/LICENSE
+-rw-r--r--   0        0        0        0 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/__init__.py
+-rw-r--r--   0        0        0      292 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/grammar/account.lark
+-rw-r--r--   0        0        0     2552 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/grammar/beancount.lark
+-rw-r--r--   0        0        0       22 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/grammar/comment.lark
+-rw-r--r--   0        0        0      174 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/grammar/currency.lark
+-rw-r--r--   0        0        0      247 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/grammar/date.lark
+-rw-r--r--   0        0        0       60 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/grammar/flag.lark
+-rw-r--r--   0        0        0       84 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/grammar/link.lark
+-rw-r--r--   0        0        0      627 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/grammar/metadata.lark
+-rw-r--r--   0        0        0      198 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/grammar/numbers.lark
+-rw-r--r--   0        0        0       29 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/grammar/section_header.lark
+-rw-r--r--   0        0        0      150 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/grammar/tag.lark
+-rw-r--r--   0        0        0      403 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/beancount_parser/parser.py
+-rw-r--r--   0        0        0      508 2022-04-05 05:15:30.273076 beancount-parser-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      782 2022-04-05 05:15:33.713347 beancount-parser-0.1.9/setup.py
+-rw-r--r--   0        0        0      641 2022-04-05 05:15:33.713600 beancount-parser-0.1.9/PKG-INFO
```

### Comparing `beancount-parser-0.1.8/LICENSE` & `beancount-parser-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount-parser-0.1.8/beancount_parser/grammar/beancount.lark` & `beancount-parser-0.1.9/beancount_parser/grammar/beancount.lark`

 * *Files 7% similar despite different names*

```diff
@@ -50,19 +50,19 @@
 // Posting
 ?per_unit_cost: "{" amount "}"
 ?total_cost: "{{" amount "}}"
 ?both_cost: "{" SIGNED_NUMBER  "#" amount "}"
 ?dated_cost: "{" amount "," DATE "}"
 cost: per_unit_cost | total_cost | both_cost | dated_cost
 
-?per_unit_price: "@" amount
-?total_price: "@@" amount
-tx_price: per_unit_price | total_price
+per_unit_price: "@" amount
+total_price: "@@" amount
+?posting_price: per_unit_price | total_price
 
-?detailed_posting: [FLAG] ACCOUNT amount [cost] [tx_price]
+?detailed_posting: [FLAG] ACCOUNT amount [cost] [posting_price]
 // the special case where only Account is present
 ?simple_posting: [FLAG] ACCOUNT
 posting: detailed_posting | simple_posting
 
 ?directive: date_directive
         | simple_directive
         | posting
```

### Comparing `beancount-parser-0.1.8/beancount_parser/grammar/metadata.lark` & `beancount-parser-0.1.9/beancount_parser/grammar/metadata.lark`

 * *Files identical despite different names*

### Comparing `beancount-parser-0.1.8/setup.py` & `beancount-parser-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*'], 'beancount_parser': ['grammar/*']}
 
 install_requires = \
 ['lark>=1.1.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'beancount-parser',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Standalone Lark based Beancount syntax parser (not relying on Beancount library), MIT license',
     'long_description': None,
     'author': 'Fang-Pen Lin',
     'author_email': 'fangpen@launchplatform.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/LaunchPlatform/beancount-parser',
```

### Comparing `beancount-parser-0.1.8/PKG-INFO` & `beancount-parser-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-parser
-Version: 0.1.8
+Version: 0.1.9
 Summary: Standalone Lark based Beancount syntax parser (not relying on Beancount library), MIT license
 Home-page: https://github.com/LaunchPlatform/beancount-parser
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

