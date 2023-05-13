# Comparing `tmp/xspf-lib-0.2.0.tar.gz` & `tmp/xspf-lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspf-lib-0.2.0.tar", last modified: Sat Feb  6 12:00:03 2021, max compression
+gzip compressed data, was "xspf-lib-0.3.0.tar", last modified: Sat May 13 23:06:31 2023, max compression
```

## Comparing `xspf-lib-0.2.0.tar` & `xspf-lib-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 dem214    (1000) dem214    (1000)        0 2021-02-06 12:00:03.796715 xspf-lib-0.2.0/
--rw-r--r--   0 dem214    (1000) dem214    (1000)     4080 2021-02-06 12:00:03.793382 xspf-lib-0.2.0/PKG-INFO
--rw-r--r--   0 dem214    (1000) dem214    (1000)     2908 2021-02-06 11:42:33.000000 xspf-lib-0.2.0/README.rst
--rw-r--r--   0 dem214    (1000) dem214    (1000)       38 2021-02-06 12:00:03.796715 xspf-lib-0.2.0/setup.cfg
--rw-r--r--   0 dem214    (1000) dem214    (1000)      818 2021-02-06 11:41:28.000000 xspf-lib-0.2.0/setup.py
-drwxr-xr-x   0 dem214    (1000) dem214    (1000)        0 2021-02-06 12:00:03.793382 xspf-lib-0.2.0/test/
--rw-r--r--   0 dem214    (1000) dem214    (1000)     7657 2020-10-12 21:22:50.000000 xspf-lib-0.2.0/test/test_module.py
--rw-r--r--   0 dem214    (1000) dem214    (1000)    11102 2020-10-12 20:10:21.000000 xspf-lib-0.2.0/test/test_testcases_fail_validation.py
--rw-r--r--   0 dem214    (1000) dem214    (1000)     7562 2020-10-12 20:10:21.000000 xspf-lib-0.2.0/test/test_testcases_pass_validation.py
--rw-r--r--   0 dem214    (1000) dem214    (1000)      200 2021-02-06 11:13:49.000000 xspf-lib-0.2.0/test/test_uri.py
-drwxr-xr-x   0 dem214    (1000) dem214    (1000)        0 2021-02-06 12:00:03.793382 xspf-lib-0.2.0/xspf_lib/
--rw-r--r--   0 dem214    (1000) dem214    (1000)    33989 2021-02-06 11:09:50.000000 xspf-lib-0.2.0/xspf_lib/__init__.py
-drwxr-xr-x   0 dem214    (1000) dem214    (1000)        0 2021-02-06 12:00:03.793382 xspf-lib-0.2.0/xspf_lib.egg-info/
--rw-r--r--   0 dem214    (1000) dem214    (1000)     4080 2021-02-06 12:00:03.000000 xspf-lib-0.2.0/xspf_lib.egg-info/PKG-INFO
--rw-r--r--   0 dem214    (1000) dem214    (1000)      283 2021-02-06 12:00:03.000000 xspf-lib-0.2.0/xspf_lib.egg-info/SOURCES.txt
--rw-r--r--   0 dem214    (1000) dem214    (1000)        1 2021-02-06 12:00:03.000000 xspf-lib-0.2.0/xspf_lib.egg-info/dependency_links.txt
--rw-r--r--   0 dem214    (1000) dem214    (1000)        9 2021-02-06 12:00:03.000000 xspf-lib-0.2.0/xspf_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:06:31.407983 xspf-lib-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-13 23:06:31.407983 xspf-lib-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 23:06:31.407983 xspf-lib-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:06:31.407983 xspf-lib-0.3.0/xspf_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:06:31.407983 xspf-lib-0.3.0/xspf_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-13 23:06:31.000000 xspf-lib-0.3.0/xspf_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-13 23:06:31.000000 xspf-lib-0.3.0/xspf_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 23:06:31.000000 xspf-lib-0.3.0/xspf_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-13 23:06:31.000000 xspf-lib-0.3.0/xspf_lib.egg-info/top_level.txt
```

### Comparing `xspf-lib-0.2.0/PKG-INFO` & `xspf-lib-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: xspf-lib
-Version: 0.2.0
+Version: 0.3.0
 Summary: Library for work with xspf format
 Home-page: https://github.com/dem214/xspf-lib
 Author: Dzmitry Izaitka
 Author-email: dem214overlord@gmail.com
 License: UNKNOWN
 Description: ========
         xspf-lib
         ========
         
         .. image:: https://github.com/dem214/xspf-lib/workflows/Python%20package/badge.svg?branch=master
             :alt: Python package
+        .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+            :target: https://pycqa.github.io/isort/
+        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+           :target: https://github.com/psf/black
+        .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+           :target: https://github.com/pre-commit/pre-commit
+           :alt: pre-commit
+        
         
         Library to work with xspf.
         
         Requirements
         ------------
         
         * `Python 3.8 or higher <https://www.python.org/downloads/>`_
@@ -77,9 +85,9 @@
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

#### html2text {}

```diff
@@ -1,13 +1,19 @@
-Metadata-Version: 2.1 Name: xspf-lib Version: 0.2.0 Summary: Library for work
+Metadata-Version: 2.1 Name: xspf-lib Version: 0.3.0 Summary: Library for work
 with xspf format Home-page: https://github.com/dem214/xspf-lib Author: Dzmitry
 Izaitka Author-email: dem214overlord@gmail.com License: UNKNOWN Description:
 ======== xspf-lib ======== .. image:: https://github.com/dem214/xspf-lib/
-workflows/Python%20package/badge.svg?branch=master :alt: Python package Library
-to work with xspf. Requirements ------------ * `Python 3.8 or higher
+workflows/Python%20package/badge.svg?branch=master :alt: Python package ..
+image:: https://img.shields.io/badge/%20imports-isort-
+%231674b1?style=flat&labelColor=ef8336 :target: https://pycqa.github.io/isort/
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg :target:
+https://github.com/psf/black .. image:: https://img.shields.io/badge/pre--
+commit-enabled-brightgreen?logo=pre-commit :target: https://github.com/pre-
+commit/pre-commit :alt: pre-commit Library to work with xspf. Requirements ----
+-------- * `Python 3.8 or higher
 www.python.org/downloads/>`_ Installing ---------- Install and update via
 `pip`_: .. code-block:: text pip install -U xspf-lib Example ------- 1.
 Generating new playlist. >>> import xspf_lib as xspf >>> killer_queen =
 xspf.Track(location="file:///home/music/killer_queen.mp3", title="Killer
 Queen", creator="Queen", album="Sheer Heart Attack", trackNum=2,
 duration=177000, annotation="#2 in GB 1975", info="https://ru.wikipedia.org/
 wiki/Killer_Queen", image="file:///home/images/killer_queen_cover.png") >>>
@@ -30,8 +36,8 @@
 License ------- The license of the project is MIT License - see LICENSE_ file
 for details. .. _LICENSE: https://github.com/dem214/xspf-lib/blob/master/
 LICENSE .. _pip: https://pip.pypa.io/en/stable/quickstart Keywords: xspf
 playlist Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic ::
-Multimedia :: Video Requires-Python: >=3.8 Description-Content-Type: text/x-rst
+Multimedia :: Video Requires-Python: >=3.7 Description-Content-Type: text/x-rst
```

### Comparing `xspf-lib-0.2.0/README.rst` & `xspf-lib-0.3.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 ========
 xspf-lib
 ========
 
 .. image:: https://github.com/dem214/xspf-lib/workflows/Python%20package/badge.svg?branch=master
     :alt: Python package
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+    :target: https://pycqa.github.io/isort/
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
+
 
 Library to work with xspf.
 
 Requirements
 ------------
 
 * `Python 3.8 or higher <https://www.python.org/downloads/>`_
```

#### html2text {}

```diff
@@ -1,10 +1,16 @@
 ======== xspf-lib ======== .. image:: https://github.com/dem214/xspf-lib/
-workflows/Python%20package/badge.svg?branch=master :alt: Python package Library
-to work with xspf. Requirements ------------ * `Python 3.8 or higher
+workflows/Python%20package/badge.svg?branch=master :alt: Python package ..
+image:: https://img.shields.io/badge/%20imports-isort-
+%231674b1?style=flat&labelColor=ef8336 :target: https://pycqa.github.io/isort/
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg :target:
+https://github.com/psf/black .. image:: https://img.shields.io/badge/pre--
+commit-enabled-brightgreen?logo=pre-commit :target: https://github.com/pre-
+commit/pre-commit :alt: pre-commit Library to work with xspf. Requirements ----
+-------- * `Python 3.8 or higher
 www.python.org/downloads/>`_ Installing ---------- Install and update via
 `pip`_: .. code-block:: text pip install -U xspf-lib Example ------- 1.
 Generating new playlist. >>> import xspf_lib as xspf >>> killer_queen =
 xspf.Track(location="file:///home/music/killer_queen.mp3", title="Killer
 Queen", creator="Queen", album="Sheer Heart Attack", trackNum=2,
 duration=177000, annotation="#2 in GB 1975", info="https://ru.wikipedia.org/
 wiki/Killer_Queen", image="file:///home/images/killer_queen_cover.png") >>>
```

### Comparing `xspf-lib-0.2.0/setup.py` & `xspf-lib-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
-with open("README.rst", 'r') as readme:
+with open("README.rst", "r") as readme:
     long_desc = readme.read()
 
 setuptools.setup(
     name="xspf-lib",
-    version="0.2.0",
+    version="0.3.0",
     author="Dzmitry Izaitka",
     author_email="dem214overlord@gmail.com",
     description="Library for work with xspf format",
     long_description=long_desc,
     long_description_content_type="text/x-rst",
     url="https://github.com/dem214/xspf-lib",
     packages=["xspf_lib"],
@@ -17,10 +17,10 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Multimedia :: Sound/Audio",
         "Topic :: Multimedia :: Video",
     ],
-    keywords='xspf playlist',
-    python_requires='>=3.8',
+    keywords="xspf playlist",
+    python_requires=">=3.7",
 )
```

### Comparing `xspf-lib-0.2.0/xspf_lib.egg-info/PKG-INFO` & `xspf-lib-0.3.0/xspf_lib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: xspf-lib
-Version: 0.2.0
+Version: 0.3.0
 Summary: Library for work with xspf format
 Home-page: https://github.com/dem214/xspf-lib
 Author: Dzmitry Izaitka
 Author-email: dem214overlord@gmail.com
 License: UNKNOWN
 Description: ========
         xspf-lib
         ========
         
         .. image:: https://github.com/dem214/xspf-lib/workflows/Python%20package/badge.svg?branch=master
             :alt: Python package
+        .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+            :target: https://pycqa.github.io/isort/
+        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+           :target: https://github.com/psf/black
+        .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+           :target: https://github.com/pre-commit/pre-commit
+           :alt: pre-commit
+        
         
         Library to work with xspf.
         
         Requirements
         ------------
         
         * `Python 3.8 or higher <https://www.python.org/downloads/>`_
@@ -77,9 +85,9 @@
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

#### html2text {}

```diff
@@ -1,13 +1,19 @@
-Metadata-Version: 2.1 Name: xspf-lib Version: 0.2.0 Summary: Library for work
+Metadata-Version: 2.1 Name: xspf-lib Version: 0.3.0 Summary: Library for work
 with xspf format Home-page: https://github.com/dem214/xspf-lib Author: Dzmitry
 Izaitka Author-email: dem214overlord@gmail.com License: UNKNOWN Description:
 ======== xspf-lib ======== .. image:: https://github.com/dem214/xspf-lib/
-workflows/Python%20package/badge.svg?branch=master :alt: Python package Library
-to work with xspf. Requirements ------------ * `Python 3.8 or higher
+workflows/Python%20package/badge.svg?branch=master :alt: Python package ..
+image:: https://img.shields.io/badge/%20imports-isort-
+%231674b1?style=flat&labelColor=ef8336 :target: https://pycqa.github.io/isort/
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg :target:
+https://github.com/psf/black .. image:: https://img.shields.io/badge/pre--
+commit-enabled-brightgreen?logo=pre-commit :target: https://github.com/pre-
+commit/pre-commit :alt: pre-commit Library to work with xspf. Requirements ----
+-------- * `Python 3.8 or higher
 www.python.org/downloads/>`_ Installing ---------- Install and update via
 `pip`_: .. code-block:: text pip install -U xspf-lib Example ------- 1.
 Generating new playlist. >>> import xspf_lib as xspf >>> killer_queen =
 xspf.Track(location="file:///home/music/killer_queen.mp3", title="Killer
 Queen", creator="Queen", album="Sheer Heart Attack", trackNum=2,
 duration=177000, annotation="#2 in GB 1975", info="https://ru.wikipedia.org/
 wiki/Killer_Queen", image="file:///home/images/killer_queen_cover.png") >>>
@@ -30,8 +36,8 @@
 License ------- The license of the project is MIT License - see LICENSE_ file
 for details. .. _LICENSE: https://github.com/dem214/xspf-lib/blob/master/
 LICENSE .. _pip: https://pip.pypa.io/en/stable/quickstart Keywords: xspf
 playlist Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic ::
-Multimedia :: Video Requires-Python: >=3.8 Description-Content-Type: text/x-rst
+Multimedia :: Video Requires-Python: >=3.7 Description-Content-Type: text/x-rst
```

