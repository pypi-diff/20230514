# Comparing `tmp/pydbml-1.0.7.tar.gz` & `tmp/pydbml-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbml-1.0.7.tar", last modified: Sun Dec 11 11:28:37 2022, max compression
+gzip compressed data, was "pydbml-1.0.8.tar", last modified: Sun May 14 11:55:57 2023, max compression
```

## Comparing `pydbml-1.0.7.tar` & `pydbml-1.0.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:28:37.479510 pydbml-1.0.7/
--rw-r--r--   0 user      (1000) user      (1000)     1056 2022-08-27 12:11:12.000000 pydbml-1.0.7/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     3900 2022-12-11 11:28:37.479510 pydbml-1.0.7/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     3214 2022-11-20 08:37:21.000000 pydbml-1.0.7/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:28:37.476176 pydbml-1.0.7/pydbml/
--rw-r--r--   0 user      (1000) user      (1000)      202 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:28:37.476176 pydbml-1.0.7/pydbml/classes/
--rw-r--r--   0 user      (1000) user      (1000)      283 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/classes/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1122 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/classes/base.py
--rw-r--r--   0 user      (1000) user      (1000)     4935 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/classes/column.py
--rw-r--r--   0 user      (1000) user      (1000)     3911 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/classes/enum.py
--rw-r--r--   0 user      (1000) user      (1000)      589 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/classes/expression.py
--rw-r--r--   0 user      (1000) user      (1000)     5009 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/classes/index.py
--rw-r--r--   0 user      (1000) user      (1000)     2563 2022-10-23 09:04:28.000000 pydbml-1.0.7/pydbml/classes/note.py
--rw-r--r--   0 user      (1000) user      (1000)     1447 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/classes/project.py
--rw-r--r--   0 user      (1000) user      (1000)     9058 2022-11-20 08:34:11.000000 pydbml-1.0.7/pydbml/classes/reference.py
--rw-r--r--   0 user      (1000) user      (1000)     8651 2022-12-11 11:12:03.000000 pydbml-1.0.7/pydbml/classes/table.py
--rw-r--r--   0 user      (1000) user      (1000)     1470 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/classes/table_group.py
--rw-r--r--   0 user      (1000) user      (1000)       73 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/constants.py
--rw-r--r--   0 user      (1000) user      (1000)     7738 2022-11-20 08:34:11.000000 pydbml-1.0.7/pydbml/database.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:28:37.476176 pydbml-1.0.7/pydbml/definitions/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/definitions/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     3463 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/definitions/column.py
--rw-r--r--   0 user      (1000) user      (1000)      991 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/definitions/common.py
--rw-r--r--   0 user      (1000) user      (1000)     2123 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/definitions/enum.py
--rw-r--r--   0 user      (1000) user      (1000)     1137 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/definitions/generic.py
--rw-r--r--   0 user      (1000) user      (1000)     2777 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/definitions/index.py
--rw-r--r--   0 user      (1000) user      (1000)     1369 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/definitions/project.py
--rw-r--r--   0 user      (1000) user      (1000)     4357 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/definitions/reference.py
--rw-r--r--   0 user      (1000) user      (1000)     2613 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/definitions/table.py
--rw-r--r--   0 user      (1000) user      (1000)      903 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/definitions/table_group.py
--rw-r--r--   0 user      (1000) user      (1000)      389 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/exceptions.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:28:37.476176 pydbml-1.0.7/pydbml/parser/
--rw-r--r--   0 user      (1000) user      (1000)       27 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/parser/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     8642 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/parser/blueprints.py
--rw-r--r--   0 user      (1000) user      (1000)     6616 2022-08-27 12:11:12.000000 pydbml-1.0.7/pydbml/parser/parser.py
--rw-r--r--   0 user      (1000) user      (1000)     1578 2022-12-11 11:28:25.000000 pydbml-1.0.7/pydbml/tools.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:28:37.476176 pydbml-1.0.7/pydbml.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3900 2022-12-11 11:28:37.000000 pydbml-1.0.7/pydbml.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1074 2022-12-11 11:28:37.000000 pydbml-1.0.7/pydbml.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-12-11 11:28:37.000000 pydbml-1.0.7/pydbml.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2022-12-11 11:28:37.000000 pydbml-1.0.7/pydbml.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2022-12-11 11:28:37.000000 pydbml-1.0.7/pydbml.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2022-12-11 11:28:37.479510 pydbml-1.0.7/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1149 2022-12-11 11:28:25.000000 pydbml-1.0.7/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-12-11 11:28:37.479510 pydbml-1.0.7/test/
--rw-r--r--   0 user      (1000) user      (1000)    14118 2022-10-23 09:24:06.000000 pydbml-1.0.7/test/test_database.py
--rw-r--r--   0 user      (1000) user      (1000)     9929 2022-08-27 12:11:12.000000 pydbml-1.0.7/test/test_docs.py
--rw-r--r--   0 user      (1000) user      (1000)      996 2022-08-27 12:11:12.000000 pydbml-1.0.7/test/test_doctest.py
--rw-r--r--   0 user      (1000) user      (1000)     3073 2022-08-27 12:11:12.000000 pydbml-1.0.7/test/test_editing.py
--rw-r--r--   0 user      (1000) user      (1000)     3952 2022-08-27 12:11:12.000000 pydbml-1.0.7/test/test_integration.py
--rw-r--r--   0 user      (1000) user      (1000)     5975 2022-08-27 12:11:12.000000 pydbml-1.0.7/test/test_parser.py
--rw-r--r--   0 user      (1000) user      (1000)     3515 2022-12-11 11:28:25.000000 pydbml-1.0.7/test/test_tools.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.296517 pydbml-1.0.8/
+-rw-r--r--   0 user      (1000) user      (1000)     1056 2022-08-27 12:11:12.000000 pydbml-1.0.8/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     3897 2023-05-14 11:55:57.296517 pydbml-1.0.8/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     3211 2023-05-14 11:55:38.000000 pydbml-1.0.8/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.293184 pydbml-1.0.8/pydbml/
+-rw-r--r--   0 user      (1000) user      (1000)      202 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.293184 pydbml-1.0.8/pydbml/classes/
+-rw-r--r--   0 user      (1000) user      (1000)      283 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1122 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/base.py
+-rw-r--r--   0 user      (1000) user      (1000)     4935 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/column.py
+-rw-r--r--   0 user      (1000) user      (1000)     3911 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/enum.py
+-rw-r--r--   0 user      (1000) user      (1000)      589 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/expression.py
+-rw-r--r--   0 user      (1000) user      (1000)     5009 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/index.py
+-rw-r--r--   0 user      (1000) user      (1000)     2563 2022-10-23 09:04:28.000000 pydbml-1.0.8/pydbml/classes/note.py
+-rw-r--r--   0 user      (1000) user      (1000)     1447 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/project.py
+-rw-r--r--   0 user      (1000) user      (1000)     9058 2022-11-20 08:34:11.000000 pydbml-1.0.8/pydbml/classes/reference.py
+-rw-r--r--   0 user      (1000) user      (1000)     8651 2022-12-11 11:12:03.000000 pydbml-1.0.8/pydbml/classes/table.py
+-rw-r--r--   0 user      (1000) user      (1000)     1470 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/classes/table_group.py
+-rw-r--r--   0 user      (1000) user      (1000)       73 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/constants.py
+-rw-r--r--   0 user      (1000) user      (1000)     7738 2022-11-20 08:34:11.000000 pydbml-1.0.8/pydbml/database.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.296517 pydbml-1.0.8/pydbml/definitions/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3463 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/column.py
+-rw-r--r--   0 user      (1000) user      (1000)     1019 2023-05-14 11:55:38.000000 pydbml-1.0.8/pydbml/definitions/common.py
+-rw-r--r--   0 user      (1000) user      (1000)     2123 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/enum.py
+-rw-r--r--   0 user      (1000) user      (1000)     1137 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/generic.py
+-rw-r--r--   0 user      (1000) user      (1000)     2777 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/index.py
+-rw-r--r--   0 user      (1000) user      (1000)     1369 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/project.py
+-rw-r--r--   0 user      (1000) user      (1000)     4357 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/reference.py
+-rw-r--r--   0 user      (1000) user      (1000)     2613 2023-05-14 11:41:15.000000 pydbml-1.0.8/pydbml/definitions/table.py
+-rw-r--r--   0 user      (1000) user      (1000)      903 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/definitions/table_group.py
+-rw-r--r--   0 user      (1000) user      (1000)      389 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/exceptions.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.296517 pydbml-1.0.8/pydbml/parser/
+-rw-r--r--   0 user      (1000) user      (1000)       27 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/parser/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     8642 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/parser/blueprints.py
+-rw-r--r--   0 user      (1000) user      (1000)     6616 2022-08-27 12:11:12.000000 pydbml-1.0.8/pydbml/parser/parser.py
+-rw-r--r--   0 user      (1000) user      (1000)     1578 2022-12-11 11:28:25.000000 pydbml-1.0.8/pydbml/tools.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.293184 pydbml-1.0.8/pydbml.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3897 2023-05-14 11:55:57.000000 pydbml-1.0.8/pydbml.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1074 2023-05-14 11:55:57.000000 pydbml-1.0.8/pydbml.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-14 11:55:57.000000 pydbml-1.0.8/pydbml.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-05-14 11:55:57.000000 pydbml-1.0.8/pydbml.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-14 11:55:57.000000 pydbml-1.0.8/pydbml.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-14 11:55:57.296517 pydbml-1.0.8/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-14 11:55:38.000000 pydbml-1.0.8/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-14 11:55:57.296517 pydbml-1.0.8/test/
+-rw-r--r--   0 user      (1000) user      (1000)    14118 2022-10-23 09:24:06.000000 pydbml-1.0.8/test/test_database.py
+-rw-r--r--   0 user      (1000) user      (1000)     9929 2022-08-27 12:11:12.000000 pydbml-1.0.8/test/test_docs.py
+-rw-r--r--   0 user      (1000) user      (1000)      996 2022-08-27 12:11:12.000000 pydbml-1.0.8/test/test_doctest.py
+-rw-r--r--   0 user      (1000) user      (1000)     3073 2022-08-27 12:11:12.000000 pydbml-1.0.8/test/test_editing.py
+-rw-r--r--   0 user      (1000) user      (1000)     3952 2022-08-27 12:11:12.000000 pydbml-1.0.8/test/test_integration.py
+-rw-r--r--   0 user      (1000) user      (1000)     5975 2022-08-27 12:11:12.000000 pydbml-1.0.8/test/test_parser.py
+-rw-r--r--   0 user      (1000) user      (1000)     3515 2022-12-11 11:28:25.000000 pydbml-1.0.8/test/test_tools.py
```

### Comparing `pydbml-1.0.7/LICENSE` & `pydbml-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/PKG-INFO` & `pydbml-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbml
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python parser and builder for DBML
 Home-page: https://github.com/Vanderhoof/PyDBML
 Author: Daniil Minukhin
 Author-email: ddddsa@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -20,19 +20,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![](https://img.shields.io/pypi/v/pydbml.svg)](https://pypi.org/project/pydbml/) [![](https://img.shields.io/pypi/dm/pydbml.svg)](https://pypi.org/project/pydbml/)  [![](https://img.shields.io/github/v/tag/Vanderhoof/PyDBML.svg?label=GitHub)](https://github.com/Vanderhoof/PyDBML) ![](coverage.svg)
 
 # DBML parser for Python
 
-*Compliant with DBML **v2.4.4** syntax*
+*Compliant with DBML **v2.5.3** syntax*
 
 PyDBML is a Python parser and builder for [DBML](https://www.dbml.org) syntax. 
 
-> The project was rewritten in May 2022, the new version 1.0.0 is not compatible with the previous ones. See details in [Upgrading to PyDBML 1.0.0](docs/upgrading.md).
+> The project was rewritten in May 2022, the new version 1.0.0 is not compatible with versions 0.x.x. See details in [Upgrading to PyDBML 1.0.0](docs/upgrading.md).
 
 **Docs:**
 
 * [Class Reference](docs/classes.md)
 * [Creating DBML schema](docs/creating_schema.md)
 * [Upgrading to PyDBML 1.0.0](docs/upgrading.md)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: pydbml Version: 1.0.7 Summary: Python parser and
+Metadata-Version: 2.1 Name: pydbml Version: 1.0.8 Summary: Python parser and
 builder for DBML Home-page: https://github.com/Vanderhoof/PyDBML Author: Daniil
 Minukhin Author-email: ddddsa@gmail.com License: MIT Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python Classifier: Topic :: Documentation Classifier: Topic :: Text
 Processing :: Markup Classifier: Topic :: Utilities Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE [![](https://
 img.shields.io/pypi/v/pydbml.svg)](https://pypi.org/project/pydbml/) [![]
 (https://img.shields.io/pypi/dm/pydbml.svg)](https://pypi.org/project/pydbml/)
 [![](https://img.shields.io/github/v/tag/Vanderhoof/PyDBML.svg?label=GitHub)]
 (https://github.com/Vanderhoof/PyDBML) ![](coverage.svg) # DBML parser for
-Python *Compliant with DBML **v2.4.4** syntax* PyDBML is a Python parser and
+Python *Compliant with DBML **v2.5.3** syntax* PyDBML is a Python parser and
 builder for [DBML](https://www.dbml.org) syntax. > The project was rewritten in
-May 2022, the new version 1.0.0 is not compatible with the previous ones. See
+May 2022, the new version 1.0.0 is not compatible with versions 0.x.x. See
 details in [Upgrading to PyDBML 1.0.0](docs/upgrading.md). **Docs:** * [Class
 Reference](docs/classes.md) * [Creating DBML schema](docs/creating_schema.md) *
 [Upgrading to PyDBML 1.0.0](docs/upgrading.md) > PyDBML requires Python v3.8 or
 higher ## Installation You can install PyDBML using pip: ```bash pip3 install
 pydbml ``` ## Quick start To parse a DBML file, import the `PyDBML` class and
 initialize it with Path object ```python >>> from pydbml import PyDBML >>> from
 pathlib import Path >>> parsed = PyDBML(Path('test_schema.dbml')) ``` or with
```

### Comparing `pydbml-1.0.7/README.md` & `pydbml-1.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [![](https://img.shields.io/pypi/v/pydbml.svg)](https://pypi.org/project/pydbml/) [![](https://img.shields.io/pypi/dm/pydbml.svg)](https://pypi.org/project/pydbml/)  [![](https://img.shields.io/github/v/tag/Vanderhoof/PyDBML.svg?label=GitHub)](https://github.com/Vanderhoof/PyDBML) ![](coverage.svg)
 
 # DBML parser for Python
 
-*Compliant with DBML **v2.4.4** syntax*
+*Compliant with DBML **v2.5.3** syntax*
 
 PyDBML is a Python parser and builder for [DBML](https://www.dbml.org) syntax. 
 
-> The project was rewritten in May 2022, the new version 1.0.0 is not compatible with the previous ones. See details in [Upgrading to PyDBML 1.0.0](docs/upgrading.md).
+> The project was rewritten in May 2022, the new version 1.0.0 is not compatible with versions 0.x.x. See details in [Upgrading to PyDBML 1.0.0](docs/upgrading.md).
 
 **Docs:**
 
 * [Class Reference](docs/classes.md)
 * [Creating DBML schema](docs/creating_schema.md)
 * [Upgrading to PyDBML 1.0.0](docs/upgrading.md)
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 [![](https://img.shields.io/pypi/v/pydbml.svg)](https://pypi.org/project/
 pydbml/) [![](https://img.shields.io/pypi/dm/pydbml.svg)](https://pypi.org/
 project/pydbml/) [![](https://img.shields.io/github/v/tag/Vanderhoof/
 PyDBML.svg?label=GitHub)](https://github.com/Vanderhoof/PyDBML) ![]
-(coverage.svg) # DBML parser for Python *Compliant with DBML **v2.4.4** syntax*
+(coverage.svg) # DBML parser for Python *Compliant with DBML **v2.5.3** syntax*
 PyDBML is a Python parser and builder for [DBML](https://www.dbml.org) syntax.
 > The project was rewritten in May 2022, the new version 1.0.0 is not
-compatible with the previous ones. See details in [Upgrading to PyDBML 1.0.0]
+compatible with versions 0.x.x. See details in [Upgrading to PyDBML 1.0.0]
 (docs/upgrading.md). **Docs:** * [Class Reference](docs/classes.md) * [Creating
 DBML schema](docs/creating_schema.md) * [Upgrading to PyDBML 1.0.0](docs/
 upgrading.md) > PyDBML requires Python v3.8 or higher ## Installation You can
 install PyDBML using pip: ```bash pip3 install pydbml ``` ## Quick start To
 parse a DBML file, import the `PyDBML` class and initialize it with Path object
 ```python >>> from pydbml import PyDBML >>> from pathlib import Path >>> parsed
 = PyDBML(Path('test_schema.dbml')) ``` or with file stream ```python >>> with
```

### Comparing `pydbml-1.0.7/pydbml/classes/base.py` & `pydbml-1.0.8/pydbml/classes/base.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/classes/column.py` & `pydbml-1.0.8/pydbml/classes/column.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/classes/enum.py` & `pydbml-1.0.8/pydbml/classes/enum.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/classes/expression.py` & `pydbml-1.0.8/pydbml/classes/expression.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/classes/index.py` & `pydbml-1.0.8/pydbml/classes/index.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/classes/note.py` & `pydbml-1.0.8/pydbml/classes/note.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/classes/project.py` & `pydbml-1.0.8/pydbml/classes/project.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/classes/reference.py` & `pydbml-1.0.8/pydbml/classes/reference.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/classes/table.py` & `pydbml-1.0.8/pydbml/classes/table.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/classes/table_group.py` & `pydbml-1.0.8/pydbml/classes/table_group.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/database.py` & `pydbml-1.0.8/pydbml/database.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/definitions/column.py` & `pydbml-1.0.8/pydbml/definitions/column.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/definitions/common.py` & `pydbml-1.0.8/pydbml/definitions/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 # optional comment or newline, but comments are captured
 _c = (pp.Suppress('\n') | comment('comment_before*'))[...]
 
 # optional captured comment
 c = comment('comment')[0, 1]
 
 n = pp.LineEnd()
-end = n | pp.StringEnd()
+
+end = comment[...].suppress() + n | pp.StringEnd()
+
 # obligatory newline
 # n = pp.Suppress('\n')[1, ...]
 
 note = pp.CaselessLiteral("note:") + _ - string_literal('text')
 note.set_parse_action(lambda s, loc, tok: NoteBlueprint(tok['text']))
 
 note_object = pp.CaselessLiteral('note') + _ - '{' + _ - string_literal('text') + _ - '}'
```

### Comparing `pydbml-1.0.7/pydbml/definitions/enum.py` & `pydbml-1.0.8/pydbml/definitions/enum.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/definitions/generic.py` & `pydbml-1.0.8/pydbml/definitions/generic.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/definitions/index.py` & `pydbml-1.0.8/pydbml/definitions/index.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/definitions/project.py` & `pydbml-1.0.8/pydbml/definitions/project.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/definitions/reference.py` & `pydbml-1.0.8/pydbml/definitions/reference.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/definitions/table.py` & `pydbml-1.0.8/pydbml/definitions/table.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/definitions/table_group.py` & `pydbml-1.0.8/pydbml/definitions/table_group.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/parser/blueprints.py` & `pydbml-1.0.8/pydbml/parser/blueprints.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/parser/parser.py` & `pydbml-1.0.8/pydbml/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml/tools.py` & `pydbml-1.0.8/pydbml/tools.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/pydbml.egg-info/PKG-INFO` & `pydbml-1.0.8/pydbml.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbml
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python parser and builder for DBML
 Home-page: https://github.com/Vanderhoof/PyDBML
 Author: Daniil Minukhin
 Author-email: ddddsa@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -20,19 +20,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![](https://img.shields.io/pypi/v/pydbml.svg)](https://pypi.org/project/pydbml/) [![](https://img.shields.io/pypi/dm/pydbml.svg)](https://pypi.org/project/pydbml/)  [![](https://img.shields.io/github/v/tag/Vanderhoof/PyDBML.svg?label=GitHub)](https://github.com/Vanderhoof/PyDBML) ![](coverage.svg)
 
 # DBML parser for Python
 
-*Compliant with DBML **v2.4.4** syntax*
+*Compliant with DBML **v2.5.3** syntax*
 
 PyDBML is a Python parser and builder for [DBML](https://www.dbml.org) syntax. 
 
-> The project was rewritten in May 2022, the new version 1.0.0 is not compatible with the previous ones. See details in [Upgrading to PyDBML 1.0.0](docs/upgrading.md).
+> The project was rewritten in May 2022, the new version 1.0.0 is not compatible with versions 0.x.x. See details in [Upgrading to PyDBML 1.0.0](docs/upgrading.md).
 
 **Docs:**
 
 * [Class Reference](docs/classes.md)
 * [Creating DBML schema](docs/creating_schema.md)
 * [Upgrading to PyDBML 1.0.0](docs/upgrading.md)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: pydbml Version: 1.0.7 Summary: Python parser and
+Metadata-Version: 2.1 Name: pydbml Version: 1.0.8 Summary: Python parser and
 builder for DBML Home-page: https://github.com/Vanderhoof/PyDBML Author: Daniil
 Minukhin Author-email: ddddsa@gmail.com License: MIT Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python Classifier: Topic :: Documentation Classifier: Topic :: Text
 Processing :: Markup Classifier: Topic :: Utilities Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE [![](https://
 img.shields.io/pypi/v/pydbml.svg)](https://pypi.org/project/pydbml/) [![]
 (https://img.shields.io/pypi/dm/pydbml.svg)](https://pypi.org/project/pydbml/)
 [![](https://img.shields.io/github/v/tag/Vanderhoof/PyDBML.svg?label=GitHub)]
 (https://github.com/Vanderhoof/PyDBML) ![](coverage.svg) # DBML parser for
-Python *Compliant with DBML **v2.4.4** syntax* PyDBML is a Python parser and
+Python *Compliant with DBML **v2.5.3** syntax* PyDBML is a Python parser and
 builder for [DBML](https://www.dbml.org) syntax. > The project was rewritten in
-May 2022, the new version 1.0.0 is not compatible with the previous ones. See
+May 2022, the new version 1.0.0 is not compatible with versions 0.x.x. See
 details in [Upgrading to PyDBML 1.0.0](docs/upgrading.md). **Docs:** * [Class
 Reference](docs/classes.md) * [Creating DBML schema](docs/creating_schema.md) *
 [Upgrading to PyDBML 1.0.0](docs/upgrading.md) > PyDBML requires Python v3.8 or
 higher ## Installation You can install PyDBML using pip: ```bash pip3 install
 pydbml ``` ## Quick start To parse a DBML file, import the `PyDBML` class and
 initialize it with Path object ```python >>> from pydbml import PyDBML >>> from
 pathlib import Path >>> parsed = PyDBML(Path('test_schema.dbml')) ``` or with
```

### Comparing `pydbml-1.0.7/pydbml.egg-info/SOURCES.txt` & `pydbml-1.0.8/pydbml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/setup.py` & `pydbml-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='pydbml',
     python_requires='>=3.8',
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
-    version='1.0.7',
+    version='1.0.8',
     author='Daniil Minukhin',
     author_email='ddddsa@gmail.com',
     url='https://github.com/Vanderhoof/PyDBML',
     packages=['pydbml', 'pydbml.classes', 'pydbml.definitions', 'pydbml.parser'],
     license='MIT',
     platforms='any',
     install_requires=[
```

### Comparing `pydbml-1.0.7/test/test_database.py` & `pydbml-1.0.8/test/test_database.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/test/test_docs.py` & `pydbml-1.0.8/test/test_docs.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/test/test_doctest.py` & `pydbml-1.0.8/test/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/test/test_editing.py` & `pydbml-1.0.8/test/test_editing.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/test/test_integration.py` & `pydbml-1.0.8/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/test/test_parser.py` & `pydbml-1.0.8/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydbml-1.0.7/test/test_tools.py` & `pydbml-1.0.8/test/test_tools.py`

 * *Files identical despite different names*

