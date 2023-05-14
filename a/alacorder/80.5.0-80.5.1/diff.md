# Comparing `tmp/alacorder-80.5.0.tar.gz` & `tmp/alacorder-80.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.5.0.tar", max compression
+gzip compressed data, was "alacorder-80.5.1.tar", max compression
```

## Comparing `alacorder-80.5.0.tar` & `alacorder-80.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.5.0/LICENSE
--rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.5.0/README.md
--rw-r--r--   0        0        0      746 2023-05-13 17:24:49.150698 alacorder-80.5.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-13 17:21:52.692111 alacorder-80.5.0/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.5.0/src/alacorder/__init__.py
--rw-r--r--   0        0        0   218037 2023-05-13 17:24:31.186328 alacorder-80.5.0/src/alacorder/__main__.py
--rw-r--r--   0        0        0   218037 2023-05-13 17:24:35.983482 alacorder-80.5.0/src/alacorder/alac.py
--rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 alacorder-80.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.5.1/LICENSE
+-rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.5.1/README.md
+-rw-r--r--   0        0        0      746 2023-05-14 14:16:27.040873 alacorder-80.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-14 00:21:47.679650 alacorder-80.5.1/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.5.1/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   218348 2023-05-14 14:13:42.945251 alacorder-80.5.1/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   218348 2023-05-14 14:12:36.830180 alacorder-80.5.1/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 alacorder-80.5.1/PKG-INFO
```

### Comparing `alacorder-80.5.0/LICENSE` & `alacorder-80.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.0/README.md` & `alacorder-80.5.1/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.0/pyproject.toml` & `alacorder-80.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.5.0"
+version = "80.5.1"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.5.0/src/alacorder/.DS_Store` & `alacorder-80.5.1/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.0/src/alacorder/__main__.py` & `alacorder-80.5.1/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.5.0"
+version = "80.5.1"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1684,15 +1684,15 @@
             .str.extract(r"Domestic Violence: ([YES|NO])")
             .cast(pl.Categorical)
             .alias("DomesticViolence"),
             pl.col("AllPagesText")
             .str.extract(r"Agency ORI: ([A-Z\s]+)")
             .str.rstrip("C")
             .str.replace(r"\n", "")
-            .str.replace(r"\s+", " ")
+            .str.replace_all(r"\s+", " ")
             .str.strip()
             .alias("AgencyORI"),
             pl.col("AllPagesText")
             .str.extract(r"Driver License N°: ([A-Z0-9]+)")
             .alias("DLRAW"),
             pl.col("AllPagesText")
             .str.extract(r"SSN: ([X\d]{3}\-[X\d]{2}-[X\d]{4})")
@@ -2896,14 +2896,19 @@
             pl.col("Sentence")
             .str.extract(r"Attorney Fees\: (.+?) (Confinement|Split|Restitution)")
             .str.replace("© Alacourt.com", "", literal=True)
             .str.replace(r"Split.+", "")
             .str.replace(r"Confinement.+", "")
             .str.replace(r"\d?\d/\d?\d/\d\d\d\d \d", "")
             .str.replace(r"\$|Recipient", "")
+            .str.replace(r'PrelimHearing\:X?','')
+            .str.replace(r'SX10\:X?','')
+            .str.replace(r'DemandReductionHearing\:\d+\.\d\d','')
+            .str.replace(r'Subpoena\:X?','')
+            .str.replace(r'AttorneyFees\:','')
             .str.replace_all(r"\s+", "")
             .alias("AttorneyFees"),
             pl.col("Sentence")
             .str.extract(
                 r"Imposed Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("ImposedConfinementPeriod"),
@@ -2948,14 +2953,15 @@
             .str.extract(r"Electronic Monitoring\: (.+?) Reverse Split")
             .str.replace_all(r"[-0\s]", "")
             .cast(pl.Categorical)
             .alias("ElectronicMonitoring"),
             pl.col("Sentence")
             .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)")
             .str.replace_all(r"Death\: Life\:", "")
+            .str.replace(r'Life Without Parole\: ?X?','')
             .str.strip()
             .cast(pl.Categorical)
             .alias("ReverseSplit"),
             pl.col("Sentence")
             .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
             .alias("CoterminousSentence"),
             pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
```

### Comparing `alacorder-80.5.0/src/alacorder/alac.py` & `alacorder-80.5.1/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.5.0"
+version = "80.5.1"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1684,15 +1684,15 @@
             .str.extract(r"Domestic Violence: ([YES|NO])")
             .cast(pl.Categorical)
             .alias("DomesticViolence"),
             pl.col("AllPagesText")
             .str.extract(r"Agency ORI: ([A-Z\s]+)")
             .str.rstrip("C")
             .str.replace(r"\n", "")
-            .str.replace(r"\s+", " ")
+            .str.replace_all(r"\s+", " ")
             .str.strip()
             .alias("AgencyORI"),
             pl.col("AllPagesText")
             .str.extract(r"Driver License N°: ([A-Z0-9]+)")
             .alias("DLRAW"),
             pl.col("AllPagesText")
             .str.extract(r"SSN: ([X\d]{3}\-[X\d]{2}-[X\d]{4})")
@@ -2896,14 +2896,19 @@
             pl.col("Sentence")
             .str.extract(r"Attorney Fees\: (.+?) (Confinement|Split|Restitution)")
             .str.replace("© Alacourt.com", "", literal=True)
             .str.replace(r"Split.+", "")
             .str.replace(r"Confinement.+", "")
             .str.replace(r"\d?\d/\d?\d/\d\d\d\d \d", "")
             .str.replace(r"\$|Recipient", "")
+            .str.replace(r'PrelimHearing\:X?','')
+            .str.replace(r'SX10\:X?','')
+            .str.replace(r'DemandReductionHearing\:\d+\.\d\d','')
+            .str.replace(r'Subpoena\:X?','')
+            .str.replace(r'AttorneyFees\:','')
             .str.replace_all(r"\s+", "")
             .alias("AttorneyFees"),
             pl.col("Sentence")
             .str.extract(
                 r"Imposed Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("ImposedConfinementPeriod"),
@@ -2948,14 +2953,15 @@
             .str.extract(r"Electronic Monitoring\: (.+?) Reverse Split")
             .str.replace_all(r"[-0\s]", "")
             .cast(pl.Categorical)
             .alias("ElectronicMonitoring"),
             pl.col("Sentence")
             .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)")
             .str.replace_all(r"Death\: Life\:", "")
+            .str.replace(r'Life Without Parole\: ?X?','')
             .str.strip()
             .cast(pl.Categorical)
             .alias("ReverseSplit"),
             pl.col("Sentence")
             .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
             .alias("CoterminousSentence"),
             pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
```

### Comparing `alacorder-80.5.0/PKG-INFO` & `alacorder-80.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.5.0
+Version: 80.5.1
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

