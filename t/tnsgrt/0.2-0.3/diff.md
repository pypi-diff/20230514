# Comparing `tmp/tnsgrt-0.2.tar.gz` & `tmp/tnsgrt-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tnsgrt-0.2.tar", last modified: Sun May 14 01:06:50 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `tnsgrt-0.2.tar` & `tnsgrt-0.3.tar`

### file list

```diff
@@ -1,18 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 01:06:50.183207 tnsgrt-0.2/
--rw-rw-rw-   0        0        0     1098 2023-05-12 00:36:53.000000 tnsgrt-0.2/LICENSE
--rw-rw-rw-   0        0        0     2062 2023-05-14 01:06:50.183207 tnsgrt-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      164 2023-05-12 05:06:43.000000 tnsgrt-0.2/README.md
--rw-rw-rw-   0        0        0      822 2023-05-14 01:05:41.000000 tnsgrt-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 01:06:50.183207 tnsgrt-0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 01:06:50.183207 tnsgrt-0.2/tests/
--rw-rw-rw-   0        0        0     1056 2023-05-12 04:29:28.000000 tnsgrt-0.2/tests/test_michell.py
--rw-rw-rw-   0        0        0     2173 2023-05-11 05:29:13.000000 tnsgrt-0.2/tests/test_snelson.py
--rw-rw-rw-   0        0        0     6465 2023-05-13 13:55:14.000000 tnsgrt-0.2/tests/test_stiffness.py
--rw-rw-rw-   0        0        0    39014 2023-05-14 00:03:27.000000 tnsgrt-0.2/tests/test_structure.py
--rw-rw-rw-   0        0        0     1727 2023-05-11 05:29:13.000000 tnsgrt-0.2/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-14 01:06:50.183207 tnsgrt-0.2/tnsgrt.egg-info/
--rw-rw-rw-   0        0        0     2062 2023-05-14 01:06:50.000000 tnsgrt-0.2/tnsgrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-14 01:06:50.000000 tnsgrt-0.2/tnsgrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 01:06:50.000000 tnsgrt-0.2/tnsgrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-14 01:06:50.000000 tnsgrt-0.2/tnsgrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 01:06:50.000000 tnsgrt-0.2/tnsgrt.egg-info/top_level.txt
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 tnsgrt-0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/Makefile
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/conf.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/make.bat
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/requirements.txt
+-rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/loaded.png
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/planar.png
+-rw-r--r--   0        0        0    80392 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/prisms.png
+-rw-r--r--   0        0        0    41183 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson.png
+-rw-r--r--   0        0        0    40684 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson1.png
+-rw-r--r--   0        0        0    40836 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson2.png
+-rw-r--r--   0        0        0    52327 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson3.png
+-rw-r--r--   0        0        0    52431 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson4.png
+-rw-r--r--   0        0        0    56067 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson5.png
+-rw-r--r--   0        0        0    55206 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson6.png
+-rw-r--r--   0        0        0    64370 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson7.png
+-rw-r--r--   0        0        0    19296 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/stiffness1.png
+-rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/examples.rst
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/modules.rst
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/quickstart.rst
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/structure.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/tab1.csv
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/tab2.csv
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/tab3.csv
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/tab4.csv
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/tab5.csv
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/tab6.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tnsgrt-0.3/examples/__init__.py
+-rw-r--r--   0        0        0   428768 2020-02-02 00:00:00.000000 tnsgrt-0.3/examples/examples.ipynb
+-rw-r--r--   0        0        0   176856 2020-02-02 00:00:00.000000 tnsgrt-0.3/examples/quick_start.ipynb
+-rw-r--r--   0        0        0    51229 2020-02-02 00:00:00.000000 tnsgrt-0.3/examples/working_with_structures.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/__init__.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/michell.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/optim.py
+-rw-r--r--   0        0        0     7122 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/prism.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/snelson.py
+-rw-r--r--   0        0        0    20270 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/stiffness.py
+-rw-r--r--   0        0        0    46802 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/structure.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/utils.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/plotter/__init__.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/plotter/matplotlib.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/plotter/plotter.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/plotter/vispy.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 tnsgrt-0.3/tests/test_michell.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tnsgrt-0.3/tests/test_snelson.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 tnsgrt-0.3/tests/test_stiffness.py
+-rw-r--r--   0        0        0    39003 2020-02-02 00:00:00.000000 tnsgrt-0.3/tests/test_structure.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 tnsgrt-0.3/tests/test_utils.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 tnsgrt-0.3/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 tnsgrt-0.3/LICENSE
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 tnsgrt-0.3/README.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 tnsgrt-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 tnsgrt-0.3/PKG-INFO
```

### Comparing `tnsgrt-0.2/LICENSE` & `tnsgrt-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.2/PKG-INFO` & `tnsgrt-0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,64 @@
-Metadata-Version: 2.1
-Name: tnsgrt
-Version: 0.2
-Summary: Python library with support for analysis and design of Tensegrity structures
-Author-email: "Mauricio C. de Oliveira" <mcdeoliveira@duck.com>
-License: MIT License
-        
-        Copyright (c) 2023 Mauricio de Oliveira
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/mcdeoliveira/tensegrity
-Keywords: Tensegrity,structures,trusses
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Other Audience
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# tnsgrt
-
-## Installation
-
-Install with pip by typing:
-
-    pip install tnsgrt
-
-
-## Documentation
-
-See on [read the docs](https://tnsgrt.readthedocs.io).
+Metadata-Version: 2.1
+Name: tnsgrt
+Version: 0.3
+Summary: Python library with support for analysis and design of Tensegrity structures
+Project-URL: Homepage, https://github.com/mcdeoliveira/tensegrity
+Author-email: "Mauricio C. de Oliveira" <mcdeoliveira@duck.com>
+License: MIT License
+        
+        Copyright (c) 2023 Mauricio de Oliveira
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+License-File: LICENSE
+Keywords: Tensegrity,structures,trusses
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Other Audience
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: cvxpy
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: parameterized
+Requires-Dist: scipy
+Requires-Dist: vispy
+Description-Content-Type: text/markdown
+
+# tnsgrt
+
+This package contains classes and functions that facilitate the design and analysis of tensegrity structures.
+It started as a matlab toolbox many years ago written by Mauricio de Oliveira and Joseph Cessna, which is now been
+ported to Python.
+
+It relies heavily on [numpy](https://numpy.org>), [scipy](https://scipy.org), [pandas](https://pandas.org), and
+[cvxpy](https://cvxpy.org) for computations.
+
+Visualization is supported via [matplotlib](https://matplotlib.org) and
+[vispy](https://vispy.org).
+
+## Installation
+
+Install with pip by typing:
+
+    pip install tnsgrt
+
+## Documentation
+
+See on [read the docs](https://tnsgrt.readthedocs.io).
```

### Comparing `tnsgrt-0.2/tests/test_michell.py` & `tnsgrt-0.3/tests/test_michell.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import unittest
 
 import itertools
 from parameterized import parameterized
-import numpy as np
 
 from tnsgrt.michell import Michell
 
 
 class TestMichell(unittest.TestCase):
 
     @parameterized.expand(itertools.product([4, 6, 12], [3, 4, 10, 12]))
```

### Comparing `tnsgrt-0.2/tests/test_snelson.py` & `tnsgrt-0.3/tests/test_snelson.py`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.2/tests/test_stiffness.py` & `tnsgrt-0.3/tests/test_stiffness.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import unittest
 from typing import Optional
 
 import numpy as np
-import scipy
 
 from tnsgrt.prism import Prism
-from tnsgrt.stiffness import Stiffness, NodeConstraint
+from tnsgrt.stiffness import NodeConstraint
 
 
 class TestStiffness(unittest.TestCase):
 
     def test_stiffness(self):
         s = Prism(3)
         S, F, v = s.stiffness()
```

### Comparing `tnsgrt-0.2/tests/test_structure.py` & `tnsgrt-0.3/tests/test_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 import pandas as pd
 import scipy
 
 from tnsgrt import utils
-from tnsgrt.stiffness import NodeConstraint, Stiffness
+from tnsgrt.stiffness import NodeConstraint
 from tnsgrt.structure import Structure
 
 
 class TestStructure(unittest.TestCase):
 
     def test_constructor(self):
```

### Comparing `tnsgrt-0.2/tests/test_utils.py` & `tnsgrt-0.3/tests/test_utils.py`

 * *Files identical despite different names*

