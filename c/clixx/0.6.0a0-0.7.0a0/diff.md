# Comparing `tmp/clixx-0.6.0a0.tar.gz` & `tmp/clixx-0.7.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clixx-0.6.0a0.tar", last modified: Sat Dec 24 12:07:16 2022, max compression
+gzip compressed data, was "clixx-0.7.0a0.tar", last modified: Sun May 14 07:44:18 2023, max compression
```

## Comparing `clixx-0.6.0a0.tar` & `clixx-0.7.0a0.tar`

### file list

```diff
@@ -1,28 +1,44 @@
-drwxrwxrwx   0        0        0        0 2022-12-24 12:07:16.616934 clixx-0.6.0a0/
--rw-rw-rw-   0        0        0      258 2022-08-20 12:06:12.000000 clixx-0.6.0a0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1082 2022-08-20 12:20:32.000000 clixx-0.6.0a0/LICENSE
--rw-rw-rw-   0        0        0       73 2022-08-17 02:28:13.000000 clixx-0.6.0a0/MANIFEST.in
--rw-rw-rw-   0        0        0     1942 2022-12-24 12:07:16.616934 clixx-0.6.0a0/PKG-INFO
--rw-rw-rw-   0        0        0      694 2022-10-30 07:27:55.000000 clixx-0.6.0a0/README.md
--rw-rw-rw-   0        0        0      649 2022-12-04 07:21:52.000000 clixx-0.6.0a0/pyproject.toml
--rw-rw-rw-   0        0        0     1359 2022-12-24 12:07:16.617934 clixx-0.6.0a0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-24 12:07:16.589929 clixx-0.6.0a0/src/
-drwxrwxrwx   0        0        0        0 2022-12-24 12:07:16.605932 clixx-0.6.0a0/src/clixx/
--rw-rw-rw-   0        0        0     1259 2022-12-24 12:06:13.000000 clixx-0.6.0a0/src/clixx/__init__.py
--rw-rw-rw-   0        0        0     6338 2022-12-03 14:08:20.000000 clixx-0.6.0a0/src/clixx/_rich.py
--rw-rw-rw-   0        0        0    19509 2022-12-08 12:17:21.000000 clixx-0.6.0a0/src/clixx/arguments.py
--rw-rw-rw-   0        0        0     8341 2022-12-24 12:02:53.000000 clixx-0.6.0a0/src/clixx/commands.py
--rw-rw-rw-   0        0        0      235 2022-12-08 12:17:33.000000 clixx-0.6.0a0/src/clixx/constants.py
--rw-rw-rw-   0        0        0     1620 2022-11-13 12:34:28.000000 clixx-0.6.0a0/src/clixx/exceptions.py
--rw-rw-rw-   0        0        0     5411 2022-11-18 02:16:14.000000 clixx-0.6.0a0/src/clixx/groups.py
--rw-rw-rw-   0        0        0    12312 2022-12-04 07:40:14.000000 clixx-0.6.0a0/src/clixx/parsers.py
--rw-rw-rw-   0        0        0     6931 2022-12-04 07:48:17.000000 clixx-0.6.0a0/src/clixx/printers.py
--rw-rw-rw-   0        0        0        0 2022-08-20 08:21:13.000000 clixx-0.6.0a0/src/clixx/py.typed
--rw-rw-rw-   0        0        0    19839 2022-12-05 06:50:35.000000 clixx-0.6.0a0/src/clixx/types.py
-drwxrwxrwx   0        0        0        0 2022-12-24 12:07:16.615934 clixx-0.6.0a0/src/clixx.egg-info/
--rw-rw-rw-   0        0        0     1942 2022-12-24 12:07:16.000000 clixx-0.6.0a0/src/clixx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2022-12-24 12:07:16.000000 clixx-0.6.0a0/src/clixx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-24 12:07:16.000000 clixx-0.6.0a0/src/clixx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-12-24 12:07:16.000000 clixx-0.6.0a0/src/clixx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-12-24 12:07:16.000000 clixx-0.6.0a0/src/clixx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-10-09 02:10:23.000000 clixx-0.6.0a0/src/clixx.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.908827 clixx-0.7.0a0/
+-rw-rw-rw-   0        0        0      258 2022-08-20 12:06:12.000000 clixx-0.7.0a0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1087 2023-02-14 02:01:01.000000 clixx-0.7.0a0/LICENSE
+-rw-rw-rw-   0        0        0      151 2023-05-01 02:49:08.000000 clixx-0.7.0a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2202 2023-05-14 07:44:18.909827 clixx-0.7.0a0/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-05-14 07:39:38.000000 clixx-0.7.0a0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.876828 clixx-0.7.0a0/docs/
+-rw-rw-rw-   0        0        0      638 2022-10-15 01:44:45.000000 clixx-0.7.0a0/docs/Makefile
+-rwxrwxrwx   0        0        0      804 2022-10-15 01:44:45.000000 clixx-0.7.0a0/docs/make.bat
+-rw-rw-rw-   0        0        0      997 2023-05-01 02:56:19.000000 clixx-0.7.0a0/docs/release.py
+-rw-rw-rw-   0        0        0       78 2023-04-28 02:42:53.000000 clixx-0.7.0a0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.879829 clixx-0.7.0a0/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.887828 clixx-0.7.0a0/docs/source/api/
+-rw-rw-rw-   0        0        0      638 2022-11-21 08:42:57.000000 clixx-0.7.0a0/docs/source/api/arguments.rst
+-rw-rw-rw-   0        0        0     1189 2022-11-24 08:57:53.000000 clixx-0.7.0a0/docs/source/api/exceptions.rst
+-rw-rw-rw-   0        0        0      657 2022-11-18 02:37:53.000000 clixx-0.7.0a0/docs/source/api/groups.rst
+-rw-rw-rw-   0        0        0      134 2022-12-04 02:13:38.000000 clixx-0.7.0a0/docs/source/api/index.rst
+-rw-rw-rw-   0        0        0      573 2022-12-04 02:30:04.000000 clixx-0.7.0a0/docs/source/api/printers.rst
+-rw-rw-rw-   0        0        0     1058 2022-11-23 12:44:53.000000 clixx-0.7.0a0/docs/source/api/types.rst
+-rw-rw-rw-   0        0        0     2903 2023-02-15 06:42:24.000000 clixx-0.7.0a0/docs/source/conf.py
+-rw-rw-rw-   0        0        0      810 2022-10-30 07:36:12.000000 clixx-0.7.0a0/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1157 2023-05-01 02:54:06.000000 clixx-0.7.0a0/pyproject.toml
+-rw-rw-rw-   0        0        0     1528 2023-05-14 07:44:18.910828 clixx-0.7.0a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.862829 clixx-0.7.0a0/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.901829 clixx-0.7.0a0/src/clixx/
+-rw-rw-rw-   0        0        0     1814 2023-05-14 07:42:54.000000 clixx-0.7.0a0/src/clixx/__init__.py
+-rw-rw-rw-   0        0        0     6430 2023-01-07 09:23:51.000000 clixx-0.7.0a0/src/clixx/_rich.py
+-rw-rw-rw-   0        0        0    19776 2023-03-14 14:34:27.000000 clixx-0.7.0a0/src/clixx/arguments.py
+-rw-rw-rw-   0        0        0    12117 2023-03-15 03:02:39.000000 clixx-0.7.0a0/src/clixx/commands.py
+-rw-rw-rw-   0        0        0      242 2023-03-14 14:01:46.000000 clixx-0.7.0a0/src/clixx/constants.py
+-rw-rw-rw-   0        0        0    13810 2023-01-09 08:49:13.000000 clixx-0.7.0a0/src/clixx/decorators.py
+-rw-rw-rw-   0        0        0     1620 2022-11-13 12:34:28.000000 clixx-0.7.0a0/src/clixx/exceptions.py
+-rw-rw-rw-   0        0        0     5387 2023-03-17 08:08:59.000000 clixx-0.7.0a0/src/clixx/groups.py
+-rw-rw-rw-   0        0        0    12440 2023-03-15 02:58:49.000000 clixx-0.7.0a0/src/clixx/parsers.py
+-rw-rw-rw-   0        0        0     6902 2023-03-15 03:01:45.000000 clixx-0.7.0a0/src/clixx/printers.py
+-rw-rw-rw-   0        0        0        0 2022-08-20 08:21:13.000000 clixx-0.7.0a0/src/clixx/py.typed
+-rw-rw-rw-   0        0        0    19894 2023-03-14 15:41:00.000000 clixx-0.7.0a0/src/clixx/types.py
+drwxrwxrwx   0        0        0        0 2023-05-14 07:44:18.907827 clixx-0.7.0a0/src/clixx.egg-info/
+-rw-rw-rw-   0        0        0     2202 2023-05-14 07:44:18.000000 clixx-0.7.0a0/src/clixx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      794 2023-05-14 07:44:18.000000 clixx-0.7.0a0/src/clixx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 07:44:18.000000 clixx-0.7.0a0/src/clixx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2023-05-14 07:44:18.000000 clixx-0.7.0a0/src/clixx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-14 07:44:18.000000 clixx-0.7.0a0/src/clixx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-10-09 02:10:23.000000 clixx-0.7.0a0/src/clixx.egg-info/zip-safe
```

### Comparing `clixx-0.6.0a0/LICENSE` & `clixx-0.7.0a0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 xymy
+Copyright (c) 2022-2023 xymy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `clixx-0.6.0a0/PKG-INFO` & `clixx-0.7.0a0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clixx
-Version: 0.6.0a0
+Version: 0.7.0a0
 Summary: Command-line interface parser & framework for Python
 Home-page: https://github.com/xymy/clixx
 Author: xymy
 Author-email: thyfan@163.com
 Maintainer: xymy
 Maintainer-email: thyfan@163.com
 License: MIT
@@ -24,19 +24,30 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: lint
+Provides-Extra: test
 License-File: LICENSE
 
 # CLIXX
 
 [![PyPI](https://img.shields.io/pypi/v/clixx)](https://pypi.org/project/clixx/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/clixx)](https://pypi.org/project/clixx/)
 [![PyPI - Downloads](https://pepy.tech/badge/clixx/month)](https://pepy.tech/project/clixx)
 [![PyPI - License](https://img.shields.io/pypi/l/clixx)](https://pypi.org/project/clixx/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 CLIXX is a command-line interface parser & framework for Python.
+
+## Installation
+
+Install from PyPI:
+
+```shell
+$ pip install clixx
+```
```

### Comparing `clixx-0.6.0a0/README.md` & `clixx-0.7.0a0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,19 @@
-# CLIXX
-
-[![PyPI](https://img.shields.io/pypi/v/clixx)](https://pypi.org/project/clixx/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/clixx)](https://pypi.org/project/clixx/)
-[![PyPI - Downloads](https://pepy.tech/badge/clixx/month)](https://pepy.tech/project/clixx)
-[![PyPI - License](https://img.shields.io/pypi/l/clixx)](https://pypi.org/project/clixx/)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-
-CLIXX is a command-line interface parser & framework for Python.
+# CLIXX
+
+[![PyPI](https://img.shields.io/pypi/v/clixx)](https://pypi.org/project/clixx/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/clixx)](https://pypi.org/project/clixx/)
+[![PyPI - Downloads](https://pepy.tech/badge/clixx/month)](https://pepy.tech/project/clixx)
+[![PyPI - License](https://img.shields.io/pypi/l/clixx)](https://pypi.org/project/clixx/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
+CLIXX is a command-line interface parser & framework for Python.
+
+## Installation
+
+Install from PyPI:
+
+```shell
+$ pip install clixx
+```
```

### Comparing `clixx-0.6.0a0/setup.cfg` & `clixx-0.7.0a0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 00000060: 6520 7061 7273 6572 2026 2066 7261 6d65  e parser & frame
 00000070: 776f 726b 2066 6f72 2050 7974 686f 6e0d  work for Python.
 00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000090: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
 000000a0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
 000000b0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
 000000c0: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
-000000d0: 776e 0d0a 6175 7468 6f72 203d 2078 796d  wn..author = xym
-000000e0: 790d 0a61 7574 686f 725f 656d 6169 6c20  y..author_email 
-000000f0: 3d20 7468 7966 616e 4031 3633 2e63 6f6d  = thyfan@163.com
-00000100: 0d0a 6d61 696e 7461 696e 6572 203d 2078  ..maintainer = x
-00000110: 796d 790d 0a6d 6169 6e74 6169 6e65 725f  ymy..maintainer_
-00000120: 656d 6169 6c20 3d20 7468 7966 616e 4031  email = thyfan@1
-00000130: 3633 2e63 6f6d 0d0a 6c69 6365 6e73 6520  63.com..license 
-00000140: 3d20 4d49 540d 0a6c 6963 656e 7365 5f66  = MIT..license_f
-00000150: 696c 6573 203d 204c 4943 454e 5345 0d0a  iles = LICENSE..
+000000d0: 776e 0d0a 6c69 6365 6e73 6520 3d20 4d49  wn..license = MI
+000000e0: 540d 0a6c 6963 656e 7365 5f66 696c 6573  T..license_files
+000000f0: 203d 204c 4943 454e 5345 0d0a 6175 7468   = LICENSE..auth
+00000100: 6f72 203d 2078 796d 790d 0a61 7574 686f  or = xymy..autho
+00000110: 725f 656d 6169 6c20 3d20 7468 7966 616e  r_email = thyfan
+00000120: 4031 3633 2e63 6f6d 0d0a 6d61 696e 7461  @163.com..mainta
+00000130: 696e 6572 203d 2078 796d 790d 0a6d 6169  iner = xymy..mai
+00000140: 6e74 6169 6e65 725f 656d 6169 6c20 3d20  ntainer_email = 
+00000150: 7468 7966 616e 4031 3633 2e63 6f6d 0d0a  thyfan@163.com..
 00000160: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
 00000170: 7468 7562 2e63 6f6d 2f78 796d 792f 636c  thub.com/xymy/cl
 00000180: 6978 780d 0a70 726f 6a65 6374 5f75 726c  ixx..project_url
 00000190: 7320 3d20 0d0a 0944 6f63 756d 656e 7461  s = ...Documenta
 000001a0: 7469 6f6e 203d 2068 7474 7073 3a2f 2f67  tion = https://g
 000001b0: 6974 6875 622e 636f 6d2f 7879 6d79 2f63  ithub.com/xymy/c
 000001c0: 6c69 7878 0d0a 0949 7373 7565 2054 7261  lixx...Issue Tra
@@ -73,13 +73,24 @@
 00000480: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
 00000490: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
 000004a0: 655f 6461 7461 203d 2054 7275 650d 0a7a  e_data = True..z
 000004b0: 6970 5f73 6166 6520 3d20 5472 7565 0d0a  ip_safe = True..
 000004c0: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
 000004d0: 3d20 3e3d 332e 380d 0a69 6e73 7461 6c6c  = >=3.8..install
 000004e0: 5f72 6571 7569 7265 7320 3d20 0d0a 0972  _requires = ...r
-000004f0: 6963 683e 3d31 322e 300d 0a0d 0a5b 6f70  ich>=12.0....[op
-00000500: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000510: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-00000520: 630d 0a0d 0a5b 6567 675f 696e 666f 5d0d  c....[egg_info].
-00000530: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000540: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+000004f0: 6963 683e 3d31 332e 300d 0a0d 0a5b 6f70  ich>=13.0....[op
+00000500: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
+00000510: 7569 7265 5d0d 0a6c 696e 7420 3d20 0d0a  uire]..lint = ..
+00000520: 0962 6c61 636b 3e3d 3233 2e33 0d0a 0969  .black>=23.3...i
+00000530: 736f 7274 3e3d 352e 3132 0d0a 0972 7566  sort>=5.12...ruf
+00000540: 663e 3d30 2e30 2e32 3630 0d0a 096d 7970  f>=0.0.260...myp
+00000550: 793e 3d31 2e32 0d0a 7465 7374 203d 200d  y>=1.2..test = .
+00000560: 0a09 636f 7665 7261 6765 3e3d 372e 320d  ..coverage>=7.2.
+00000570: 0a09 6879 706f 7468 6573 6973 3e3d 362e  ..hypothesis>=6.
+00000580: 3730 0d0a 0970 7974 6573 743e 3d37 2e32  70...pytest>=7.2
+00000590: 0d0a 0970 7974 6573 742d 636f 763e 3d34  ...pytest-cov>=4
+000005a0: 2e30 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .0....[options.p
+000005b0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+000005c0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
+000005d0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+000005e0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000005f0: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `clixx-0.6.0a0/src/clixx/_rich.py` & `clixx-0.7.0a0/src/clixx/_rich.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,16 @@
 
         for command_group in cmd.iter_command_group():
             if command_group.hidden:
                 continue
             console.print(f"\n{command_group.title}:")
 
             # TODO
+            for cmd_name in command_group:
+                console.print(f"  {cmd_name}")
 
         for option_group in cmd.option_groups:
             if option_group.hidden:
                 continue
             console.print(f"\n{option_group.title}:")
             table = Table(box=None, padding=(0, 0, 0, 2), show_header=False, show_edge=False)
             table.add_column("Options")
```

### Comparing `clixx-0.6.0a0/src/clixx/arguments.py` & `clixx-0.7.0a0/src/clixx/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from keyword import iskeyword
-from typing import Any, Sequence, cast
+from typing import Any, Final, Sequence, cast
 
 from .constants import LONG_PREFIX, LONG_PREFIX_LEN, SHORT_PREFIX, SHORT_PREFIX_LEN
 from .exceptions import DefinitionError, HelpSignal, TypeConversionError, VersionSignal
 from .types import Int, Str, Type, resolve_type
 
 # The reserved characters for arguments and options.
-_RESERVED = "<>'\""
+_RESERVED: Final = frozenset("\"'<>")
 
 
 def _check_dest(dest: str) -> str:
     dest = dest.replace("-", "_")
     if not dest.isidentifier():
         raise DefinitionError(f"{dest!r} is not a valid identifier.")
     if iskeyword(dest):
@@ -56,17 +56,17 @@
                 raise DefinitionError(f"Short option {decl!r} is too long.")
             short_options.append(decl)
         elif not decl:
             raise DefinitionError("Option must be non-empty.")
         else:
             raise DefinitionError(f"Option must start with {LONG_PREFIX!r} or {SHORT_PREFIX!r}, got {decl!r}.")
 
-        for rc in _RESERVED:
-            if rc in decl:
-                raise DefinitionError(f"Option {decl!r} contains reserved character {rc!r}.")
+        if inter := _RESERVED.intersection(decl):
+            inter_str = ", ".join(map(repr, sorted(inter)))
+            raise DefinitionError(f"Option {decl!r} contains reserved character {inter_str}.")
     return long_options, short_options
 
 
 class Argument:
     """The argument, aka positional argument.
 
     Parameters:
@@ -120,15 +120,15 @@
         self.help = help
 
     @staticmethod
     def _parse(decl: str, *, dest: str | None) -> tuple[str, str]:
         argument = _parse_decl(decl)
 
         # Infer destination from declaration if ``dest`` not given.
-        if dest is not None:
+        if dest is not None:  # noqa
             dest = _check_dest(dest) if dest else ""
         else:
             dest = _check_dest(argument)
         return dest, argument
 
     def store(self, args: dict[str, Any], value: str) -> None:
         """Store value to destination."""
@@ -197,15 +197,15 @@
                 value = [self._verify(v) for v in value]
         self._default = value
 
     def _verify(self, value: Any) -> Any:
         try:
             return self.type.safe_convert(value)
         except TypeConversionError as e:
-            raise DefinitionError(f"Invalid default value for argument {self.format_decl()}. {str(e)}")
+            raise DefinitionError(f"Invalid default value for argument {self.format_decl()}. {str(e)}") from e
 
 
 class Option:
     """The option, aka optional argument.
 
     Parameters:
         decls (tuple[str, ...]):
@@ -308,29 +308,33 @@
         elif self.long_options:
             return _norm_metavar(self.long_options[0][LONG_PREFIX_LEN:])
         else:
             return _norm_metavar(self.short_options[0][SHORT_PREFIX_LEN:])
 
     @property
     def nargs(self) -> int:
-        """Return ``1``."""
+        """Return ``1``.
+
+        Note:
+            The option requires exactly one value.
+        """
 
         return 1
 
     @property
     def default(self) -> Any:
         return self._default
 
     @default.setter
     def default(self, value: Any) -> None:
         if value is not None:
             try:
                 value = self.type.safe_convert(value)
             except TypeConversionError as e:
-                raise DefinitionError(f"Invalid default value for option {self.format_decls()}. {str(e)}")
+                raise DefinitionError(f"Invalid default value for option {self.format_decls()}. {str(e)}") from e
         self._default = value
 
 
 class FlagOption(Option):
     """The flag option.
 
     Parameters:
@@ -379,29 +383,33 @@
             return
 
         result = None if self.const is None else self.type(self.const)
         args[self.dest] = result
 
     @property
     def nargs(self) -> int:
-        """Return ``0``."""
+        """Return ``0``.
+
+        Note:
+            The flag option does not take a value.
+        """
 
         return 0
 
     @property
     def const(self) -> Any:
         return self._const
 
     @const.setter
     def const(self, value: Any) -> None:
         if value is not None:
             try:
                 value = self.type.safe_convert(value)
             except TypeConversionError as e:
-                raise DefinitionError(f"Invalid constant value for option {self.format_decls()}. {str(e)}")
+                raise DefinitionError(f"Invalid constant value for option {self.format_decls()}. {str(e)}") from e
         self._const = value
 
 
 class AppendOption(Option):
     """The append option.
 
     Parameters:
```

### Comparing `clixx-0.6.0a0/src/clixx/exceptions.py` & `clixx-0.7.0a0/src/clixx/exceptions.py`

 * *Files identical despite different names*

### Comparing `clixx-0.6.0a0/src/clixx/groups.py` & `clixx-0.7.0a0/src/clixx/groups.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,56 +39,56 @@
 
 class _Group(Generic[T]):
     """The group.
 
     Parameters:
         title (str):
             The group title.
-        hidden (bool, default=False):
+        hidden (bool):
             If ``True``, hide this group from help information.
     """
 
-    def __init__(self, title: str, *, hidden: bool = False) -> None:
+    def __init__(self, title: str, *, hidden: bool) -> None:
         self.title = title
         self.hidden = hidden
         self.members: list[T] = []
 
     def __len__(self) -> int:
         """Return the number of members."""
 
         return len(self.members)
 
     def __iter__(self) -> Iterator[T]:
         """Iterate members."""
 
         yield from self.members
 
-    def __iadd__(self, member: T) -> Self:  # type: ignore [valid-type]
+    def __iadd__(self, member: T) -> Self:
         """Add the member to this group."""
 
         return self.add(member)
 
-    def add(self, member: T) -> Self:  # type: ignore [valid-type]
+    def add(self, member: T) -> Self:
         """Add the member to this group."""
 
         self.members.append(member)
         return self
 
 
 class ArgumentGroup(_Group[Argument]):
     """The argument group.
 
     Parameters:
         title (str):
             The group title.
-        hidden (bool, default=False):
+        hidden (bool, default=True):
             If ``True``, hide this argument group from help information.
     """
 
-    def __init__(self, title: str, *, hidden: bool = False) -> None:
+    def __init__(self, title: str, *, hidden: bool = True) -> None:
         super().__init__(title, hidden=hidden)
 
 
 class OptionGroup(_Group[Option]):
     """The option group.
 
     Parameters:
@@ -110,24 +110,26 @@
         Parameters:
             num_occurred (int):
                 The number of occurred options.
         """
 
         if self.type == ANY:
             return self._check_any(num_occurred)
-        if self.type == ALL:
+        elif self.type == ALL:
             return self._check_all(num_occurred)
-        if self.type == NONE:
+        elif self.type == NONE:
             return self._check_none(num_occurred)
-        if self.type == AT_LEAST_ONE:
+        elif self.type == AT_LEAST_ONE:
             return self._check_at_least_one(num_occurred)
-        if self.type == AT_MOST_ONE:
+        elif self.type == AT_MOST_ONE:
             return self._check_at_most_one(num_occurred)
-        if self.type == EXACTLY_ONE:
+        elif self.type == EXACTLY_ONE:
             return self._check_exactly_one(num_occurred)
+        else:
+            raise AssertionError
 
     def _check_any(self, num_occurred: int) -> None:
         pass
 
     def _check_all(self, num_occurred: int) -> None:
         num_options = len(self)
         if num_occurred != num_options:
```

### Comparing `clixx-0.6.0a0/src/clixx/parsers.py` & `clixx-0.7.0a0/src/clixx/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import weakref
 from contextlib import contextmanager
-from typing import Any, Generator, cast
+from typing import Any, Callable, Generator, cast
 
 from .arguments import Argument, Option
 from .constants import DEST_COMMAND_NAME, LONG_PREFIX, LONG_PREFIX_LEN, SEPARATOR, SHORT_PREFIX, SHORT_PREFIX_LEN
 from .exceptions import (
     InvalidArgumentValue,
     InvalidOptionValue,
     MissingOption,
@@ -18,47 +18,49 @@
     TypeConversionError,
     UnknownOption,
 )
 from .groups import ArgumentGroup, OptionGroup
 
 
 @contextmanager
-def _raise_invalid_argument_value(name: str) -> Generator[None, None, None]:
+def _raise_invalid_argument_value(format_decl: Callable[[], str]) -> Generator[None, None, None]:
     try:
         yield
     except TypeConversionError as e:
-        raise InvalidArgumentValue(f"Invalid value for argument {name}. {str(e)}")
+        name = format_decl()
+        raise InvalidArgumentValue(f"Invalid value for argument {name}. {str(e)}") from e
 
 
 @contextmanager
-def _raise_invalid_option_value(name: str) -> Generator[None, None, None]:
+def _raise_invalid_option_value(format_decls: Callable[[], str]) -> Generator[None, None, None]:
     try:
         yield
     except TypeConversionError as e:
-        raise InvalidOptionValue(f"Invalid value for option {name}. {str(e)}")
+        name = format_decls()
+        raise InvalidOptionValue(f"Invalid value for option {name}. {str(e)}") from e
 
 
 class ArgumentNode:
     def __init__(self, argument: Argument, parent: ArgumentGroupNode) -> None:
         self._argument = argument
         self.parent = cast(ArgumentGroupNode, weakref.proxy(parent))
         self.occurred = False
 
     def _inc_occurred(self) -> None:
         if not self.occurred:
             self.occurred = True
             self.parent.num_occurred += 1
 
     def store(self, args: dict[str, Any], value: str) -> None:
-        with _raise_invalid_argument_value(self.format_decl()):
+        with _raise_invalid_argument_value(self.format_decl):
             self._argument.store(args, value)
         self._inc_occurred()
 
     def store_default(self, args: dict[str, Any]) -> None:
-        with _raise_invalid_argument_value(self.format_decl()):
+        with _raise_invalid_argument_value(self.format_decl):
             self._argument.store_default(args)
 
     def format_decl(self) -> str:
         return self._argument.format_decl()
 
     @property
     def nargs(self) -> int:
@@ -84,25 +86,25 @@
 
     def _inc_occurred(self) -> None:
         if not self.occurred:
             self.occurred = True
             self.parent.num_occurred += 1
 
     def store(self, args: dict[str, Any], value: str, *, key: str) -> None:
-        with _raise_invalid_option_value(repr(key)):
+        with _raise_invalid_option_value(lambda: repr(key)):
             self._option.store(args, value)
         self._inc_occurred()
 
     def store_const(self, args: dict[str, Any]) -> None:
-        with _raise_invalid_option_value(self.format_decls()):
+        with _raise_invalid_option_value(self.format_decls):
             self._option.store_const(args)
         self._inc_occurred()
 
     def store_default(self, args: dict[str, Any]) -> None:
-        with _raise_invalid_option_value(self.format_decls()):
+        with _raise_invalid_option_value(self.format_decls):
             self._option.store_default(args)
 
     def format_decls(self) -> str:
         return self._option.format_decls()
 
     @property
     def nargs(self) -> int:
```

### Comparing `clixx-0.6.0a0/src/clixx/printers.py` & `clixx-0.7.0a0/src/clixx/printers.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     ) -> None:
         self.cmd = cmd
         self.printer_factory = printer_factory
         self.printer_config = printer_config
         self.is_exit = is_exit
         self.is_raise = is_raise
 
-    def __enter__(self) -> Self:  # type: ignore [valid-type]
+    def __enter__(self) -> Self:
         """Attach exception and signal handlers."""
 
         return self
 
     def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> bool:
         """Detach exception and signal handlers."""
```

### Comparing `clixx-0.6.0a0/src/clixx/types.py` & `clixx-0.7.0a0/src/clixx/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from contextlib import suppress
 from typing import IO, Any, Callable, Sequence, cast
 
 from .exceptions import DefinitionError, TypeConversionError
 
 
 def _force_decode(filename: Any) -> str:
-    filename = os.fspath(filename)
-    if isinstance(filename, str):
-        return filename
-    return filename.decode(sys.getfilesystemencoding(), "backslashreplace")
+    fn = os.fspath(filename)
+    if isinstance(fn, str):
+        return fn
+    return fn.decode(sys.getfilesystemencoding(), "backslashreplace")
 
 
 def _resolve_norm(case_sensitive: bool) -> Callable[[str], str]:
     if case_sensitive:
         return str
     return str.casefold
 
@@ -137,25 +137,25 @@
         if isinstance(value, int):
             return value
         raise TypeConversionError(f"{value!r} is not a valid integer.")
 
     def convert_str(self, value: str) -> Any:
         try:
             return int(value, base=self.base)
-        except ValueError:
+        except ValueError as e:
             if self.base in {0, 10}:
-                raise TypeConversionError(f"{value!r} is not a valid integer.")
+                raise TypeConversionError(f"{value!r} is not a valid integer.") from e
             elif self.base == 16:
-                raise TypeConversionError(f"{value!r} is not a valid hexadecimal integer.")
+                raise TypeConversionError(f"{value!r} is not a valid hexadecimal integer.") from e
             elif self.base == 8:
-                raise TypeConversionError(f"{value!r} is not a valid octal integer.")
+                raise TypeConversionError(f"{value!r} is not a valid octal integer.") from e
             elif self.base == 2:
-                raise TypeConversionError(f"{value!r} is not a valid binary integer.")
+                raise TypeConversionError(f"{value!r} is not a valid binary integer.") from e
             else:
-                raise TypeConversionError(f"{value!r} is not a valid integer with base {self.base!r}.")
+                raise TypeConversionError(f"{value!r} is not a valid integer with base {self.base!r}.") from e
 
     def suggest_metavar(self) -> str | None:
         return "INTEGER"
 
 
 class Float(Type):
     """The class used to convert command-line arguments to floating point number.
@@ -170,16 +170,16 @@
         if isinstance(value, float):
             return value
         raise TypeConversionError(f"{value!r} is not a valid floating point number.")
 
     def convert_str(self, value: str) -> Any:
         try:
             return float(value)
-        except ValueError:
-            raise TypeConversionError(f"{value!r} is not a valid floating point number.")
+        except ValueError as e:
+            raise TypeConversionError(f"{value!r} is not a valid floating point number.") from e
 
     def suggest_metavar(self) -> str | None:
         return "FLOAT"
 
 
 class Choice(Type):
     """The class used to convert command-line arguments to string in choices.
@@ -364,15 +364,15 @@
 
     def convert_str(self, value: str) -> Any:
         for format in self.formats:
             with suppress(ValueError):
                 return datetime.datetime.strptime(value, format)
 
         formats_str = ", ".join(map(repr, self.formats))
-        if len(self.formats) == 1:
+        if len(self.formats) == 1:  # noqa
             hint = f"Valid format is {formats_str}."
         else:
             hint = f"Valid formats are {formats_str}."
         raise TypeConversionError(f"{value!r} is not a valid datetime. {hint}")
 
     def suggest_metavar(self) -> str | None:
         return "DATETIME"
@@ -439,15 +439,15 @@
 
     def _open(self, path: str | pathlib.Path) -> IO:
         try:
             return open(  # noqa
                 path, self.mode, self.buffering, encoding=self.encoding, errors=self.errors, newline=self.newline
             )
         except OSError as e:
-            raise TypeConversionError(f"Can not open {str(path)!r}. {e.strerror}.")
+            raise TypeConversionError(f"Can not open {str(path)!r}. {e.strerror}.") from e
 
     def safe_convert(self, value: Any) -> Any:
         if isinstance(value, (str, pathlib.Path)) or hasattr(value, "read") or hasattr(value, "write"):
             return value
         raise TypeConversionError(f"{value!r} is not a valid file.")
 
     def format(self, value: Any) -> str:
@@ -508,18 +508,18 @@
 
     def _check_path(self, path: pathlib.Path) -> pathlib.Path:
         if self.resolve:
             path = path.resolve()
 
         try:
             st = path.stat()
-        except OSError:
+        except OSError as e:
             if not self.exists:
                 return path
-            raise TypeConversionError(f"{str(path)!r} does not exist.")
+            raise TypeConversionError(f"{str(path)!r} does not exist.") from e
 
         self._check_path_stat(path, st)
         if self.readable and not os.access(path, os.R_OK):
             raise TypeConversionError(f"{str(path)!r} is not readable.")
         if self.writable and not os.access(path, os.W_OK):
             raise TypeConversionError(f"{str(path)!r} is not writable.")
         if self.executable and not os.access(path, os.X_OK):
```

### Comparing `clixx-0.6.0a0/src/clixx.egg-info/PKG-INFO` & `clixx-0.7.0a0/src/clixx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clixx
-Version: 0.6.0a0
+Version: 0.7.0a0
 Summary: Command-line interface parser & framework for Python
 Home-page: https://github.com/xymy/clixx
 Author: xymy
 Author-email: thyfan@163.com
 Maintainer: xymy
 Maintainer-email: thyfan@163.com
 License: MIT
@@ -24,19 +24,30 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: lint
+Provides-Extra: test
 License-File: LICENSE
 
 # CLIXX
 
 [![PyPI](https://img.shields.io/pypi/v/clixx)](https://pypi.org/project/clixx/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/clixx)](https://pypi.org/project/clixx/)
 [![PyPI - Downloads](https://pepy.tech/badge/clixx/month)](https://pepy.tech/project/clixx)
 [![PyPI - License](https://img.shields.io/pypi/l/clixx)](https://pypi.org/project/clixx/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 CLIXX is a command-line interface parser & framework for Python.
+
+## Installation
+
+Install from PyPI:
+
+```shell
+$ pip install clixx
+```
```

