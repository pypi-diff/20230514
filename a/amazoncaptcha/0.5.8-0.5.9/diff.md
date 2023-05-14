# Comparing `tmp/amazoncaptcha-0.5.8.tar.gz` & `tmp/amazoncaptcha-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazoncaptcha-0.5.8.tar", last modified: Thu Jul 21 13:02:23 2022, max compression
+gzip compressed data, was "amazoncaptcha-0.5.9.tar", last modified: Thu Jan 19 21:01:02 2023, max compression
```

## Comparing `amazoncaptcha-0.5.8.tar` & `amazoncaptcha-0.5.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 13:02:23.576671 amazoncaptcha-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7917 2022-07-21 13:02:23.576671 amazoncaptcha-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8845 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 13:02:23.564671 amazoncaptcha-0.5.8/amazoncaptcha/
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5370 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/devtools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8935 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 13:02:23.576671 amazoncaptcha-0.5.8/amazoncaptcha/training_data/
--rw-r--r--   0 runner    (1001) docker     (121)   198935 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/A.json
--rw-r--r--   0 runner    (1001) docker     (121)   184130 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/B.json
--rw-r--r--   0 runner    (1001) docker     (121)   163342 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/C.json
--rw-r--r--   0 runner    (1001) docker     (121)   144071 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/E.json
--rw-r--r--   0 runner    (1001) docker     (121)   106554 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/F.json
--rw-r--r--   0 runner    (1001) docker     (121)   201277 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/G.json
--rw-r--r--   0 runner    (1001) docker     (121)   124537 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/H.json
--rw-r--r--   0 runner    (1001) docker     (121)    82771 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/J.json
--rw-r--r--   0 runner    (1001) docker     (121)   162508 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/K.json
--rw-r--r--   0 runner    (1001) docker     (121)    67974 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/L.json
--rw-r--r--   0 runner    (1001) docker     (121)   219167 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/M.json
--rw-r--r--   0 runner    (1001) docker     (121)   154630 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/N.json
--rw-r--r--   0 runner    (1001) docker     (121)   134241 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/P.json
--rw-r--r--   0 runner    (1001) docker     (121)   165410 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/R.json
--rw-r--r--   0 runner    (1001) docker     (121)    65433 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/T.json
--rw-r--r--   0 runner    (1001) docker     (121)   117048 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/U.json
--rw-r--r--   0 runner    (1001) docker     (121)   168884 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/X.json
--rw-r--r--   0 runner    (1001) docker     (121)   121831 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/training_data/Y.json
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/amazoncaptcha/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 13:02:23.568671 amazoncaptcha-0.5.8/amazoncaptcha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7917 2022-07-21 13:02:23.000000 amazoncaptcha-0.5.8/amazoncaptcha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-07-21 13:02:23.000000 amazoncaptcha-0.5.8/amazoncaptcha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 13:02:23.000000 amazoncaptcha-0.5.8/amazoncaptcha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-07-21 13:02:23.000000 amazoncaptcha-0.5.8/amazoncaptcha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-21 13:02:23.000000 amazoncaptcha-0.5.8/amazoncaptcha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-21 13:02:23.576671 amazoncaptcha-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-07-21 13:02:14.000000 amazoncaptcha-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:01:02.359275 amazoncaptcha-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-01-19 21:01:02.359275 amazoncaptcha-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:01:02.355275 amazoncaptcha-0.5.9/amazoncaptcha/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/devtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:01:02.359275 amazoncaptcha-0.5.9/amazoncaptcha/training_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   198935 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/A.json
+-rw-r--r--   0 runner    (1001) docker     (123)   184130 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/B.json
+-rw-r--r--   0 runner    (1001) docker     (123)   163342 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/C.json
+-rw-r--r--   0 runner    (1001) docker     (123)   144071 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/E.json
+-rw-r--r--   0 runner    (1001) docker     (123)   106554 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/F.json
+-rw-r--r--   0 runner    (1001) docker     (123)   201277 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/G.json
+-rw-r--r--   0 runner    (1001) docker     (123)   124537 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/H.json
+-rw-r--r--   0 runner    (1001) docker     (123)    82771 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/J.json
+-rw-r--r--   0 runner    (1001) docker     (123)   162508 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/K.json
+-rw-r--r--   0 runner    (1001) docker     (123)    67974 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/L.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219167 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/M.json
+-rw-r--r--   0 runner    (1001) docker     (123)   154630 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/N.json
+-rw-r--r--   0 runner    (1001) docker     (123)   134241 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/P.json
+-rw-r--r--   0 runner    (1001) docker     (123)   165410 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/R.json
+-rw-r--r--   0 runner    (1001) docker     (123)    65433 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/T.json
+-rw-r--r--   0 runner    (1001) docker     (123)   117048 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/U.json
+-rw-r--r--   0 runner    (1001) docker     (123)   168884 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/X.json
+-rw-r--r--   0 runner    (1001) docker     (123)   121831 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/training_data/Y.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/amazoncaptcha/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:01:02.355275 amazoncaptcha-0.5.9/amazoncaptcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-01-19 21:01:02.000000 amazoncaptcha-0.5.9/amazoncaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-01-19 21:01:02.000000 amazoncaptcha-0.5.9/amazoncaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 21:01:02.000000 amazoncaptcha-0.5.9/amazoncaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-19 21:01:02.000000 amazoncaptcha-0.5.9/amazoncaptcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-19 21:01:02.000000 amazoncaptcha-0.5.9/amazoncaptcha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 21:01:02.359275 amazoncaptcha-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-01-19 21:00:52.000000 amazoncaptcha-0.5.9/setup.py
```

### Comparing `amazoncaptcha-0.5.8/LICENSE` & `amazoncaptcha-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/PKG-INFO` & `amazoncaptcha-0.5.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: amazoncaptcha
-Version: 0.5.8
+Version: 0.5.9
 Summary: "Pure Python, lightweight, Pillow-based solver for the Amazon text captcha."
 Home-page: https://github.com/a-maliarov/amazoncaptcha
 Author: Anatolii Maliarov
 Author-email: tly.mov@gmail.com
-License: UNKNOWN
 Project-URL: Documentation, https://amazoncaptcha.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/a-maliarov/amazoncaptcha
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,16 +30,16 @@
 ![Timing](https://img.shields.io/badge/response%20time-0.2s-success)
 [![Size](https://img.shields.io/badge/wheel%20size-0.9%20MB-informational)](https://pypi.org/project/amazoncaptcha/)
 [![Version](https://img.shields.io/pypi/v/amazoncaptcha?color=informational)](https://pypi.org/project/amazoncaptcha/)
 [![Python version](https://img.shields.io/badge/python-3.7%2B-informational)](https://pypi.org/project/amazoncaptcha/)
 [![Downloads](https://img.shields.io/pypi/dm/amazoncaptcha?color=success)](https://pypi.org/project/amazoncaptcha/)
 
 ## Recent News
-+ *July 21, 2022*: tested and approved compatibility with Pillow 9.2.0
-+ *January 25, 2022*: tested and approved compatibility with Python 3.10-dev
++ *January 19, 2023*: tested and approved compatibility with Pillow 9.4.0
++ *January 25, 2022*: tested and approved compatibility with Python 3.10
 + *January 25, 2022*: dropped support for Python 3.6
 
 ## Installation
 You can simply install the library from [PyPi](https://pypi.org/project/amazoncaptcha/) using **pip**. For more methods check the [docs](https://amazoncaptcha.readthedocs.io/en/latest/installation.html).
 ```bash
 pip install amazoncaptcha
 ```
@@ -57,15 +55,14 @@
 # Or: solution = AmazonCaptcha('captcha.jpg').solve()
 ```
 
 ## Status
 [![Status](https://img.shields.io/pypi/status/amazoncaptcha)](https://pypi.org/project/amazoncaptcha/)
 [![Build Status](https://img.shields.io/circleci/build/github/a-maliarov/amazoncaptcha)](https://app.circleci.com/pipelines/github/a-maliarov/amazoncaptcha)
 [![Documentation Status](https://readthedocs.org/projects/amazoncaptcha/badge/?version=latest)](https://amazoncaptcha.readthedocs.io/en/latest/)
-[![Requirements Status](https://requires.io/github/a-maliarov/amazoncaptcha/requirements.svg?branch=master)](https://requires.io/github/a-maliarov/amazoncaptcha/requirements/?branch=master)
 [![Code Coverage](https://img.shields.io/codecov/c/gh/a-maliarov/amazoncaptcha?label=code%20coverage)](https://codecov.io/gh/a-maliarov/amazoncaptcha)
 [![CodeFactor Grade](https://img.shields.io/codefactor/grade/github/a-maliarov/amazoncaptcha/master)](https://www.codefactor.io/repository/github/a-maliarov/amazoncaptcha/overview/master)
 
 ## Usage and Class Methods
 Browsing Amazon using `selenium` and stuck on captcha? The class method below will do all the dirty work of extracting an image from the webpage for you. Practically, it takes a screenshot from your webdriver, crops the captcha and stores it into bytes array which is then used to create an `AmazonCaptcha` instance. This also means avoiding any local savings. **For consistency across different devices, it is highly recommended to use `fromlink` class method instead of `fromdriver`**.
 ```python
 from amazoncaptcha import AmazonCaptcha
@@ -108,9 +105,7 @@
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/amaliarov)
 
 ## Additional
 + If you want to see the [**History of Changes**](https://github.com/a-maliarov/amazoncaptcha/blob/master/HISTORY.md), [**Code of Conduct**](https://github.com/a-maliarov/amazoncaptcha/blob/master/.github/CODE_OF_CONDUCT.md), [**Contributing Policy**](https://github.com/a-maliarov/amazoncaptcha/blob/master/.github/CONTRIBUTING.md), or [**License**](https://github.com/a-maliarov/amazoncaptcha/blob/master/LICENSE), use these inline links to navigate based on your needs.
 + If you are facing any errors, please, report your situation via an issue.
 + This project is for educational and research purposes only. Any actions and/or activities related to the material contained on this GitHub Repository is solely your responsibility. The author will not be held responsible in the event any criminal charges be brought against any individuals misusing the information in this GitHub Repository to break the law.
 + Amazon is the registered trademark of Amazon.com, Inc. Amazon name used in this project is for identification purposes only. The project is not associated in any way with Amazon.com, Inc. and is not an official solution of Amazon.com, Inc.
-
-
```

### Comparing `amazoncaptcha-0.5.8/README.md` & `amazoncaptcha-0.5.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -188,366 +188,354 @@
 00000bb0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
 00000bc0: 656c 6473 2e69 6f2f 7079 7069 2f64 6d2f  elds.io/pypi/dm/
 00000bd0: 616d 617a 6f6e 6361 7074 6368 613f 636f  amazoncaptcha?co
 00000be0: 6c6f 723d 7375 6363 6573 7329 5d28 6874  lor=success)](ht
 00000bf0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
 00000c00: 726f 6a65 6374 2f61 6d61 7a6f 6e63 6170  roject/amazoncap
 00000c10: 7463 6861 2f29 0d0a 0d0a 2323 2052 6563  tcha/)....## Rec
-00000c20: 656e 7420 4e65 7773 0d0a 2b20 2a4a 756c  ent News..+ *Jul
-00000c30: 7920 3231 2c20 3230 3232 2a3a 2074 6573  y 21, 2022*: tes
-00000c40: 7465 6420 616e 6420 6170 7072 6f76 6564  ted and approved
-00000c50: 2063 6f6d 7061 7469 6269 6c69 7479 2077   compatibility w
-00000c60: 6974 6820 5069 6c6c 6f77 2039 2e32 2e30  ith Pillow 9.2.0
-00000c70: 0d0a 2b20 2a4a 616e 7561 7279 2032 352c  ..+ *January 25,
-00000c80: 2032 3032 322a 3a20 7465 7374 6564 2061   2022*: tested a
-00000c90: 6e64 2061 7070 726f 7665 6420 636f 6d70  nd approved comp
-00000ca0: 6174 6962 696c 6974 7920 7769 7468 2050  atibility with P
-00000cb0: 7974 686f 6e20 332e 3130 2d64 6576 0d0a  ython 3.10-dev..
-00000cc0: 2b20 2a4a 616e 7561 7279 2032 352c 2032  + *January 25, 2
-00000cd0: 3032 322a 3a20 6472 6f70 7065 6420 7375  022*: dropped su
-00000ce0: 7070 6f72 7420 666f 7220 5079 7468 6f6e  pport for Python
-00000cf0: 2033 2e36 0d0a 0d0a 2323 2049 6e73 7461   3.6....## Insta
-00000d00: 6c6c 6174 696f 6e0d 0a59 6f75 2063 616e  llation..You can
-00000d10: 2073 696d 706c 7920 696e 7374 616c 6c20   simply install 
-00000d20: 7468 6520 6c69 6272 6172 7920 6672 6f6d  the library from
-00000d30: 205b 5079 5069 5d28 6874 7470 733a 2f2f   [PyPi](https://
-00000d40: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000d50: 2f61 6d61 7a6f 6e63 6170 7463 6861 2f29  /amazoncaptcha/)
-00000d60: 2075 7369 6e67 202a 2a70 6970 2a2a 2e20   using **pip**. 
-00000d70: 466f 7220 6d6f 7265 206d 6574 686f 6473  For more methods
-00000d80: 2063 6865 636b 2074 6865 205b 646f 6373   check the [docs
-00000d90: 5d28 6874 7470 733a 2f2f 616d 617a 6f6e  ](https://amazon
-00000da0: 6361 7074 6368 612e 7265 6164 7468 6564  captcha.readthed
-00000db0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00000dc0: 2f69 6e73 7461 6c6c 6174 696f 6e2e 6874  /installation.ht
-00000dd0: 6d6c 292e 0d0a 6060 6062 6173 680d 0a70  ml)...```bash..p
-00000de0: 6970 2069 6e73 7461 6c6c 2061 6d61 7a6f  ip install amazo
-00000df0: 6e63 6170 7463 6861 0d0a 6060 600d 0a0d  ncaptcha..```...
-00000e00: 0a23 2320 5175 6963 6b20 536e 6970 7065  .## Quick Snippe
-00000e10: 740d 0a41 6e20 6578 616d 706c 6520 6f66  t..An example of
-00000e20: 2074 6865 2063 6f6e 7374 7275 6374 6f72   the constructor
-00000e30: 2075 7361 6765 2e20 5363 726f 6c6c 2061   usage. Scroll a
-00000e40: 2062 6974 2064 6f77 6e20 746f 2073 6565   bit down to see
-00000e50: 2073 6f6d 6520 7461 7374 7920 636c 6173   some tasty clas
-00000e60: 7320 6d65 7468 6f64 732e 202a 2a46 6f72  s methods. **For
-00000e70: 2063 6f6e 7369 7374 656e 6379 2061 6372   consistency acr
-00000e80: 6f73 7320 6469 6666 6572 656e 7420 6465  oss different de
-00000e90: 7669 6365 732c 2069 7420 6973 2068 6967  vices, it is hig
-00000ea0: 686c 7920 7265 636f 6d6d 656e 6465 6420  hly recommended 
-00000eb0: 746f 2075 7365 2060 6672 6f6d 6c69 6e6b  to use `fromlink
-00000ec0: 6020 636c 6173 7320 6d65 7468 6f64 2a2a  ` class method**
-00000ed0: 2e0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
-00000ee0: 6f6d 2061 6d61 7a6f 6e63 6170 7463 6861  om amazoncaptcha
-00000ef0: 2069 6d70 6f72 7420 416d 617a 6f6e 4361   import AmazonCa
-00000f00: 7074 6368 610d 0a0d 0a63 6170 7463 6861  ptcha....captcha
-00000f10: 203d 2041 6d61 7a6f 6e43 6170 7463 6861   = AmazonCaptcha
-00000f20: 2827 6361 7074 6368 612e 6a70 6727 290d  ('captcha.jpg').
-00000f30: 0a73 6f6c 7574 696f 6e20 3d20 6361 7074  .solution = capt
-00000f40: 6368 612e 736f 6c76 6528 290d 0a0d 0a23  cha.solve()....#
-00000f50: 204f 723a 2073 6f6c 7574 696f 6e20 3d20   Or: solution = 
-00000f60: 416d 617a 6f6e 4361 7074 6368 6128 2763  AmazonCaptcha('c
-00000f70: 6170 7463 6861 2e6a 7067 2729 2e73 6f6c  aptcha.jpg').sol
-00000f80: 7665 2829 0d0a 6060 600d 0a0d 0a23 2320  ve()..```....## 
-00000f90: 5374 6174 7573 0d0a 5b21 5b53 7461 7475  Status..[![Statu
-00000fa0: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
-00000fb0: 6869 656c 6473 2e69 6f2f 7079 7069 2f73  hields.io/pypi/s
-00000fc0: 7461 7475 732f 616d 617a 6f6e 6361 7074  tatus/amazoncapt
-00000fd0: 6368 6129 5d28 6874 7470 733a 2f2f 7079  cha)](https://py
-00000fe0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f61  pi.org/project/a
-00000ff0: 6d61 7a6f 6e63 6170 7463 6861 2f29 0d0a  mazoncaptcha/)..
-00001000: 5b21 5b42 7569 6c64 2053 7461 7475 735d  [![Build Status]
-00001010: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00001020: 656c 6473 2e69 6f2f 6369 7263 6c65 6369  elds.io/circleci
-00001030: 2f62 7569 6c64 2f67 6974 6875 622f 612d  /build/github/a-
-00001040: 6d61 6c69 6172 6f76 2f61 6d61 7a6f 6e63  maliarov/amazonc
-00001050: 6170 7463 6861 295d 2868 7474 7073 3a2f  aptcha)](https:/
-00001060: 2f61 7070 2e63 6972 636c 6563 692e 636f  /app.circleci.co
-00001070: 6d2f 7069 7065 6c69 6e65 732f 6769 7468  m/pipelines/gith
-00001080: 7562 2f61 2d6d 616c 6961 726f 762f 616d  ub/a-maliarov/am
-00001090: 617a 6f6e 6361 7074 6368 6129 0d0a 5b21  azoncaptcha)..[!
-000010a0: 5b44 6f63 756d 656e 7461 7469 6f6e 2053  [Documentation S
-000010b0: 7461 7475 735d 2868 7474 7073 3a2f 2f72  tatus](https://r
-000010c0: 6561 6474 6865 646f 6373 2e6f 7267 2f70  eadthedocs.org/p
-000010d0: 726f 6a65 6374 732f 616d 617a 6f6e 6361  rojects/amazonca
-000010e0: 7074 6368 612f 6261 6467 652f 3f76 6572  ptcha/badge/?ver
-000010f0: 7369 6f6e 3d6c 6174 6573 7429 5d28 6874  sion=latest)](ht
-00001100: 7470 733a 2f2f 616d 617a 6f6e 6361 7074  tps://amazoncapt
-00001110: 6368 612e 7265 6164 7468 6564 6f63 732e  cha.readthedocs.
-00001120: 696f 2f65 6e2f 6c61 7465 7374 2f29 0d0a  io/en/latest/)..
-00001130: 5b21 5b52 6571 7569 7265 6d65 6e74 7320  [![Requirements 
-00001140: 5374 6174 7573 5d28 6874 7470 733a 2f2f  Status](https://
-00001150: 7265 7175 6972 6573 2e69 6f2f 6769 7468  requires.io/gith
-00001160: 7562 2f61 2d6d 616c 6961 726f 762f 616d  ub/a-maliarov/am
-00001170: 617a 6f6e 6361 7074 6368 612f 7265 7175  azoncaptcha/requ
-00001180: 6972 656d 656e 7473 2e73 7667 3f62 7261  irements.svg?bra
-00001190: 6e63 683d 6d61 7374 6572 295d 2868 7474  nch=master)](htt
-000011a0: 7073 3a2f 2f72 6571 7569 7265 732e 696f  ps://requires.io
-000011b0: 2f67 6974 6875 622f 612d 6d61 6c69 6172  /github/a-maliar
-000011c0: 6f76 2f61 6d61 7a6f 6e63 6170 7463 6861  ov/amazoncaptcha
-000011d0: 2f72 6571 7569 7265 6d65 6e74 732f 3f62  /requirements/?b
-000011e0: 7261 6e63 683d 6d61 7374 6572 290d 0a5b  ranch=master)..[
-000011f0: 215b 436f 6465 2043 6f76 6572 6167 655d  ![Code Coverage]
-00001200: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00001210: 656c 6473 2e69 6f2f 636f 6465 636f 762f  elds.io/codecov/
-00001220: 632f 6768 2f61 2d6d 616c 6961 726f 762f  c/gh/a-maliarov/
-00001230: 616d 617a 6f6e 6361 7074 6368 613f 6c61  amazoncaptcha?la
-00001240: 6265 6c3d 636f 6465 2532 3063 6f76 6572  bel=code%20cover
-00001250: 6167 6529 5d28 6874 7470 733a 2f2f 636f  age)](https://co
-00001260: 6465 636f 762e 696f 2f67 682f 612d 6d61  decov.io/gh/a-ma
-00001270: 6c69 6172 6f76 2f61 6d61 7a6f 6e63 6170  liarov/amazoncap
-00001280: 7463 6861 290d 0a5b 215b 436f 6465 4661  tcha)..[![CodeFa
-00001290: 6374 6f72 2047 7261 6465 5d28 6874 7470  ctor Grade](http
-000012a0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000012b0: 696f 2f63 6f64 6566 6163 746f 722f 6772  io/codefactor/gr
-000012c0: 6164 652f 6769 7468 7562 2f61 2d6d 616c  ade/github/a-mal
-000012d0: 6961 726f 762f 616d 617a 6f6e 6361 7074  iarov/amazoncapt
-000012e0: 6368 612f 6d61 7374 6572 295d 2868 7474  cha/master)](htt
-000012f0: 7073 3a2f 2f77 7777 2e63 6f64 6566 6163  ps://www.codefac
-00001300: 746f 722e 696f 2f72 6570 6f73 6974 6f72  tor.io/repositor
-00001310: 792f 6769 7468 7562 2f61 2d6d 616c 6961  y/github/a-malia
-00001320: 726f 762f 616d 617a 6f6e 6361 7074 6368  rov/amazoncaptch
-00001330: 612f 6f76 6572 7669 6577 2f6d 6173 7465  a/overview/maste
-00001340: 7229 0d0a 0d0a 2323 2055 7361 6765 2061  r)....## Usage a
-00001350: 6e64 2043 6c61 7373 204d 6574 686f 6473  nd Class Methods
-00001360: 0d0a 4272 6f77 7369 6e67 2041 6d61 7a6f  ..Browsing Amazo
-00001370: 6e20 7573 696e 6720 6073 656c 656e 6975  n using `seleniu
-00001380: 6d60 2061 6e64 2073 7475 636b 206f 6e20  m` and stuck on 
-00001390: 6361 7074 6368 613f 2054 6865 2063 6c61  captcha? The cla
-000013a0: 7373 206d 6574 686f 6420 6265 6c6f 7720  ss method below 
-000013b0: 7769 6c6c 2064 6f20 616c 6c20 7468 6520  will do all the 
-000013c0: 6469 7274 7920 776f 726b 206f 6620 6578  dirty work of ex
-000013d0: 7472 6163 7469 6e67 2061 6e20 696d 6167  tracting an imag
-000013e0: 6520 6672 6f6d 2074 6865 2077 6562 7061  e from the webpa
-000013f0: 6765 2066 6f72 2079 6f75 2e20 5072 6163  ge for you. Prac
-00001400: 7469 6361 6c6c 792c 2069 7420 7461 6b65  tically, it take
-00001410: 7320 6120 7363 7265 656e 7368 6f74 2066  s a screenshot f
-00001420: 726f 6d20 796f 7572 2077 6562 6472 6976  rom your webdriv
-00001430: 6572 2c20 6372 6f70 7320 7468 6520 6361  er, crops the ca
-00001440: 7074 6368 6120 616e 6420 7374 6f72 6573  ptcha and stores
-00001450: 2069 7420 696e 746f 2062 7974 6573 2061   it into bytes a
-00001460: 7272 6179 2077 6869 6368 2069 7320 7468  rray which is th
-00001470: 656e 2075 7365 6420 746f 2063 7265 6174  en used to creat
-00001480: 6520 616e 2060 416d 617a 6f6e 4361 7074  e an `AmazonCapt
-00001490: 6368 6160 2069 6e73 7461 6e63 652e 2054  cha` instance. T
-000014a0: 6869 7320 616c 736f 206d 6561 6e73 2061  his also means a
-000014b0: 766f 6964 696e 6720 616e 7920 6c6f 6361  voiding any loca
-000014c0: 6c20 7361 7669 6e67 732e 202a 2a46 6f72  l savings. **For
-000014d0: 2063 6f6e 7369 7374 656e 6379 2061 6372   consistency acr
-000014e0: 6f73 7320 6469 6666 6572 656e 7420 6465  oss different de
-000014f0: 7669 6365 732c 2069 7420 6973 2068 6967  vices, it is hig
-00001500: 686c 7920 7265 636f 6d6d 656e 6465 6420  hly recommended 
-00001510: 746f 2075 7365 2060 6672 6f6d 6c69 6e6b  to use `fromlink
-00001520: 6020 636c 6173 7320 6d65 7468 6f64 2069  ` class method i
-00001530: 6e73 7465 6164 206f 6620 6066 726f 6d64  nstead of `fromd
-00001540: 7269 7665 7260 2a2a 2e0d 0a60 6060 7079  river`**...```py
-00001550: 7468 6f6e 0d0a 6672 6f6d 2061 6d61 7a6f  thon..from amazo
-00001560: 6e63 6170 7463 6861 2069 6d70 6f72 7420  ncaptcha import 
-00001570: 416d 617a 6f6e 4361 7074 6368 610d 0a66  AmazonCaptcha..f
-00001580: 726f 6d20 7365 6c65 6e69 756d 2069 6d70  rom selenium imp
-00001590: 6f72 7420 7765 6264 7269 7665 720d 0a0d  ort webdriver...
-000015a0: 0a64 7269 7665 7220 3d20 7765 6264 7269  .driver = webdri
-000015b0: 7665 722e 4368 726f 6d65 2829 2023 2054  ver.Chrome() # T
-000015c0: 6869 7320 6973 2061 2073 696d 706c 6966  his is a simplif
-000015d0: 6965 6420 6578 616d 706c 650d 0a64 7269  ied example..dri
-000015e0: 7665 722e 6765 7428 2768 7474 7073 3a2f  ver.get('https:/
-000015f0: 2f77 7777 2e61 6d61 7a6f 6e2e 636f 6d2f  /www.amazon.com/
-00001600: 6572 726f 7273 2f76 616c 6964 6174 6543  errors/validateC
-00001610: 6170 7463 6861 2729 0d0a 0d0a 6361 7074  aptcha')....capt
-00001620: 6368 6120 3d20 416d 617a 6f6e 4361 7074  cha = AmazonCapt
-00001630: 6368 612e 6672 6f6d 6472 6976 6572 2864  cha.fromdriver(d
-00001640: 7269 7665 7229 0d0a 736f 6c75 7469 6f6e  river)..solution
-00001650: 203d 2063 6170 7463 6861 2e73 6f6c 7665   = captcha.solve
-00001660: 2829 0d0a 6060 600d 0a0d 0a49 6620 796f  ()..```....If yo
-00001670: 7520 6172 6520 6e6f 7420 7573 696e 6720  u are not using 
-00001680: 6073 656c 656e 6975 6d60 206f 7220 7468  `selenium` or th
-00001690: 6520 7072 6576 696f 7573 206d 6574 686f  e previous metho
-000016a0: 6420 6973 206e 6f74 206a 7573 7420 7468  d is not just th
-000016b0: 6520 6361 7365 2066 6f72 2079 6f75 2c20  e case for you, 
-000016c0: 6974 2069 7320 706f 7373 6962 6c65 2074  it is possible t
-000016d0: 6f20 7573 6520 6120 6361 7074 6368 6120  o use a captcha 
-000016e0: 6c69 6e6b 2064 6972 6563 746c 792e 2054  link directly. T
-000016f0: 6869 7320 636c 6173 7320 6d65 7468 6f64  his class method
-00001700: 2077 696c 6c20 7265 7175 6573 7420 7468   will request th
-00001710: 6520 7572 6c2c 2063 6865 636b 2074 6865  e url, check the
-00001720: 2063 6f6e 7465 6e74 2074 7970 6520 616e   content type an
-00001730: 6420 7374 6f72 6520 7468 6520 7265 7370  d store the resp
-00001740: 6f6e 7365 2063 6f6e 7465 6e74 2069 6e74  onse content int
-00001750: 6f20 6279 7465 7320 6172 7261 7920 746f  o bytes array to
-00001760: 2063 7265 6174 6520 616e 2069 6e73 7461   create an insta
-00001770: 6e63 6520 6f66 2060 416d 617a 6f6e 4361  nce of `AmazonCa
-00001780: 7074 6368 6160 2e0d 0a60 6060 7079 7468  ptcha`...```pyth
-00001790: 6f6e 0d0a 6672 6f6d 2061 6d61 7a6f 6e63  on..from amazonc
-000017a0: 6170 7463 6861 2069 6d70 6f72 7420 416d  aptcha import Am
-000017b0: 617a 6f6e 4361 7074 6368 610d 0a0d 0a6c  azonCaptcha....l
-000017c0: 696e 6b20 3d20 2768 7474 7073 3a2f 2f69  ink = 'https://i
-000017d0: 6d61 6765 732d 6e61 2e73 736c 2d69 6d61  mages-na.ssl-ima
-000017e0: 6765 732d 616d 617a 6f6e 2e63 6f6d 2f63  ges-amazon.com/c
-000017f0: 6170 7463 6861 2f75 7376 6d67 6c6f 712f  aptcha/usvmgloq/
-00001800: 4361 7074 6368 615f 6b77 7272 6e71 776b  Captcha_kwrrnqwk
-00001810: 7068 2e6a 7067 270d 0a0d 0a63 6170 7463  ph.jpg'....captc
-00001820: 6861 203d 2041 6d61 7a6f 6e43 6170 7463  ha = AmazonCaptc
-00001830: 6861 2e66 726f 6d6c 696e 6b28 6c69 6e6b  ha.fromlink(link
-00001840: 290d 0a73 6f6c 7574 696f 6e20 3d20 6361  )..solution = ca
-00001850: 7074 6368 612e 736f 6c76 6528 290d 0a60  ptcha.solve()..`
-00001860: 6060 0d0a 0d0a 496e 2061 6464 6974 696f  ``....In additio
-00001870: 6e2c 2069 6620 796f 7520 6172 6520 6120  n, if you are a 
-00001880: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
-00001890: 206f 7220 6e65 7572 616c 206e 6574 776f   or neural netwo
-000018a0: 726b 2064 6576 656c 6f70 6572 2061 6e64  rk developer and
-000018b0: 2061 7265 206c 6f6f 6b69 6e67 2066 6f72   are looking for
-000018c0: 2073 6f6d 6520 7472 6169 6e69 6e67 2064   some training d
-000018d0: 6174 612c 2063 6865 636b 205b 7468 6973  ata, check [this
-000018e0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000018f0: 2e63 6f6d 2f61 2d6d 616c 6961 726f 762f  .com/a-maliarov/
-00001900: 616d 617a 6f6e 2d63 6170 7463 6861 2d64  amazon-captcha-d
-00001910: 6174 6162 6173 6529 2072 6570 6f73 6974  atabase) reposit
-00001920: 6f72 792c 2077 6869 6368 2077 6173 2063  ory, which was c
-00001930: 7265 6174 6564 2074 6f20 7374 6f72 6520  reated to store 
-00001940: 696d 6167 6573 2061 6e64 206f 7468 6572  images and other
-00001950: 206e 6f6e 2d73 6372 6970 7420 6461 7461   non-script data
-00001960: 2066 6f72 2074 6865 2073 6f6c 7665 722e   for the solver.
-00001970: 0d0a 0d0a 2323 2048 656c 7020 7468 6520  ....## Help the 
-00001980: 4465 7665 6c6f 706d 656e 740d 0a49 6620  Development..If 
-00001990: 796f 7520 6172 6520 7769 6c6c 696e 6720  you are willing 
-000019a0: 746f 2068 656c 7020 7468 6520 6465 7665  to help the deve
-000019b0: 6c6f 706d 656e 742c 2063 6f6e 7369 6465  lopment, conside
-000019c0: 7220 7365 7474 696e 6720 606b 6565 705f  r setting `keep_
-000019d0: 6c6f 6773 6020 6172 6775 6d65 6e74 206f  logs` argument o
-000019e0: 6620 7468 6520 6073 6f6c 7665 6020 6d65  f the `solve` me
-000019f0: 7468 6f64 2074 6f20 6054 7275 6560 2e20  thod to `True`. 
-00001a00: 4865 7265 2069 7320 7468 6520 6578 616d  Here is the exam
-00001a10: 706c 652c 2069 6620 796f 7520 6172 6520  ple, if you are 
-00001a20: 7573 696e 6720 6066 726f 6d64 7269 7665  using `fromdrive
-00001a30: 7260 2063 6c61 7373 206d 6574 686f 642e  r` class method.
-00001a40: 2049 6620 7365 7420 746f 2060 5472 7565   If set to `True
-00001a50: 602c 2061 6c6c 2074 6865 206c 696e 6b73  `, all the links
-00001a60: 206f 6620 7468 6520 756e 736f 6c76 6564   of the unsolved
-00001a70: 2063 6170 7463 6861 2077 696c 6c20 6265   captcha will be
-00001a80: 2073 746f 7265 6420 736f 2074 6861 7420   stored so that 
-00001a90: 6c61 7465 7220 796f 7520 6361 6e20 5b6f  later you can [o
-00001aa0: 7065 6e20 7468 6520 6973 7375 6520 616e  pen the issue an
-00001ab0: 6420 7365 6e64 2074 6865 206c 6f67 735d  d send the logs]
-00001ac0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001ad0: 636f 6d2f 612d 6d61 6c69 6172 6f76 2f61  com/a-maliarov/a
-00001ae0: 6d61 7a6f 6e63 6170 7463 6861 2f69 7373  mazoncaptcha/iss
-00001af0: 7565 732f 6e65 773f 6173 7369 676e 6565  ues/new?assignee
-00001b00: 733d 612d 6d61 6c69 6172 6f76 266c 6162  s=a-maliarov&lab
-00001b10: 656c 733d 7472 6169 6e69 6e67 2b64 6174  els=training+dat
-00001b20: 6126 7465 6d70 6c61 7465 3d73 656e 645f  a&template=send_
-00001b30: 6c6f 6773 2e6d 6426 7469 746c 653d 4164  logs.md&title=Ad
-00001b40: 642b 7472 6169 6e69 6e67 2b64 6174 6129  d+training+data)
-00001b50: 2e0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
-00001b60: 6f6d 2061 6d61 7a6f 6e63 6170 7463 6861  om amazoncaptcha
-00001b70: 2069 6d70 6f72 7420 416d 617a 6f6e 4361   import AmazonCa
-00001b80: 7074 6368 610d 0a66 726f 6d20 7365 6c65  ptcha..from sele
-00001b90: 6e69 756d 2069 6d70 6f72 7420 7765 6264  nium import webd
-00001ba0: 7269 7665 720d 0a0d 0a64 7269 7665 7220  river....driver 
-00001bb0: 3d20 7765 6264 7269 7665 722e 4368 726f  = webdriver.Chro
-00001bc0: 6d65 2829 2023 2054 6869 7320 6973 2061  me() # This is a
-00001bd0: 2073 696d 706c 6966 6965 6420 6578 616d   simplified exam
-00001be0: 706c 650d 0a64 7269 7665 722e 6765 7428  ple..driver.get(
-00001bf0: 2768 7474 7073 3a2f 2f77 7777 2e61 6d61  'https://www.ama
-00001c00: 7a6f 6e2e 636f 6d2f 6572 726f 7273 2f76  zon.com/errors/v
-00001c10: 616c 6964 6174 6543 6170 7463 6861 2729  alidateCaptcha')
-00001c20: 0d0a 0d0a 6361 7074 6368 6120 3d20 416d  ....captcha = Am
-00001c30: 617a 6f6e 4361 7074 6368 612e 6672 6f6d  azonCaptcha.from
-00001c40: 6472 6976 6572 2864 7269 7665 7229 0d0a  driver(driver)..
-00001c50: 736f 6c75 7469 6f6e 203d 2063 6170 7463  solution = captc
-00001c60: 6861 2e73 6f6c 7665 286b 6565 705f 6c6f  ha.solve(keep_lo
-00001c70: 6773 3d54 7275 6529 0d0a 6060 600d 0a0d  gs=True)..```...
-00001c80: 0a49 6620 796f 7520 6861 7665 2061 6e79  .If you have any
-00001c90: 2073 7567 6765 7374 696f 6e73 206f 7220   suggestions or 
-00001ca0: 6964 6561 7320 6f66 2061 6464 6974 696f  ideas of additio
-00001cb0: 6e61 6c20 696e 7374 616e 6365 7320 616e  nal instances an
-00001cc0: 6420 6d65 7468 6f64 732c 2077 6869 6368  d methods, which
-00001cd0: 2079 6f75 2077 6f75 6c64 206c 696b 6520   you would like 
-00001ce0: 746f 2073 6565 2069 6e20 7468 6973 206c  to see in this l
-00001cf0: 6962 7261 7279 2c20 706c 6561 7365 2c20  ibrary, please, 
-00001d00: 6665 656c 2066 7265 6520 746f 2063 6f6e  feel free to con
-00001d10: 7461 6374 2074 6865 206f 776e 6572 2076  tact the owner v
-00001d20: 6961 2065 6d61 696c 206f 7220 666f 726b  ia email or fork
-00001d30: 276e 2770 756c 6c20 746f 2072 6570 6f73  'n'pull to repos
-00001d40: 6974 6f72 792e 2041 6e79 2063 6f6e 7472  itory. Any contr
-00001d50: 6962 7574 696f 6e20 6973 2068 6967 686c  ibution is highl
-00001d60: 7920 6170 7072 6563 6961 7465 6421 0d0a  y appreciated!..
-00001d70: 0d0a 5b21 5b22 4275 7920 4d65 2041 2043  ..[!["Buy Me A C
-00001d80: 6f66 6665 6522 5d28 6874 7470 733a 2f2f  offee"](https://
-00001d90: 7777 772e 6275 796d 6561 636f 6666 6565  www.buymeacoffee
-00001da0: 2e63 6f6d 2f61 7373 6574 732f 696d 672f  .com/assets/img/
-00001db0: 6375 7374 6f6d 5f69 6d61 6765 732f 6f72  custom_images/or
-00001dc0: 616e 6765 5f69 6d67 2e70 6e67 295d 2868  ange_img.png)](h
-00001dd0: 7474 7073 3a2f 2f77 7777 2e62 7579 6d65  ttps://www.buyme
-00001de0: 6163 6f66 6665 652e 636f 6d2f 616d 616c  acoffee.com/amal
-00001df0: 6961 726f 7629 0d0a 0d0a 2323 2041 6464  iarov)....## Add
-00001e00: 6974 696f 6e61 6c0d 0a2b 2049 6620 796f  itional..+ If yo
-00001e10: 7520 7761 6e74 2074 6f20 7365 6520 7468  u want to see th
-00001e20: 6520 5b2a 2a48 6973 746f 7279 206f 6620  e [**History of 
-00001e30: 4368 616e 6765 732a 2a5d 2868 7474 7073  Changes**](https
-00001e40: 3a2f 2f67 6974 6875 622e 636f 6d2f 612d  ://github.com/a-
-00001e50: 6d61 6c69 6172 6f76 2f61 6d61 7a6f 6e63  maliarov/amazonc
-00001e60: 6170 7463 6861 2f62 6c6f 622f 6d61 7374  aptcha/blob/mast
-00001e70: 6572 2f48 4953 544f 5259 2e6d 6429 2c20  er/HISTORY.md), 
-00001e80: 5b2a 2a43 6f64 6520 6f66 2043 6f6e 6475  [**Code of Condu
-00001e90: 6374 2a2a 5d28 6874 7470 733a 2f2f 6769  ct**](https://gi
-00001ea0: 7468 7562 2e63 6f6d 2f61 2d6d 616c 6961  thub.com/a-malia
-00001eb0: 726f 762f 616d 617a 6f6e 6361 7074 6368  rov/amazoncaptch
-00001ec0: 612f 626c 6f62 2f6d 6173 7465 722f 2e67  a/blob/master/.g
-00001ed0: 6974 6875 622f 434f 4445 5f4f 465f 434f  ithub/CODE_OF_CO
-00001ee0: 4e44 5543 542e 6d64 292c 205b 2a2a 436f  NDUCT.md), [**Co
-00001ef0: 6e74 7269 6275 7469 6e67 2050 6f6c 6963  ntributing Polic
-00001f00: 792a 2a5d 2868 7474 7073 3a2f 2f67 6974  y**](https://git
-00001f10: 6875 622e 636f 6d2f 612d 6d61 6c69 6172  hub.com/a-maliar
-00001f20: 6f76 2f61 6d61 7a6f 6e63 6170 7463 6861  ov/amazoncaptcha
-00001f30: 2f62 6c6f 622f 6d61 7374 6572 2f2e 6769  /blob/master/.gi
-00001f40: 7468 7562 2f43 4f4e 5452 4942 5554 494e  thub/CONTRIBUTIN
-00001f50: 472e 6d64 292c 206f 7220 5b2a 2a4c 6963  G.md), or [**Lic
-00001f60: 656e 7365 2a2a 5d28 6874 7470 733a 2f2f  ense**](https://
-00001f70: 6769 7468 7562 2e63 6f6d 2f61 2d6d 616c  github.com/a-mal
-00001f80: 6961 726f 762f 616d 617a 6f6e 6361 7074  iarov/amazoncapt
-00001f90: 6368 612f 626c 6f62 2f6d 6173 7465 722f  cha/blob/master/
-00001fa0: 4c49 4345 4e53 4529 2c20 7573 6520 7468  LICENSE), use th
-00001fb0: 6573 6520 696e 6c69 6e65 206c 696e 6b73  ese inline links
-00001fc0: 2074 6f20 6e61 7669 6761 7465 2062 6173   to navigate bas
-00001fd0: 6564 206f 6e20 796f 7572 206e 6565 6473  ed on your needs
-00001fe0: 2e0d 0a2b 2049 6620 796f 7520 6172 6520  ...+ If you are 
-00001ff0: 6661 6369 6e67 2061 6e79 2065 7272 6f72  facing any error
-00002000: 732c 2070 6c65 6173 652c 2072 6570 6f72  s, please, repor
-00002010: 7420 796f 7572 2073 6974 7561 7469 6f6e  t your situation
-00002020: 2076 6961 2061 6e20 6973 7375 652e 0d0a   via an issue...
-00002030: 2b20 5468 6973 2070 726f 6a65 6374 2069  + This project i
-00002040: 7320 666f 7220 6564 7563 6174 696f 6e61  s for educationa
-00002050: 6c20 616e 6420 7265 7365 6172 6368 2070  l and research p
-00002060: 7572 706f 7365 7320 6f6e 6c79 2e20 416e  urposes only. An
-00002070: 7920 6163 7469 6f6e 7320 616e 642f 6f72  y actions and/or
-00002080: 2061 6374 6976 6974 6965 7320 7265 6c61   activities rela
-00002090: 7465 6420 746f 2074 6865 206d 6174 6572  ted to the mater
-000020a0: 6961 6c20 636f 6e74 6169 6e65 6420 6f6e  ial contained on
-000020b0: 2074 6869 7320 4769 7448 7562 2052 6570   this GitHub Rep
-000020c0: 6f73 6974 6f72 7920 6973 2073 6f6c 656c  ository is solel
-000020d0: 7920 796f 7572 2072 6573 706f 6e73 6962  y your responsib
-000020e0: 696c 6974 792e 2054 6865 2061 7574 686f  ility. The autho
-000020f0: 7220 7769 6c6c 206e 6f74 2062 6520 6865  r will not be he
-00002100: 6c64 2072 6573 706f 6e73 6962 6c65 2069  ld responsible i
-00002110: 6e20 7468 6520 6576 656e 7420 616e 7920  n the event any 
-00002120: 6372 696d 696e 616c 2063 6861 7267 6573  criminal charges
-00002130: 2062 6520 6272 6f75 6768 7420 6167 6169   be brought agai
-00002140: 6e73 7420 616e 7920 696e 6469 7669 6475  nst any individu
-00002150: 616c 7320 6d69 7375 7369 6e67 2074 6865  als misusing the
-00002160: 2069 6e66 6f72 6d61 7469 6f6e 2069 6e20   information in 
-00002170: 7468 6973 2047 6974 4875 6220 5265 706f  this GitHub Repo
-00002180: 7369 746f 7279 2074 6f20 6272 6561 6b20  sitory to break 
-00002190: 7468 6520 6c61 772e 0d0a 2b20 416d 617a  the law...+ Amaz
-000021a0: 6f6e 2069 7320 7468 6520 7265 6769 7374  on is the regist
-000021b0: 6572 6564 2074 7261 6465 6d61 726b 206f  ered trademark o
-000021c0: 6620 416d 617a 6f6e 2e63 6f6d 2c20 496e  f Amazon.com, In
-000021d0: 632e 2041 6d61 7a6f 6e20 6e61 6d65 2075  c. Amazon name u
-000021e0: 7365 6420 696e 2074 6869 7320 7072 6f6a  sed in this proj
-000021f0: 6563 7420 6973 2066 6f72 2069 6465 6e74  ect is for ident
-00002200: 6966 6963 6174 696f 6e20 7075 7270 6f73  ification purpos
-00002210: 6573 206f 6e6c 792e 2054 6865 2070 726f  es only. The pro
-00002220: 6a65 6374 2069 7320 6e6f 7420 6173 736f  ject is not asso
-00002230: 6369 6174 6564 2069 6e20 616e 7920 7761  ciated in any wa
-00002240: 7920 7769 7468 2041 6d61 7a6f 6e2e 636f  y with Amazon.co
-00002250: 6d2c 2049 6e63 2e20 616e 6420 6973 206e  m, Inc. and is n
-00002260: 6f74 2061 6e20 6f66 6669 6369 616c 2073  ot an official s
-00002270: 6f6c 7574 696f 6e20 6f66 2041 6d61 7a6f  olution of Amazo
-00002280: 6e2e 636f 6d2c 2049 6e63 2e0d 0a         n.com, Inc...
+00000c20: 656e 7420 4e65 7773 0d0a 2b20 2a4a 616e  ent News..+ *Jan
+00000c30: 7561 7279 2031 392c 2032 3032 332a 3a20  uary 19, 2023*: 
+00000c40: 7465 7374 6564 2061 6e64 2061 7070 726f  tested and appro
+00000c50: 7665 6420 636f 6d70 6174 6962 696c 6974  ved compatibilit
+00000c60: 7920 7769 7468 2050 696c 6c6f 7720 392e  y with Pillow 9.
+00000c70: 342e 300d 0a2b 202a 4a61 6e75 6172 7920  4.0..+ *January 
+00000c80: 3235 2c20 3230 3232 2a3a 2074 6573 7465  25, 2022*: teste
+00000c90: 6420 616e 6420 6170 7072 6f76 6564 2063  d and approved c
+00000ca0: 6f6d 7061 7469 6269 6c69 7479 2077 6974  ompatibility wit
+00000cb0: 6820 5079 7468 6f6e 2033 2e31 300d 0a2b  h Python 3.10..+
+00000cc0: 202a 4a61 6e75 6172 7920 3235 2c20 3230   *January 25, 20
+00000cd0: 3232 2a3a 2064 726f 7070 6564 2073 7570  22*: dropped sup
+00000ce0: 706f 7274 2066 6f72 2050 7974 686f 6e20  port for Python 
+00000cf0: 332e 360d 0a0d 0a23 2320 496e 7374 616c  3.6....## Instal
+00000d00: 6c61 7469 6f6e 0d0a 596f 7520 6361 6e20  lation..You can 
+00000d10: 7369 6d70 6c79 2069 6e73 7461 6c6c 2074  simply install t
+00000d20: 6865 206c 6962 7261 7279 2066 726f 6d20  he library from 
+00000d30: 5b50 7950 695d 2868 7474 7073 3a2f 2f70  [PyPi](https://p
+00000d40: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000d50: 616d 617a 6f6e 6361 7074 6368 612f 2920  amazoncaptcha/) 
+00000d60: 7573 696e 6720 2a2a 7069 702a 2a2e 2046  using **pip**. F
+00000d70: 6f72 206d 6f72 6520 6d65 7468 6f64 7320  or more methods 
+00000d80: 6368 6563 6b20 7468 6520 5b64 6f63 735d  check the [docs]
+00000d90: 2868 7474 7073 3a2f 2f61 6d61 7a6f 6e63  (https://amazonc
+00000da0: 6170 7463 6861 2e72 6561 6474 6865 646f  aptcha.readthedo
+00000db0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000dc0: 696e 7374 616c 6c61 7469 6f6e 2e68 746d  installation.htm
+00000dd0: 6c29 2e0d 0a60 6060 6261 7368 0d0a 7069  l)...```bash..pi
+00000de0: 7020 696e 7374 616c 6c20 616d 617a 6f6e  p install amazon
+00000df0: 6361 7074 6368 610d 0a60 6060 0d0a 0d0a  captcha..```....
+00000e00: 2323 2051 7569 636b 2053 6e69 7070 6574  ## Quick Snippet
+00000e10: 0d0a 416e 2065 7861 6d70 6c65 206f 6620  ..An example of 
+00000e20: 7468 6520 636f 6e73 7472 7563 746f 7220  the constructor 
+00000e30: 7573 6167 652e 2053 6372 6f6c 6c20 6120  usage. Scroll a 
+00000e40: 6269 7420 646f 776e 2074 6f20 7365 6520  bit down to see 
+00000e50: 736f 6d65 2074 6173 7479 2063 6c61 7373  some tasty class
+00000e60: 206d 6574 686f 6473 2e20 2a2a 466f 7220   methods. **For 
+00000e70: 636f 6e73 6973 7465 6e63 7920 6163 726f  consistency acro
+00000e80: 7373 2064 6966 6665 7265 6e74 2064 6576  ss different dev
+00000e90: 6963 6573 2c20 6974 2069 7320 6869 6768  ices, it is high
+00000ea0: 6c79 2072 6563 6f6d 6d65 6e64 6564 2074  ly recommended t
+00000eb0: 6f20 7573 6520 6066 726f 6d6c 696e 6b60  o use `fromlink`
+00000ec0: 2063 6c61 7373 206d 6574 686f 642a 2a2e   class method**.
+00000ed0: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
+00000ee0: 6d20 616d 617a 6f6e 6361 7074 6368 6120  m amazoncaptcha 
+00000ef0: 696d 706f 7274 2041 6d61 7a6f 6e43 6170  import AmazonCap
+00000f00: 7463 6861 0d0a 0d0a 6361 7074 6368 6120  tcha....captcha 
+00000f10: 3d20 416d 617a 6f6e 4361 7074 6368 6128  = AmazonCaptcha(
+00000f20: 2763 6170 7463 6861 2e6a 7067 2729 0d0a  'captcha.jpg')..
+00000f30: 736f 6c75 7469 6f6e 203d 2063 6170 7463  solution = captc
+00000f40: 6861 2e73 6f6c 7665 2829 0d0a 0d0a 2320  ha.solve()....# 
+00000f50: 4f72 3a20 736f 6c75 7469 6f6e 203d 2041  Or: solution = A
+00000f60: 6d61 7a6f 6e43 6170 7463 6861 2827 6361  mazonCaptcha('ca
+00000f70: 7074 6368 612e 6a70 6727 292e 736f 6c76  ptcha.jpg').solv
+00000f80: 6528 290d 0a60 6060 0d0a 0d0a 2323 2053  e()..```....## S
+00000f90: 7461 7475 730d 0a5b 215b 5374 6174 7573  tatus..[![Status
+00000fa0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000fb0: 6965 6c64 732e 696f 2f70 7970 692f 7374  ields.io/pypi/st
+00000fc0: 6174 7573 2f61 6d61 7a6f 6e63 6170 7463  atus/amazoncaptc
+00000fd0: 6861 295d 2868 7474 7073 3a2f 2f70 7970  ha)](https://pyp
+00000fe0: 692e 6f72 672f 7072 6f6a 6563 742f 616d  i.org/project/am
+00000ff0: 617a 6f6e 6361 7074 6368 612f 290d 0a5b  azoncaptcha/)..[
+00001000: 215b 4275 696c 6420 5374 6174 7573 5d28  ![Build Status](
+00001010: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00001020: 6c64 732e 696f 2f63 6972 636c 6563 692f  lds.io/circleci/
+00001030: 6275 696c 642f 6769 7468 7562 2f61 2d6d  build/github/a-m
+00001040: 616c 6961 726f 762f 616d 617a 6f6e 6361  aliarov/amazonca
+00001050: 7074 6368 6129 5d28 6874 7470 733a 2f2f  ptcha)](https://
+00001060: 6170 702e 6369 7263 6c65 6369 2e63 6f6d  app.circleci.com
+00001070: 2f70 6970 656c 696e 6573 2f67 6974 6875  /pipelines/githu
+00001080: 622f 612d 6d61 6c69 6172 6f76 2f61 6d61  b/a-maliarov/ama
+00001090: 7a6f 6e63 6170 7463 6861 290d 0a5b 215b  zoncaptcha)..[![
+000010a0: 446f 6375 6d65 6e74 6174 696f 6e20 5374  Documentation St
+000010b0: 6174 7573 5d28 6874 7470 733a 2f2f 7265  atus](https://re
+000010c0: 6164 7468 6564 6f63 732e 6f72 672f 7072  adthedocs.org/pr
+000010d0: 6f6a 6563 7473 2f61 6d61 7a6f 6e63 6170  ojects/amazoncap
+000010e0: 7463 6861 2f62 6164 6765 2f3f 7665 7273  tcha/badge/?vers
+000010f0: 696f 6e3d 6c61 7465 7374 295d 2868 7474  ion=latest)](htt
+00001100: 7073 3a2f 2f61 6d61 7a6f 6e63 6170 7463  ps://amazoncaptc
+00001110: 6861 2e72 6561 6474 6865 646f 6373 2e69  ha.readthedocs.i
+00001120: 6f2f 656e 2f6c 6174 6573 742f 290d 0a5b  o/en/latest/)..[
+00001130: 215b 436f 6465 2043 6f76 6572 6167 655d  ![Code Coverage]
+00001140: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00001150: 656c 6473 2e69 6f2f 636f 6465 636f 762f  elds.io/codecov/
+00001160: 632f 6768 2f61 2d6d 616c 6961 726f 762f  c/gh/a-maliarov/
+00001170: 616d 617a 6f6e 6361 7074 6368 613f 6c61  amazoncaptcha?la
+00001180: 6265 6c3d 636f 6465 2532 3063 6f76 6572  bel=code%20cover
+00001190: 6167 6529 5d28 6874 7470 733a 2f2f 636f  age)](https://co
+000011a0: 6465 636f 762e 696f 2f67 682f 612d 6d61  decov.io/gh/a-ma
+000011b0: 6c69 6172 6f76 2f61 6d61 7a6f 6e63 6170  liarov/amazoncap
+000011c0: 7463 6861 290d 0a5b 215b 436f 6465 4661  tcha)..[![CodeFa
+000011d0: 6374 6f72 2047 7261 6465 5d28 6874 7470  ctor Grade](http
+000011e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000011f0: 696f 2f63 6f64 6566 6163 746f 722f 6772  io/codefactor/gr
+00001200: 6164 652f 6769 7468 7562 2f61 2d6d 616c  ade/github/a-mal
+00001210: 6961 726f 762f 616d 617a 6f6e 6361 7074  iarov/amazoncapt
+00001220: 6368 612f 6d61 7374 6572 295d 2868 7474  cha/master)](htt
+00001230: 7073 3a2f 2f77 7777 2e63 6f64 6566 6163  ps://www.codefac
+00001240: 746f 722e 696f 2f72 6570 6f73 6974 6f72  tor.io/repositor
+00001250: 792f 6769 7468 7562 2f61 2d6d 616c 6961  y/github/a-malia
+00001260: 726f 762f 616d 617a 6f6e 6361 7074 6368  rov/amazoncaptch
+00001270: 612f 6f76 6572 7669 6577 2f6d 6173 7465  a/overview/maste
+00001280: 7229 0d0a 0d0a 2323 2055 7361 6765 2061  r)....## Usage a
+00001290: 6e64 2043 6c61 7373 204d 6574 686f 6473  nd Class Methods
+000012a0: 0d0a 4272 6f77 7369 6e67 2041 6d61 7a6f  ..Browsing Amazo
+000012b0: 6e20 7573 696e 6720 6073 656c 656e 6975  n using `seleniu
+000012c0: 6d60 2061 6e64 2073 7475 636b 206f 6e20  m` and stuck on 
+000012d0: 6361 7074 6368 613f 2054 6865 2063 6c61  captcha? The cla
+000012e0: 7373 206d 6574 686f 6420 6265 6c6f 7720  ss method below 
+000012f0: 7769 6c6c 2064 6f20 616c 6c20 7468 6520  will do all the 
+00001300: 6469 7274 7920 776f 726b 206f 6620 6578  dirty work of ex
+00001310: 7472 6163 7469 6e67 2061 6e20 696d 6167  tracting an imag
+00001320: 6520 6672 6f6d 2074 6865 2077 6562 7061  e from the webpa
+00001330: 6765 2066 6f72 2079 6f75 2e20 5072 6163  ge for you. Prac
+00001340: 7469 6361 6c6c 792c 2069 7420 7461 6b65  tically, it take
+00001350: 7320 6120 7363 7265 656e 7368 6f74 2066  s a screenshot f
+00001360: 726f 6d20 796f 7572 2077 6562 6472 6976  rom your webdriv
+00001370: 6572 2c20 6372 6f70 7320 7468 6520 6361  er, crops the ca
+00001380: 7074 6368 6120 616e 6420 7374 6f72 6573  ptcha and stores
+00001390: 2069 7420 696e 746f 2062 7974 6573 2061   it into bytes a
+000013a0: 7272 6179 2077 6869 6368 2069 7320 7468  rray which is th
+000013b0: 656e 2075 7365 6420 746f 2063 7265 6174  en used to creat
+000013c0: 6520 616e 2060 416d 617a 6f6e 4361 7074  e an `AmazonCapt
+000013d0: 6368 6160 2069 6e73 7461 6e63 652e 2054  cha` instance. T
+000013e0: 6869 7320 616c 736f 206d 6561 6e73 2061  his also means a
+000013f0: 766f 6964 696e 6720 616e 7920 6c6f 6361  voiding any loca
+00001400: 6c20 7361 7669 6e67 732e 202a 2a46 6f72  l savings. **For
+00001410: 2063 6f6e 7369 7374 656e 6379 2061 6372   consistency acr
+00001420: 6f73 7320 6469 6666 6572 656e 7420 6465  oss different de
+00001430: 7669 6365 732c 2069 7420 6973 2068 6967  vices, it is hig
+00001440: 686c 7920 7265 636f 6d6d 656e 6465 6420  hly recommended 
+00001450: 746f 2075 7365 2060 6672 6f6d 6c69 6e6b  to use `fromlink
+00001460: 6020 636c 6173 7320 6d65 7468 6f64 2069  ` class method i
+00001470: 6e73 7465 6164 206f 6620 6066 726f 6d64  nstead of `fromd
+00001480: 7269 7665 7260 2a2a 2e0d 0a60 6060 7079  river`**...```py
+00001490: 7468 6f6e 0d0a 6672 6f6d 2061 6d61 7a6f  thon..from amazo
+000014a0: 6e63 6170 7463 6861 2069 6d70 6f72 7420  ncaptcha import 
+000014b0: 416d 617a 6f6e 4361 7074 6368 610d 0a66  AmazonCaptcha..f
+000014c0: 726f 6d20 7365 6c65 6e69 756d 2069 6d70  rom selenium imp
+000014d0: 6f72 7420 7765 6264 7269 7665 720d 0a0d  ort webdriver...
+000014e0: 0a64 7269 7665 7220 3d20 7765 6264 7269  .driver = webdri
+000014f0: 7665 722e 4368 726f 6d65 2829 2023 2054  ver.Chrome() # T
+00001500: 6869 7320 6973 2061 2073 696d 706c 6966  his is a simplif
+00001510: 6965 6420 6578 616d 706c 650d 0a64 7269  ied example..dri
+00001520: 7665 722e 6765 7428 2768 7474 7073 3a2f  ver.get('https:/
+00001530: 2f77 7777 2e61 6d61 7a6f 6e2e 636f 6d2f  /www.amazon.com/
+00001540: 6572 726f 7273 2f76 616c 6964 6174 6543  errors/validateC
+00001550: 6170 7463 6861 2729 0d0a 0d0a 6361 7074  aptcha')....capt
+00001560: 6368 6120 3d20 416d 617a 6f6e 4361 7074  cha = AmazonCapt
+00001570: 6368 612e 6672 6f6d 6472 6976 6572 2864  cha.fromdriver(d
+00001580: 7269 7665 7229 0d0a 736f 6c75 7469 6f6e  river)..solution
+00001590: 203d 2063 6170 7463 6861 2e73 6f6c 7665   = captcha.solve
+000015a0: 2829 0d0a 6060 600d 0a0d 0a49 6620 796f  ()..```....If yo
+000015b0: 7520 6172 6520 6e6f 7420 7573 696e 6720  u are not using 
+000015c0: 6073 656c 656e 6975 6d60 206f 7220 7468  `selenium` or th
+000015d0: 6520 7072 6576 696f 7573 206d 6574 686f  e previous metho
+000015e0: 6420 6973 206e 6f74 206a 7573 7420 7468  d is not just th
+000015f0: 6520 6361 7365 2066 6f72 2079 6f75 2c20  e case for you, 
+00001600: 6974 2069 7320 706f 7373 6962 6c65 2074  it is possible t
+00001610: 6f20 7573 6520 6120 6361 7074 6368 6120  o use a captcha 
+00001620: 6c69 6e6b 2064 6972 6563 746c 792e 2054  link directly. T
+00001630: 6869 7320 636c 6173 7320 6d65 7468 6f64  his class method
+00001640: 2077 696c 6c20 7265 7175 6573 7420 7468   will request th
+00001650: 6520 7572 6c2c 2063 6865 636b 2074 6865  e url, check the
+00001660: 2063 6f6e 7465 6e74 2074 7970 6520 616e   content type an
+00001670: 6420 7374 6f72 6520 7468 6520 7265 7370  d store the resp
+00001680: 6f6e 7365 2063 6f6e 7465 6e74 2069 6e74  onse content int
+00001690: 6f20 6279 7465 7320 6172 7261 7920 746f  o bytes array to
+000016a0: 2063 7265 6174 6520 616e 2069 6e73 7461   create an insta
+000016b0: 6e63 6520 6f66 2060 416d 617a 6f6e 4361  nce of `AmazonCa
+000016c0: 7074 6368 6160 2e0d 0a60 6060 7079 7468  ptcha`...```pyth
+000016d0: 6f6e 0d0a 6672 6f6d 2061 6d61 7a6f 6e63  on..from amazonc
+000016e0: 6170 7463 6861 2069 6d70 6f72 7420 416d  aptcha import Am
+000016f0: 617a 6f6e 4361 7074 6368 610d 0a0d 0a6c  azonCaptcha....l
+00001700: 696e 6b20 3d20 2768 7474 7073 3a2f 2f69  ink = 'https://i
+00001710: 6d61 6765 732d 6e61 2e73 736c 2d69 6d61  mages-na.ssl-ima
+00001720: 6765 732d 616d 617a 6f6e 2e63 6f6d 2f63  ges-amazon.com/c
+00001730: 6170 7463 6861 2f75 7376 6d67 6c6f 712f  aptcha/usvmgloq/
+00001740: 4361 7074 6368 615f 6b77 7272 6e71 776b  Captcha_kwrrnqwk
+00001750: 7068 2e6a 7067 270d 0a0d 0a63 6170 7463  ph.jpg'....captc
+00001760: 6861 203d 2041 6d61 7a6f 6e43 6170 7463  ha = AmazonCaptc
+00001770: 6861 2e66 726f 6d6c 696e 6b28 6c69 6e6b  ha.fromlink(link
+00001780: 290d 0a73 6f6c 7574 696f 6e20 3d20 6361  )..solution = ca
+00001790: 7074 6368 612e 736f 6c76 6528 290d 0a60  ptcha.solve()..`
+000017a0: 6060 0d0a 0d0a 496e 2061 6464 6974 696f  ``....In additio
+000017b0: 6e2c 2069 6620 796f 7520 6172 6520 6120  n, if you are a 
+000017c0: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
+000017d0: 206f 7220 6e65 7572 616c 206e 6574 776f   or neural netwo
+000017e0: 726b 2064 6576 656c 6f70 6572 2061 6e64  rk developer and
+000017f0: 2061 7265 206c 6f6f 6b69 6e67 2066 6f72   are looking for
+00001800: 2073 6f6d 6520 7472 6169 6e69 6e67 2064   some training d
+00001810: 6174 612c 2063 6865 636b 205b 7468 6973  ata, check [this
+00001820: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001830: 2e63 6f6d 2f61 2d6d 616c 6961 726f 762f  .com/a-maliarov/
+00001840: 616d 617a 6f6e 2d63 6170 7463 6861 2d64  amazon-captcha-d
+00001850: 6174 6162 6173 6529 2072 6570 6f73 6974  atabase) reposit
+00001860: 6f72 792c 2077 6869 6368 2077 6173 2063  ory, which was c
+00001870: 7265 6174 6564 2074 6f20 7374 6f72 6520  reated to store 
+00001880: 696d 6167 6573 2061 6e64 206f 7468 6572  images and other
+00001890: 206e 6f6e 2d73 6372 6970 7420 6461 7461   non-script data
+000018a0: 2066 6f72 2074 6865 2073 6f6c 7665 722e   for the solver.
+000018b0: 0d0a 0d0a 2323 2048 656c 7020 7468 6520  ....## Help the 
+000018c0: 4465 7665 6c6f 706d 656e 740d 0a49 6620  Development..If 
+000018d0: 796f 7520 6172 6520 7769 6c6c 696e 6720  you are willing 
+000018e0: 746f 2068 656c 7020 7468 6520 6465 7665  to help the deve
+000018f0: 6c6f 706d 656e 742c 2063 6f6e 7369 6465  lopment, conside
+00001900: 7220 7365 7474 696e 6720 606b 6565 705f  r setting `keep_
+00001910: 6c6f 6773 6020 6172 6775 6d65 6e74 206f  logs` argument o
+00001920: 6620 7468 6520 6073 6f6c 7665 6020 6d65  f the `solve` me
+00001930: 7468 6f64 2074 6f20 6054 7275 6560 2e20  thod to `True`. 
+00001940: 4865 7265 2069 7320 7468 6520 6578 616d  Here is the exam
+00001950: 706c 652c 2069 6620 796f 7520 6172 6520  ple, if you are 
+00001960: 7573 696e 6720 6066 726f 6d64 7269 7665  using `fromdrive
+00001970: 7260 2063 6c61 7373 206d 6574 686f 642e  r` class method.
+00001980: 2049 6620 7365 7420 746f 2060 5472 7565   If set to `True
+00001990: 602c 2061 6c6c 2074 6865 206c 696e 6b73  `, all the links
+000019a0: 206f 6620 7468 6520 756e 736f 6c76 6564   of the unsolved
+000019b0: 2063 6170 7463 6861 2077 696c 6c20 6265   captcha will be
+000019c0: 2073 746f 7265 6420 736f 2074 6861 7420   stored so that 
+000019d0: 6c61 7465 7220 796f 7520 6361 6e20 5b6f  later you can [o
+000019e0: 7065 6e20 7468 6520 6973 7375 6520 616e  pen the issue an
+000019f0: 6420 7365 6e64 2074 6865 206c 6f67 735d  d send the logs]
+00001a00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001a10: 636f 6d2f 612d 6d61 6c69 6172 6f76 2f61  com/a-maliarov/a
+00001a20: 6d61 7a6f 6e63 6170 7463 6861 2f69 7373  mazoncaptcha/iss
+00001a30: 7565 732f 6e65 773f 6173 7369 676e 6565  ues/new?assignee
+00001a40: 733d 612d 6d61 6c69 6172 6f76 266c 6162  s=a-maliarov&lab
+00001a50: 656c 733d 7472 6169 6e69 6e67 2b64 6174  els=training+dat
+00001a60: 6126 7465 6d70 6c61 7465 3d73 656e 645f  a&template=send_
+00001a70: 6c6f 6773 2e6d 6426 7469 746c 653d 4164  logs.md&title=Ad
+00001a80: 642b 7472 6169 6e69 6e67 2b64 6174 6129  d+training+data)
+00001a90: 2e0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
+00001aa0: 6f6d 2061 6d61 7a6f 6e63 6170 7463 6861  om amazoncaptcha
+00001ab0: 2069 6d70 6f72 7420 416d 617a 6f6e 4361   import AmazonCa
+00001ac0: 7074 6368 610d 0a66 726f 6d20 7365 6c65  ptcha..from sele
+00001ad0: 6e69 756d 2069 6d70 6f72 7420 7765 6264  nium import webd
+00001ae0: 7269 7665 720d 0a0d 0a64 7269 7665 7220  river....driver 
+00001af0: 3d20 7765 6264 7269 7665 722e 4368 726f  = webdriver.Chro
+00001b00: 6d65 2829 2023 2054 6869 7320 6973 2061  me() # This is a
+00001b10: 2073 696d 706c 6966 6965 6420 6578 616d   simplified exam
+00001b20: 706c 650d 0a64 7269 7665 722e 6765 7428  ple..driver.get(
+00001b30: 2768 7474 7073 3a2f 2f77 7777 2e61 6d61  'https://www.ama
+00001b40: 7a6f 6e2e 636f 6d2f 6572 726f 7273 2f76  zon.com/errors/v
+00001b50: 616c 6964 6174 6543 6170 7463 6861 2729  alidateCaptcha')
+00001b60: 0d0a 0d0a 6361 7074 6368 6120 3d20 416d  ....captcha = Am
+00001b70: 617a 6f6e 4361 7074 6368 612e 6672 6f6d  azonCaptcha.from
+00001b80: 6472 6976 6572 2864 7269 7665 7229 0d0a  driver(driver)..
+00001b90: 736f 6c75 7469 6f6e 203d 2063 6170 7463  solution = captc
+00001ba0: 6861 2e73 6f6c 7665 286b 6565 705f 6c6f  ha.solve(keep_lo
+00001bb0: 6773 3d54 7275 6529 0d0a 6060 600d 0a0d  gs=True)..```...
+00001bc0: 0a49 6620 796f 7520 6861 7665 2061 6e79  .If you have any
+00001bd0: 2073 7567 6765 7374 696f 6e73 206f 7220   suggestions or 
+00001be0: 6964 6561 7320 6f66 2061 6464 6974 696f  ideas of additio
+00001bf0: 6e61 6c20 696e 7374 616e 6365 7320 616e  nal instances an
+00001c00: 6420 6d65 7468 6f64 732c 2077 6869 6368  d methods, which
+00001c10: 2079 6f75 2077 6f75 6c64 206c 696b 6520   you would like 
+00001c20: 746f 2073 6565 2069 6e20 7468 6973 206c  to see in this l
+00001c30: 6962 7261 7279 2c20 706c 6561 7365 2c20  ibrary, please, 
+00001c40: 6665 656c 2066 7265 6520 746f 2063 6f6e  feel free to con
+00001c50: 7461 6374 2074 6865 206f 776e 6572 2076  tact the owner v
+00001c60: 6961 2065 6d61 696c 206f 7220 666f 726b  ia email or fork
+00001c70: 276e 2770 756c 6c20 746f 2072 6570 6f73  'n'pull to repos
+00001c80: 6974 6f72 792e 2041 6e79 2063 6f6e 7472  itory. Any contr
+00001c90: 6962 7574 696f 6e20 6973 2068 6967 686c  ibution is highl
+00001ca0: 7920 6170 7072 6563 6961 7465 6421 0d0a  y appreciated!..
+00001cb0: 0d0a 5b21 5b22 4275 7920 4d65 2041 2043  ..[!["Buy Me A C
+00001cc0: 6f66 6665 6522 5d28 6874 7470 733a 2f2f  offee"](https://
+00001cd0: 7777 772e 6275 796d 6561 636f 6666 6565  www.buymeacoffee
+00001ce0: 2e63 6f6d 2f61 7373 6574 732f 696d 672f  .com/assets/img/
+00001cf0: 6375 7374 6f6d 5f69 6d61 6765 732f 6f72  custom_images/or
+00001d00: 616e 6765 5f69 6d67 2e70 6e67 295d 2868  ange_img.png)](h
+00001d10: 7474 7073 3a2f 2f77 7777 2e62 7579 6d65  ttps://www.buyme
+00001d20: 6163 6f66 6665 652e 636f 6d2f 616d 616c  acoffee.com/amal
+00001d30: 6961 726f 7629 0d0a 0d0a 2323 2041 6464  iarov)....## Add
+00001d40: 6974 696f 6e61 6c0d 0a2b 2049 6620 796f  itional..+ If yo
+00001d50: 7520 7761 6e74 2074 6f20 7365 6520 7468  u want to see th
+00001d60: 6520 5b2a 2a48 6973 746f 7279 206f 6620  e [**History of 
+00001d70: 4368 616e 6765 732a 2a5d 2868 7474 7073  Changes**](https
+00001d80: 3a2f 2f67 6974 6875 622e 636f 6d2f 612d  ://github.com/a-
+00001d90: 6d61 6c69 6172 6f76 2f61 6d61 7a6f 6e63  maliarov/amazonc
+00001da0: 6170 7463 6861 2f62 6c6f 622f 6d61 7374  aptcha/blob/mast
+00001db0: 6572 2f48 4953 544f 5259 2e6d 6429 2c20  er/HISTORY.md), 
+00001dc0: 5b2a 2a43 6f64 6520 6f66 2043 6f6e 6475  [**Code of Condu
+00001dd0: 6374 2a2a 5d28 6874 7470 733a 2f2f 6769  ct**](https://gi
+00001de0: 7468 7562 2e63 6f6d 2f61 2d6d 616c 6961  thub.com/a-malia
+00001df0: 726f 762f 616d 617a 6f6e 6361 7074 6368  rov/amazoncaptch
+00001e00: 612f 626c 6f62 2f6d 6173 7465 722f 2e67  a/blob/master/.g
+00001e10: 6974 6875 622f 434f 4445 5f4f 465f 434f  ithub/CODE_OF_CO
+00001e20: 4e44 5543 542e 6d64 292c 205b 2a2a 436f  NDUCT.md), [**Co
+00001e30: 6e74 7269 6275 7469 6e67 2050 6f6c 6963  ntributing Polic
+00001e40: 792a 2a5d 2868 7474 7073 3a2f 2f67 6974  y**](https://git
+00001e50: 6875 622e 636f 6d2f 612d 6d61 6c69 6172  hub.com/a-maliar
+00001e60: 6f76 2f61 6d61 7a6f 6e63 6170 7463 6861  ov/amazoncaptcha
+00001e70: 2f62 6c6f 622f 6d61 7374 6572 2f2e 6769  /blob/master/.gi
+00001e80: 7468 7562 2f43 4f4e 5452 4942 5554 494e  thub/CONTRIBUTIN
+00001e90: 472e 6d64 292c 206f 7220 5b2a 2a4c 6963  G.md), or [**Lic
+00001ea0: 656e 7365 2a2a 5d28 6874 7470 733a 2f2f  ense**](https://
+00001eb0: 6769 7468 7562 2e63 6f6d 2f61 2d6d 616c  github.com/a-mal
+00001ec0: 6961 726f 762f 616d 617a 6f6e 6361 7074  iarov/amazoncapt
+00001ed0: 6368 612f 626c 6f62 2f6d 6173 7465 722f  cha/blob/master/
+00001ee0: 4c49 4345 4e53 4529 2c20 7573 6520 7468  LICENSE), use th
+00001ef0: 6573 6520 696e 6c69 6e65 206c 696e 6b73  ese inline links
+00001f00: 2074 6f20 6e61 7669 6761 7465 2062 6173   to navigate bas
+00001f10: 6564 206f 6e20 796f 7572 206e 6565 6473  ed on your needs
+00001f20: 2e0d 0a2b 2049 6620 796f 7520 6172 6520  ...+ If you are 
+00001f30: 6661 6369 6e67 2061 6e79 2065 7272 6f72  facing any error
+00001f40: 732c 2070 6c65 6173 652c 2072 6570 6f72  s, please, repor
+00001f50: 7420 796f 7572 2073 6974 7561 7469 6f6e  t your situation
+00001f60: 2076 6961 2061 6e20 6973 7375 652e 0d0a   via an issue...
+00001f70: 2b20 5468 6973 2070 726f 6a65 6374 2069  + This project i
+00001f80: 7320 666f 7220 6564 7563 6174 696f 6e61  s for educationa
+00001f90: 6c20 616e 6420 7265 7365 6172 6368 2070  l and research p
+00001fa0: 7572 706f 7365 7320 6f6e 6c79 2e20 416e  urposes only. An
+00001fb0: 7920 6163 7469 6f6e 7320 616e 642f 6f72  y actions and/or
+00001fc0: 2061 6374 6976 6974 6965 7320 7265 6c61   activities rela
+00001fd0: 7465 6420 746f 2074 6865 206d 6174 6572  ted to the mater
+00001fe0: 6961 6c20 636f 6e74 6169 6e65 6420 6f6e  ial contained on
+00001ff0: 2074 6869 7320 4769 7448 7562 2052 6570   this GitHub Rep
+00002000: 6f73 6974 6f72 7920 6973 2073 6f6c 656c  ository is solel
+00002010: 7920 796f 7572 2072 6573 706f 6e73 6962  y your responsib
+00002020: 696c 6974 792e 2054 6865 2061 7574 686f  ility. The autho
+00002030: 7220 7769 6c6c 206e 6f74 2062 6520 6865  r will not be he
+00002040: 6c64 2072 6573 706f 6e73 6962 6c65 2069  ld responsible i
+00002050: 6e20 7468 6520 6576 656e 7420 616e 7920  n the event any 
+00002060: 6372 696d 696e 616c 2063 6861 7267 6573  criminal charges
+00002070: 2062 6520 6272 6f75 6768 7420 6167 6169   be brought agai
+00002080: 6e73 7420 616e 7920 696e 6469 7669 6475  nst any individu
+00002090: 616c 7320 6d69 7375 7369 6e67 2074 6865  als misusing the
+000020a0: 2069 6e66 6f72 6d61 7469 6f6e 2069 6e20   information in 
+000020b0: 7468 6973 2047 6974 4875 6220 5265 706f  this GitHub Repo
+000020c0: 7369 746f 7279 2074 6f20 6272 6561 6b20  sitory to break 
+000020d0: 7468 6520 6c61 772e 0d0a 2b20 416d 617a  the law...+ Amaz
+000020e0: 6f6e 2069 7320 7468 6520 7265 6769 7374  on is the regist
+000020f0: 6572 6564 2074 7261 6465 6d61 726b 206f  ered trademark o
+00002100: 6620 416d 617a 6f6e 2e63 6f6d 2c20 496e  f Amazon.com, In
+00002110: 632e 2041 6d61 7a6f 6e20 6e61 6d65 2075  c. Amazon name u
+00002120: 7365 6420 696e 2074 6869 7320 7072 6f6a  sed in this proj
+00002130: 6563 7420 6973 2066 6f72 2069 6465 6e74  ect is for ident
+00002140: 6966 6963 6174 696f 6e20 7075 7270 6f73  ification purpos
+00002150: 6573 206f 6e6c 792e 2054 6865 2070 726f  es only. The pro
+00002160: 6a65 6374 2069 7320 6e6f 7420 6173 736f  ject is not asso
+00002170: 6369 6174 6564 2069 6e20 616e 7920 7761  ciated in any wa
+00002180: 7920 7769 7468 2041 6d61 7a6f 6e2e 636f  y with Amazon.co
+00002190: 6d2c 2049 6e63 2e20 616e 6420 6973 206e  m, Inc. and is n
+000021a0: 6f74 2061 6e20 6f66 6669 6369 616c 2073  ot an official s
+000021b0: 6f6c 7574 696f 6e20 6f66 2041 6d61 7a6f  olution of Amazo
+000021c0: 6e2e 636f 6d2c 2049 6e63 2e0d 0a         n.com, Inc...
```

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/__init__.py` & `amazoncaptcha-0.5.9/amazoncaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/devtools.py` & `amazoncaptcha-0.5.9/amazoncaptcha/devtools.py`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/exceptions.py` & `amazoncaptcha-0.5.9/amazoncaptcha/exceptions.py`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/solver.py` & `amazoncaptcha-0.5.9/amazoncaptcha/solver.py`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/A.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/A.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/B.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/B.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/C.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/C.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/E.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/E.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/F.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/F.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/G.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/G.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/H.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/H.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/J.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/J.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/K.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/K.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/L.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/L.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/M.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/M.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/N.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/N.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/P.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/P.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/R.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/R.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/T.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/T.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/U.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/U.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/X.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/X.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/training_data/Y.json` & `amazoncaptcha-0.5.9/amazoncaptcha/training_data/Y.json`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha/utils.py` & `amazoncaptcha-0.5.9/amazoncaptcha/utils.py`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha.egg-info/PKG-INFO` & `amazoncaptcha-0.5.9/amazoncaptcha.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: amazoncaptcha
-Version: 0.5.8
+Version: 0.5.9
 Summary: "Pure Python, lightweight, Pillow-based solver for the Amazon text captcha."
 Home-page: https://github.com/a-maliarov/amazoncaptcha
 Author: Anatolii Maliarov
 Author-email: tly.mov@gmail.com
-License: UNKNOWN
 Project-URL: Documentation, https://amazoncaptcha.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/a-maliarov/amazoncaptcha
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,16 +30,16 @@
 ![Timing](https://img.shields.io/badge/response%20time-0.2s-success)
 [![Size](https://img.shields.io/badge/wheel%20size-0.9%20MB-informational)](https://pypi.org/project/amazoncaptcha/)
 [![Version](https://img.shields.io/pypi/v/amazoncaptcha?color=informational)](https://pypi.org/project/amazoncaptcha/)
 [![Python version](https://img.shields.io/badge/python-3.7%2B-informational)](https://pypi.org/project/amazoncaptcha/)
 [![Downloads](https://img.shields.io/pypi/dm/amazoncaptcha?color=success)](https://pypi.org/project/amazoncaptcha/)
 
 ## Recent News
-+ *July 21, 2022*: tested and approved compatibility with Pillow 9.2.0
-+ *January 25, 2022*: tested and approved compatibility with Python 3.10-dev
++ *January 19, 2023*: tested and approved compatibility with Pillow 9.4.0
++ *January 25, 2022*: tested and approved compatibility with Python 3.10
 + *January 25, 2022*: dropped support for Python 3.6
 
 ## Installation
 You can simply install the library from [PyPi](https://pypi.org/project/amazoncaptcha/) using **pip**. For more methods check the [docs](https://amazoncaptcha.readthedocs.io/en/latest/installation.html).
 ```bash
 pip install amazoncaptcha
 ```
@@ -57,15 +55,14 @@
 # Or: solution = AmazonCaptcha('captcha.jpg').solve()
 ```
 
 ## Status
 [![Status](https://img.shields.io/pypi/status/amazoncaptcha)](https://pypi.org/project/amazoncaptcha/)
 [![Build Status](https://img.shields.io/circleci/build/github/a-maliarov/amazoncaptcha)](https://app.circleci.com/pipelines/github/a-maliarov/amazoncaptcha)
 [![Documentation Status](https://readthedocs.org/projects/amazoncaptcha/badge/?version=latest)](https://amazoncaptcha.readthedocs.io/en/latest/)
-[![Requirements Status](https://requires.io/github/a-maliarov/amazoncaptcha/requirements.svg?branch=master)](https://requires.io/github/a-maliarov/amazoncaptcha/requirements/?branch=master)
 [![Code Coverage](https://img.shields.io/codecov/c/gh/a-maliarov/amazoncaptcha?label=code%20coverage)](https://codecov.io/gh/a-maliarov/amazoncaptcha)
 [![CodeFactor Grade](https://img.shields.io/codefactor/grade/github/a-maliarov/amazoncaptcha/master)](https://www.codefactor.io/repository/github/a-maliarov/amazoncaptcha/overview/master)
 
 ## Usage and Class Methods
 Browsing Amazon using `selenium` and stuck on captcha? The class method below will do all the dirty work of extracting an image from the webpage for you. Practically, it takes a screenshot from your webdriver, crops the captcha and stores it into bytes array which is then used to create an `AmazonCaptcha` instance. This also means avoiding any local savings. **For consistency across different devices, it is highly recommended to use `fromlink` class method instead of `fromdriver`**.
 ```python
 from amazoncaptcha import AmazonCaptcha
@@ -108,9 +105,7 @@
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/amaliarov)
 
 ## Additional
 + If you want to see the [**History of Changes**](https://github.com/a-maliarov/amazoncaptcha/blob/master/HISTORY.md), [**Code of Conduct**](https://github.com/a-maliarov/amazoncaptcha/blob/master/.github/CODE_OF_CONDUCT.md), [**Contributing Policy**](https://github.com/a-maliarov/amazoncaptcha/blob/master/.github/CONTRIBUTING.md), or [**License**](https://github.com/a-maliarov/amazoncaptcha/blob/master/LICENSE), use these inline links to navigate based on your needs.
 + If you are facing any errors, please, report your situation via an issue.
 + This project is for educational and research purposes only. Any actions and/or activities related to the material contained on this GitHub Repository is solely your responsibility. The author will not be held responsible in the event any criminal charges be brought against any individuals misusing the information in this GitHub Repository to break the law.
 + Amazon is the registered trademark of Amazon.com, Inc. Amazon name used in this project is for identification purposes only. The project is not associated in any way with Amazon.com, Inc. and is not an official solution of Amazon.com, Inc.
-
-
```

### Comparing `amazoncaptcha-0.5.8/amazoncaptcha.egg-info/SOURCES.txt` & `amazoncaptcha-0.5.9/amazoncaptcha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazoncaptcha-0.5.8/setup.py` & `amazoncaptcha-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Information Technology",
 ]
 
 requires = [
-    "pillow >= 9.0.1,< 9.3.0",
+    "pillow >= 9.0.1,< 9.5.0",
     "requests >= 2.27.1,< 2.29.0"
 ]
 
 #--------------------------------------------------------------------------------------------------------------
 
 setuptools.setup(
     name=about['__title__'],
```

