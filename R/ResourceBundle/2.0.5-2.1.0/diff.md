# Comparing `tmp/ResourceBundle-2.0.5.tar.gz` & `tmp/ResourceBundle-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ResourceBundle-2.0.5.tar", last modified: Tue Nov  1 16:28:21 2022, max compression
+gzip compressed data, was "ResourceBundle-2.1.0.tar", last modified: Sun May 14 20:17:03 2023, max compression
```

## Comparing `ResourceBundle-2.0.5.tar` & `ResourceBundle-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 16:28:21.441504 ResourceBundle-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-01 16:27:59.000000 ResourceBundle-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3332 2022-11-01 16:28:21.441504 ResourceBundle-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2440 2022-11-01 16:27:59.000000 ResourceBundle-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 16:28:21.441504 ResourceBundle-2.0.5/ResourceBundle/
--rw-r--r--   0 runner    (1001) docker     (121)     7827 2022-11-01 16:27:59.000000 ResourceBundle-2.0.5/ResourceBundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-11-01 16:27:59.000000 ResourceBundle-2.0.5/ResourceBundle/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 16:28:21.441504 ResourceBundle-2.0.5/ResourceBundle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3332 2022-11-01 16:28:21.000000 ResourceBundle-2.0.5/ResourceBundle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-11-01 16:28:21.000000 ResourceBundle-2.0.5/ResourceBundle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 16:28:21.000000 ResourceBundle-2.0.5/ResourceBundle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-01 16:28:21.000000 ResourceBundle-2.0.5/ResourceBundle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 16:28:21.441504 ResourceBundle-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-11-01 16:27:59.000000 ResourceBundle-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:17:03.897961 ResourceBundle-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 20:16:52.000000 ResourceBundle-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-14 20:17:03.897961 ResourceBundle-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-14 20:16:52.000000 ResourceBundle-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:17:03.893961 ResourceBundle-2.1.0/ResourceBundle/
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-14 20:16:52.000000 ResourceBundle-2.1.0/ResourceBundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-14 20:16:52.000000 ResourceBundle-2.1.0/ResourceBundle/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:17:03.893961 ResourceBundle-2.1.0/ResourceBundle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-14 20:17:03.000000 ResourceBundle-2.1.0/ResourceBundle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-14 20:17:03.000000 ResourceBundle-2.1.0/ResourceBundle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:17:03.000000 ResourceBundle-2.1.0/ResourceBundle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-14 20:17:03.000000 ResourceBundle-2.1.0/ResourceBundle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:17:03.897961 ResourceBundle-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-14 20:16:52.000000 ResourceBundle-2.1.0/setup.py
```

### Comparing `ResourceBundle-2.0.5/LICENSE` & `ResourceBundle-2.1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020-2021 Felix Zenk
+Copyright (c) 2020-2023 Felix Zenk
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ResourceBundle-2.0.5/PKG-INFO` & `ResourceBundle-2.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResourceBundle
-Version: 2.0.5
+Version: 2.1.0
 Summary: ResourceBundle is a module that manages internationalization of string resources
 Home-page: https://felix-zenk.github.io/projects/ResourceBundle
 Author: Felix Zenk
 Author-email: felix.zenk@web.de
 Project-URL: Bug Reports, https://github.com/felix-zenk/ResourceBundle/issues
 Project-URL: Source, https://github.com/felix-zenk/ResourceBundle
 Classifier: Programming Language :: Python :: 3
@@ -27,77 +27,66 @@
 [![PyPI version](https://badge.fury.io/py/ResourceBundle.svg)](https://pypi.org/project/ResourceBundle)
 [![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/onboardapis/blob/main/LICENSE)
 
 
 ResourceBundle is a module that manages internationalization of string resources.
 It is inspired by javas ResourceBundle and accepts the same format as a java PropertyResourceBundle.
 
+> **Note:** ResourceBundle is not the python way of doing internationalization.
+> This package is only intended to be used if you *absolutely have* to work with ResourceBundle files
+> or need a quick working way when porting from java.
+>
+> For information on how to do internationalization in python,
+> see the [official documentation](https://docs.python.org/3/library/gettext.html).
+> You can use the `ResourceBundle.Converter.to_gettext()` method to convert your ResourceBundle files to gettext po files.
+
 ---
 ### Installation
 
 The ResourceBundle module can be downloaded from [PyPI](https://pypi.org/project/ResourceBundle):
 
 ```bash
-$  python -m pip install ResourceBundle
-```
-
-### Usage
+# linux / macOS
+$  python3 -m pip install ResourceBundle
 
-Each translation file you provide should have key-value pairs inside:
+# windows
+>  py -m pip install ResourceBundle
 ```
-# This is a comment
 
-key=value
-another_key=Another value
-```
-
-Save the files of your ResourceBundle in the following structure and file name format:
-```
-./
-├── BundleName.properties  # Recommended as a fallback
-├── BundleName_languageCode_countryCode_variant.properties
-└── ...
-```
+### Usage
 
-For example:
-```
-./
-├── Strings.properties
-├── Strings_en.properties
-├── Strings_en_US.properties
-└── ...
-```
+Assuming you come from java, you are probably familiar with the ResourceBundle file format.
+If not,you can read about it
+[here](https://docs.oracle.com/en/java/javase/20/docs/api/java.base/java/util/PropertyResourceBundle.html).
 
-The recommended way to get a ResourceBundle instance is by using ``ResourceBundle.get_bundle(name, locale)``.
-This function also provides support for pythons builtin ``locale`` moudule.
+Get a ResourceBundle instance is by using ``ResourceBundle.get_bundle(name, locale)``.
 
 ```python
-import locale
 import ResourceBundle
 
 bundle = ResourceBundle.get_bundle("Strings", "en")
-bundle = ResourceBundle.get_bundle("Strings", locale.getlocale())
 
 # It is now possible to get a resource with the get() method
 bundle.get("key")
 ```
 
 If the key could not be found in the ResourceBundle the parent ResourceBundles will be searched
-until a matching key was found, or it is determined that the key is not present in any parent ResourceBundle.
+until a matching key was found.
+If the key is not present in any of its parents a ``ResourceBundle.exceptions.NotInResourceBundleError`` will be raised.
 
 ---
 
-#### Accessing the available key-value items in your code:
+### gettext
 
-ResourceBundles can be converted into dict objects with ``dict(bundle)``.
-If you want to include the whole chain to get every accessible key and value, just iterate over the bundles parent.
+The ResourceBundle module can convert ResourceBundle files to gettext pot / po files.
+This can be done by using the ``ResourceBundle.Converter.to_gettext()`` function.
 
 ```python
-import ResourceBundle
-
-bundle = ResourceBundle.get_bundle("Strings")
+from ResourceBundle import Converter
 
-everything = dict(bundle)
-while bundle.parent is not None:
-    bundle = bundle.parent
-    everything.update(dict(bundle))
+# convert all .properties files in the current directory to .po files
+Converter.to_gettext(".", ".")
 ```
+
+Note however that this step is obsolete if you are using gettext properly
+as this will include automatically extracting strings from your source code.
+The function is only intended as a head start to keep existing translations.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ResourceBundle-2.0.5/README.md` & `ResourceBundle-2.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -4,77 +4,66 @@
 [![PyPI version](https://badge.fury.io/py/ResourceBundle.svg)](https://pypi.org/project/ResourceBundle)
 [![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/onboardapis/blob/main/LICENSE)
 
 
 ResourceBundle is a module that manages internationalization of string resources.
 It is inspired by javas ResourceBundle and accepts the same format as a java PropertyResourceBundle.
 
+> **Note:** ResourceBundle is not the python way of doing internationalization.
+> This package is only intended to be used if you *absolutely have* to work with ResourceBundle files
+> or need a quick working way when porting from java.
+>
+> For information on how to do internationalization in python,
+> see the [official documentation](https://docs.python.org/3/library/gettext.html).
+> You can use the `ResourceBundle.Converter.to_gettext()` method to convert your ResourceBundle files to gettext po files.
+
 ---
 ### Installation
 
 The ResourceBundle module can be downloaded from [PyPI](https://pypi.org/project/ResourceBundle):
 
 ```bash
-$  python -m pip install ResourceBundle
-```
-
-### Usage
+# linux / macOS
+$  python3 -m pip install ResourceBundle
 
-Each translation file you provide should have key-value pairs inside:
+# windows
+>  py -m pip install ResourceBundle
 ```
-# This is a comment
 
-key=value
-another_key=Another value
-```
-
-Save the files of your ResourceBundle in the following structure and file name format:
-```
-./
-├── BundleName.properties  # Recommended as a fallback
-├── BundleName_languageCode_countryCode_variant.properties
-└── ...
-```
+### Usage
 
-For example:
-```
-./
-├── Strings.properties
-├── Strings_en.properties
-├── Strings_en_US.properties
-└── ...
-```
+Assuming you come from java, you are probably familiar with the ResourceBundle file format.
+If not,you can read about it
+[here](https://docs.oracle.com/en/java/javase/20/docs/api/java.base/java/util/PropertyResourceBundle.html).
 
-The recommended way to get a ResourceBundle instance is by using ``ResourceBundle.get_bundle(name, locale)``.
-This function also provides support for pythons builtin ``locale`` moudule.
+Get a ResourceBundle instance is by using ``ResourceBundle.get_bundle(name, locale)``.
 
 ```python
-import locale
 import ResourceBundle
 
 bundle = ResourceBundle.get_bundle("Strings", "en")
-bundle = ResourceBundle.get_bundle("Strings", locale.getlocale())
 
 # It is now possible to get a resource with the get() method
 bundle.get("key")
 ```
 
 If the key could not be found in the ResourceBundle the parent ResourceBundles will be searched
-until a matching key was found, or it is determined that the key is not present in any parent ResourceBundle.
+until a matching key was found.
+If the key is not present in any of its parents a ``ResourceBundle.exceptions.NotInResourceBundleError`` will be raised.
 
 ---
 
-#### Accessing the available key-value items in your code:
+### gettext
 
-ResourceBundles can be converted into dict objects with ``dict(bundle)``.
-If you want to include the whole chain to get every accessible key and value, just iterate over the bundles parent.
+The ResourceBundle module can convert ResourceBundle files to gettext pot / po files.
+This can be done by using the ``ResourceBundle.Converter.to_gettext()`` function.
 
 ```python
-import ResourceBundle
-
-bundle = ResourceBundle.get_bundle("Strings")
+from ResourceBundle import Converter
 
-everything = dict(bundle)
-while bundle.parent is not None:
-    bundle = bundle.parent
-    everything.update(dict(bundle))
+# convert all .properties files in the current directory to .po files
+Converter.to_gettext(".", ".")
 ```
+
+Note however that this step is obsolete if you are using gettext properly
+as this will include automatically extracting strings from your source code.
+The function is only intended as a head start to keep existing translations.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ResourceBundle-2.0.5/ResourceBundle/exceptions.py` & `ResourceBundle-2.1.0/ResourceBundle/exceptions.py`

 * *Files identical despite different names*

### Comparing `ResourceBundle-2.0.5/ResourceBundle.egg-info/PKG-INFO` & `ResourceBundle-2.1.0/ResourceBundle.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResourceBundle
-Version: 2.0.5
+Version: 2.1.0
 Summary: ResourceBundle is a module that manages internationalization of string resources
 Home-page: https://felix-zenk.github.io/projects/ResourceBundle
 Author: Felix Zenk
 Author-email: felix.zenk@web.de
 Project-URL: Bug Reports, https://github.com/felix-zenk/ResourceBundle/issues
 Project-URL: Source, https://github.com/felix-zenk/ResourceBundle
 Classifier: Programming Language :: Python :: 3
@@ -27,77 +27,66 @@
 [![PyPI version](https://badge.fury.io/py/ResourceBundle.svg)](https://pypi.org/project/ResourceBundle)
 [![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/onboardapis/blob/main/LICENSE)
 
 
 ResourceBundle is a module that manages internationalization of string resources.
 It is inspired by javas ResourceBundle and accepts the same format as a java PropertyResourceBundle.
 
+> **Note:** ResourceBundle is not the python way of doing internationalization.
+> This package is only intended to be used if you *absolutely have* to work with ResourceBundle files
+> or need a quick working way when porting from java.
+>
+> For information on how to do internationalization in python,
+> see the [official documentation](https://docs.python.org/3/library/gettext.html).
+> You can use the `ResourceBundle.Converter.to_gettext()` method to convert your ResourceBundle files to gettext po files.
+
 ---
 ### Installation
 
 The ResourceBundle module can be downloaded from [PyPI](https://pypi.org/project/ResourceBundle):
 
 ```bash
-$  python -m pip install ResourceBundle
-```
-
-### Usage
+# linux / macOS
+$  python3 -m pip install ResourceBundle
 
-Each translation file you provide should have key-value pairs inside:
+# windows
+>  py -m pip install ResourceBundle
 ```
-# This is a comment
 
-key=value
-another_key=Another value
-```
-
-Save the files of your ResourceBundle in the following structure and file name format:
-```
-./
-├── BundleName.properties  # Recommended as a fallback
-├── BundleName_languageCode_countryCode_variant.properties
-└── ...
-```
+### Usage
 
-For example:
-```
-./
-├── Strings.properties
-├── Strings_en.properties
-├── Strings_en_US.properties
-└── ...
-```
+Assuming you come from java, you are probably familiar with the ResourceBundle file format.
+If not,you can read about it
+[here](https://docs.oracle.com/en/java/javase/20/docs/api/java.base/java/util/PropertyResourceBundle.html).
 
-The recommended way to get a ResourceBundle instance is by using ``ResourceBundle.get_bundle(name, locale)``.
-This function also provides support for pythons builtin ``locale`` moudule.
+Get a ResourceBundle instance is by using ``ResourceBundle.get_bundle(name, locale)``.
 
 ```python
-import locale
 import ResourceBundle
 
 bundle = ResourceBundle.get_bundle("Strings", "en")
-bundle = ResourceBundle.get_bundle("Strings", locale.getlocale())
 
 # It is now possible to get a resource with the get() method
 bundle.get("key")
 ```
 
 If the key could not be found in the ResourceBundle the parent ResourceBundles will be searched
-until a matching key was found, or it is determined that the key is not present in any parent ResourceBundle.
+until a matching key was found.
+If the key is not present in any of its parents a ``ResourceBundle.exceptions.NotInResourceBundleError`` will be raised.
 
 ---
 
-#### Accessing the available key-value items in your code:
+### gettext
 
-ResourceBundles can be converted into dict objects with ``dict(bundle)``.
-If you want to include the whole chain to get every accessible key and value, just iterate over the bundles parent.
+The ResourceBundle module can convert ResourceBundle files to gettext pot / po files.
+This can be done by using the ``ResourceBundle.Converter.to_gettext()`` function.
 
 ```python
-import ResourceBundle
-
-bundle = ResourceBundle.get_bundle("Strings")
+from ResourceBundle import Converter
 
-everything = dict(bundle)
-while bundle.parent is not None:
-    bundle = bundle.parent
-    everything.update(dict(bundle))
+# convert all .properties files in the current directory to .po files
+Converter.to_gettext(".", ".")
 ```
+
+Note however that this step is obsolete if you are using gettext properly
+as this will include automatically extracting strings from your source code.
+The function is only intended as a head start to keep existing translations.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ResourceBundle-2.0.5/setup.py` & `ResourceBundle-2.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
-from ResourceBundle import __version__, __author__, __email__
+from ResourceBundle import __version__
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 homepage = "https://felix-zenk.github.io/projects/ResourceBundle"
 source = "https://github.com/felix-zenk/ResourceBundle"
 
 
 setuptools.setup(
     name="ResourceBundle",
     version=__version__,
-    author=__author__,
-    author_email=__email__,
+    author='Felix Zenk',
+    author_email='felix.zenk@web.de',
     description="ResourceBundle is a module that manages internationalization of string resources",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=homepage,
     project_urls={
         "Bug Reports": f"{source}/issues",
         "Source": source
```

