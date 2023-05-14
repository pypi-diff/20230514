# Comparing `tmp/tnsgrt-0.3.tar.gz` & `tmp/tnsgrt-0.4.tar.gz`

## Comparing `tnsgrt-0.3.tar` & `tnsgrt-0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 tnsgrt-0.3/.readthedocs.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/Makefile
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/conf.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/make.bat
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/requirements.txt
--rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/loaded.png
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/planar.png
--rw-r--r--   0        0        0    80392 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/prisms.png
--rw-r--r--   0        0        0    41183 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson.png
--rw-r--r--   0        0        0    40684 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson1.png
--rw-r--r--   0        0        0    40836 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson2.png
--rw-r--r--   0        0        0    52327 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson3.png
--rw-r--r--   0        0        0    52431 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson4.png
--rw-r--r--   0        0        0    56067 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson5.png
--rw-r--r--   0        0        0    55206 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson6.png
--rw-r--r--   0        0        0    64370 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/snelson7.png
--rw-r--r--   0        0        0    19296 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/images/stiffness1.png
--rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/examples.rst
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/modules.rst
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/quickstart.rst
--rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/structure.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/tab1.csv
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/tab2.csv
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/tab3.csv
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/tab4.csv
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/tab5.csv
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tnsgrt-0.3/doc/usage/tab6.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tnsgrt-0.3/examples/__init__.py
--rw-r--r--   0        0        0   428768 2020-02-02 00:00:00.000000 tnsgrt-0.3/examples/examples.ipynb
--rw-r--r--   0        0        0   176856 2020-02-02 00:00:00.000000 tnsgrt-0.3/examples/quick_start.ipynb
--rw-r--r--   0        0        0    51229 2020-02-02 00:00:00.000000 tnsgrt-0.3/examples/working_with_structures.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/__init__.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/michell.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/optim.py
--rw-r--r--   0        0        0     7122 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/prism.py
--rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/snelson.py
--rw-r--r--   0        0        0    20270 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/stiffness.py
--rw-r--r--   0        0        0    46802 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/structure.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/utils.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/plotter/__init__.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/plotter/matplotlib.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/plotter/plotter.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 tnsgrt-0.3/src/tnsgrt/plotter/vispy.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 tnsgrt-0.3/tests/test_michell.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tnsgrt-0.3/tests/test_snelson.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 tnsgrt-0.3/tests/test_stiffness.py
--rw-r--r--   0        0        0    39003 2020-02-02 00:00:00.000000 tnsgrt-0.3/tests/test_structure.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 tnsgrt-0.3/tests/test_utils.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 tnsgrt-0.3/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 tnsgrt-0.3/LICENSE
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 tnsgrt-0.3/README.md
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 tnsgrt-0.3/pyproject.toml
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 tnsgrt-0.3/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 tnsgrt-0.4/.readthedocs.yaml
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 tnsgrt-0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/Makefile
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/conf.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/make.bat
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/requirements.txt
+-rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/images/loaded.png
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/images/planar.png
+-rw-r--r--   0        0        0    80392 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/images/prisms.png
+-rw-r--r--   0        0        0    41183 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/images/snelson.png
+-rw-r--r--   0        0        0    40684 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/images/snelson1.png
+-rw-r--r--   0        0        0    40836 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/images/snelson2.png
+-rw-r--r--   0        0        0    52327 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/images/snelson3.png
+-rw-r--r--   0        0        0    52431 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/images/snelson4.png
+-rw-r--r--   0        0        0    56067 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/images/snelson5.png
+-rw-r--r--   0        0        0    55206 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/images/snelson6.png
+-rw-r--r--   0        0        0    64370 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/images/snelson7.png
+-rw-r--r--   0        0        0    19296 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/images/stiffness1.png
+-rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/usage/examples.rst
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/usage/modules.rst
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/usage/quickstart.rst
+-rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/usage/structure.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/usage/tab1.csv
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/usage/tab2.csv
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/usage/tab3.csv
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/usage/tab4.csv
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/usage/tab5.csv
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tnsgrt-0.4/doc/usage/tab6.csv
+-rw-r--r--   0        0        0   428768 2020-02-02 00:00:00.000000 tnsgrt-0.4/examples/examples.ipynb
+-rw-r--r--   0        0        0   176856 2020-02-02 00:00:00.000000 tnsgrt-0.4/examples/quick_start.ipynb
+-rw-r--r--   0        0        0    51229 2020-02-02 00:00:00.000000 tnsgrt-0.4/examples/working_with_structures.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tnsgrt-0.4/src/tnsgrt/__init__.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 tnsgrt-0.4/src/tnsgrt/michell.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 tnsgrt-0.4/src/tnsgrt/optim.py
+-rw-r--r--   0        0        0     6927 2020-02-02 00:00:00.000000 tnsgrt-0.4/src/tnsgrt/prism.py
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 tnsgrt-0.4/src/tnsgrt/snelson.py
+-rw-r--r--   0        0        0    19736 2020-02-02 00:00:00.000000 tnsgrt-0.4/src/tnsgrt/stiffness.py
+-rw-r--r--   0        0        0    45642 2020-02-02 00:00:00.000000 tnsgrt-0.4/src/tnsgrt/structure.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 tnsgrt-0.4/src/tnsgrt/utils.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tnsgrt-0.4/src/tnsgrt/plotter/__init__.py
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 tnsgrt-0.4/src/tnsgrt/plotter/matplotlib.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 tnsgrt-0.4/src/tnsgrt/plotter/plotter.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 tnsgrt-0.4/src/tnsgrt/plotter/vispy.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 tnsgrt-0.4/tests/test_michell.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 tnsgrt-0.4/tests/test_snelson.py
+-rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 tnsgrt-0.4/tests/test_stiffness.py
+-rw-r--r--   0        0        0    38224 2020-02-02 00:00:00.000000 tnsgrt-0.4/tests/test_structure.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tnsgrt-0.4/tests/test_utils.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tnsgrt-0.4/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 tnsgrt-0.4/LICENSE
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 tnsgrt-0.4/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 tnsgrt-0.4/pyproject.toml
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 tnsgrt-0.4/PKG-INFO
```

### Comparing `tnsgrt-0.3/.readthedocs.yaml` & `tnsgrt-0.4/.readthedocs.yaml`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# .readthedocs.yaml
-# Read the Docs configuration file
-# See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
-
-# Required
-version: 2
-
-# Set the version of Python and other tools you might need
-build:
-  os: ubuntu-22.04
-  tools:
-    python: "3.11"
-    # You can also specify other tool versions:
-    # nodejs: "19"
-    # rust: "1.64"
-    # golang: "1.19"
-
-# Build documentation in the docs/ directory with Sphinx
-sphinx:
-   configuration: doc/conf.py
-
-# If using Sphinx, optionally build your docs in additional formats such as PDF
-# formats:
-#    - pdf
-
-# Optionally declare the Python requirements required to build your docs
-python:
-   install:
+# .readthedocs.yaml
+# Read the Docs configuration file
+# See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
+
+# Required
+version: 2
+
+# Set the version of Python and other tools you might need
+build:
+  os: ubuntu-22.04
+  tools:
+    python: "3.11"
+    # You can also specify other tool versions:
+    # nodejs: "19"
+    # rust: "1.64"
+    # golang: "1.19"
+
+# Build documentation in the docs/ directory with Sphinx
+sphinx:
+   configuration: doc/conf.py
+
+# If using Sphinx, optionally build your docs in additional formats such as PDF
+# formats:
+#    - pdf
+
+# Optionally declare the Python requirements required to build your docs
+python:
+   install:
    - requirements: doc/requirements.txt
```

### Comparing `tnsgrt-0.3/doc/Makefile` & `tnsgrt-0.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/conf.py` & `tnsgrt-0.4/doc/conf.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# For the full list of built-in configuration values, see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-import os
-import sys
-import pathlib
-
-
-# sys.path.insert(0, os.path.abspath('../src'))
-path = pathlib.Path(__file__).resolve() / '..' / '..' / 'src'
-sys.path.insert(0, os.path.abspath(path))
-
-# -- Project information -----------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
-
-project = 'tnsgrt'
-copyright = '2023, Mauricio de Oliveira'
-author = 'Mauricio de Oliveira'
-
-# -- General configuration ---------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
-
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.mathjax']
-
-templates_path = ['_templates']
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-
-
-# -- Options for HTML output -------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
-
-html_theme = 'sphinx_rtd_theme'
-html_static_path = ['_static']
-html_theme_options = {
-    "navigation_depth": 4,
-    "includehidden": True
+# Configuration file for the Sphinx documentation builder.
+#
+# For the full list of built-in configuration values, see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+import os
+import sys
+import pathlib
+
+
+# sys.path.insert(0, os.path.abspath('../src'))
+path = pathlib.Path(__file__).resolve() / '..' / '..' / 'src'
+sys.path.insert(0, os.path.abspath(path))
+
+# -- Project information -----------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
+
+project = 'tnsgrt'
+copyright = '2023, Mauricio de Oliveira'
+author = 'Mauricio de Oliveira'
+
+# -- General configuration ---------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
+
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.mathjax']
+
+templates_path = ['_templates']
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+
+
+# -- Options for HTML output -------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
+
+html_theme = 'sphinx_rtd_theme'
+html_static_path = ['_static']
+html_theme_options = {
+    "navigation_depth": 4,
+    "includehidden": True
 }
```

### Comparing `tnsgrt-0.3/doc/index.rst` & `tnsgrt-0.4/doc/index.rst`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-.. tnsgrt documentation master file, created by
-   sphinx-quickstart on Sat May  6 16:31:07 2023.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
-
-Welcome to tnsgrt's documentation!
-======================================
-
-This package contains classes and functions that facilitate the design and analysis of tensegrity structures.
-It started as a matlab toolbox many years ago written by Mauricio de Oliveira and Joseph Cessna, which is now been
-ported to Python.
-
-It relies heavily on `numpy <https://numpy.org>`_, `scipy <https://scipy.org>`_, `pandas <https://pandas.org>`_, and
-`cvxpy <https://cvxpy.org>`_ for computations.
-
-Visualization is supported via `matplotlib <https://matplotlib.org>`_ and
-`vispy <https://vispy.org>`_.
-
-.. toctree::
-   :maxdepth: 2
-   :caption: User guide
-
-   usage/quickstart
-   usage/structure
-   usage/examples
-
-.. toctree::
-   :maxdepth: 3
-   :caption: Reference
-
-   usage/modules
-
-Indices and tables
-==================
-
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+.. tnsgrt documentation master file, created by
+   sphinx-quickstart on Sat May  6 16:31:07 2023.
+   You can adapt this file completely to your liking, but it should at least
+   contain the root `toctree` directive.
+
+Welcome to tnsgrt's documentation!
+======================================
+
+This package contains classes and functions that facilitate the design and analysis of tensegrity structures.
+It started as a matlab toolbox many years ago written by Mauricio de Oliveira and Joseph Cessna, which is now been
+ported to Python.
+
+It relies heavily on `numpy <https://numpy.org>`_, `scipy <https://scipy.org>`_, `pandas <https://pandas.org>`_, and
+`cvxpy <https://cvxpy.org>`_ for computations.
+
+Visualization is supported via `matplotlib <https://matplotlib.org>`_ and
+`vispy <https://vispy.org>`_.
+
+.. toctree::
+   :maxdepth: 2
+   :caption: User guide
+
+   usage/quickstart
+   usage/structure
+   usage/examples
+
+.. toctree::
+   :maxdepth: 3
+   :caption: Reference
+
+   usage/modules
+
+Indices and tables
+==================
+
+* :ref:`genindex`
+* :ref:`modindex`
+* :ref:`search`
```

### Comparing `tnsgrt-0.3/doc/make.bat` & `tnsgrt-0.4/doc/make.bat`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=sphinx-build
-)
-set SOURCEDIR=.
-set BUILDDIR=_build
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
-	echo.installed, then set the SPHINXBUILD environment variable to point
-	echo.to the full path of the 'sphinx-build' executable. Alternatively you
-	echo.may add the Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.https://www.sphinx-doc.org/
-	exit /b 1
-)
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=sphinx-build
+)
+set SOURCEDIR=.
+set BUILDDIR=_build
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+	echo.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.https://www.sphinx-doc.org/
+	exit /b 1
+)
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+
+:end
+popd
```

### Comparing `tnsgrt-0.3/doc/images/loaded.png` & `tnsgrt-0.4/doc/images/loaded.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/images/planar.png` & `tnsgrt-0.4/doc/images/planar.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/images/prisms.png` & `tnsgrt-0.4/doc/images/prisms.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/images/snelson.png` & `tnsgrt-0.4/doc/images/snelson.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/images/snelson1.png` & `tnsgrt-0.4/doc/images/snelson1.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/images/snelson2.png` & `tnsgrt-0.4/doc/images/snelson2.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/images/snelson3.png` & `tnsgrt-0.4/doc/images/snelson3.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/images/snelson4.png` & `tnsgrt-0.4/doc/images/snelson4.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/images/snelson5.png` & `tnsgrt-0.4/doc/images/snelson5.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/images/snelson6.png` & `tnsgrt-0.4/doc/images/snelson6.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/images/snelson7.png` & `tnsgrt-0.4/doc/images/snelson7.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/images/stiffness1.png` & `tnsgrt-0.4/doc/images/stiffness1.png`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/usage/examples.rst` & `tnsgrt-0.4/doc/usage/examples.rst`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/doc/usage/quickstart.rst` & `tnsgrt-0.4/doc/usage/quickstart.rst`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-Quick start
-===========
-
-Installation
-------------
-
-Install using pip
-
-.. code-block:: python
-
-    pip install tnsgrt
-
-See `matplotlib <https://matplotlib.org>`_ and `vispy <https://vispy.org>`_ for tweaking visualization settings.
-
-Source code
------------
-
-Code corresponding to the sections in this guide are distributed in the form of Jupiter notebooks and can be found at
-the `examples directory <https://github.com/mcdeoliveira/tensegrity/tree/main/examples>`_
-in the `source code repo <https://github.com/mcdeoliveira/tensegrity>`_.
-
-Hello World
------------
-
-Try the following code
-
-.. code-block:: python
-
-    from tnsgrt.prism import Prism
-    s = Prism()
-
-The object ``s`` is a :class:`tnsgrt.structure.Structure` representing a **Snelson Tensegrity Prism** with three
-bars and nine strings such as the one in the following figure:
-
-.. image:: /images/snelson1.png
-   :scale: 50%
-
-The structure can be visualized using `matplotlib <https://matplotlib.org>`_
-
-.. code-block:: python
-
-    from matplotlib import pyplot as plt
-    # add your favorite matplotlib magic below
-    %matplotlib widget
-
-and :class:`tnsgrt.plotter.MatplotlibPlotter`
-
-.. code-block:: python
-
-    from tnsgrt.plotter.matplotlib import MatplotlibPlotter
-
-to produce a 3D plot like the one in the figure above
-
-.. code-block:: python
-
-    plotter = MatplotlibPlotter()
-    plotter.plot(s)
-    plt.axis('equal')
-    plt.axis('off')
-    plt.show()
-
-The underlying ``figure`` and ``axis`` can be retrieved and used to manipulate the plot
-
-.. code-block:: python
-
-    fig, ax = plotter.get_handles()
-    ax.view_init(elev=20, azim=45, roll=0)
-    plt.show()
-
-which in this case rotates the plot to obtain the better viewpoint
-
-.. image:: /images/snelson2.png
-  :scale: 50%
-
-Prisms, lots of prisms
-----------------------
-
-It is possible to construct Snelson prisms with different number of bars
-
-.. code-block:: python
-
-    prisms = [Prism(n) for n in (3, 4, 6, 12)]
-
-All prisms are constructed centered at the origin. They can be translated
-
-.. code-block:: python
-
-    import numpy as np
-    prisms = [prism.translate(np.array([3*i,0,0])) for i, prism in enumerate(prisms)]
-
-before plotting
-
-.. code-block:: python
-
-    plotter = MatplotlibPlotter()
-    plotter.plot(prisms)
-    plt.axis('equal')
-    plt.axis('off')
-    plt.show()
-    fig, ax = plotter.get_handles()
-    ax.view_init(elev=30, azim=60)
-    ax.set_box_aspect(None, zoom=1.8)
-
-to produce a plot such as:
-
-.. image:: /images/prisms.png
-  :scale: 50%
-
-Plotting with VisPy
--------------------
-
-It is also possible to plot structures using `VisPy <https://vispy.org/>`_.
-Certain users might need to tweak their installations.
-See `installation instructions <https://vispy.org/installation.html>`_ for details.
-
-The above prisms can be plotted with VisPy
-
-.. code-block:: python
-
-    from IPython.display import display
-    import jupyter_rfb
-    from tnsgrt.plotter.vispy import VisPyPlotter
-    plotter = VisPyPlotter(scene={'size': (800,200), 'app': 'jupyter_rfb'},
-                           camera={'scale_factor': 6, 'center': (4.5,2,0)})
-    plotter.plot(prisms)
-    plotter.get_canvas()
-
+Quick start
+===========
+
+Installation
+------------
+
+Install using pip
+
+.. code-block:: python
+
+    pip install tnsgrt
+
+See `matplotlib <https://matplotlib.org>`_ and `vispy <https://vispy.org>`_ for tweaking visualization settings.
+
+Source code
+-----------
+
+Code corresponding to the sections in this guide are distributed in the form of Jupiter notebooks and can be found at
+the `examples directory <https://github.com/mcdeoliveira/tensegrity/tree/main/examples>`_
+in the `source code repo <https://github.com/mcdeoliveira/tensegrity>`_.
+
+Hello World
+-----------
+
+Try the following code
+
+.. code-block:: python
+
+    from tnsgrt.prism import Prism
+    s = Prism()
+
+The object ``s`` is a :class:`tnsgrt.structure.Structure` representing a **Snelson Tensegrity Prism** with three
+bars and nine strings such as the one in the following figure:
+
+.. image:: /images/snelson1.png
+   :scale: 50%
+
+The structure can be visualized using `matplotlib <https://matplotlib.org>`_
+
+.. code-block:: python
+
+    from matplotlib import pyplot as plt
+    # add your favorite matplotlib magic below
+    %matplotlib widget
+
+and :class:`tnsgrt.plotter.MatplotlibPlotter`
+
+.. code-block:: python
+
+    from tnsgrt.plotter.matplotlib import MatplotlibPlotter
+
+to produce a 3D plot like the one in the figure above
+
+.. code-block:: python
+
+    plotter = MatplotlibPlotter()
+    plotter.plot(s)
+    plt.axis('equal')
+    plt.axis('off')
+    plt.show()
+
+The underlying ``figure`` and ``axis`` can be retrieved and used to manipulate the plot
+
+.. code-block:: python
+
+    fig, ax = plotter.get_handles()
+    ax.view_init(elev=20, azim=45, roll=0)
+    plt.show()
+
+which in this case rotates the plot to obtain the better viewpoint
+
+.. image:: /images/snelson2.png
+  :scale: 50%
+
+Prisms, lots of prisms
+----------------------
+
+It is possible to construct Snelson prisms with different number of bars
+
+.. code-block:: python
+
+    prisms = [Prism(n) for n in (3, 4, 6, 12)]
+
+All prisms are constructed centered at the origin. They can be translated
+
+.. code-block:: python
+
+    import numpy as np
+    prisms = [prism.translate(np.array([3*i,0,0])) for i, prism in enumerate(prisms)]
+
+before plotting
+
+.. code-block:: python
+
+    plotter = MatplotlibPlotter()
+    plotter.plot(prisms)
+    plt.axis('equal')
+    plt.axis('off')
+    plt.show()
+    fig, ax = plotter.get_handles()
+    ax.view_init(elev=30, azim=60)
+    ax.set_box_aspect(None, zoom=1.8)
+
+to produce a plot such as:
+
+.. image:: /images/prisms.png
+  :scale: 50%
+
+Plotting with VisPy
+-------------------
+
+It is also possible to plot structures using `VisPy <https://vispy.org/>`_.
+Certain users might need to tweak their installations.
+See `installation instructions <https://vispy.org/installation.html>`_ for details.
+
+The above prisms can be plotted with VisPy
+
+.. code-block:: python
+
+    from IPython.display import display
+    import jupyter_rfb
+    from tnsgrt.plotter.vispy import VisPyPlotter
+    plotter = VisPyPlotter(scene={'size': (800,200), 'app': 'jupyter_rfb'},
+                           camera={'scale_factor': 6, 'center': (4.5,2,0)})
+    plotter.plot(prisms)
+    plotter.get_canvas()
+
```

### Comparing `tnsgrt-0.3/doc/usage/structure.rst` & `tnsgrt-0.4/doc/usage/structure.rst`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,362 +1,362 @@
-Working with Structures
-=======================
-
-The prisms seen in the quick start are members of :class:`tnsgrt.structure.Structure`. In fact,
-:class:`tnsgrt.prism.Prism` overloads only the constructor of :class:`tnsgrt.structure.Structure`, which provides most
-of the functionality.
-
-Construction
-------------
-
-Object of class :class:`tnsgrt.structure.Structure` are composed of *nodes* and *members*.
-Nodes are `3 x n` numpy arrays:
-
-.. code-block:: python
-
-    import numpy as np
-    nodes = np.array([[0,0,0],[0,1,0],[1,0,0],[1,1,0]]).transpose()
-
-Members are *bars* or *strings*, which are specified by a `2 x m` array with the indices of the nodes that define the
-members, as in:
-
-.. code-block:: python
-
-    members = np.array([[0,1],[1,2],[2,3],[3,0],[0,2],[1,3]]).transpose()
-
-Nodes and members are then combined to build a :class:`tnsgrt.structure.Structure`:
-
-.. code-block:: python
-
-    from tnsgrt import Structure
-    s = Structure(nodes, members, number_of_strings=4)
-
-The parameter ``number_of_strings = 4`` means that the first four members are to be considered strings.
-
-As before, the resulting structure can be plotted using :class:`tnsgrt.plotter.MatplotlibPlotter`:
-
-.. code-block:: python
-
-    from tnsgrt.plotter.matplotlib import MatplotlibPlotter
-    plotter = MatplotlibPlotter()
-    plotter.plot(s)
-    fig, ax = plotter.get_handles()
-    ax.view_init(-90,0)
-
-to visualize the resulting planar tensegrity structure below:
-
-.. image:: /images/planar.png
-  :scale: 50%
-
-Equilibrium
------------
-
-Once a structure is built, one can perform various calculations. For example one can determine the member forces so that
-the structure is in equilibrium in various cases.
-
-The key method is :meth:`tnsgrt.structure.Structure.equilibrium`, which calculates the internal forces required to
-maintain a structure in equilibrium. It is assumed that all nodes act as *ball joints*.
-
-Unloaded
-^^^^^^^^
-
-In the *unloaded* case, no external forces are applied to the structure, and equilibrium is achieved by *pretensioning*
-the structure. The result of calling :meth:`tnsgrt.structure.Structure.equilibrium`, as in
-
-.. code-block:: python
-
-    s.equilibrium()
-
-is a set of *force coefficients*, which are forces divided by member length.
-
-The result of the equilibrium calculation can be found in the member properties
-`lambda_` (the force coefficient) and `force`:
-
-.. code-block:: python
-
-    s.member_properties[['lambda_', 'force']]
-
-which, in this example, returns:
-
-.. csv-table::
-   :file: tab1.csv
-   :header-rows: 1
-
-Pretension is set so that the average of the magnitude of the force coefficient on all bars is equal to the parameter
-``lambda_bar``, which is by default equal to one.
-
-Loaded
-^^^^^^
-
-In this case an equilibrium is sought in the presence of external forces, given as a `3 x n` array as the following one:
-
-.. code-block:: python
-
-    f = 0.125*np.array([[0,1,0],[0,-1,0],[0,-2,0],[0,2,0]]).transpose()
-
-Each column is to be interpreted as a force vector to be applied at the corresponding node.
-
-The external force array ``f`` can then be passed on to the method :meth:`tnsgrt.structure.Structure.equilibrium`:
-
-.. code-block:: python
-
-    s.equilibrium(f)
-
-resulting in the new set of member forces and force coefficients:
-
-.. code-block:: python
-
-    s.member_properties[['lambda_', 'force']]
-
-that returns:
-
-.. csv-table::
-   :file: tab2.csv
-   :header-rows: 1
-
-The following code produces a visualization of the applied forces superimposed on the structure:
-
-.. code-block:: python
-
-    plotter = MatplotlibPlotter()
-    plotter.plot(s)
-    fig, ax = plotter.get_handles()
-    ax.quiver(s.nodes[0,:], s.nodes[1,:], s.nodes[2,:], f[0,:], f[1,:], f[2,:], arrow_length_ratio=0.2, color='g')
-    ax.view_init(90,-90)
-    ax.axis('off')
-    plt.show()
-
-resulting in a figure like
-
-.. image:: /images/loaded.png
-   :scale: 50%
-
-The forces are represented by the green arrows.
-
-When it is not possible to find a set of internal forces that satisfy the equilibrium conditions an Exception with a
-message "could not find equilibrium" is produced. For example:
-
-.. code-block:: python
-
-    f = 0.125*np.array([[0,1,0],[0,-1,0],[0,-1,0],[0,2,0]]).transpose()
-    s.equilibrium(f)
-
-can not be in equilibrium.
-
-Stiffness
----------
-
-Once a structure is in equilibrium, its response to forces can be calculated in terms of its *stiffness matrix*. For
-that it is necessary to characterize the members' geometry and material properties. The fundamental properties are the
-member radius, and elasticity modulus:
-
-.. code-block:: python
-
-    s.member_properties[['radius', 'inner_radius', 'modulus']]
-
-The current default values for such properties are:
-
-.. csv-table::
-   :file: tab3.csv
-   :header-rows: 1
-
-For calculating the stiffness matrix of a pretensioned structure, it is also necessary to know the member's force
-coefficient and the derived member stiffness property. As seen before, the force coefficient and the force are obtained
-during the equilibrium calculation:
-
-.. code-block:: python
-
-    s.equilibrium()
-    s.member_properties[['lambda_', 'force', 'stiffness']]
-
-which returns:
-
-.. csv-table::
-   :file: tab4.csv
-   :header-rows: 1
-
-Because the stiffness is a "derived" property, it does not get automatically populated, which can be done by calling
-:meth:`tnsgrt.structure.Structure.update_member_properties`:
-
-.. code-block:: python
-
-    s.update_member_properties('stiffness')
-    s.member_properties[['stiffness']]
-
-to obtain:
-
-.. csv-table::
-   :file: tab5.csv
-   :header-rows: 1
-
-After setting the material properties, one can calculate the stiffness model associated with the current equilibrium:
-
-.. code-block:: python
-
-    stiffness, _, _ = s.stiffness()
-
-For large models, the stiffness is stored and calculated as sparse arrays. However, for small models, such as this one,
-the model is stored in dense arrays. The warning message can be suppressed by explicitly setting the parameter
-``storage=dense``:
-
-.. code-block:: python
-
-    stiffness, _, _ = s.stiffness(storage='dense')
-
-**WARNING:** setting ``storage='dense'`` for large models is not advised.
-
-Rigid-body constraints
-^^^^^^^^^^^^^^^^^^^^^^
-
-The stiffness model can be used to calculate various quantities of interest. For example:
-
-.. code-block:: python
-
-    d, v = stiffness.eigs()
-
-returns the eigenvalues and eigenvectors of the stiffness matrix. In this case, because there are no constraints in the
-structure, we should expect to encounter various eigenvalues numerically close to zero:
-
-.. code-block:: python
-
-    d
-
-returns:
-
-.. code::
-
-    -6.237207e-09
-    -4.329203e-10
-    1.415459e-11
-    9.183017e-10
-    4.478545e-09
-    7.290895e-09
-    4.000000e+00
-    3.141592e+07
-    3.141593e+07
-    3.141593e+07
-
-
-Six of these are the so-called "rigid body modes," associated to rigid translations and rotations of the structure.
-They can be "removed" by applying certain constraints to the set of allowed displacements. Enforcement of these
-constraints can be done by passing the parameter ``apply_rigid_body_constraint=True`` when calculating the stiffness
-model:
-
-.. code-block:: python
-
-    stiffness, _, _ = s.stiffness(storage='dense', apply_rigid_body_constraint=True)
-
-To see that the six near zero eigenvalues of the stiffness matrix have been removed by the rigid body constraints
-recalculate:
-
-.. code-block:: python
-
-    d, v = stiffness.eigs()
-    d
-
-to obtain:
-
-.. code::
-
-    4.000000e+00
-    3.141592e+07
-    3.141593e+07
-    3.141593e+07
-    8.885766e+07
-    1.202736e+08
-
-Interestingly, in this case, there still remains one eigenvalue that is much smaller than the rest.
-We shall deal with this small eigenvalue later.
-
-For now, even though the smallest eigenvalue is small, the resulting stiffness matrix is not singular, and therefore
-suitable for computing displacements. This time:
-
-.. code-block:: python
-
-    x = stiffness.displacements(f)
-    x
-
-successfully calculates the resulting approximate displacements:
-
-.. code::
-
-    -2.20468248e-09, -2.20468248e-09,  2.20468248e-09,  2.20468248e-09
-     1.77419161e-09, -1.77419161e-09, -5.75306493e-09,  5.75306493e-09
-     4.02657501e-18, -4.02657481e-18,  4.02657460e-18, -4.02657419e-18
-
-which can be visualized, after much enlargement, along with the applied forces in the figure:
-
-.. image:: /images/stiffness1.png
-    :scale: 50%
-
-in which the forces are in green and the vectors indicating the resulting displacement are in yellow.
-This figure is generated by the code:
-
-.. code-block:: python
-
-    X = f
-    Y = 5e7*x
-
-    plotter = MatplotlibPlotter()
-    plotter.plot(s)
-    fig, ax = plotter.get_handles()
-    ax.quiver(s.nodes[0,:], s.nodes[1,:], s.nodes[2,:], X[0,:], X[1,:], X[2,:], arrow_length_ratio=.2, color='g')
-    ax.quiver(s.nodes[0,:], s.nodes[1,:], s.nodes[2,:], Y[0,:], Y[1,:], Y[2,:], arrow_length_ratio=.2, color='y')
-    ax.view_init(90,-90)
-    ax.axis('off')
-    plt.show()
-
-
-Planar constraints
-^^^^^^^^^^^^^^^^^^
-
-Back to the small eigenvalue, which is sometimes associated with what is called a *soft mode*, in this case it appeared
-because the structure is planar, and its ball joints offer little resistance to out-of-plane forces. Indeed, the
-eigenvector associated with the eigenvalue is:
-
-.. code-block:: python
-
-    v[:,0].reshape((3, 4), order='F')
-
-which equals:
-
-.. code::
-
-    +2.27657232e-16,  6.97069602e-17, -6.05872973e-17, -1.78599980e-16
-    -1.50805456e-16,  4.09366810e-18,  1.79720993e-17,  5.96054627e-17
-    -5.00000000e-01,  5.00000000e-01, -5.00000000e-01,  5.00000000e-01
-
-which constitutes a pair of "couples" in the out-of-plane z-direction.
-
-As with rigid body modes, constraining the node displacements to be planar "eliminates" such mode, as in:
-
-.. code-block:: python
-
-    stiffness, _, _ = s.stiffness(storage='dense', apply_rigid_body_constraint=True, apply_planar_constraint=True)
-
-Resulting in a structure in which:
-
-.. code-block:: python
-
-    d, v = stiffness.eigs()
-    d
-
-equals:
-
-.. code::
-
-    3.141592e+07
-    3.141593e+07
-    3.141593e+07
-    8.885766e+07
-    1.202736e+08
-
-indicating that there are no soft modes.
-
-Of course one should expect no impact in the displacements if the forces do not have out-of-plane components and:
-
-.. code-block:: python
-
-    x = stiffness.displacements(f)
-    x
-
-indeed returns displacements that are very similar to the ones calculated before.
+Working with Structures
+=======================
+
+The prisms seen in the quick start are members of :class:`tnsgrt.structure.Structure`. In fact,
+:class:`tnsgrt.prism.Prism` overloads only the constructor of :class:`tnsgrt.structure.Structure`, which provides most
+of the functionality.
+
+Construction
+------------
+
+Object of class :class:`tnsgrt.structure.Structure` are composed of *nodes* and *members*.
+Nodes are `3 x n` numpy arrays:
+
+.. code-block:: python
+
+    import numpy as np
+    nodes = np.array([[0,0,0],[0,1,0],[1,0,0],[1,1,0]]).transpose()
+
+Members are *bars* or *strings*, which are specified by a `2 x m` array with the indices of the nodes that define the
+members, as in:
+
+.. code-block:: python
+
+    members = np.array([[0,1],[1,2],[2,3],[3,0],[0,2],[1,3]]).transpose()
+
+Nodes and members are then combined to build a :class:`tnsgrt.structure.Structure`:
+
+.. code-block:: python
+
+    from tnsgrt import Structure
+    s = Structure(nodes, members, number_of_strings=4)
+
+The parameter ``number_of_strings = 4`` means that the first four members are to be considered strings.
+
+As before, the resulting structure can be plotted using :class:`tnsgrt.plotter.MatplotlibPlotter`:
+
+.. code-block:: python
+
+    from tnsgrt.plotter.matplotlib import MatplotlibPlotter
+    plotter = MatplotlibPlotter()
+    plotter.plot(s)
+    fig, ax = plotter.get_handles()
+    ax.view_init(-90,0)
+
+to visualize the resulting planar tensegrity structure below:
+
+.. image:: /images/planar.png
+  :scale: 50%
+
+Equilibrium
+-----------
+
+Once a structure is built, one can perform various calculations. For example one can determine the member forces so that
+the structure is in equilibrium in various cases.
+
+The key method is :meth:`tnsgrt.structure.Structure.equilibrium`, which calculates the internal forces required to
+maintain a structure in equilibrium. It is assumed that all nodes act as *ball joints*.
+
+Unloaded
+^^^^^^^^
+
+In the *unloaded* case, no external forces are applied to the structure, and equilibrium is achieved by *pretensioning*
+the structure. The result of calling :meth:`tnsgrt.structure.Structure.equilibrium`, as in
+
+.. code-block:: python
+
+    s.equilibrium()
+
+is a set of *force coefficients*, which are forces divided by member length.
+
+The result of the equilibrium calculation can be found in the member properties
+`lambda_` (the force coefficient) and `force`:
+
+.. code-block:: python
+
+    s.member_properties[['lambda_', 'force']]
+
+which, in this example, returns:
+
+.. csv-table::
+   :file: tab1.csv
+   :header-rows: 1
+
+Pretension is set so that the average of the magnitude of the force coefficient on all bars is equal to the parameter
+``lambda_bar``, which is by default equal to one.
+
+Loaded
+^^^^^^
+
+In this case an equilibrium is sought in the presence of external forces, given as a `3 x n` array as the following one:
+
+.. code-block:: python
+
+    f = 0.125*np.array([[0,1,0],[0,-1,0],[0,-2,0],[0,2,0]]).transpose()
+
+Each column is to be interpreted as a force vector to be applied at the corresponding node.
+
+The external force array ``f`` can then be passed on to the method :meth:`tnsgrt.structure.Structure.equilibrium`:
+
+.. code-block:: python
+
+    s.equilibrium(f)
+
+resulting in the new set of member forces and force coefficients:
+
+.. code-block:: python
+
+    s.member_properties[['lambda_', 'force']]
+
+that returns:
+
+.. csv-table::
+   :file: tab2.csv
+   :header-rows: 1
+
+The following code produces a visualization of the applied forces superimposed on the structure:
+
+.. code-block:: python
+
+    plotter = MatplotlibPlotter()
+    plotter.plot(s)
+    fig, ax = plotter.get_handles()
+    ax.quiver(s.nodes[0,:], s.nodes[1,:], s.nodes[2,:], f[0,:], f[1,:], f[2,:], arrow_length_ratio=0.2, color='g')
+    ax.view_init(90,-90)
+    ax.axis('off')
+    plt.show()
+
+resulting in a figure like
+
+.. image:: /images/loaded.png
+   :scale: 50%
+
+The forces are represented by the green arrows.
+
+When it is not possible to find a set of internal forces that satisfy the equilibrium conditions an Exception with a
+message "could not find equilibrium" is produced. For example:
+
+.. code-block:: python
+
+    f = 0.125*np.array([[0,1,0],[0,-1,0],[0,-1,0],[0,2,0]]).transpose()
+    s.equilibrium(f)
+
+can not be in equilibrium.
+
+Stiffness
+---------
+
+Once a structure is in equilibrium, its response to forces can be calculated in terms of its *stiffness matrix*. For
+that it is necessary to characterize the members' geometry and material properties. The fundamental properties are the
+member radius, and elasticity modulus:
+
+.. code-block:: python
+
+    s.member_properties[['radius', 'inner_radius', 'modulus']]
+
+The current default values for such properties are:
+
+.. csv-table::
+   :file: tab3.csv
+   :header-rows: 1
+
+For calculating the stiffness matrix of a pretensioned structure, it is also necessary to know the member's force
+coefficient and the derived member stiffness property. As seen before, the force coefficient and the force are obtained
+during the equilibrium calculation:
+
+.. code-block:: python
+
+    s.equilibrium()
+    s.member_properties[['lambda_', 'force', 'stiffness']]
+
+which returns:
+
+.. csv-table::
+   :file: tab4.csv
+   :header-rows: 1
+
+Because the stiffness is a "derived" property, it does not get automatically populated, which can be done by calling
+:meth:`tnsgrt.structure.Structure.update_member_properties`:
+
+.. code-block:: python
+
+    s.update_member_properties('stiffness')
+    s.member_properties[['stiffness']]
+
+to obtain:
+
+.. csv-table::
+   :file: tab5.csv
+   :header-rows: 1
+
+After setting the material properties, one can calculate the stiffness model associated with the current equilibrium:
+
+.. code-block:: python
+
+    stiffness, _, _ = s.stiffness()
+
+For large models, the stiffness is stored and calculated as sparse arrays. However, for small models, such as this one,
+the model is stored in dense arrays. The warning message can be suppressed by explicitly setting the parameter
+``storage=dense``:
+
+.. code-block:: python
+
+    stiffness, _, _ = s.stiffness(storage='dense')
+
+**WARNING:** setting ``storage='dense'`` for large models is not advised.
+
+Rigid-body constraints
+^^^^^^^^^^^^^^^^^^^^^^
+
+The stiffness model can be used to calculate various quantities of interest. For example:
+
+.. code-block:: python
+
+    d, v = stiffness.eigs()
+
+returns the eigenvalues and eigenvectors of the stiffness matrix. In this case, because there are no constraints in the
+structure, we should expect to encounter various eigenvalues numerically close to zero:
+
+.. code-block:: python
+
+    d
+
+returns:
+
+.. code::
+
+    -6.237207e-09
+    -4.329203e-10
+    1.415459e-11
+    9.183017e-10
+    4.478545e-09
+    7.290895e-09
+    4.000000e+00
+    3.141592e+07
+    3.141593e+07
+    3.141593e+07
+
+
+Six of these are the so-called "rigid body modes," associated to rigid translations and rotations of the structure.
+They can be "removed" by applying certain constraints to the set of allowed displacements. Enforcement of these
+constraints can be done by passing the parameter ``apply_rigid_body_constraint=True`` when calculating the stiffness
+model:
+
+.. code-block:: python
+
+    stiffness, _, _ = s.stiffness(storage='dense', apply_rigid_body_constraint=True)
+
+To see that the six near zero eigenvalues of the stiffness matrix have been removed by the rigid body constraints
+recalculate:
+
+.. code-block:: python
+
+    d, v = stiffness.eigs()
+    d
+
+to obtain:
+
+.. code::
+
+    4.000000e+00
+    3.141592e+07
+    3.141593e+07
+    3.141593e+07
+    8.885766e+07
+    1.202736e+08
+
+Interestingly, in this case, there still remains one eigenvalue that is much smaller than the rest.
+We shall deal with this small eigenvalue later.
+
+For now, even though the smallest eigenvalue is small, the resulting stiffness matrix is not singular, and therefore
+suitable for computing displacements. This time:
+
+.. code-block:: python
+
+    x = stiffness.displacements(f)
+    x
+
+successfully calculates the resulting approximate displacements:
+
+.. code::
+
+    -2.20468248e-09, -2.20468248e-09,  2.20468248e-09,  2.20468248e-09
+     1.77419161e-09, -1.77419161e-09, -5.75306493e-09,  5.75306493e-09
+     4.02657501e-18, -4.02657481e-18,  4.02657460e-18, -4.02657419e-18
+
+which can be visualized, after much enlargement, along with the applied forces in the figure:
+
+.. image:: /images/stiffness1.png
+    :scale: 50%
+
+in which the forces are in green and the vectors indicating the resulting displacement are in yellow.
+This figure is generated by the code:
+
+.. code-block:: python
+
+    X = f
+    Y = 5e7*x
+
+    plotter = MatplotlibPlotter()
+    plotter.plot(s)
+    fig, ax = plotter.get_handles()
+    ax.quiver(s.nodes[0,:], s.nodes[1,:], s.nodes[2,:], X[0,:], X[1,:], X[2,:], arrow_length_ratio=.2, color='g')
+    ax.quiver(s.nodes[0,:], s.nodes[1,:], s.nodes[2,:], Y[0,:], Y[1,:], Y[2,:], arrow_length_ratio=.2, color='y')
+    ax.view_init(90,-90)
+    ax.axis('off')
+    plt.show()
+
+
+Planar constraints
+^^^^^^^^^^^^^^^^^^
+
+Back to the small eigenvalue, which is sometimes associated with what is called a *soft mode*, in this case it appeared
+because the structure is planar, and its ball joints offer little resistance to out-of-plane forces. Indeed, the
+eigenvector associated with the eigenvalue is:
+
+.. code-block:: python
+
+    v[:,0].reshape((3, 4), order='F')
+
+which equals:
+
+.. code::
+
+    +2.27657232e-16,  6.97069602e-17, -6.05872973e-17, -1.78599980e-16
+    -1.50805456e-16,  4.09366810e-18,  1.79720993e-17,  5.96054627e-17
+    -5.00000000e-01,  5.00000000e-01, -5.00000000e-01,  5.00000000e-01
+
+which constitutes a pair of "couples" in the out-of-plane z-direction.
+
+As with rigid body modes, constraining the node displacements to be planar "eliminates" such mode, as in:
+
+.. code-block:: python
+
+    stiffness, _, _ = s.stiffness(storage='dense', apply_rigid_body_constraint=True, apply_planar_constraint=True)
+
+Resulting in a structure in which:
+
+.. code-block:: python
+
+    d, v = stiffness.eigs()
+    d
+
+equals:
+
+.. code::
+
+    3.141592e+07
+    3.141593e+07
+    3.141593e+07
+    8.885766e+07
+    1.202736e+08
+
+indicating that there are no soft modes.
+
+Of course one should expect no impact in the displacements if the forces do not have out-of-plane components and:
+
+.. code-block:: python
+
+    x = stiffness.displacements(f)
+    x
+
+indeed returns displacements that are very similar to the ones calculated before.
```

### Comparing `tnsgrt-0.3/examples/examples.ipynb` & `tnsgrt-0.4/examples/examples.ipynb`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/examples/quick_start.ipynb` & `tnsgrt-0.4/examples/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/examples/working_with_structures.ipynb` & `tnsgrt-0.4/examples/working_with_structures.ipynb`

 * *Files identical despite different names*

### Comparing `tnsgrt-0.3/src/tnsgrt/optim.py` & `tnsgrt-0.4/src/tnsgrt/optim.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-import cvxpy as cvx
-import numpy as np
-
-
-def qp(n, m, Q, c, A, blo, bup, xlo, xup, **kwargs):
-    """
-    Minimize 1/2 x^T Q x + 1/2 f^T D f + c^T x
-      s.t.   blo <= A x <= bup
-             xlo <= x <= xup
-             f = F^T x
-    kwargs:
-     - F and D
-    """
-
-    # variable
-    x = cvx.Variable(n)
-
-    # factored cost
-    F = kwargs.pop('F', None)
-    D = kwargs.pop('D', None)
-
-    # objective function
-    objective = 0
-    if Q is not None:
-        objective += (1 / 2) * cvx.quad_form(x, Q)
-    if F is not None and D is not None:
-        objective += (1 / 2) * cvx.quad_form(F.T @ x, D)
-    if c is not None:
-        objective += c.T @ x
-    objective = cvx.Minimize(objective)
-
-    # constraints
-    constraints = []
-
-    # variable upper bounds
-    if xup is not None:
-        isconstrained = np.logical_not(np.isinf(xup))
-        constraints.append(x[isconstrained] <= xup[isconstrained])
-
-    # variable lower bounds
-    if xlo is not None:
-        isconstrained = np.logical_not(np.isneginf(xlo))
-        constraints.append(x[isconstrained] >= xlo[isconstrained])
-
-    # constraints
-    if m > 0:
-        # upper and lower bounds
-        if bup is not None and blo is not None:
-            # equality constraints?
-            isequal = blo == bup
-            if np.any(isequal):
-                constraints.append(A[isequal, :] @ x == bup[isequal])
-
-            # upper bound constraints?
-            isconstrained = np.logical_not(np.logical_or(np.isinf(bup), isequal))
-            if np.any(isconstrained):
-                constraints.append(A[isconstrained, :] @ x <= bup[isconstrained])
-
-            isconstrained = np.logical_not(np.logical_or(np.isneginf(blo), isequal))
-            if np.any(isconstrained):
-                constraints.append(A[isconstrained, :] @ x >= blo[isconstrained])
-
-        else:
-
-            # a upper bounds
-            if bup is not None:
-                isconstrained = np.logical_not(np.isinf(bup))
-                constraints.append(A[isconstrained, :] @ x <= bup[isconstrained])
-
-            # a lower bounds
-            if blo is not None:
-                isconstrained = np.logical_not(np.isneginf(blo))
-                constraints.append(A[isconstrained, :] @ x >= blo[isconstrained])
-
-    # problem
-    problem = cvx.Problem(objective, constraints)
-
-    try:
-
-        # solve
-        defaults = {
-            # 'solver': cvx.OSQP,
-            # 'eps_abs': 1e-8
-        }
-        defaults.update(**kwargs)
-        problem.solve(**defaults)
-
-    except cvx.error.SolverError:
-
-        # solve using default solver
-        problem.solve(eps_abs=1e-8, **kwargs)
-
-    return objective.value, x.value, problem.status
-
-
-def lp(n, m, c, A, blo, bup, xlo, xup, **kwargs):
-    """
-    Minimize c^T x
-      s.t.   blo <= A x <= bup
-             xlo <= x <= xup
-    """
-    return qp(n, m, None, c, A, blo, bup, xlo, xup, **kwargs)
+import cvxpy as cvx
+import numpy as np
+
+
+def qp(n, m, Q, c, A, blo, bup, xlo, xup, **kwargs):
+    """
+    Minimize 1/2 x^T Q x + 1/2 f^T D f + c^T x
+      s.t.   blo <= A x <= bup
+             xlo <= x <= xup
+             f = F^T x
+    kwargs:
+     - F and D
+    """
+
+    # variable
+    x = cvx.Variable(n)
+
+    # factored cost
+    F = kwargs.pop('F', None)
+    D = kwargs.pop('D', None)
+
+    # objective function
+    objective = 0
+    if Q is not None:
+        objective += (1 / 2) * cvx.quad_form(x, Q)
+    if F is not None and D is not None:
+        objective += (1 / 2) * cvx.quad_form(F.T @ x, D)
+    if c is not None:
+        objective += c.T @ x
+    objective = cvx.Minimize(objective)
+
+    # constraints
+    constraints = []
+
+    # variable upper bounds
+    if xup is not None:
+        isconstrained = np.logical_not(np.isinf(xup))
+        constraints.append(x[isconstrained] <= xup[isconstrained])
+
+    # variable lower bounds
+    if xlo is not None:
+        isconstrained = np.logical_not(np.isneginf(xlo))
+        constraints.append(x[isconstrained] >= xlo[isconstrained])
+
+    # constraints
+    if m > 0:
+        # upper and lower bounds
+        if bup is not None and blo is not None:
+            # equality constraints?
+            isequal = blo == bup
+            if np.any(isequal):
+                constraints.append(A[isequal, :] @ x == bup[isequal])
+
+            # upper bound constraints?
+            isconstrained = np.logical_not(np.logical_or(np.isinf(bup), isequal))
+            if np.any(isconstrained):
+                constraints.append(A[isconstrained, :] @ x <= bup[isconstrained])
+
+            isconstrained = np.logical_not(np.logical_or(np.isneginf(blo), isequal))
+            if np.any(isconstrained):
+                constraints.append(A[isconstrained, :] @ x >= blo[isconstrained])
+
+        else:
+
+            # a upper bounds
+            if bup is not None:
+                isconstrained = np.logical_not(np.isinf(bup))
+                constraints.append(A[isconstrained, :] @ x <= bup[isconstrained])
+
+            # a lower bounds
+            if blo is not None:
+                isconstrained = np.logical_not(np.isneginf(blo))
+                constraints.append(A[isconstrained, :] @ x >= blo[isconstrained])
+
+    # problem
+    problem = cvx.Problem(objective, constraints)
+
+    try:
+
+        # solve
+        defaults = {
+            # 'solver': cvx.OSQP,
+            # 'eps_abs': 1e-8
+        }
+        defaults.update(**kwargs)
+        problem.solve(**defaults)
+
+    except cvx.error.SolverError:
+
+        # solve using default solver
+        problem.solve(eps_abs=1e-8, **kwargs)
+
+    return objective.value, x.value, problem.status
+
+
+def lp(n, m, c, A, blo, bup, xlo, xup, **kwargs):
+    """
+    Minimize c^T x
+      s.t.   blo <= A x <= bup
+             xlo <= x <= xup
+    """
+    return qp(n, m, None, c, A, blo, bup, xlo, xup, **kwargs)
```

### Comparing `tnsgrt-0.3/src/tnsgrt/prism.py` & `tnsgrt-0.4/src/tnsgrt/prism.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,176 +1,174 @@
-from typing import Literal, Optional
-
-import numpy as np
-
-from .structure import Structure
-from .utils import rotation_2d
-
-
-class Prism(Structure):
-    """
-    Constructs a Snelson prism with ``p`` bars
-
-    :param p: number of bars
-    :param top_radius: the top radius
-    :param bottom_radius: the bottom radius
-    :param height: the radius of the prism
-    :param alpha: the twist angle
-    :param calculate_equilibrium: if ``True`` calculates equilibrium
-    :param equilibrium_method: choice of method for computing equilibrium
-    :param \\**kwargs: See below
-
-    :Keyword Arguments:
-        * **bar** (``bool=True``) --
-          if ``True`` add *bars*
-        * **bottom** (``bool=True``) --
-          if ``True`` add *bottom strings*
-        * **top** (``bool=True``) --
-          if ``True`` add *top strings*
-        * **vertical** (``bool=True``) --
-          if ``True`` add *vertical strings*
-        * **diagonal** (``bool=False``) --
-          if ``True`` add *diagonal strings*
-
-    **Notes:**
-
-    1. Unloaded equilibrium is possible only if
-
-       .. math::
-          \\frac{\\pi}{2} - \\frac{\\pi}{p} \\leq \\alpha \\leq \\frac{\\pi}{2}
-
-       when both *vertical* and *diagonal* strings are present
-    2. If *diagonal* strings are not present, then unloaded equilibrium is possible only
-       if
-
-       .. math::
-          \\alpha = \\frac{\\pi}{2} - \\frac{\\pi}{p}
-
-       This is the default prism configuration
-    3. If *vertical* strings are not present, then unloaded equilibrium is possible only
-       if
-
-       .. math::
-          \\alpha = \\frac{\\pi}{2}
-    4. Additional keyword arguments are passed to :class:`tnsgrt.structure.Structure`
-    """
-
-    def __init__(self, p: int = 3,
-                 top_radius: float = 1, bottom_radius: float = 1, height: float = 1, alpha: Optional[float] = None,
-                 calculate_equilibrium=True, equilibrium_method=Literal['analytic', 'numeric'],
-                 **kwargs):
-
-        # proper size
-        assert p >= 3, 'p must be greater or equal to 3'
-
-        # twist angle
-        if alpha is None:
-            alpha = np.pi/2 - np.pi/p
-
-        # other options
-        options = {
-            'bottom': True,
-            'top': True,
-            'vertical': True,
-            'diagonal': False,
-            'bar': True
-        }
-        options.update(kwargs)
-
-        # clean up kwargs
-        for key in ['bottom', 'top', 'vertical', 'diagonal', 'bar']:
-            if key in kwargs:
-                del kwargs[key]
-
-        # valid equilibrium?
-        if calculate_equilibrium:
-            assert 'bottom' in options, 'equilibrium is not possible without bottom strings'
-            assert 'top' in options, 'equilibrium is not possible without top strings'
-            assert 'bar' in options, 'equilibrium is not possible without bars'
-            if not options['diagonal']:
-                assert np.abs(np.pi/2 - np.pi/p - alpha) < 1e-8, 'equilibrium is not possible with given twist angle'
-            if not options['vertical']:
-                assert np.abs(np.pi/2 - alpha) < 1e-8, 'equilibrium is not possible with given twist angle'
-            if options['vertical'] and options['diagonal']:
-                assert np.pi/2 - np.pi/p <= alpha <= np.pi/2, 'equilibrium is not possible with given twist angle'
-
-        # base angle
-        beta = 2 * np.pi/p
-
-        # rotation matrices
-        rotation_beta = rotation_2d(beta)
-        rotation_alpha = rotation_2d(alpha)
-
-        # nodes
-        nodes = np.zeros((3, 2 * p))
-        # bottom nodes
-        nodes[2, :p] = -height / 2
-        nodes[:2, 0] = np.array([bottom_radius, 0])
-        for i in range(1, p):
-            nodes[:2, i] = rotation_beta @ nodes[:2, i-1]
-        # top nodes
-        nodes[2, p:2 * p] = height / 2
-        nodes[:2, p] = np.array([top_radius, 0])
-        nodes[:2, p] = rotation_alpha @ nodes[:2, p]
-        for i in range(1, p):
-            nodes[:2, p + i] = rotation_beta @ nodes[:2, p + i - 1]
-
-        # strings
-        members = np.zeros((2, 0))
-        number_of_strings = 0
-        string_tags = {}
-        # bottom strings
-        bottom_strings = np.vstack((np.arange(p), np.mod(1 + np.arange(p), p)))
-        if options['bottom']:
-            members = np.hstack((members, bottom_strings))
-            string_tags['bottom'] = number_of_strings + np.arange(p)
-            number_of_strings += p
-        # top strings
-        top_strings = np.vstack((p + np.arange(p), p + np.mod(1 + np.arange(p), p)))
-        if options['top']:
-            members = np.hstack((members, top_strings))
-            string_tags['top'] = number_of_strings + np.arange(p)
-            number_of_strings += p
-        # vertical strings
-        vertical_strings = np.vstack((np.arange(p), p + np.arange(p)))
-        if options['vertical']:
-            members = np.hstack((members, vertical_strings))
-            string_tags['vertical'] = number_of_strings + np.arange(p)
-            number_of_strings += p
-        # diagonal strings
-        diagonal_strings = np.vstack((np.arange(p), p + np.mod(np.arange(p) - 1, p)))
-        if options['diagonal']:
-            members = np.hstack((members, diagonal_strings))
-            string_tags['diagonal'] = number_of_strings + np.arange(p)
-            number_of_strings += p
-
-        # bars
-        bars = np.vstack((np.arange(p), p + np.mod(1 + np.arange(p), p)))
-        if options['bar']:
-            members = np.hstack((members, bars))
-
-        # call super
-        super().__init__(nodes=nodes, members=members, number_of_strings=number_of_strings,
-                         member_tags=string_tags, **kwargs)
-
-        if calculate_equilibrium:
-            if equilibrium_method == 'analytic':
-                # top/bottom ratio
-                rho = top_radius / bottom_radius
-                # force coefficients
-                lambda_ = np.array([
-                    rho * np.cos(np.pi / p) / np.cos(alpha - np.pi / p),                # bottom
-                    (1 / rho) * np.cos(np.pi / p) / np.cos(alpha - np.pi / p),          # top
-                    2 * np.cos(alpha) * np.cos(np.pi / p) / np.cos(alpha - np.pi / p),  # vertical
-                    -np.cos(alpha + np.pi / p) / np.cos(alpha - np.pi / p),             # diagonal
-                    -1                                                                  # bars
-                ]).reshape((1, 5))
-                # select appropriate string sets
-                index = [True, True, options['vertical'], options['diagonal'], True]
-                # construct coefficients
-                self.member_properties['lambda_'] = (np.ones((p, 1)) @ lambda_[:, index]).flatten(order='F')
-            else:
-                # solve for equilibrium
-                self.equilibrium(equalities=[np.arange(number_of_strings, members.shape[1])])
-
-            # update mass, volume, stiffness and rest length
-            self.update_member_properties()
+from typing import Literal, Optional
+
+import numpy as np
+
+from .structure import Structure
+from .utils import rotation_2d
+
+
+class Prism(Structure):
+    """
+    Constructs a Snelson prism with ``p`` bars
+
+    :param p: number of bars
+    :param top_radius: the top radius
+    :param bottom_radius: the bottom radius
+    :param height: the radius of the prism
+    :param alpha: the twist angle
+    :param calculate_equilibrium: if ``True`` calculates equilibrium
+    :param equilibrium_method: choice of method for computing equilibrium
+    :param \\**kwargs: See below
+
+    :Keyword Arguments:
+        * **bar** (``bool=True``) --
+          if ``True`` add *bars*
+        * **bottom** (``bool=True``) --
+          if ``True`` add *bottom strings*
+        * **top** (``bool=True``) --
+          if ``True`` add *top strings*
+        * **vertical** (``bool=True``) --
+          if ``True`` add *vertical strings*
+        * **diagonal** (``bool=False``) --
+          if ``True`` add *diagonal strings*
+
+    **Notes:**
+
+    1. Unloaded equilibrium is possible only if
+
+       .. math::
+          \\frac{\\pi}{2} - \\frac{\\pi}{p} \\leq \\alpha \\leq \\frac{\\pi}{2}
+
+       when both *vertical* and *diagonal* strings are present
+    2. If *diagonal* strings are not present, then unloaded equilibrium is possible only
+       if
+
+       .. math::
+          \\alpha = \\frac{\\pi}{2} - \\frac{\\pi}{p}
+
+       This is the default prism configuration
+    3. If *vertical* strings are not present, then unloaded equilibrium is possible only
+       if
+
+       .. math::
+          \\alpha = \\frac{\\pi}{2}
+    4. Additional keyword arguments are passed to :class:`tnsgrt.structure.Structure`
+    """
+
+    def __init__(self, p: int = 3,
+                 top_radius: float = 1, bottom_radius: float = 1, height: float = 1, alpha: Optional[float] = None,
+                 calculate_equilibrium=True, equilibrium_method=Literal['analytic', 'numeric'],
+                 **kwargs):
+
+        # proper size
+        assert p >= 3, 'p must be greater or equal to 3'
+
+        # twist angle
+        if alpha is None:
+            alpha = np.pi/2 - np.pi/p
+
+        # other options
+        options = {
+            'bottom': True,
+            'top': True,
+            'vertical': True,
+            'diagonal': False,
+            'bar': True
+        }
+        options.update(kwargs)
+
+        # clean up kwargs
+        kwargs = {k: v for k, v in kwargs.items() if k not in ['bottom', 'top', 'vertical', 'diagonal', 'bar']}
+
+        # valid equilibrium?
+        if calculate_equilibrium:
+            assert 'bottom' in options, 'equilibrium is not possible without bottom strings'
+            assert 'top' in options, 'equilibrium is not possible without top strings'
+            assert 'bar' in options, 'equilibrium is not possible without bars'
+            if not options['diagonal']:
+                assert np.abs(np.pi/2 - np.pi/p - alpha) < 1e-8, 'equilibrium is not possible with given twist angle'
+            if not options['vertical']:
+                assert np.abs(np.pi/2 - alpha) < 1e-8, 'equilibrium is not possible with given twist angle'
+            if options['vertical'] and options['diagonal']:
+                assert np.pi/2 - np.pi/p <= alpha <= np.pi/2, 'equilibrium is not possible with given twist angle'
+
+        # base angle
+        beta = 2 * np.pi/p
+
+        # rotation matrices
+        rotation_beta = rotation_2d(beta)
+        rotation_alpha = rotation_2d(alpha)
+
+        # nodes
+        nodes = np.zeros((3, 2 * p))
+        # bottom nodes
+        nodes[2, :p] = -height / 2
+        nodes[:2, 0] = np.array([bottom_radius, 0])
+        for i in range(1, p):
+            nodes[:2, i] = rotation_beta @ nodes[:2, i-1]
+        # top nodes
+        nodes[2, p:2 * p] = height / 2
+        nodes[:2, p] = np.array([top_radius, 0])
+        nodes[:2, p] = rotation_alpha @ nodes[:2, p]
+        for i in range(1, p):
+            nodes[:2, p + i] = rotation_beta @ nodes[:2, p + i - 1]
+
+        # strings
+        members = np.zeros((2, 0))
+        number_of_strings = 0
+        string_tags = {}
+        # bottom strings
+        bottom_strings = np.vstack((np.arange(p), np.mod(1 + np.arange(p), p)))
+        if options['bottom']:
+            members = np.hstack((members, bottom_strings))
+            string_tags['bottom'] = number_of_strings + np.arange(p)
+            number_of_strings += p
+        # top strings
+        top_strings = np.vstack((p + np.arange(p), p + np.mod(1 + np.arange(p), p)))
+        if options['top']:
+            members = np.hstack((members, top_strings))
+            string_tags['top'] = number_of_strings + np.arange(p)
+            number_of_strings += p
+        # vertical strings
+        vertical_strings = np.vstack((np.arange(p), p + np.arange(p)))
+        if options['vertical']:
+            members = np.hstack((members, vertical_strings))
+            string_tags['vertical'] = number_of_strings + np.arange(p)
+            number_of_strings += p
+        # diagonal strings
+        diagonal_strings = np.vstack((np.arange(p), p + np.mod(np.arange(p) - 1, p)))
+        if options['diagonal']:
+            members = np.hstack((members, diagonal_strings))
+            string_tags['diagonal'] = number_of_strings + np.arange(p)
+            number_of_strings += p
+
+        # bars
+        bars = np.vstack((np.arange(p), p + np.mod(1 + np.arange(p), p)))
+        if options['bar']:
+            members = np.hstack((members, bars))
+
+        # call super
+        super().__init__(nodes=nodes, members=members, number_of_strings=number_of_strings,
+                         member_tags=string_tags, **kwargs)
+
+        if calculate_equilibrium:
+            if equilibrium_method == 'analytic':
+                # top/bottom ratio
+                rho = top_radius / bottom_radius
+                # force coefficients
+                lambda_ = np.array([
+                    rho * np.cos(np.pi / p) / np.cos(alpha - np.pi / p),                # bottom
+                    (1 / rho) * np.cos(np.pi / p) / np.cos(alpha - np.pi / p),          # top
+                    2 * np.cos(alpha) * np.cos(np.pi / p) / np.cos(alpha - np.pi / p),  # vertical
+                    -np.cos(alpha + np.pi / p) / np.cos(alpha - np.pi / p),             # diagonal
+                    -1                                                                  # bars
+                ]).reshape((1, 5))
+                # select appropriate string sets
+                index = [True, True, options['vertical'], options['diagonal'], True]
+                # construct coefficients
+                self.member_properties['lambda_'] = (np.ones((p, 1)) @ lambda_[:, index]).flatten(order='F')
+            else:
+                # solve for equilibrium
+                self.equilibrium(equalities=[np.arange(number_of_strings, members.shape[1])])
+
+            # update mass, volume, stiffness and rest length
+            self.update_member_properties()
```

### Comparing `tnsgrt-0.3/src/tnsgrt/snelson.py` & `tnsgrt-0.4/src/tnsgrt/snelson.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-import numpy as np
-from .structure import Structure
-
-
-class Snelson(Structure):
-
-    @staticmethod
-    def __init__(self, height: float = 1, radius: float = 1, alpha: float = np.pi/6, label: str = None):
-        # height
-        # radius
-        # alpha = twist angle (in degrees)
-
-        lambdaBar = 1
-        delta = 0.5
-        zeta = 0
-        delH = 0
-        doSimple = True
-
-        # convert alpha to radians
-        # alpha = alpha * np.pi / 180
-        beta = 2 * np.pi / 3
-
-        n1 = np.array([radius, 0])
-        rotation_beta = Snelson.rotation_2d(beta)
-        rotation_alpha = Snelson.rotation_2d(alpha)
-        bar_nodes = np.vstack((n1, np.dot(rotation_beta, n1), np.dot(rotation_beta @ rotation_beta, n1),
-                              np.dot(rotation_beta @ rotation_alpha, n1),
-                              np.dot(rotation_beta @ (rotation_beta @ rotation_alpha), n1),
-                              np.dot(rotation_alpha, n1))).transpose()
-        btm_rot = (1 - zeta) * (delta * np.eye(2) + (1 - delta) * rotation_beta) + zeta * rotation_beta @ rotation_beta
-        top_rot = (1 - zeta) * (delta * np.eye(2) + (1 - delta) * rotation_beta @ rotation_beta) + zeta * rotation_beta
-        string_nodes = np.hstack((np.dot(btm_rot, bar_nodes[:, :3]), np.dot(top_rot, bar_nodes[:, 4:6]),
-                                 np.dot(top_rot, bar_nodes[:, [3]])))
-        z_pos = np.hstack((-(height / 2) * np.ones((1, 3)), (height / 2) * np.ones((1, 3))))
-        z_pos = np.hstack((z_pos, (1 - delH) * z_pos))
-        nodes = np.vstack((np.hstack((bar_nodes, string_nodes)), z_pos))
-
-        # member indices are given starting at 1 below:
-        members = np.array([
-            [1, 7], [2, 8], [3, 9],        # btm long(1: 3)
-            [1, 9], [2, 7], [3, 8],        # btm short(4: 6)
-            [4, 12], [5, 10], [6, 11],     # top long(7: 9)
-            [4, 10], [5, 11], [6, 12],     # top short(8: 12)
-            [1, 6], [2, 4], [3, 5],        # vert(13: 15)
-            [1, 5], [2, 6], [3, 4],        # diag(16: 18)
-            [7, 8], [8, 9], [7, 9],        # btm  overlap(19: 21)
-            [10, 11], [11, 12], [10, 12],  # top overlap(22: 24)
-            [1, 11], [2, 12], [3, 10],     # reach1(25: 27)
-            [7, 11], [8, 12], [9, 10],     # reach2(28: 30)
-            [7, 12], [8, 10], [9, 11],     # reach3(31: 33)
-            [1, 4], [2, 5], [3, 6]         # bars(34: 36)
-        ]).transpose() - 1
-        number_of_strings = 33
-
-        # string tags
-        member_tags = {
-            'bottom': np.hstack((np.arange(6), 18 + np.arange(3))),      # [1:6 19:21]
-            'top': np.hstack((6 + np.arange(6), 21 + np.arange(3))),     # [7:12, 22:24]
-            'long': np.hstack((np.arange(3), 6 + np.arange(3))),         # [1: 3, 7: 9];
-            'short': np.hstack((3 + np.arange(3), 9 + np.arange(3))),    # [4: 6, 10: 12];
-            'vertical': 12 + np.arange(3),                               # [13: 15];
-            'diagonal': 15 + np.arange(3),                               # [16: 18];
-            'thick': np.hstack((12 + np.arange(6), 24 + np.arange(9))),  # [13: 18, 25: 33];
-            'reach': 24 + np.arange(9),                                  # [25: 33];
-            'string2string': 27 + np.arange(6),                          # [28: 33];
-            'overlap': 18 + np.arange(6)                                 # [19: 24]
-        }
-
-        # call super
-        super().__init__(nodes=nodes, members=members, number_of_strings=number_of_strings,
-                         member_tags=member_tags, label=label)
-
-        # self.equilibrium()
-
-        # barDiam = 4e-3
-        # stringDiam = 2e-3
-        # modulus = 230e9  # Carbon        Fiber
-        # yld = 2e9
-        # density = 1850
-
-        # s = addSubStructure(s, label);
-        # s = addLocalNodes(s, 1, nodeIndex);
-        # s = addMembers(s, 1, memberIndex, numberOfStrings);
-        # s = computeEquil(s, lambdaBar);
-        #
-        #
-        # for index = 1:size(tags, 1)
-        # ind = makeIndex(s, 1, tags
-        # {index, 2});
-        # s = add(s, ind, tags
-        # {index, 1});
-        # end
-        #
-        # sp.height = h;
-        # sp.radius = r;
-        # sp.alpha = alpha * 180 / pi;
-        # sp.delta = delta;
-        # sp.zeta = zeta;
-        # sp.delH = delH;
-        #
-        # if (doSimple)
-        #     sp.delta = [];
-        #     sp.zeta = [];
-        #     s = removeSlackMembers(s);
-        #     s = removeDependentNodes(s);
-        #     s = removeUnusedNodes(s);
-        # end
-        #
-        # s = materialProperties(s, barDiam, stringDiam, modulus, modulus,
-        # yield, yield, density, density );
-        # s = updateMemberStiffness(s);
-        # s = updateMemberMass(s);
-        #
-        # s =
-        #
-        # class(sp, 'snelson', s);
-        #
-        # property = {'color', {[1 0 0]}, 'top';
-        # 'color', {[0 0 1]}, 'bottom';
-        # 'color', {[1 1 0]}, 'thick';
-        # 'width', 2, 'bar';
-        # 'width', 1.5, 'string'};
-        #
-        # for index = 1:size(property, 1)
-        # ind = makeIndex(s, 'all', property
-        # {index, 3});
-        # s = set(s, property
-        # {index, 1}, ind, property
-        # {index, 2} );
-        # end
-
+import numpy as np
+from .structure import Structure
+
+
+class Snelson(Structure):
+
+    @staticmethod
+    def __init__(self, height: float = 1, radius: float = 1, alpha: float = np.pi/6, label: str = None):
+        # height
+        # radius
+        # alpha = twist angle (in degrees)
+
+        lambdaBar = 1
+        delta = 0.5
+        zeta = 0
+        delH = 0
+        doSimple = True
+
+        # convert alpha to radians
+        # alpha = alpha * np.pi / 180
+        beta = 2 * np.pi / 3
+
+        n1 = np.array([radius, 0])
+        rotation_beta = Snelson.rotation_2d(beta)
+        rotation_alpha = Snelson.rotation_2d(alpha)
+        bar_nodes = np.vstack((n1, np.dot(rotation_beta, n1), np.dot(rotation_beta @ rotation_beta, n1),
+                              np.dot(rotation_beta @ rotation_alpha, n1),
+                              np.dot(rotation_beta @ (rotation_beta @ rotation_alpha), n1),
+                              np.dot(rotation_alpha, n1))).transpose()
+        btm_rot = (1 - zeta) * (delta * np.eye(2) + (1 - delta) * rotation_beta) + zeta * rotation_beta @ rotation_beta
+        top_rot = (1 - zeta) * (delta * np.eye(2) + (1 - delta) * rotation_beta @ rotation_beta) + zeta * rotation_beta
+        string_nodes = np.hstack((np.dot(btm_rot, bar_nodes[:, :3]), np.dot(top_rot, bar_nodes[:, 4:6]),
+                                 np.dot(top_rot, bar_nodes[:, [3]])))
+        z_pos = np.hstack((-(height / 2) * np.ones((1, 3)), (height / 2) * np.ones((1, 3))))
+        z_pos = np.hstack((z_pos, (1 - delH) * z_pos))
+        nodes = np.vstack((np.hstack((bar_nodes, string_nodes)), z_pos))
+
+        # member indices are given starting at 1 below:
+        members = np.array([
+            [1, 7], [2, 8], [3, 9],        # btm long(1: 3)
+            [1, 9], [2, 7], [3, 8],        # btm short(4: 6)
+            [4, 12], [5, 10], [6, 11],     # top long(7: 9)
+            [4, 10], [5, 11], [6, 12],     # top short(8: 12)
+            [1, 6], [2, 4], [3, 5],        # vert(13: 15)
+            [1, 5], [2, 6], [3, 4],        # diag(16: 18)
+            [7, 8], [8, 9], [7, 9],        # btm  overlap(19: 21)
+            [10, 11], [11, 12], [10, 12],  # top overlap(22: 24)
+            [1, 11], [2, 12], [3, 10],     # reach1(25: 27)
+            [7, 11], [8, 12], [9, 10],     # reach2(28: 30)
+            [7, 12], [8, 10], [9, 11],     # reach3(31: 33)
+            [1, 4], [2, 5], [3, 6]         # bars(34: 36)
+        ]).transpose() - 1
+        number_of_strings = 33
+
+        # string tags
+        member_tags = {
+            'bottom': np.hstack((np.arange(6), 18 + np.arange(3))),      # [1:6 19:21]
+            'top': np.hstack((6 + np.arange(6), 21 + np.arange(3))),     # [7:12, 22:24]
+            'long': np.hstack((np.arange(3), 6 + np.arange(3))),         # [1: 3, 7: 9];
+            'short': np.hstack((3 + np.arange(3), 9 + np.arange(3))),    # [4: 6, 10: 12];
+            'vertical': 12 + np.arange(3),                               # [13: 15];
+            'diagonal': 15 + np.arange(3),                               # [16: 18];
+            'thick': np.hstack((12 + np.arange(6), 24 + np.arange(9))),  # [13: 18, 25: 33];
+            'reach': 24 + np.arange(9),                                  # [25: 33];
+            'string2string': 27 + np.arange(6),                          # [28: 33];
+            'overlap': 18 + np.arange(6)                                 # [19: 24]
+        }
+
+        # call super
+        super().__init__(nodes=nodes, members=members, number_of_strings=number_of_strings,
+                         member_tags=member_tags, label=label)
+
+        # self.equilibrium()
+
+        # barDiam = 4e-3
+        # stringDiam = 2e-3
+        # modulus = 230e9  # Carbon        Fiber
+        # yld = 2e9
+        # density = 1850
+
+        # s = addSubStructure(s, label);
+        # s = addLocalNodes(s, 1, nodeIndex);
+        # s = addMembers(s, 1, memberIndex, numberOfStrings);
+        # s = computeEquil(s, lambdaBar);
+        #
+        #
+        # for index = 1:size(tags, 1)
+        # ind = makeIndex(s, 1, tags
+        # {index, 2});
+        # s = add(s, ind, tags
+        # {index, 1});
+        # end
+        #
+        # sp.height = h;
+        # sp.radius = r;
+        # sp.alpha = alpha * 180 / pi;
+        # sp.delta = delta;
+        # sp.zeta = zeta;
+        # sp.delH = delH;
+        #
+        # if (doSimple)
+        #     sp.delta = [];
+        #     sp.zeta = [];
+        #     s = removeSlackMembers(s);
+        #     s = removeDependentNodes(s);
+        #     s = removeUnusedNodes(s);
+        # end
+        #
+        # s = materialProperties(s, barDiam, stringDiam, modulus, modulus,
+        # yield, yield, density, density );
+        # s = updateMemberStiffness(s);
+        # s = updateMemberMass(s);
+        #
+        # s =
+        #
+        # class(sp, 'snelson', s);
+        #
+        # property = {'color', {[1 0 0]}, 'top';
+        # 'color', {[0 0 1]}, 'bottom';
+        # 'color', {[1 1 0]}, 'thick';
+        # 'width', 2, 'bar';
+        # 'width', 1.5, 'string'};
+        #
+        # for index = 1:size(property, 1)
+        # ind = makeIndex(s, 'all', property
+        # {index, 3});
+        # s = set(s, property
+        # {index, 1}, ind, property
+        # {index, 2} );
+        # end
+
```

### Comparing `tnsgrt-0.3/src/tnsgrt/stiffness.py` & `tnsgrt-0.4/src/tnsgrt/stiffness.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,534 +1,534 @@
-import warnings
-from typing import Optional, Tuple, Sequence, Union, Literal
-import numpy as np
-import numpy.typing as npt
-import scipy
-
-from .utils import orthogonalize, norm
-
-
-class NodeConstraint:
-    """
-    Object representing a node constraint
-
-    :param constraint: the constraint coefficient array
-    :param epsilon: precision used to assess numerical rank
-
-    **Notes:**
-
-    1. If :math:`x` is the node coordinate and :math:`A` is the constraint coefficient then
-
-       .. math::
-           A x = 0
-
-       then the equivalent constraint and its null space
-
-       .. math::
-           R \\, x = 0, \\quad x = T \\, y, \\quad R R^T = I, \\quad T^T T = I
-
-       is constructed using :func:`tnsgrt.utils.orthogonalize`
-    """
-
-    def __init__(self, constraint: Optional[npt.NDArray] = None, epsilon: float = 1e-8):
-        if constraint is None:
-            self.dof = 0
-            self.basis = None
-            self.normal = np.eye(3)
-        else:
-            assert constraint.ndim == 2 and constraint.shape[1] == 3 and constraint.shape[0] < 3, \
-                'normal must be a m x 3, m < 3, array'
-            # first orthogonalize
-            rank, r, t = orthogonalize(constraint.transpose(), mode='complete', epsilon=epsilon)
-            self.dof = 3 - rank
-            if self.dof == 0:
-                self.basis = None
-                self.normal = np.eye(3)
-            else:
-                self.normal = r.transpose()
-                self.basis = t
-
-    @staticmethod
-    def node_constraint(nodes: npt.NDArray, constraints: Sequence['NodeConstraint'],
-                        storage: Literal['sparse', 'dense'] = 'sparse') \
-            -> Union[Tuple[npt.NDArray, npt.NDArray], Tuple[scipy.sparse.csr_array, scipy.sparse.csr_array]]:
-        """
-        Construct the constraint associated with the given nodes and node constraints
-
-        The resulting tuple is compatible with :meth:`~tnsgrt.stiffness.Stiffness.apply_constraint`
-
-        :param nodes: 3 x n array of nodes
-        :param constraints: list with n constraints
-        :param storage: if ``sparse``, returns sparse arrays
-        :return: tuple with the constraint matrix, and its null space
-        """
-        assert nodes.shape[0] == 3, 'nodes must be a 3 x m array'
-        assert nodes.shape[1] == len(constraints), \
-            'number of columns of nodes must be equal to to the number of constraints'
-
-        # calculate degrees of freedom
-        m = nodes.shape[1]
-        noc = sum(3 - c.dof for c in constraints if c is not None)
-        dof = 3*m - noc
-
-        if storage == 'sparse':
-            row_col_r = np.zeros((2, 3*noc))
-            data_r = np.zeros((3*noc))
-            row_col_t = np.zeros((2, 3*dof))
-            data_t = np.zeros((3*dof))
-            jj = kk = 0
-            for i, c in enumerate(constraints):
-                if c is None:
-                    # add identity to basis
-                    dofj = 3
-                    row_col_t[0, 3*kk:3*kk+3*dofj] = np.kron(np.arange(3*i, 3*(i+1)), np.ones((3,)))
-                    row_col_t[1, 3*kk:3*kk+3*dofj] = np.kron(np.arange(kk, kk+dofj), np.ones((3,)))
-                    data_t[3*kk:3*kk+3*dofj] = np.eye(dofj).flatten(order='C')
-                    kk += dofj
-                else:
-                    # add to normal
-                    nocj = 3-c.dof
-                    row_col_r[0, 3*jj:3*jj+3*nocj] = np.kron(np.arange(jj, jj+nocj), np.ones((3,)))      # row
-                    row_col_r[1, 3*jj:3*jj+3*nocj] = np.kron(np.ones((nocj,)), np.arange(3*i, 3*(i+1)))  # col
-                    data_r[3*jj:3*jj+3*nocj] = c.normal.flatten(order='C')
-                    jj += nocj
-                    if c.dof:
-                        # add to basis
-                        dofj = c.dof
-                        row_col_t[0, 3*kk:3*kk+3*dofj] = np.kron(np.arange(3*i, 3*(i+1)), np.ones((dofj,)))  # row
-                        row_col_t[1, 3*kk:3*kk+3*dofj] = np.kron(np.ones((3,)), np.arange(kk, kk+dofj))      # col
-                        data_t[3*kk:3*kk+3*dofj] = c.basis.flatten(order='C')
-                        kk += dofj
-            R = scipy.sparse.coo_matrix((data_r, row_col_r),
-                                        shape=(noc, 3*m)).tocsr()
-            T = scipy.sparse.coo_matrix((data_t, row_col_t),
-                                        shape=(3*m, dof)).tocsr()
-        else:
-            R = np.zeros((noc, 3*m))
-            T = np.zeros((3*m, dof))
-            jj = kk = 0
-            for i, c in enumerate(constraints):
-                if c is None:
-                    # add identity to basis
-                    T[3*i:3*(i+1), kk:kk+3] = np.eye(3)
-                    kk += 3
-                else:
-                    # add to constraint
-                    nocj = 3-c.dof
-                    R[jj:jj+nocj, 3*i:3*(i+1)] = c.normal
-                    jj += nocj
-                    if c.dof:
-                        # add to basis
-                        T[3*i:3*(i+1), kk:kk+c.dof] = c.basis
-                        kk += c.dof
-
-        return R, T
-
-    @staticmethod
-    def rigid_body_three_point_constraint(nodes: npt.NDArray, epsilon: float = 1e-8) \
-            -> Tuple['NodeConstraint', 'NodeConstraint', 'NodeConstraint']:
-        """
-        Return three constraints on three given nodes to prevent rigid motion.
-
-        :param nodes: 3 x 3 array of nodes (column oriented)
-        :param epsilon: accuracy to assess co-linearity
-        :return: tuple with 3 node constraints
-
-        **Notes:**
-
-        1. The constraints are as follows:
-           - Node 0 is fixed
-           - Node 1 is allowed to move in the line 0-1
-           - Node 2 is allowed to move in the plane 0-1-2
-        """
-        assert nodes.shape[0] == 3 and nodes.shape[1] == 3, '3 nodes should be provided'
-
-        # determine vector normal to plane
-        v10 = (nodes[:, 1] - nodes[:, 0]).flatten()
-        v20 = (nodes[:, 2] - nodes[:, 0]).flatten()
-        v012p = np.cross(v10, v20)
-
-        if np.linalg.norm(v012p) < epsilon:
-            raise Exception('the three given points do not form a plane')
-
-        # determine normal to vp and v10
-        v10p = np.cross(v10, v012p)
-
-        # constraints are:
-        # - node 0 to be fixed,
-        # - node 1 to be in line from 0 to 1,
-        # - node 2 to be in the plane
-        return NodeConstraint(), NodeConstraint(np.vstack((v012p, v10p))), NodeConstraint(v012p.reshape((1, 3)))
-
-    @staticmethod
-    def rigid_body_constraint(nodes: npt.NDArray, epsilon: float = 1e-8) -> Tuple[npt.NDArray, npt.NDArray]:
-        """
-        Construct rigid-body constraint associated with the given nodes
-
-        The resulting tuple is compatible with :meth:`~tnsgrt.stiffness.Stiffness.apply_constraint`
-
-        :param nodes: 3 x n array of nodes
-        :param epsilon: precision used to assess numerical rank
-        :return: tuple with the constraint matrix, and its null space
-        """
-
-        assert len(nodes.shape) == 2 and nodes.shape[0] == 3, 'nodes must be a 3 x m matrix'
-
-        number_of_nodes = nodes.shape[1]
-
-        # rigid translation
-        t1 = np.zeros((3, number_of_nodes), order='F')
-        t1[0, :] = 1 / np.sqrt(number_of_nodes)
-
-        t2 = np.zeros((3, number_of_nodes), order='F')
-        t2[1, :] = 1 / np.sqrt(number_of_nodes)
-
-        t3 = np.zeros((3, number_of_nodes), order='F')
-        t3[2, :] = 1 / np.sqrt(number_of_nodes)
-
-        # rigid rotations
-        r1 = (np.array([[0, 0, 0], [0, 0, -1], [0, 1, 0]]) @ nodes).ravel(order='F')
-        r2 = (np.array([[0, 0, 1], [0, 0, 0], [-1, 0, 0]]) @ nodes).ravel(order='F')
-        r3 = (np.array([[0, -1, 0], [1, 0, 0], [0, 0, 0]]) @ nodes).ravel(order='F')
-
-        r = np.vstack((t1.ravel(order='F'), t2.ravel(order='F'), t3.ravel(order='F'),
-                       r1 / np.linalg.norm(r1), r2 / np.linalg.norm(r2), r3 / np.linalg.norm(r3)))
-
-        rank, r, t = orthogonalize(r.transpose(), epsilon=epsilon, mode='complete')
-
-        return r.transpose(), t
-
-    @staticmethod
-    def planar_constraint(nodes: npt.NDArray, normal: Optional[npt.NDArray] = None, epsilon: float = 1e-8, storage='sparse'):
-        """
-        Construct the planar constraint associated with the given nodes and normal vector
-
-        The resulting tuple is compatible with :meth:`~tnsgrt.stiffness.Stiffness.apply_constraint`
-
-        :param nodes: 3 x n array of nodes
-        :param normal: list with n constraints
-        :param storage: if ``sparse``, returns sparse arrays
-        :return: tuple with the constraint matrix, and its null space
-        """
-        assert nodes.shape[0] == 3, 'nodes must be a 3 x m array'
-        if normal is None:
-            normal = np.array([[0], [0], [1]])
-        elif normal.ndim == 1 and normal.shape[0] == 3:
-            normal = normal.reshape((3, 1))
-        elif normal.ndim == 2 and normal.shape[0] == 1 and normal.shape[1] == 3:
-            normal = normal.transpose()
-        assert normal.ndim == 2 and normal.shape[0] == 3 and normal.shape[1] == 1, 'normal must be a 3D vector'
-
-        # calculate normal and basis
-        _, normal, basis = orthogonalize(normal, mode='complete', epsilon=epsilon)
-
-        # calculate degrees of freedom
-        n = nodes.shape[1]
-        noc = n
-        dof = 2*n
-
-        if storage == 'sparse':
-            row_col_r = np.zeros((2, 3*noc))
-            data_r = np.zeros((3*noc))
-            row_col_t = np.zeros((2, 3*dof))
-            data_t = np.zeros((3*dof))
-            jj = kk = 0
-            # flatten normal and basis
-            normal = normal.flatten(order='C')
-            basis = basis.flatten(order='C')
-            nocj, dofj = 1, 2
-            for i in range(n):
-                # add to constraint
-                row_col_r[0, 3*jj:3*jj+3*nocj] = np.kron(np.arange(jj, jj+nocj), np.ones((3,)))      # row
-                row_col_r[1, 3*jj:3*jj+3*nocj] = np.kron(np.ones((nocj,)), np.arange(3*i, 3*(i+1)))  # col
-                data_r[3*jj:3*jj+3*nocj] = normal
-                jj += nocj
-                # add to basis
-                row_col_t[0, 3*kk:3*kk+3*dofj] = np.kron(np.arange(3*i, 3*(i+1)), np.ones((dofj,)))  # row
-                row_col_t[1, 3*kk:3*kk+3*dofj] = np.kron(np.ones((3,)), np.arange(kk, kk+dofj))      # col
-                data_t[3*kk:3*kk+3*dofj] = basis
-                kk += dofj
-            R = scipy.sparse.coo_matrix((data_r, row_col_r),
-                                        shape=(noc, 3*n)).tocsr()
-            T = scipy.sparse.coo_matrix((data_t, row_col_t),
-                                        shape=(3*n, dof)).tocsr()
-        else:
-            R = np.zeros((noc, 3*n))
-            T = np.zeros((3*n, dof))
-            jj = kk = 0
-            nocj, dofj = 1, 2
-            normal = normal.flatten()
-            for i in range(n):
-                # add to constraint
-                R[jj:jj+nocj, 3*i:3*(i+1)] = normal
-                jj += nocj
-                # add to basis
-                T[3*i:3*(i+1), kk:kk+dofj] = basis
-                kk += dofj
-
-        return R, T
-
-
-class Stiffness:
-    """
-    Model for a constrained mechanical system consisting of
-
-    - :math:`K`: the stiffness matrix
-    - :math:`M`: the mass matrix
-    - :math:`R`: a matrix representing node displacement constraints
-    - :math:`T`: a matrix representing allowed node displacements
-
-    such that
-
-    .. math::
-        V = \\frac{1}{2} y^T K y + \\frac{1}{2} \\ddot{y}^T M \\ddot{y}, \\qquad R \\, x = 0, \\qquad x = T y
-
-    Constructor parameters:
-
-    :param K: the stiffness matrix
-    :param M: the mass matrix
-
-    **Notes:**
-
-    1. The stiffness and mass matrices are stored in the reduced coordinates :math:`y`
-
-    2. In global coordinates
-
-       .. math::
-           V = \\frac{1}{2} x^T K_x x + \\frac{1}{2} \\ddot{x}^T M_x \\ddot{x}
-
-       in which
-
-       .. math::
-           K_x = T^T K T, \\qquad M_x = T^T M T
-
-    3. Use :meth:`tnsgrt.stiffness.Stiffness.apply_constraint` to apply constraints to the model
-
-    4. Node constraints are enforced to be orthogonal so that
-
-       .. math::
-           R \\, x = 0, \\quad x = T y, \\qquad R R^T = I, \\quad T^T T = I, \\quad R \\, T = 0
-    """
-
-    def __init__(self,
-                 K: Union[npt.NDArray, scipy.sparse.csr_matrix],
-                 M: Optional[Union[npt.NDArray, scipy.sparse.csr_matrix]] = None):
-
-        self.K = K
-        self.M = M
-        self.T: Optional[Union[npt.NDArray, scipy.sparse.csr_matrix]] = None
-        self.R: Optional[Union[npt.NDArray, scipy.sparse.csr_matrix]] = None
-
-        assert K.ndim == 2 and K.shape[0] == K.shape[1], 'K must be a square matrix'
-
-        if M is not None:
-            assert M.ndim == 2 and M.shape[0] == M.shape[1] and M.shape[0] == K.shape[0], \
-                'M must be a square matrix of same size as K'
-
-    def apply_constraint(self,
-                         R: Union[npt.NDArray, scipy.sparse.csr_matrix],
-                         T: Optional[Union[npt.NDArray, scipy.sparse.csr_matrix]] = None,
-                         local: bool = True, epsilon: float = 1e-8):
-        """
-        Apply the constraint
-
-        .. math::
-            R \\, y = 0, \\qquad y = T z
-
-        to the current or the global ``Stiffness`` object coordinate
-
-        :param R: the constraint coefficient matrix
-        :param T: the allowed node displacements; if ``None`` constraint is normalized
-        :param local: if ``True`` the constraint is applied
-        :param epsilon: precision used to assess numerical rank
-        :return:
-
-        **Notes:**
-
-        1. If ``local = True`` and the current constraints are
-
-           .. math::
-               R_y \\, x = 0, \\quad x = T_y \\, y, \\qquad R^{}_y R_y^T = I, \\quad T_y^T T^{}_y = I, \\quad R_y T_y = 0
-
-           then after applying the new constraints
-
-           .. math::
-               R \\, y = R \\, T_y^T x = R_z x = 0, \\qquad x = T_y \\, y = T_y T z = T_z z,
-
-           in which
-
-           .. math::
-               R_z = R \\, T_y^T, \\qquad T_z = T_y T
-
-           and
-
-           .. math::
-               V = \\frac{1}{2} z^T K_z \\, z + \\frac{1}{2} \\ddot{z}^T M_z \\, \\ddot{z}, \\qquad R_z x = 0, \\quad x = R_z \\, z,
-
-           in which
-
-           .. math::
-               K_z = T^T K T, \\qquad M_z = T^T M T
-
-        2. If ``local = False`` and the constraints are interpreted as
-
-           .. math::
-               R \\, x = 0, \\quad x = T \\, z
-
-           which is first converted to the local constraint
-
-           .. math::
-               R \\, x = R \\, T_y y = \\tilde{R} y = 0, \\qquad \\tilde{R} = R \\, T_y,
-
-           before applying
-        """
-
-        if local or self.T is None:
-            # local constraint
-            if T is None:
-                # normalize before applying
-                rank, r, t = orthogonalize(R.transpose(), mode='complete', epsilon=epsilon)
-                r = r.transpose()
-            else:
-                # test orthogonality
-                assert norm(R @ T) < epsilon, 'R and T must be orthogonal'
-                assert norm(R @ R.transpose() - scipy.sparse.eye(R.shape[0])) < epsilon, 'R must be unitary'
-                assert norm(T.transpose() @ T - scipy.sparse.eye(T.shape[1])) < epsilon, 'T must be unitary'
-                r, t = R, T
-
-            # apply constraint
-
-            if scipy.sparse.issparse(self.K):
-                # make sure it is sparse
-                if scipy.sparse.issparse(r):
-                    r = scipy.sparse.csr_matrix(r)
-                if scipy.sparse.issparse(t):
-                    t = scipy.sparse.csr_matrix(t)
-
-            # project stiffness
-            self.K = t.transpose() @ self.K @ t
-
-            # symmetrize
-            self.K += self.K.transpose()
-            self.K /= 2
-
-            if self.M is not None:
-                # project mass
-                self.M = t.transpose() @ self.M @ t
-                self.M += self.M.transpose()
-                self.M /= 2
-
-            if self.R is None:
-                self.R = r
-            else:
-                if self.T is None:
-                    self.R = r
-                else:
-                    self.R = r @ self.T.transpose()
-
-            if self.T is None:
-                self.T = t
-            else:
-                self.T = self.T @ t
-
-        else:
-            # not local and self.T is not None
-            if T is not None:
-                warnings.warn("allowed displacements parameter 'T' ignored when 'local=False'")
-            self.apply_constraint(R @ self.T, epsilon=epsilon)
-
-    def displacements(self, f: npt.NDArray):
-        """
-        Calculate displacements due to the application of a global force
-
-        :param f: 3 x m array of forces
-        :return: the displacements
-
-        **Notes:**
-
-        1. The displacements are calculated in global coordinates
-
-           .. math::
-               x = T K^{-1} T^T f
-        """
-        m = self.K.shape[0] if self.T is None else self.T.shape[0]
-        assert f.shape[0] == 3 and f.shape[1] == m/3, 'f must be a 3 x m array'
-        x = self.T @ np.linalg.solve(self.K, self.T.transpose() @ f.flatten(order='F')) \
-            if self.T is not None else \
-            np.linalg.solve(self.K, f.flatten(order='F'))
-        return x.reshape((3, int(m/3)), order='F')
-
-    def eigs(self, k: int = 12, which: Literal['LM', 'SM', 'LR', 'SR', 'LI', 'SI'] = 'SM'):
-        """
-        Compute the eigenvalues and eigenvectors of the stiffness matrix
-
-        If the stiffness matrix is stored as a sparse array, return only the first k eigenvalue/eigenvector pairs
-
-        :param k: the number of eigenvalues
-        :param which: which eigenvalues to compute; see :func:`scipy.sparse.linalg.eigsh` for details
-        :return: tuple with eigenvalues, and eigenvectors
-
-        **Notes:**
-
-        1. The eigenvalues and eigenvectors are calculated by solving the eigenvalue problem
-
-           .. math::
-               K y = \\lambda \\, y, \\qquad x = T \\, y
-        """
-
-        if scipy.sparse.issparse(self.K):
-            # calculate sparse eigenvalues
-            d, v = scipy.sparse.linalg.eigsh(self.K, k=k, which=which)
-
-        else:
-            # calculate dense eigenvalues
-            d, v = np.linalg.eigh(self.K)
-
-        # sort
-        ind = np.argsort(d)
-
-        # project eigenvectors
-        if self.T is not None:
-            v = self.T @ v
-
-        return d[ind], v[:, ind]
-
-    def modes(self, k: int = 12, units='Hz', which: Literal['LM', 'SM'] = 'SM'):
-        """
-        Compute the natural frequencies [rad/s] and mode vectors
-
-        :param k: the number of eigenvalues
-        :param which: which eigenvalues to compute; see :func:`scipy.sparse.linalg.eigsh` for details
-        :param units: return frequencies in Hz if ``units = 'Hz'``
-        :return: tuple with eigenvalues, and eigenvectors
-
-        **Notes:**
-
-        1. The natural frequencies and mode vectors are calculated by solving the generalized eigenvalue problem
-
-           .. math::
-               K y = \\omega^2 M y, \\qquad x = T \\, y
-        """
-
-        assert self.M is not None, 'modes cannot be calculated without mass information'
-
-        if scipy.sparse.issparse(self.K):
-            # calculate sparse eigenvalues
-            d, v = scipy.sparse.linalg.eigsh(self.K, k=k, M=self.M, which=which)
-        else:
-            # calculate dense eigenvalues
-            d, v = scipy.linalg.eigh(self.K, self.M)
-
-        # calculate frequencies
-        d = np.sqrt(np.abs(d))
-        if units == 'Hz':
-            d /= 2*np.pi
-
-        # sort
-        ind = np.argsort(d)
-
-        # project eigenvectors
-        if self.T is not None:
-            v = self.T @ v
-
-        return d[ind], v[:, ind]
-
+import warnings
+from typing import Optional, Tuple, Sequence, Union, Literal
+import numpy as np
+import numpy.typing as npt
+import scipy
+
+from .utils import orthogonalize, norm
+
+
+class NodeConstraint:
+    """
+    Object representing a node constraint
+
+    :param constraint: the constraint coefficient array
+    :param epsilon: precision used to assess numerical rank
+
+    **Notes:**
+
+    1. If :math:`x` is the node coordinate and :math:`A` is the constraint coefficient then
+
+       .. math::
+           A x = 0
+
+       then the equivalent constraint and its null space
+
+       .. math::
+           R \\, x = 0, \\quad x = T \\, y, \\quad R R^T = I, \\quad T^T T = I
+
+       is constructed using :func:`tnsgrt.utils.orthogonalize`
+    """
+
+    def __init__(self, constraint: Optional[npt.NDArray] = None, epsilon: float = 1e-8):
+        if constraint is None:
+            self.dof = 0
+            self.basis = None
+            self.normal = np.eye(3)
+        else:
+            assert constraint.ndim == 2 and constraint.shape[1] == 3 and constraint.shape[0] < 3, \
+                'normal must be a m x 3, m < 3, array'
+            # first orthogonalize
+            rank, r, t = orthogonalize(constraint.transpose(), mode='complete', epsilon=epsilon)
+            self.dof = 3 - rank
+            if self.dof == 0:
+                self.basis = None
+                self.normal = np.eye(3)
+            else:
+                self.normal = r.transpose()
+                self.basis = t
+
+    @staticmethod
+    def node_constraint(nodes: npt.NDArray, constraints: Sequence['NodeConstraint'],
+                        storage: Literal['sparse', 'dense'] = 'sparse') \
+            -> Union[Tuple[npt.NDArray, npt.NDArray], Tuple[scipy.sparse.csr_array, scipy.sparse.csr_array]]:
+        """
+        Construct the constraint associated with the given nodes and node constraints
+
+        The resulting tuple is compatible with :meth:`~tnsgrt.stiffness.Stiffness.apply_constraint`
+
+        :param nodes: 3 x n array of nodes
+        :param constraints: list with n constraints
+        :param storage: if ``sparse``, returns sparse arrays
+        :return: tuple with the constraint matrix, and its null space
+        """
+        assert nodes.shape[0] == 3, 'nodes must be a 3 x m array'
+        assert nodes.shape[1] == len(constraints), \
+            'number of columns of nodes must be equal to to the number of constraints'
+
+        # calculate degrees of freedom
+        m = nodes.shape[1]
+        noc = sum(3 - c.dof for c in constraints if c is not None)
+        dof = 3*m - noc
+
+        if storage == 'sparse':
+            row_col_r = np.zeros((2, 3*noc))
+            data_r = np.zeros((3*noc))
+            row_col_t = np.zeros((2, 3*dof))
+            data_t = np.zeros((3*dof))
+            jj = kk = 0
+            for i, c in enumerate(constraints):
+                if c is None:
+                    # add identity to basis
+                    dofj = 3
+                    row_col_t[0, 3*kk:3*kk+3*dofj] = np.kron(np.arange(3*i, 3*(i+1)), np.ones((3,)))
+                    row_col_t[1, 3*kk:3*kk+3*dofj] = np.kron(np.arange(kk, kk+dofj), np.ones((3,)))
+                    data_t[3*kk:3*kk+3*dofj] = np.eye(dofj).flatten(order='C')
+                    kk += dofj
+                else:
+                    # add to normal
+                    nocj = 3-c.dof
+                    row_col_r[0, 3*jj:3*jj+3*nocj] = np.kron(np.arange(jj, jj+nocj), np.ones((3,)))      # row
+                    row_col_r[1, 3*jj:3*jj+3*nocj] = np.kron(np.ones((nocj,)), np.arange(3*i, 3*(i+1)))  # col
+                    data_r[3*jj:3*jj+3*nocj] = c.normal.flatten(order='C')
+                    jj += nocj
+                    if c.dof:
+                        # add to basis
+                        dofj = c.dof
+                        row_col_t[0, 3*kk:3*kk+3*dofj] = np.kron(np.arange(3*i, 3*(i+1)), np.ones((dofj,)))  # row
+                        row_col_t[1, 3*kk:3*kk+3*dofj] = np.kron(np.ones((3,)), np.arange(kk, kk+dofj))      # col
+                        data_t[3*kk:3*kk+3*dofj] = c.basis.flatten(order='C')
+                        kk += dofj
+            R = scipy.sparse.coo_matrix((data_r, row_col_r),
+                                        shape=(noc, 3*m)).tocsr()
+            T = scipy.sparse.coo_matrix((data_t, row_col_t),
+                                        shape=(3*m, dof)).tocsr()
+        else:
+            R = np.zeros((noc, 3*m))
+            T = np.zeros((3*m, dof))
+            jj = kk = 0
+            for i, c in enumerate(constraints):
+                if c is None:
+                    # add identity to basis
+                    T[3*i:3*(i+1), kk:kk+3] = np.eye(3)
+                    kk += 3
+                else:
+                    # add to constraint
+                    nocj = 3-c.dof
+                    R[jj:jj+nocj, 3*i:3*(i+1)] = c.normal
+                    jj += nocj
+                    if c.dof:
+                        # add to basis
+                        T[3*i:3*(i+1), kk:kk+c.dof] = c.basis
+                        kk += c.dof
+
+        return R, T
+
+    @staticmethod
+    def rigid_body_three_point_constraint(nodes: npt.NDArray, epsilon: float = 1e-8) \
+            -> Tuple['NodeConstraint', 'NodeConstraint', 'NodeConstraint']:
+        """
+        Return three constraints on three given nodes to prevent rigid motion.
+
+        :param nodes: 3 x 3 array of nodes (column oriented)
+        :param epsilon: accuracy to assess co-linearity
+        :return: tuple with 3 node constraints
+
+        **Notes:**
+
+        1. The constraints are as follows:
+           - Node 0 is fixed
+           - Node 1 is allowed to move in the line 0-1
+           - Node 2 is allowed to move in the plane 0-1-2
+        """
+        assert nodes.shape[0] == 3 and nodes.shape[1] == 3, '3 nodes should be provided'
+
+        # determine vector normal to plane
+        v10 = (nodes[:, 1] - nodes[:, 0]).flatten()
+        v20 = (nodes[:, 2] - nodes[:, 0]).flatten()
+        v012p = np.cross(v10, v20)
+
+        if np.linalg.norm(v012p) < epsilon:
+            raise Exception('the three given points do not form a plane')
+
+        # determine normal to vp and v10
+        v10p = np.cross(v10, v012p)
+
+        # constraints are:
+        # - node 0 to be fixed,
+        # - node 1 to be in line from 0 to 1,
+        # - node 2 to be in the plane
+        return NodeConstraint(), NodeConstraint(np.vstack((v012p, v10p))), NodeConstraint(v012p.reshape((1, 3)))
+
+    @staticmethod
+    def rigid_body_constraint(nodes: npt.NDArray, epsilon: float = 1e-8) -> Tuple[npt.NDArray, npt.NDArray]:
+        """
+        Construct rigid-body constraint associated with the given nodes
+
+        The resulting tuple is compatible with :meth:`~tnsgrt.stiffness.Stiffness.apply_constraint`
+
+        :param nodes: 3 x n array of nodes
+        :param epsilon: precision used to assess numerical rank
+        :return: tuple with the constraint matrix, and its null space
+        """
+
+        assert len(nodes.shape) == 2 and nodes.shape[0] == 3, 'nodes must be a 3 x m matrix'
+
+        number_of_nodes = nodes.shape[1]
+
+        # rigid translation
+        t1 = np.zeros((3, number_of_nodes), order='F')
+        t1[0, :] = 1 / np.sqrt(number_of_nodes)
+
+        t2 = np.zeros((3, number_of_nodes), order='F')
+        t2[1, :] = 1 / np.sqrt(number_of_nodes)
+
+        t3 = np.zeros((3, number_of_nodes), order='F')
+        t3[2, :] = 1 / np.sqrt(number_of_nodes)
+
+        # rigid rotations
+        r1 = (np.array([[0, 0, 0], [0, 0, -1], [0, 1, 0]]) @ nodes).ravel(order='F')
+        r2 = (np.array([[0, 0, 1], [0, 0, 0], [-1, 0, 0]]) @ nodes).ravel(order='F')
+        r3 = (np.array([[0, -1, 0], [1, 0, 0], [0, 0, 0]]) @ nodes).ravel(order='F')
+
+        r = np.vstack((t1.ravel(order='F'), t2.ravel(order='F'), t3.ravel(order='F'),
+                       r1 / np.linalg.norm(r1), r2 / np.linalg.norm(r2), r3 / np.linalg.norm(r3)))
+
+        rank, r, t = orthogonalize(r.transpose(), epsilon=epsilon, mode='complete')
+
+        return r.transpose(), t
+
+    @staticmethod
+    def planar_constraint(nodes: npt.NDArray, normal: Optional[npt.NDArray] = None, epsilon: float = 1e-8, storage='sparse'):
+        """
+        Construct the planar constraint associated with the given nodes and normal vector
+
+        The resulting tuple is compatible with :meth:`~tnsgrt.stiffness.Stiffness.apply_constraint`
+
+        :param nodes: 3 x n array of nodes
+        :param normal: list with n constraints
+        :param storage: if ``sparse``, returns sparse arrays
+        :return: tuple with the constraint matrix, and its null space
+        """
+        assert nodes.shape[0] == 3, 'nodes must be a 3 x m array'
+        if normal is None:
+            normal = np.array([[0], [0], [1]])
+        elif normal.ndim == 1 and normal.shape[0] == 3:
+            normal = normal.reshape((3, 1))
+        elif normal.ndim == 2 and normal.shape[0] == 1 and normal.shape[1] == 3:
+            normal = normal.transpose()
+        assert normal.ndim == 2 and normal.shape[0] == 3 and normal.shape[1] == 1, 'normal must be a 3D vector'
+
+        # calculate normal and basis
+        _, normal, basis = orthogonalize(normal, mode='complete', epsilon=epsilon)
+
+        # calculate degrees of freedom
+        n = nodes.shape[1]
+        noc = n
+        dof = 2*n
+
+        if storage == 'sparse':
+            row_col_r = np.zeros((2, 3*noc))
+            data_r = np.zeros((3*noc))
+            row_col_t = np.zeros((2, 3*dof))
+            data_t = np.zeros((3*dof))
+            jj = kk = 0
+            # flatten normal and basis
+            normal = normal.flatten(order='C')
+            basis = basis.flatten(order='C')
+            nocj, dofj = 1, 2
+            for i in range(n):
+                # add to constraint
+                row_col_r[0, 3*jj:3*jj+3*nocj] = np.kron(np.arange(jj, jj+nocj), np.ones((3,)))      # row
+                row_col_r[1, 3*jj:3*jj+3*nocj] = np.kron(np.ones((nocj,)), np.arange(3*i, 3*(i+1)))  # col
+                data_r[3*jj:3*jj+3*nocj] = normal
+                jj += nocj
+                # add to basis
+                row_col_t[0, 3*kk:3*kk+3*dofj] = np.kron(np.arange(3*i, 3*(i+1)), np.ones((dofj,)))  # row
+                row_col_t[1, 3*kk:3*kk+3*dofj] = np.kron(np.ones((3,)), np.arange(kk, kk+dofj))      # col
+                data_t[3*kk:3*kk+3*dofj] = basis
+                kk += dofj
+            R = scipy.sparse.coo_matrix((data_r, row_col_r),
+                                        shape=(noc, 3*n)).tocsr()
+            T = scipy.sparse.coo_matrix((data_t, row_col_t),
+                                        shape=(3*n, dof)).tocsr()
+        else:
+            R = np.zeros((noc, 3*n))
+            T = np.zeros((3*n, dof))
+            jj = kk = 0
+            nocj, dofj = 1, 2
+            normal = normal.flatten()
+            for i in range(n):
+                # add to constraint
+                R[jj:jj+nocj, 3*i:3*(i+1)] = normal
+                jj += nocj
+                # add to basis
+                T[3*i:3*(i+1), kk:kk+dofj] = basis
+                kk += dofj
+
+        return R, T
+
+
+class Stiffness:
+    """
+    Model for a constrained mechanical system consisting of
+
+    - :math:`K`: the stiffness matrix
+    - :math:`M`: the mass matrix
+    - :math:`R`: a matrix representing node displacement constraints
+    - :math:`T`: a matrix representing allowed node displacements
+
+    such that
+
+    .. math::
+        V = \\frac{1}{2} y^T K y + \\frac{1}{2} \\ddot{y}^T M \\ddot{y}, \\qquad R \\, x = 0, \\qquad x = T y
+
+    Constructor parameters:
+
+    :param K: the stiffness matrix
+    :param M: the mass matrix
+
+    **Notes:**
+
+    1. The stiffness and mass matrices are stored in the reduced coordinates :math:`y`
+
+    2. In global coordinates
+
+       .. math::
+           V = \\frac{1}{2} x^T K_x x + \\frac{1}{2} \\ddot{x}^T M_x \\ddot{x}
+
+       in which
+
+       .. math::
+           K_x = T^T K T, \\qquad M_x = T^T M T
+
+    3. Use :meth:`tnsgrt.stiffness.Stiffness.apply_constraint` to apply constraints to the model
+
+    4. Node constraints are enforced to be orthogonal so that
+
+       .. math::
+           R \\, x = 0, \\quad x = T y, \\qquad R R^T = I, \\quad T^T T = I, \\quad R \\, T = 0
+    """
+
+    def __init__(self,
+                 K: Union[npt.NDArray, scipy.sparse.csr_matrix],
+                 M: Optional[Union[npt.NDArray, scipy.sparse.csr_matrix]] = None):
+
+        self.K = K
+        self.M = M
+        self.T: Optional[Union[npt.NDArray, scipy.sparse.csr_matrix]] = None
+        self.R: Optional[Union[npt.NDArray, scipy.sparse.csr_matrix]] = None
+
+        assert K.ndim == 2 and K.shape[0] == K.shape[1], 'K must be a square matrix'
+
+        if M is not None:
+            assert M.ndim == 2 and M.shape[0] == M.shape[1] and M.shape[0] == K.shape[0], \
+                'M must be a square matrix of same size as K'
+
+    def apply_constraint(self,
+                         R: Union[npt.NDArray, scipy.sparse.csr_matrix],
+                         T: Optional[Union[npt.NDArray, scipy.sparse.csr_matrix]] = None,
+                         local: bool = True, epsilon: float = 1e-8):
+        """
+        Apply the constraint
+
+        .. math::
+            R \\, y = 0, \\qquad y = T z
+
+        to the current or the global ``Stiffness`` object coordinate
+
+        :param R: the constraint coefficient matrix
+        :param T: the allowed node displacements; if ``None`` constraint is normalized
+        :param local: if ``True`` the constraint is applied
+        :param epsilon: precision used to assess numerical rank
+        :return:
+
+        **Notes:**
+
+        1. If ``local = True`` and the current constraints are
+
+           .. math::
+               R_y \\, x = 0, \\quad x = T_y \\, y, \\qquad R^{}_y R_y^T = I, \\quad T_y^T T^{}_y = I, \\quad R_y T_y = 0
+
+           then after applying the new constraints
+
+           .. math::
+               R \\, y = R \\, T_y^T x = R_z x = 0, \\qquad x = T_y \\, y = T_y T z = T_z z,
+
+           in which
+
+           .. math::
+               R_z = R \\, T_y^T, \\qquad T_z = T_y T
+
+           and
+
+           .. math::
+               V = \\frac{1}{2} z^T K_z \\, z + \\frac{1}{2} \\ddot{z}^T M_z \\, \\ddot{z}, \\qquad R_z x = 0, \\quad x = R_z \\, z,
+
+           in which
+
+           .. math::
+               K_z = T^T K T, \\qquad M_z = T^T M T
+
+        2. If ``local = False`` and the constraints are interpreted as
+
+           .. math::
+               R \\, x = 0, \\quad x = T \\, z
+
+           which is first converted to the local constraint
+
+           .. math::
+               R \\, x = R \\, T_y y = \\tilde{R} y = 0, \\qquad \\tilde{R} = R \\, T_y,
+
+           before applying
+        """
+
+        if local or self.T is None:
+            # local constraint
+            if T is None:
+                # normalize before applying
+                rank, r, t = orthogonalize(R.transpose(), mode='complete', epsilon=epsilon)
+                r = r.transpose()
+            else:
+                # test orthogonality
+                assert norm(R @ T) < epsilon, 'R and T must be orthogonal'
+                assert norm(R @ R.transpose() - scipy.sparse.eye(R.shape[0])) < epsilon, 'R must be unitary'
+                assert norm(T.transpose() @ T - scipy.sparse.eye(T.shape[1])) < epsilon, 'T must be unitary'
+                r, t = R, T
+
+            # apply constraint
+
+            if scipy.sparse.issparse(self.K):
+                # make sure it is sparse
+                if scipy.sparse.issparse(r):
+                    r = scipy.sparse.csr_matrix(r)
+                if scipy.sparse.issparse(t):
+                    t = scipy.sparse.csr_matrix(t)
+
+            # project stiffness
+            self.K = t.transpose() @ self.K @ t
+
+            # symmetrize
+            self.K += self.K.transpose()
+            self.K /= 2
+
+            if self.M is not None:
+                # project mass
+                self.M = t.transpose() @ self.M @ t
+                self.M += self.M.transpose()
+                self.M /= 2
+
+            if self.R is None:
+                self.R = r
+            else:
+                if self.T is None:
+                    self.R = r
+                else:
+                    self.R = r @ self.T.transpose()
+
+            if self.T is None:
+                self.T = t
+            else:
+                self.T = self.T @ t
+
+        else:
+            # not local and self.T is not None
+            if T is not None:
+                warnings.warn("allowed displacements parameter 'T' ignored when 'local=False'")
+            self.apply_constraint(R @ self.T, epsilon=epsilon)
+
+    def displacements(self, f: npt.NDArray):
+        """
+        Calculate displacements due to the application of a global force
+
+        :param f: 3 x m array of forces
+        :return: the displacements
+
+        **Notes:**
+
+        1. The displacements are calculated in global coordinates
+
+           .. math::
+               x = T K^{-1} T^T f
+        """
+        m = self.K.shape[0] if self.T is None else self.T.shape[0]
+        assert f.shape[0] == 3 and f.shape[1] == m/3, 'f must be a 3 x m array'
+        x = self.T @ np.linalg.solve(self.K, self.T.transpose() @ f.flatten(order='F')) \
+            if self.T is not None else \
+            np.linalg.solve(self.K, f.flatten(order='F'))
+        return x.reshape((3, int(m/3)), order='F')
+
+    def eigs(self, k: int = 12, which: Literal['LM', 'SM', 'LR', 'SR', 'LI', 'SI'] = 'SM'):
+        """
+        Compute the eigenvalues and eigenvectors of the stiffness matrix
+
+        If the stiffness matrix is stored as a sparse array, return only the first k eigenvalue/eigenvector pairs
+
+        :param k: the number of eigenvalues
+        :param which: which eigenvalues to compute; see :func:`scipy.sparse.linalg.eigsh` for details
+        :return: tuple with eigenvalues, and eigenvectors
+
+        **Notes:**
+
+        1. The eigenvalues and eigenvectors are calculated by solving the eigenvalue problem
+
+           .. math::
+               K y = \\lambda \\, y, \\qquad x = T \\, y
+        """
+
+        if scipy.sparse.issparse(self.K):
+            # calculate sparse eigenvalues
+            d, v = scipy.sparse.linalg.eigsh(self.K, k=k, which=which)
+
+        else:
+            # calculate dense eigenvalues
+            d, v = np.linalg.eigh(self.K)
+
+        # sort
+        ind = np.argsort(d)
+
+        # project eigenvectors
+        if self.T is not None:
+            v = self.T @ v
+
+        return d[ind], v[:, ind]
+
+    def modes(self, k: int = 12, units='Hz', which: Literal['LM', 'SM'] = 'SM'):
+        """
+        Compute the natural frequencies [rad/s] and mode vectors
+
+        :param k: the number of eigenvalues
+        :param which: which eigenvalues to compute; see :func:`scipy.sparse.linalg.eigsh` for details
+        :param units: return frequencies in Hz if ``units = 'Hz'``
+        :return: tuple with eigenvalues, and eigenvectors
+
+        **Notes:**
+
+        1. The natural frequencies and mode vectors are calculated by solving the generalized eigenvalue problem
+
+           .. math::
+               K y = \\omega^2 M y, \\qquad x = T \\, y
+        """
+
+        assert self.M is not None, 'modes cannot be calculated without mass information'
+
+        if scipy.sparse.issparse(self.K):
+            # calculate sparse eigenvalues
+            d, v = scipy.sparse.linalg.eigsh(self.K, k=k, M=self.M, which=which)
+        else:
+            # calculate dense eigenvalues
+            d, v = scipy.linalg.eigh(self.K, self.M)
+
+        # calculate frequencies
+        d = np.sqrt(np.abs(d))
+        if units == 'Hz':
+            d /= 2*np.pi
+
+        # sort
+        ind = np.argsort(d)
+
+        # project eigenvectors
+        if self.T is not None:
+            v = self.T @ v
+
+        return d[ind], v[:, ind]
+
```

### Comparing `tnsgrt-0.3/src/tnsgrt/structure.py` & `tnsgrt-0.4/src/tnsgrt/structure.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,1160 +1,1160 @@
-import warnings
-from dataclasses import dataclass
-from functools import reduce
-from typing import Optional, Dict, get_type_hints, Union, List, Sequence, Type, Iterable, Tuple, Set, Any
-from collections import ChainMap
-
-import numpy as np
-import numpy.typing as npt
-import pandas as pd
-import scipy
-
-from . import utils
-from . import optim
-from .stiffness import Stiffness, NodeConstraint
-
-
-class Property:
-    """
-    Base class for storing properties
-
-    Derived classes should implement ``dataclass`` from ``dataclasses``
-    """
-
-    @classmethod
-    def to_dataframe(cls: Type['Property'], data: Union[list, tuple] = tuple()) -> pd.DataFrame:
-        # setup member property as pandas dataframe
-        hints = get_type_hints(cls)
-        return pd.DataFrame(data=data, columns=list(hints.keys())).astype(dtype=hints)
-
-
-class Structure:
-    """
-    A ``Structure`` object
-
-    :param nodes: a 3 x n array representing the ``Structure``'s nodes
-    :param members: a 3 x m array representing the ``Structure``'s members
-    :param number_of_strings: the number of strings in ``Structure``
-    :param node_tags: a dictionary with the node tags
-    :param member_tags: a dictionary with the member tags
-    :param label: the ``Structure``'s label
-    """
-
-    @dataclass
-    class NodeProperty(Property):
-        """
-        Subclass representing properties of nodes
-        """
-        radius: float = 0.002
-        visible: bool = True
-        constraint: object = None
-        facecolor: object = utils.Colors.BLUE.value
-        edgecolor: object = utils.Colors.BLUE.value
-
-    node_defaults = {
-    }
-
-    @dataclass
-    class MemberProperty(Property):
-        """
-        Subclass representing properties of members
-        """
-        lambda_: float = 0.
-        force: float = 0.
-        stiffness: float = 0.
-        volume: float = 0.
-        radius: float = 0.01
-        inner_radius: float = 0
-        mass: float = 1.
-        rest_length: float = 0.
-        # ASTM A36 steel
-        yld: float = 250e6
-        density: float = 7.85e3
-        modulus: float = 200e9
-        visible: bool = True
-        facecolor: object = (1, 0, 0)
-        edgecolor: object = (1, 0, 0)
-        linewidth: int = 2
-        linestyle: str = '-'
-
-    member_defaults = {
-        'bar': {
-            'facecolor': utils.Colors.BLUE.value,
-            'edgecolor': utils.Colors.BLUE.value
-        },
-        'string': {
-            'facecolor': utils.Colors.ORANGE.value,
-            'edgecolor': utils.Colors.ORANGE.value,
-            'radius': 0.005
-        }
-    }
-
-    def __init__(self,
-                 nodes: npt.ArrayLike = np.zeros((3, 0), np.float_),
-                 members: npt.ArrayLike = np.zeros((2, 0), np.int64),
-                 number_of_strings: int = 0,
-                 node_tags: Optional[Dict[str, npt.NDArray[np.uint64]]] = None,
-                 member_tags: Optional[Dict[str, npt.NDArray[np.uint64]]] = None,
-                 label: str = None):
-        # label
-        self.label: Optional[str] = label
-        # nodes
-        self.nodes: npt.NDArray[np.float_] = np.zeros((3, 0), np.float_)
-        self.node_tags: Dict[str, npt.NDArray[np.uint64]] = {}
-        self.node_properties: pd.DataFrame = Structure.NodeProperty.to_dataframe()
-        # members
-        self.members: npt.NDArray[np.uint64] = np.zeros((2, 0), np.uint64)
-        self.member_tags: Dict[str, npt.NDArray[np.uint64]] = {
-            'bar': np.zeros((0,), np.uint64),
-            'string': np.zeros((0,), np.uint64)
-        }
-        self.member_properties: pd.DataFrame = Structure.MemberProperty.to_dataframe()
-
-        # add nodes
-        self.add_nodes(nodes, node_tags)
-
-        # add members
-        self.add_members(members, number_of_strings, member_tags)
-
-    def __repr__(self) -> str:
-        """
-        :return: short description of structure as a string
-        """
-        return "Structure " + (f" labeled '{self.label}'" if self.label else '') + \
-            f"with {self.get_number_of_members_by_tag('bar')} bars " \
-            f"and {self.get_number_of_members_by_tag('string')} strings"
-
-    def copy(self) -> 'Structure':
-        """
-        :return: copy of the Structure
-        """
-
-        # instantiate copy of the current structure
-        copy = self.__class__()
-
-        # copy basic structure
-        copy.label = self.label
-        copy.nodes = self.nodes.copy()
-        copy.node_tags = self.node_tags.copy()
-        copy.node_properties = self.node_properties.copy()
-        copy.members = self.members.copy()
-        copy.member_tags = self.member_tags.copy()
-        copy.member_properties = self.member_properties.copy()
-
-        return copy
-
-    def set_nodes(self, nodes: npt.ArrayLike) -> None:
-        """
-        Set nodes of the ``Structure``
-
-        :param nodes: the nodes
-        """
-        # convert to array
-        nodes = np.array(nodes, np.float_)
-
-        # test dimensions
-        assert np.all(nodes.shape == self.nodes.shape), 'nodes shape must match current shape'
-
-        # set nodes
-        self.nodes: npt.NDArray[np.float_] = nodes
-
-    def add_nodes(self, nodes: npt.ArrayLike,
-                  node_tags: Optional[Dict[str, npt.NDArray[np.uint64]]] = None) -> None:
-        """
-        Add nodes to the ``Structure``
-
-        :param nodes: the nodes to add
-        :param node_tags: the node tags to add
-        """
-        # add nodes and tags to current structure
-
-        # convert to array
-        nodes = np.array(nodes, np.float_)
-
-        # test dimensions
-        assert nodes.shape[0] == 3, 'nodes must be a 3 x n array'
-
-        # node tags
-        number_of_new_nodes = nodes.shape[1]
-        if node_tags is None:
-            node_tags = {}
-        else:
-            # make sure node tags are unique
-            for k, v in node_tags.items():
-                node_tags[k] = np.unique(v)
-                assert np.amin(v) >= 0, \
-                    'node tag index must be greater or equal than zero'
-                assert np.amax(v) < number_of_new_nodes, \
-                    'node tag index must be less than number of new nodes'
-
-        # new node properties
-        number_of_nodes = self.get_number_of_nodes()
-        # determine tags that have defaults
-        tags_with_defaults = list(set(node_tags.keys()) & set(Structure.node_defaults.keys()))
-        # apply defaults
-        new_node_properties = [Structure.NodeProperty(**ChainMap(*[Structure.node_defaults[tag]
-                                                                   for tag in tags_with_defaults
-                                                                   if i in node_tags[tag]]))
-                               for i in range(nodes.shape[1])]
-
-        # add new nodes
-        self.nodes: npt.NDArray[np.float_] = np.hstack((self.nodes, nodes))
-
-        # add node tags
-        for k, v in node_tags.items():
-            self.node_tags[k] = np.hstack((self.node_tags[k], number_of_nodes + v)) \
-                if k in self.node_tags else number_of_nodes + v
-
-        # add default node properties
-        self.node_properties = pd.concat((self.node_properties,
-                                          Structure.NodeProperty.to_dataframe(new_node_properties)),
-                                         ignore_index=True)
-
-    def get_number_of_nodes(self) -> int:
-        """
-        :return: the number of nodes in ``Structure``
-        """
-        return self.nodes.shape[1]
-
-    def translate(self, v: npt.NDArray) -> 'Structure':
-        """
-        Translate all nodes of the ``Structure`` by the 3D vector ``normal``
-
-        :param v: the 3D translation vector
-        :return: self
-        """
-        # `translate(normal)` translates nodes of the structure by the 3D vector `normal`
-        assert v.shape == (3,), 'normal must be a three dimensional vector'
-        self.nodes += v.reshape((3, 1))
-        return self
-
-    def rotate(self, v: npt.NDArray) -> 'Structure':
-        """
-        Rotate all nodes of the ``Structure`` by the 3D vector ``normal``
-
-        :param v: the 3D rotation vector
-        :return: self
-        """
-        # `rotate(normal)` rotates the nodes of the structure around the 3D vector `normal`
-        # the magnitude of the vector equals the rotation angle in radians
-        assert v.shape == (3,), 'normal must be a three dimensional vector'
-        rotation = scipy.spatial.transform.Rotation.from_rotvec(v)
-        self.nodes = rotation.apply(self.nodes.transpose()).transpose()
-        return self
-
-    def reflect(self, v: npt.NDArray, p: Optional[npt.NDArray] = None) -> 'Structure':
-        """
-        Reflects the structure about a plane normal to the vector `normal`, passing through the point `p`.
-        If no point is given, it defaults to the origin.
-
-        :param v: the 3D normal vector
-        :param p: the 3D origin vector
-        :return: self
-        """
-        assert v.shape == (3,), 'normal must be a three dimensional vector'
-
-        if p is not None:
-            assert p.shape == (3,), 'p must be a three dimensional vector'
-            # translate by p
-            self.nodes -= p.reshape((3, 1))
-
-        # normalize normal
-        length = np.linalg.norm(v)
-        if length < 1e-6:
-            warnings.warn('norm of vector normal is too small, reflection not performed')
-            return self
-
-        # calculate reflection matrix
-        reflection_matrix = np.eye(3) - (2 / length**2) * np.outer(v, v)
-
-        # transform nodes
-        self.nodes = reflection_matrix @ self.nodes
-
-        if p is not None:
-            # translate back to p
-            self.nodes += p.reshape((3, 1))
-
-        return self
-
-    def get_unused_nodes(self) -> npt.NDArray[np.uint64]:
-        """
-        :return: an array with the indices of the unused nodes
-        """
-        # calculate nodes that are in use
-        used_nodes = np.unique(self.members)
-        # return unused nodes
-        return np.setdiff1d(np.arange(self.get_number_of_nodes()), used_nodes, assume_unique=True)
-
-    def has_unused_nodes(self) -> bool:
-        """
-        :return: ``True`` if there are no unused nodes
-        """
-        return len(self.get_unused_nodes()) > 0
-
-    def remove_nodes(self, nodes_to_be_deleted: Optional[npt.ArrayLike] = None,
-                     verify_if_unused: bool = True, verbose: bool = False) -> None:
-        """
-        Remove nodes from structure
-
-        :param nodes_to_be_deleted: the indices of the nodes to be deleted; if ``None``,
-                                    delete all currently unused nodes
-        :param verify_if_unused: if ``True`` verifies if the nodes to be deleted are not in use
-        :param verbose: if ``True`` warns of the nodes to be deleted
-        """
-        if nodes_to_be_deleted is None:
-            # delete all unused nodes
-            unused_nodes_to_be_deleted = self.get_unused_nodes()
-        elif verify_if_unused:
-            # sort nodes to be deleted
-            nodes_to_be_deleted = np.unique(nodes_to_be_deleted)
-            # calculate nodes that are in use
-            used_nodes = np.unique(self.members)
-            # find unused nodes
-            unused_nodes_to_be_deleted = np.setdiff1d(nodes_to_be_deleted, used_nodes, assume_unique=True)
-            # warn if different
-            number_of_used_nodes = len(nodes_to_be_deleted) - len(unused_nodes_to_be_deleted)
-            if number_of_used_nodes:
-                warnings.warn(f'{number_of_used_nodes} nodes are still in use and were not deleted')
-                if verbose:
-                    warnings.warn('The following nodes will not be removed: ' 
-                                  f'{np.intersect1d(nodes_to_be_deleted, used_nodes, assume_unique=True)}')
-        else:
-            # go ahead without verifying if nodes are unused
-            # WARNING: this may result in orphan members!
-            unused_nodes_to_be_deleted = nodes_to_be_deleted
-        # delete if there are any unused nodes
-        if len(unused_nodes_to_be_deleted):
-            if verbose:
-                warnings.warn('The following nodes will be removed: '
-                              f'{unused_nodes_to_be_deleted}')
-            # create new node map
-            node_index = np.delete(np.arange(self.get_number_of_nodes()), unused_nodes_to_be_deleted)
-            new_node_map = np.zeros((self.get_number_of_nodes(),), dtype=np.int_)
-            new_node_map[node_index] = np.arange(self.get_number_of_nodes() - len(unused_nodes_to_be_deleted))
-            # remove nodes
-            self.nodes = np.delete(self.nodes, unused_nodes_to_be_deleted, axis=1)
-            # remove node properties
-            self.node_properties.drop(unused_nodes_to_be_deleted, inplace=True)
-            self.node_properties.reset_index(inplace=True)
-            # remove nodes from tags
-            self.node_tags = {k: new_node_map[np.setdiff1d(v, unused_nodes_to_be_deleted)]
-                              for k, v in self.node_tags.items()}
-            # apply new node map to members
-            self.members = new_node_map[self.members]
-
-    def add_members(self, members: npt.ArrayLike,
-                    number_of_strings: Optional[int] = None,
-                    member_tags: Optional[Dict[str, npt.NDArray[np.uint64]]] = None) -> None:
-        """
-        Add members and tags to current structure
-
-        :param members: the members to be added
-        :param number_of_strings: the number of strings; if not ``None``,  then the first `number_of_strings` members
-                                  are tagged as 'strings' and the remaining members as 'bars'
-        :param  member_tags: the new members' tags
-        """
-
-        # convert to array
-        members = np.array(members, np.uint64)
-
-        # test dimensions
-        assert members.shape[0] == 2, 'members must be a 2 x m array'
-
-        # member tags
-        if number_of_strings is None and member_tags is None:
-            raise Exception('Either type or number of strings must be provided')
-
-        number_of_new_members = members.shape[1]
-        new_member_tags = {}
-        if number_of_strings is not None:
-            # number of strings given
-            assert number_of_strings <= number_of_new_members, \
-                'number of added strings must be less than number of added members'
-            number_of_new_bars = number_of_new_members - number_of_strings
-            new_member_tags = {
-                'string': np.arange(0, number_of_strings, dtype=np.uint64),
-                'bar': number_of_strings + np.arange(0, number_of_new_bars, dtype=np.uint64)
-            }
-
-        # if tags were given
-        if member_tags is not None:
-            # make sure member tags are unique
-            for k, v in member_tags.items():
-                member_tags[k] = np.unique(v)
-                assert np.amin(v) >= 0, \
-                    'member tag index must be greater or equal than zero'
-                assert np.amax(v) < number_of_new_members, \
-                    'member index must be less than number of members'
-            # make sure bars and strings are mutually exclusive
-            assert 'bar' not in member_tags or 'string' not in member_tags or \
-                   np.intersect1d(member_tags['bar'], member_tags['string'], assume_unique=True).size == 0, \
-                'bar and string tags must be mutually exclusive'
-            # update member_tags
-            new_member_tags.update(member_tags)
-
-        # new member properties
-        number_of_members = self.get_number_of_members()
-        # determine tags that have defaults
-        tags_with_defaults = list(set(new_member_tags.keys()) & set(Structure.member_defaults.keys()))
-        # apply defaults
-        new_member_properties = [Structure.MemberProperty(**ChainMap(*[Structure.member_defaults[tag]
-                                                                       for tag in tags_with_defaults
-                                                                       if i in new_member_tags[tag]]))
-                                 for i in range(members.shape[1])]
-
-        # make sure member index is valid
-        number_of_nodes = self.get_number_of_nodes()
-        assert number_of_new_members == 0 or np.amin(members) >= 0, \
-            'member index must be greater or equal than zero'
-        assert number_of_new_members == 0 or np.amax(members) < number_of_nodes, \
-            'member index must be less than number of nodes'
-
-        # add new members
-        self.members = np.hstack((self.members, members))
-        # add member tags
-        for k, v in new_member_tags.items():
-            self.member_tags[k] = np.hstack((self.member_tags[k], number_of_members + v)) \
-                if k in self.member_tags else number_of_members + v
-
-        # add default member properties
-        self.member_properties = pd.concat((self.member_properties,
-                                            Structure.MemberProperty.to_dataframe(new_member_properties)),
-                                           ignore_index=True)
-
-    def remove_members(self, members_to_be_deleted: Optional[npt.ArrayLike] = None,
-                       verbose: bool = False):
-        """
-        Remove members from ``Structure``
-
-        :param members_to_be_deleted: the indices of the members to be deleted
-        :param verbose: if ``True`` warns of the members to be deleted
-        :return:
-        """
-        if members_to_be_deleted:
-            if verbose:
-                warnings.warn('The following members will be removed: '
-                              f'{members_to_be_deleted}')
-            # create new member map
-            member_index = np.delete(np.arange(self.get_number_of_members()), members_to_be_deleted)
-            new_members_map = np.zeros((self.get_number_of_members(),), dtype=np.int_)
-            new_members_map[member_index] = np.arange(self.get_number_of_members() - len(members_to_be_deleted))
-            # remove members
-            self.members = np.delete(self.members, members_to_be_deleted, axis=1)
-            # remove member properties
-            self.member_properties.drop(members_to_be_deleted, inplace=True)
-            self.member_properties.reset_index(inplace=True)
-            # remove members from tags
-            self.member_tags = {k: new_members_map[np.setdiff1d(v, members_to_be_deleted)]
-                                 for k, v in self.member_tags.items()}
-
-    def get_number_of_members(self) -> int:
-        """
-        :return: the number of members in ``Structure``
-        """
-        return self.members.shape[1]
-
-    def get_member_tags(self, index: int) -> List[str]:
-        """
-        A list with the tags for the member with index ``index``
-
-        :param index: the index of the member
-        :return: list of tags
-        """
-        return [k for k, v in self.member_tags.items() if index in v]
-
-    def has_member_tag(self, index: int, tag: str) -> bool:
-        """
-        Return ``True`` if member with index ``index`` has tag ``tag``
-
-        :param index: the index of the member
-        :param tag: the tag
-        :return: ``True`` or ``False``
-        """
-        return tag in self.member_tags and index in self.member_tags[tag]
-
-    def get_members_by_tags(self, tags: Sequence[str]) -> npt.NDArray[np.uint64]:
-        """
-        Return a list of member indices that have tags in the sequence ``tags``
-
-        :param tags: the sequence of tags
-        :return: list of member indices
-        """
-        if len(tags) == 0:
-            return np.zeros((0,))
-        elif len(tags) == 1:
-            return self.member_tags.get(tags[0], np.zeros((0,)))
-        else:
-            return reduce(lambda a1, a2: np.intersect1d(a1, a2, assume_unique=True),
-                          [v for k, v in self.member_tags.items() if k in tags])
-
-    def get_number_of_members_by_tag(self, tag: str) -> int:
-        """
-        Return the number of members with tag ``tag``
-
-        :param tag: the tags
-        :return: the number of members
-        """
-        return len(self.member_tags.get(tag, []))
-
-    def delete_member_tag(self, tag: str) -> None:
-        """
-        Delete member tag ``tag``
-
-        :param tag: the member tag to be deleted
-        """
-        # delete member tag
-        del self.member_tags[tag]
-        if tag in self.member_defaults:
-            del self.member_defaults[tag]
-
-    def set_member_tag(self, tag: str, indices: npt.NDArray[np.uint64]) -> None:
-        """
-        Associate members with indices in ``indices`` to the new tag ``tag``
-
-        :param tag: the member tag
-        :param indices: the member indices
-        """
-        # set new member tag
-
-        # make sure tag is unique
-        assert tag not in self.member_tags, f"member tag '{tag}' already exists"
-
-        # normalize indices
-        v = np.unique(indices)
-
-        # make sure indices are valid
-        number_of_members = self.get_number_of_members()
-        assert np.amin(v) >= 0, \
-            'member tag index must be greater or equal than zero'
-        assert np.amax(v) < number_of_members, \
-            'member tag index must be less than number of members'
-
-        # set tag
-        self.member_tags[tag] = v
-
-    def add_member_tag(self, tag: str, indices: npt.NDArray[np.uint64]) -> None:
-        """
-        Add members with indices in ``indices`` to the existing member tag ``tag``
-
-        :param tag: the member tag
-        :param indices: the member indices
-        """
-
-        # make sure indices are valid
-        number_of_members = self.get_number_of_members()
-        assert np.amin(indices) >= 0, \
-            'member tag index must be greater or equal than zero'
-        assert np.amax(indices) < number_of_members, \
-            'member tag index must be less than number of members'
-
-        # set tag
-        self.member_tags[tag] = np.union1d(self.member_tags[tag], indices)
-
-    def remove_member_tag(self, tag: str, indices: npt.NDArray[np.uint64]) -> None:
-        """
-        Remove members with indices in ``indices`` from the existing member tag ``tag``
-
-        :param tag: the member tag
-        :param indices: the member indices
-        """
-        # remove indices from existing member tag
-
-        # set tag
-        self.member_tags[tag] = np.setdiff1d(self.member_tags[tag], indices)
-
-    def delete_node_tag(self, tag: str) -> None:
-        """
-        Delete node tag ``tag``
-
-        :param tag: the node tag to be deleted
-        """
-        del self.node_tags[tag]
-        if tag in self.node_defaults:
-            del self.node_defaults[tag]
-
-    def set_node_tag(self, tag: str, indices: npt.NDArray[np.uint64]) -> None:
-        """
-        Associate nodes with indices in ``indices`` to the new tag ``tag``
-
-        :param tag: the node tag
-        :param indices: the node indices
-        """
-
-        # make sure tag is unique
-        assert tag not in self.node_tags, f"node tag '{tag}' already exists"
-
-        # normalize indices
-        v = np.unique(indices)
-
-        # make sure indices are valid
-        assert np.amin(v) >= 0, \
-            'node tag index must be greater or equal than zero'
-        assert np.amax(v) < self.get_number_of_nodes(), \
-            'node tag index must be less than number of nodes'
-
-        # set tag
-        self.node_tags[tag] = v
-
-    def add_node_tag(self, tag: str, indices: npt.NDArray[np.uint64]) -> None:
-        """
-        Add nodes with indices in ``indices`` to the existing node tag ``tag``
-
-        :param tag: the node tag
-        :param indices: the node indices
-        """
-
-        # make sure indices are valid
-        assert np.amin(indices) >= 0, \
-            'node tag index must be greater or equal than zero'
-        assert np.amax(indices) < self.get_number_of_nodes(), \
-            'node tag index must be less than number of nodes'
-
-        # set tag
-        self.node_tags[tag] = np.union1d(self.node_tags[tag], indices)
-
-    def remove_node_tag(self, tag: str, indices: npt.NDArray[np.uint64]) -> None:
-        """
-        Remove nodes with indices in ``indices`` from the existing node tag ``tag``
-
-        :param tag: the node tag
-        :param indices: the node indices
-        """
-
-        # set tag
-        self.node_tags[tag] = np.setdiff1d(self.node_tags[tag], indices)
-
-    @staticmethod
-    def _set_dataframe(df: pd.DataFrame, index: Union[int, Sequence[int], slice], labels: Union[str, Sequence[str]],
-                       values: Any, wrap: bool = False, scalar: bool = True) -> None:
-        """
-        Auxiliary set method to wrap values when setting dataframe
-
-        :param df: the dataframe
-        :param index: the row index
-        :param labels: the column label(s)
-        :param values: the values to set to
-        :param wrap: if ``True``, wraps ``value`` in a ``Series`` or ``Dataframe`` before assignment
-        :param scalar: if ``True``, ``value`` is set to an array of len(index)
-
-        **Notes:**
-
-        1. This method is for convenience when assigning objects to dataframes.
-           See `this question <https://stackoverflow.com/questions/48000225/must-have-equal-len-keys-and-value-when-setting-with-an-iterable>`_
-           for details.
-        """
-        if wrap:
-            if isinstance(index, int):
-                idx = index = [index]
-                m = 1
-            else:
-                idx = df.index[index]
-                m = len(idx)
-            if scalar:
-                values = [values] * m
-            if isinstance(labels, str):
-                values = pd.Series(values, index=idx)
-            else:
-                values = pd.DataFrame(values, index=idx)
-        df.loc[index, labels] = values
-
-    def set_member_properties(self, index: Union[int, Sequence[int], slice], labels: Union[str, Sequence[str]],
-                              values: Any, wrap: bool = False, scalar: bool = True) -> None:
-        """
-        Set member properties
-
-        See :meth:`tnsgrt.structure.Structure._set_dataframe`
-
-        :param index: the element index
-        :param labels: the property label(s)
-        :param values: the values to set to
-        :param wrap: if ``True``, wraps ``value`` in a ``Series`` or ``Dataframe`` before assignment
-        :param scalar: if ``True``, ``value`` is set to an array of len(index)
-        """
-        Structure._set_dataframe(self.member_properties, index, labels, values, wrap, scalar)
-
-    def get_member_properties(self, index: Union[int, Sequence[int], slice], labels: Union[str, List[str]])\
-            -> pd.DataFrame:
-        """
-        Retrieve member properties
-
-        :param index: the member index
-        :param labels: the member property labels
-        :return: datafrome with the selected properties
-        """
-        return self.member_properties.loc[index, labels]
-
-    def set_node_properties(self, index: Union[int, Sequence[int], slice], labels: Union[str, Sequence[str]],
-                            values: Any, wrap: bool = False, scalar: bool = True) -> None:
-        """
-        Set node properties
-
-        See :meth:`tnsgrt.structure.Structure._set_dataframe`
-
-        :param index: the element index
-        :param labels: the property label(s)
-        :param values: the values to set to
-        :param wrap: if ``True``, wraps ``value`` in a ``Series`` or ``Dataframe`` before assignment
-        :param scalar: if ``True``, ``value`` is set to an array of len(index)
-        """
-        Structure._set_dataframe(self.node_properties, index, labels, values, wrap, scalar)
-
-    def get_node_properties(self, index: Union[int, Sequence[int], slice], labels: Union[str, List[str]])\
-            -> pd.DataFrame:
-        """
-        Retrieve node properties
-
-        :param index: the node index
-        :param labels: the node property labels
-        :return: datafrome with the selected properties
-        """
-        return self.node_properties.loc[index, labels]
-
-    def get_member_vectors(self) -> npt.NDArray[np.float_]:
-        """
-        :return: a 3 x m array with the ``Structure``'s members
-        """
-        return self.nodes[:, self.members[1, :]] - self.nodes[:, self.members[0, :]]
-
-    def get_member_length(self) -> npt.NDArray[np.float_]:
-        """
-        :return: an array with the ``Structure``'s member lengths
-        """
-        return np.linalg.norm(self.nodes[:, self.members[1, :]] - self.nodes[:, self.members[0, :]], axis=0)
-
-    def get_center_of_mass(self) -> npt.NDArray[np.float_]:
-        """
-        :return: the ``Structure``'s center of mass
-        """
-        # Computes the center of mass
-        mass = self.member_properties['mass'].values
-        return np.sum(mass * (self.nodes[:, self.members[0, :]] + self.nodes[:, self.members[1, :]])/2, axis=1) \
-            / np.sum(mass)
-
-    def get_centroid(self) -> npt.NDArray[np.float_]:
-        """
-        :return: the ``Structure``'s geometric center or centroid
-        """
-        # Computes the centroid (geometric center)
-        return np.sum(self.nodes, axis=1) / self.get_number_of_nodes()
-
-    def update_member_properties(self, property_name: Optional[Union[str, Iterable[str]]] = None) -> None:
-        """
-        Update ``Structure``'s member properties
-
-        If property_name is
-
-        - 'stiffness': calculate ``stiffness`` and ``rest_length`` based on ``modulus``, ``radius``, ``inner_radius``
-           and ``lambda_``
-        - 'mass': calculate ``mass`` and ``volume`` based on ``radius`` and ``density``
-        - 'force': calculate ``force`` based on ``lambda_``
-
-        :param property_name: the property name to update; if ``None``, update all properties
-        """
-
-        if isinstance(property_name, str):
-
-            # update stiffness and rest length
-            if property_name == 'stiffness':
-                member_length = self.get_member_length()
-                modulus_times_area = self.member_properties['modulus'].values * np.pi * \
-                    (self.member_properties['radius'].values ** 2 - self.member_properties['inner_radius'].values ** 2)
-                stiffness = modulus_times_area / member_length
-                if np.any(stiffness < 0):
-                    raise Exception(f'Structure::update_member_property: negative stiffness computed')
-                rest_length = member_length * (1 - self.member_properties['lambda_'].values / stiffness)
-                if np.any(rest_length < 0):
-                    raise Exception(f'Structure::update_member_property: negative rest_length computed')
-                self.member_properties['stiffness'] = stiffness
-                self.member_properties['rest_length'] = rest_length
-
-            # update mass and volume
-            elif property_name == 'mass':
-                member_length = self.get_member_length()
-                volume = np.pi * (self.member_properties['radius'] ** 2 -
-                                  self.member_properties['inner_radius'].values ** 2) * member_length
-                if np.any(volume < 0):
-                    raise Exception(f'Structure::update_member_property: negative volume computed')
-                mass = volume * self.member_properties['density']
-                if np.any(mass < 0):
-                    raise Exception(f'Structure::update_member_property: negative mass computed')
-                self.member_properties['volume'] = volume
-                self.member_properties['mass'] = mass
-
-            # update force
-            elif property_name == 'force':
-                self.member_properties['force'] = self.get_member_length() * self.member_properties['lambda_'].values
-
-            else:
-                raise Exception('Structure::update_member_property: '
-                                f'do not know how to update property {property_name}')
-
-        else:
-
-            # iterate all if None
-            if property_name is None:
-                property_name = ['mass', 'stiffness', 'force']
-
-            # iterate properties
-            for prop in property_name:
-                self.update_member_properties(prop)
-
-    def get_close_nodes(self, radius=1e-6) -> Tuple[Set[int], npt.NDArray]:
-        """
-        Returns the set of nodes that lie within ``radius`` distance to other nodes in ``Structure`` and the
-        corresponding map
-
-        For example, if::
-
-            close_nodes, close_nodes_map = s.get_close_nodes()
-
-        is such that::
-
-            close_nodes = {1, 3}
-            close_nodes_map = [0,0,2,2,4]
-
-        then node ``1`` is close to node ``0`` and node ``3`` is close to node ``2``.
-
-        :param radius: the proximity radius
-        :return: tuple with ``close_nodes`` and ``close_nodes_map``
-        """
-
-        tree = scipy.spatial.KDTree(self.nodes.transpose())
-        indices = tree.query_ball_tree(tree, r=radius)
-        close_nodes_map = np.arange(self.get_number_of_nodes())
-        close_nodes_set = set()
-        for i, neighbors in enumerate(indices):
-            for k in [j for j in neighbors if j > i]:
-                close_nodes_map[k] = i
-                close_nodes_set.add(k)
-        if close_nodes_set:
-            # apply map until no changes
-            while True:
-                last_merge_map = close_nodes_map.copy()
-                close_nodes_map = close_nodes_map[close_nodes_map]
-                if np.all(last_merge_map == close_nodes_map):
-                    break
-        return close_nodes_set, close_nodes_map
-
-    def merge_close_nodes(self, radius: float = 1e-6, verbose: bool = False) -> None:
-        """
-        Merge then remove all nodes in ``Structure`` which lie within ``radius``
-
-        :param radius: the proximity radius
-        :param verbose: if ``True`` issues a warning with number of nodes removed after the merge
-        """
-        # get close nodes
-        close_nodes_set, close_nodes_map = self.get_close_nodes(radius)
-        if close_nodes_set:
-            # list of nodes to be removed
-            nodes_to_be_removed = list(close_nodes_set)
-            # apply merge_map to members
-            self.members = close_nodes_map[self.members]
-            # remove nodes, to make sure the member node numbering is correct
-            self.remove_nodes(nodes_to_be_removed, verify_if_unused=False, verbose=verbose)
-
-    def merge(self, s: 'Structure', inplace=False) -> Optional['Structure']:
-        """
-        Return a new ``Structure`` in which the current `Structure`` and ``s`` are merged
-
-        :param s: the ``Structure`` to merge
-        :param inplace: if ``True`` merge is done in place without creating a copy
-        :return: the merged ``Structure``
-        """
-
-        if inplace:
-            target = self
-        else:
-            target = self.copy()
-
-        # offset members in s by number_of_members
-        number_of_members = self.get_number_of_members()
-        number_of_nodes = self.get_number_of_nodes()
-
-        # merge nodes
-        target.nodes = np.hstack((self.nodes, s.nodes))
-
-        # merge node tags
-        for k, v in s.node_tags.items():
-            # append or add
-            target.node_tags[k] = np.hstack((self.node_tags[k], number_of_nodes + v)) \
-                if k in self.node_tags \
-                else number_of_nodes + v
-
-        # merge node properties
-        target.node_properties = pd.concat((self.node_properties, s.node_properties), ignore_index=True)
-
-        # merge members, offset by number of nodes
-        target.members = np.hstack((self.members, number_of_nodes + s.members))
-
-        # merge member tags
-        for k, v in s.member_tags.items():
-            # append or add
-            target.member_tags[k] = np.hstack((self.member_tags[k], number_of_members + v)) \
-                if k in self.member_tags \
-                else number_of_members + v
-
-        # merge member properties
-        target.member_properties = pd.concat((self.member_properties, s.member_properties), ignore_index=True)
-
-        return target
-
-    def equilibrium(self, force: Optional[npt.ArrayLike] = None, lambda_bar: float = 1,
-                    equalities: Optional[list[npt.ArrayLike]] = None,
-                    epsilon: float = 1e-7) -> None:
-        """
-        Solves for the set of internal forces that ensures the equilibrium of the current ``Structure`` in response
-        to the vector of external forces ``forces``
-
-        Solve the force equilibrium equation
-
-        .. math::
-           A \\lambda = f
-
-        in which:
-
-        - :math:`A`: is a matrix representing the element vectors
-        - :math:`f`: is the vector of external forces
-        - :math:`\\lambda`: is the vector of resulting force coefficients
-
-        If the :math:`i` th element is a string then
-
-        .. math::
-            x_i \\geq 0
-
-        If no external force is given then the sum of the bar force coefficients equals ``lambda_bar``
-
-        All elements in the equalities are set equal. For example, if::
-
-            equalities = [[0, 1, 3], [2, 4]]
-
-        then the equilibrium is shought satisfying the constraints
-
-        .. math::
-            x_0 = x_1 = x_3, \\qquad x_2 = x_4
-
-        :param force: a 3 x n array of external forces; or zero if `None`
-        :param lambda_bar: the normalizing factor
-        :param equalities: a list of lists of member indices which are constrained to have the same force coefficient
-        :param epsilon: numerical accuracy
-        """
-
-        number_of_nodes = self.get_number_of_nodes()
-        number_of_strings = len(self.member_tags.get('string', []))
-        number_of_bars = len(self.member_tags.get('bar', []))
-        number_of_members = number_of_strings + number_of_bars
-
-        assert number_of_members == number_of_bars + number_of_strings, \
-            'number of members is not equal to the sum of number of bars and strings'
-
-        # member vectors
-        member_vectors = self.get_member_vectors()
-
-        # coefficient matrix
-        Aeq = np.zeros((3 * number_of_nodes, number_of_members))
-
-        # string coefficient
-        if number_of_strings:
-            for i in self.member_tags['string']:
-
-                ii = 3 * int(self.members[0, i])
-                Aeq[ii:ii+3, i] = -member_vectors[:, i]
-
-                jj = 3 * int(self.members[1, i])
-                Aeq[jj:jj+3, i] = member_vectors[:, i]
-
-        # bar coefficient
-        if number_of_bars:
-            for i in self.member_tags['bar']:
-
-                ii = 3 * int(self.members[0, i])
-                Aeq[ii:ii+3, i] = member_vectors[:, i]
-
-                jj = 3 * int(self.members[1, i])
-                Aeq[jj:jj+3, i] = -member_vectors[:, i]
-
-        A = Aeq
-        m = 3 * number_of_nodes
-
-        # external forces
-        if force is None:
-            A = np.vstack((A, np.ones((1, number_of_members))))
-            blo = bup = np.hstack((np.zeros((3 * number_of_nodes,)), 1))
-        else:
-            beq = np.array(force)
-            assert np.all(beq.shape == (3, number_of_nodes)), 'force must be a 3 x n matrix'
-            blo = bup = beq.flatten(order='F')
-
-        # For equilibrium: Aeq x = beq
-
-        # impose equalities
-        # indices in each row are set to be equal
-        if equalities is not None:
-            number_of_constraints = sum(map(len, equalities)) - len(equalities)
-            Aeq = np.zeros((number_of_constraints, number_of_members))
-            beq = np.zeros((number_of_constraints, ))
-            ii = 0
-            for eqs in equalities:
-                nn = len(eqs)
-                for jj in range(1, nn):
-                    Aeq[ii+jj-1, eqs[0]] = 1
-                    Aeq[ii+jj-1, eqs[jj]] = -1
-                ii += nn
-            A = np.vstack((A, Aeq))
-            blo = bup = np.hstack((blo, beq))
-
-        # enforce strings have positive force coefficients
-        # when there are no external forces set to one to avoid nontrivial solution
-        xup = None
-        if number_of_strings:
-            xlo = np.full((number_of_members, ), 0)
-            xlo[self.member_tags['string']] = 0
-        else:
-            xlo = None
-
-        # cost function
-        c = np.ones((number_of_members,))
-
-        # solve lp
-        cost, gamma, status = optim.lp(number_of_members, m, c, A, blo, bup, xlo, xup)
-
-        # if infeasible, throw error
-        if status == 'infeasible':
-            raise Exception('could not find equilibrium')
-
-        # flip sign for bars
-        lambda_ = gamma
-        if number_of_bars:
-            lambda_[self.member_tags['bar']] *= -1
-
-            if force is None:
-                # scale solution for bars
-                scale = -np.sum(lambda_[self.member_tags['bar']]) / number_of_bars
-                lambda_ *= np.abs(lambda_bar) / scale
-
-        # assign lambda
-        self.member_properties['lambda_'] = lambda_
-
-        # update force
-        self.update_member_properties('force')
-
-    def stiffness(self, epsilon: float = 1e-6, storage: str = 'sparse',
-                  apply_rigid_body_constraint: bool = False,
-                  apply_planar_constraint: bool = False):
-        """
-        Computes
-
-        - `normal`: potential energy (1 x 1)
-        - `F`: force vectors (3 x n)
-        - `K`: stiffness matrix (3 n x 3 n)
-        - `M`: mass matrix (n x 1)
-
-        for the current ``Structure``. The mass and stiffness matrices are returned in the form of an object of the
-        class :class:`tnsgrt.stiffness.Stiffness`
-
-        :param epsilon: numerical accuracy
-        :param storage: if ``sparse`` stores the resulting stiffeness and mass matrices in sparse csr format
-        :param apply_rigid_body_constraint: if ``True`` apply 3D rigid body constraints
-        :param apply_planar_constraint: if ``True`` apply 2D constraints
-        :return: tuple (`S`, `F`, `normal`)
-        """
-
-        number_of_nodes = self.get_number_of_nodes()
-        number_of_strings = len(self.member_tags.get('string', []))
-        number_of_bars = len(self.member_tags.get('bar', []))
-        number_of_members = number_of_strings + number_of_bars
-
-        assert number_of_members == number_of_bars + number_of_strings, \
-            'number of members is not equal to the sum of number of bars and strings'
-
-        if number_of_nodes <= 12 and storage == 'sparse':
-            storage = 'dense'
-            warnings.warn("number of nodes is small; storage set to 'dense'")
-
-        # member vectors
-        member_vectors = self.get_member_vectors()
-        member_length = self.get_member_length()
-
-        k = self.member_properties['stiffness'].values
-        lambda_ = self.member_properties['lambda_'].values
-        mass = self.member_properties['mass'].values
-
-        # compute potential
-        v = np.sum(((lambda_ * member_length) ** 2) / k / 2)
-
-        # Compute force and stiffness
-
-        # preallocate F
-        F = np.zeros((3, number_of_nodes))
-        # preallocate K
-        if storage == 'sparse':
-            # sparse storage
-            diag = np.unique(self.members)
-            diff = np.unique(self.members, axis=1)
-            row_col = np.hstack((np.vstack((diag, diag)), diff, np.flipud(diff)))
-            data = np.zeros((row_col.shape[1]))
-            K = scipy.sparse.kron(scipy.sparse.coo_matrix((data, row_col),
-                                                          shape=(number_of_nodes, number_of_nodes)),
-                                  np.ones((3, 3))).tocsr()
-        else:
-            # dense storage
-            K = np.zeros((3 * number_of_nodes, 3 * number_of_nodes))
-
-        lambda_ * member_vectors
-        # calculate stiffness and force
-        for i in range(number_of_members):
-
-            mij = member_vectors[:, i] / member_length[i]
-            fij = lambda_[i] * member_vectors[:, i]
-
-            mijmij = np.outer(mij, mij)
-            # kij = k[index] * Mij + lambda_[index] * (np.eye(3) - Mij)
-            kij = (k[i] - lambda_[i]) * mijmij + lambda_[i] * np.eye(3)
-
-            i, j = self.members[:, i].astype(dtype=np.int_)
-
-            F[:, i] += fij
-            F[:, j] -= fij
-
-            ii = 3 * i
-            jj = 3 * j
-
-            K[ii:ii+3, ii:ii+3] += kij
-            K[jj:jj+3, jj:jj+3] += kij
-            K[ii:ii+3, jj:jj+3] -= kij
-            K[jj:jj+3, ii:ii+3] -= kij
-
-        # Compute mass
-        M = np.zeros((number_of_nodes,))
-        M[self.members[0, :]] = mass / 2
-        M[self.members[1, :]] += mass / 2
-
-        diag = np.kron(M, np.ones((3,)))
-        if storage == 'sparse':
-            # sparse storage
-            M = scipy.sparse.diags(diag, format='csr')
-        else:
-            # dense storage
-            M = np.diag(np.kron(M, np.ones((3,))))
-
-        # Check forces
-        sum_of_forces = np.linalg.norm(F, ord='fro')
-        if sum_of_forces > epsilon:
-            warnings.warn(f'Structure::stiffness: force balance not satisfied, sum of forces = {sum_of_forces}')
-
-        # Build stiffness object
-        stiffness = Stiffness(K, M)
-
-        # node constraints
-        constraints = self.node_properties['constraint']
-        has_constraints = constraints.isna().sum() < self.get_number_of_nodes()
-        if has_constraints:
-            # apply node constraints
-            stiffness.apply_constraint(*NodeConstraint.node_constraint(self.nodes, constraints))
-        if apply_rigid_body_constraint:
-            # apply rigid body constraints
-            stiffness.apply_constraint(*NodeConstraint.rigid_body_constraint(self.nodes), local=False)
-        if apply_planar_constraint:
-            # apply planar constraints
-            stiffness.apply_constraint(*NodeConstraint.planar_constraint(self.nodes), local=False)
-
-        return stiffness, F, v
+import warnings
+from dataclasses import dataclass
+from functools import reduce
+from typing import Optional, Dict, get_type_hints, Union, List, Sequence, Type, Iterable, Tuple, Set, Any
+from collections import ChainMap
+
+import numpy as np
+import numpy.typing as npt
+import pandas as pd
+import scipy
+
+from . import utils
+from . import optim
+from .stiffness import Stiffness, NodeConstraint
+
+
+class Property:
+    """
+    Base class for storing properties
+
+    Derived classes should implement ``dataclass`` from ``dataclasses``
+    """
+
+    @classmethod
+    def to_dataframe(cls: Type['Property'], data: Union[list, tuple] = tuple()) -> pd.DataFrame:
+        # setup member property as pandas dataframe
+        hints = get_type_hints(cls)
+        return pd.DataFrame(data=data, columns=list(hints.keys())).astype(dtype=hints)
+
+
+class Structure:
+    """
+    A ``Structure`` object
+
+    :param nodes: a 3 x n array representing the ``Structure``'s nodes
+    :param members: a 3 x m array representing the ``Structure``'s members
+    :param number_of_strings: the number of strings in ``Structure``
+    :param node_tags: a dictionary with the node tags
+    :param member_tags: a dictionary with the member tags
+    :param label: the ``Structure``'s label
+    """
+
+    @dataclass
+    class NodeProperty(Property):
+        """
+        Subclass representing properties of nodes
+        """
+        radius: float = 0.002
+        visible: bool = True
+        constraint: object = None
+        facecolor: object = utils.Colors.BLUE.value
+        edgecolor: object = utils.Colors.BLUE.value
+
+    node_defaults = {
+    }
+
+    @dataclass
+    class MemberProperty(Property):
+        """
+        Subclass representing properties of members
+        """
+        lambda_: float = 0.
+        force: float = 0.
+        stiffness: float = 0.
+        volume: float = 0.
+        radius: float = 0.01
+        inner_radius: float = 0
+        mass: float = 1.
+        rest_length: float = 0.
+        # ASTM A36 steel
+        yld: float = 250e6
+        density: float = 7.85e3
+        modulus: float = 200e9
+        visible: bool = True
+        facecolor: object = (1, 0, 0)
+        edgecolor: object = (1, 0, 0)
+        linewidth: int = 2
+        linestyle: str = '-'
+
+    member_defaults = {
+        'bar': {
+            'facecolor': utils.Colors.BLUE.value,
+            'edgecolor': utils.Colors.BLUE.value
+        },
+        'string': {
+            'facecolor': utils.Colors.ORANGE.value,
+            'edgecolor': utils.Colors.ORANGE.value,
+            'radius': 0.005
+        }
+    }
+
+    def __init__(self,
+                 nodes: npt.ArrayLike = np.zeros((3, 0), np.float_),
+                 members: npt.ArrayLike = np.zeros((2, 0), np.int64),
+                 number_of_strings: int = 0,
+                 node_tags: Optional[Dict[str, npt.NDArray[np.uint64]]] = None,
+                 member_tags: Optional[Dict[str, npt.NDArray[np.uint64]]] = None,
+                 label: str = None):
+        # label
+        self.label: Optional[str] = label
+        # nodes
+        self.nodes: npt.NDArray[np.float_] = np.zeros((3, 0), np.float_)
+        self.node_tags: Dict[str, npt.NDArray[np.uint64]] = {}
+        self.node_properties: pd.DataFrame = Structure.NodeProperty.to_dataframe()
+        # members
+        self.members: npt.NDArray[np.uint64] = np.zeros((2, 0), np.uint64)
+        self.member_tags: Dict[str, npt.NDArray[np.uint64]] = {
+            'bar': np.zeros((0,), np.uint64),
+            'string': np.zeros((0,), np.uint64)
+        }
+        self.member_properties: pd.DataFrame = Structure.MemberProperty.to_dataframe()
+
+        # add nodes
+        self.add_nodes(nodes, node_tags)
+
+        # add members
+        self.add_members(members, number_of_strings, member_tags)
+
+    def __repr__(self) -> str:
+        """
+        :return: short description of structure as a string
+        """
+        return "Structure " + (f" labeled '{self.label}'" if self.label else '') + \
+            f"with {self.get_number_of_members_by_tag('bar')} bars " \
+            f"and {self.get_number_of_members_by_tag('string')} strings"
+
+    def copy(self) -> 'Structure':
+        """
+        :return: copy of the Structure
+        """
+
+        # instantiate copy of the current structure
+        copy = self.__class__()
+
+        # copy basic structure
+        copy.label = self.label
+        copy.nodes = self.nodes.copy()
+        copy.node_tags = self.node_tags.copy()
+        copy.node_properties = self.node_properties.copy()
+        copy.members = self.members.copy()
+        copy.member_tags = self.member_tags.copy()
+        copy.member_properties = self.member_properties.copy()
+
+        return copy
+
+    def set_nodes(self, nodes: npt.ArrayLike) -> None:
+        """
+        Set nodes of the ``Structure``
+
+        :param nodes: the nodes
+        """
+        # convert to array
+        nodes = np.array(nodes, np.float_)
+
+        # test dimensions
+        assert np.all(nodes.shape == self.nodes.shape), 'nodes shape must match current shape'
+
+        # set nodes
+        self.nodes: npt.NDArray[np.float_] = nodes
+
+    def add_nodes(self, nodes: npt.ArrayLike,
+                  node_tags: Optional[Dict[str, npt.NDArray[np.uint64]]] = None) -> None:
+        """
+        Add nodes to the ``Structure``
+
+        :param nodes: the nodes to add
+        :param node_tags: the node tags to add
+        """
+        # add nodes and tags to current structure
+
+        # convert to array
+        nodes = np.array(nodes, np.float_)
+
+        # test dimensions
+        assert nodes.shape[0] == 3, 'nodes must be a 3 x n array'
+
+        # node tags
+        number_of_new_nodes = nodes.shape[1]
+        if node_tags is None:
+            node_tags = {}
+        else:
+            # make sure node tags are unique
+            for k, v in node_tags.items():
+                node_tags[k] = np.unique(v)
+                assert np.amin(v) >= 0, \
+                    'node tag index must be greater or equal than zero'
+                assert np.amax(v) < number_of_new_nodes, \
+                    'node tag index must be less than number of new nodes'
+
+        # new node properties
+        number_of_nodes = self.get_number_of_nodes()
+        # determine tags that have defaults
+        tags_with_defaults = list(set(node_tags.keys()) & set(Structure.node_defaults.keys()))
+        # apply defaults
+        new_node_properties = [Structure.NodeProperty(**ChainMap(*[Structure.node_defaults[tag]
+                                                                   for tag in tags_with_defaults
+                                                                   if i in node_tags[tag]]))
+                               for i in range(nodes.shape[1])]
+
+        # add new nodes
+        self.nodes: npt.NDArray[np.float_] = np.hstack((self.nodes, nodes))
+
+        # add node tags
+        for k, v in node_tags.items():
+            self.node_tags[k] = np.hstack((self.node_tags[k], number_of_nodes + v)) \
+                if k in self.node_tags else number_of_nodes + v
+
+        # add default node properties
+        self.node_properties = pd.concat((self.node_properties,
+                                          Structure.NodeProperty.to_dataframe(new_node_properties)),
+                                         ignore_index=True)
+
+    def get_number_of_nodes(self) -> int:
+        """
+        :return: the number of nodes in ``Structure``
+        """
+        return self.nodes.shape[1]
+
+    def translate(self, v: npt.NDArray) -> 'Structure':
+        """
+        Translate all nodes of the ``Structure`` by the 3D vector ``normal``
+
+        :param v: the 3D translation vector
+        :return: self
+        """
+        # `translate(normal)` translates nodes of the structure by the 3D vector `normal`
+        assert v.shape == (3,), 'normal must be a three dimensional vector'
+        self.nodes += v.reshape((3, 1))
+        return self
+
+    def rotate(self, v: npt.NDArray) -> 'Structure':
+        """
+        Rotate all nodes of the ``Structure`` by the 3D vector ``normal``
+
+        :param v: the 3D rotation vector
+        :return: self
+        """
+        # `rotate(normal)` rotates the nodes of the structure around the 3D vector `normal`
+        # the magnitude of the vector equals the rotation angle in radians
+        assert v.shape == (3,), 'normal must be a three dimensional vector'
+        rotation = scipy.spatial.transform.Rotation.from_rotvec(v)
+        self.nodes = rotation.apply(self.nodes.transpose()).transpose()
+        return self
+
+    def reflect(self, v: npt.NDArray, p: Optional[npt.NDArray] = None) -> 'Structure':
+        """
+        Reflects the structure about a plane normal to the vector `normal`, passing through the point `p`.
+        If no point is given, it defaults to the origin.
+
+        :param v: the 3D normal vector
+        :param p: the 3D origin vector
+        :return: self
+        """
+        assert v.shape == (3,), 'normal must be a three dimensional vector'
+
+        if p is not None:
+            assert p.shape == (3,), 'p must be a three dimensional vector'
+            # translate by p
+            self.nodes -= p.reshape((3, 1))
+
+        # normalize normal
+        length = np.linalg.norm(v)
+        if length < 1e-6:
+            warnings.warn('norm of vector normal is too small, reflection not performed')
+            return self
+
+        # calculate reflection matrix
+        reflection_matrix = np.eye(3) - (2 / length**2) * np.outer(v, v)
+
+        # transform nodes
+        self.nodes = reflection_matrix @ self.nodes
+
+        if p is not None:
+            # translate back to p
+            self.nodes += p.reshape((3, 1))
+
+        return self
+
+    def get_unused_nodes(self) -> npt.NDArray[np.uint64]:
+        """
+        :return: an array with the indices of the unused nodes
+        """
+        # calculate nodes that are in use
+        used_nodes = np.unique(self.members)
+        # return unused nodes
+        return np.setdiff1d(np.arange(self.get_number_of_nodes()), used_nodes, assume_unique=True)
+
+    def has_unused_nodes(self) -> bool:
+        """
+        :return: ``True`` if there are no unused nodes
+        """
+        return len(self.get_unused_nodes()) > 0
+
+    def remove_nodes(self, nodes_to_be_deleted: Optional[npt.ArrayLike] = None,
+                     verify_if_unused: bool = True, verbose: bool = False) -> None:
+        """
+        Remove nodes from structure
+
+        :param nodes_to_be_deleted: the indices of the nodes to be deleted; if ``None``,
+                                    delete all currently unused nodes
+        :param verify_if_unused: if ``True`` verifies if the nodes to be deleted are not in use
+        :param verbose: if ``True`` warns of the nodes to be deleted
+        """
+        if nodes_to_be_deleted is None:
+            # delete all unused nodes
+            unused_nodes_to_be_deleted = self.get_unused_nodes()
+        elif verify_if_unused:
+            # sort nodes to be deleted
+            nodes_to_be_deleted = np.unique(nodes_to_be_deleted)
+            # calculate nodes that are in use
+            used_nodes = np.unique(self.members)
+            # find unused nodes
+            unused_nodes_to_be_deleted = np.setdiff1d(nodes_to_be_deleted, used_nodes, assume_unique=True)
+            # warn if different
+            number_of_used_nodes = len(nodes_to_be_deleted) - len(unused_nodes_to_be_deleted)
+            if number_of_used_nodes:
+                warnings.warn(f'{number_of_used_nodes} nodes are still in use and were not deleted')
+                if verbose:
+                    warnings.warn('The following nodes will not be removed: ' 
+                                  f'{np.intersect1d(nodes_to_be_deleted, used_nodes, assume_unique=True)}')
+        else:
+            # go ahead without verifying if nodes are unused
+            # WARNING: this may result in orphan members!
+            unused_nodes_to_be_deleted = nodes_to_be_deleted
+        # delete if there are any unused nodes
+        if len(unused_nodes_to_be_deleted):
+            if verbose:
+                warnings.warn('The following nodes will be removed: '
+                              f'{unused_nodes_to_be_deleted}')
+            # create new node map
+            node_index = np.delete(np.arange(self.get_number_of_nodes()), unused_nodes_to_be_deleted)
+            new_node_map = np.zeros((self.get_number_of_nodes(),), dtype=np.int_)
+            new_node_map[node_index] = np.arange(self.get_number_of_nodes() - len(unused_nodes_to_be_deleted))
+            # remove nodes
+            self.nodes = np.delete(self.nodes, unused_nodes_to_be_deleted, axis=1)
+            # remove node properties
+            self.node_properties.drop(unused_nodes_to_be_deleted, inplace=True)
+            self.node_properties.reset_index(inplace=True)
+            # remove nodes from tags
+            self.node_tags = {k: new_node_map[np.setdiff1d(v, unused_nodes_to_be_deleted)]
+                              for k, v in self.node_tags.items()}
+            # apply new node map to members
+            self.members = new_node_map[self.members]
+
+    def add_members(self, members: npt.ArrayLike,
+                    number_of_strings: Optional[int] = None,
+                    member_tags: Optional[Dict[str, npt.NDArray[np.uint64]]] = None) -> None:
+        """
+        Add members and tags to current structure
+
+        :param members: the members to be added
+        :param number_of_strings: the number of strings; if not ``None``,  then the first `number_of_strings` members
+                                  are tagged as 'strings' and the remaining members as 'bars'
+        :param  member_tags: the new members' tags
+        """
+
+        # convert to array
+        members = np.array(members, np.uint64)
+
+        # test dimensions
+        assert members.shape[0] == 2, 'members must be a 2 x m array'
+
+        # member tags
+        if number_of_strings is None and member_tags is None:
+            raise Exception('Either type or number of strings must be provided')
+
+        number_of_new_members = members.shape[1]
+        new_member_tags = {}
+        if number_of_strings is not None:
+            # number of strings given
+            assert number_of_strings <= number_of_new_members, \
+                'number of added strings must be less than number of added members'
+            number_of_new_bars = number_of_new_members - number_of_strings
+            new_member_tags = {
+                'string': np.arange(0, number_of_strings, dtype=np.uint64),
+                'bar': number_of_strings + np.arange(0, number_of_new_bars, dtype=np.uint64)
+            }
+
+        # if tags were given
+        if member_tags is not None:
+            # make sure member tags are unique
+            for k, v in member_tags.items():
+                member_tags[k] = np.unique(v)
+                assert np.amin(v) >= 0, \
+                    'member tag index must be greater or equal than zero'
+                assert np.amax(v) < number_of_new_members, \
+                    'member index must be less than number of members'
+            # make sure bars and strings are mutually exclusive
+            assert 'bar' not in member_tags or 'string' not in member_tags or \
+                   np.intersect1d(member_tags['bar'], member_tags['string'], assume_unique=True).size == 0, \
+                'bar and string tags must be mutually exclusive'
+            # update member_tags
+            new_member_tags.update(member_tags)
+
+        # new member properties
+        number_of_members = self.get_number_of_members()
+        # determine tags that have defaults
+        tags_with_defaults = list(set(new_member_tags.keys()) & set(Structure.member_defaults.keys()))
+        # apply defaults
+        new_member_properties = [Structure.MemberProperty(**ChainMap(*[Structure.member_defaults[tag]
+                                                                       for tag in tags_with_defaults
+                                                                       if i in new_member_tags[tag]]))
+                                 for i in range(members.shape[1])]
+
+        # make sure member index is valid
+        number_of_nodes = self.get_number_of_nodes()
+        assert number_of_new_members == 0 or np.amin(members) >= 0, \
+            'member index must be greater or equal than zero'
+        assert number_of_new_members == 0 or np.amax(members) < number_of_nodes, \
+            'member index must be less than number of nodes'
+
+        # add new members
+        self.members = np.hstack((self.members, members))
+        # add member tags
+        for k, v in new_member_tags.items():
+            self.member_tags[k] = np.hstack((self.member_tags[k], number_of_members + v)) \
+                if k in self.member_tags else number_of_members + v
+
+        # add default member properties
+        self.member_properties = pd.concat((self.member_properties,
+                                            Structure.MemberProperty.to_dataframe(new_member_properties)),
+                                           ignore_index=True)
+
+    def remove_members(self, members_to_be_deleted: Optional[npt.ArrayLike] = None,
+                       verbose: bool = False):
+        """
+        Remove members from ``Structure``
+
+        :param members_to_be_deleted: the indices of the members to be deleted
+        :param verbose: if ``True`` warns of the members to be deleted
+        :return:
+        """
+        if members_to_be_deleted:
+            if verbose:
+                warnings.warn('The following members will be removed: '
+                              f'{members_to_be_deleted}')
+            # create new member map
+            member_index = np.delete(np.arange(self.get_number_of_members()), members_to_be_deleted)
+            new_members_map = np.zeros((self.get_number_of_members(),), dtype=np.int_)
+            new_members_map[member_index] = np.arange(self.get_number_of_members() - len(members_to_be_deleted))
+            # remove members
+            self.members = np.delete(self.members, members_to_be_deleted, axis=1)
+            # remove member properties
+            self.member_properties.drop(members_to_be_deleted, inplace=True)
+            self.member_properties.reset_index(inplace=True)
+            # remove members from tags
+            self.member_tags = {k: new_members_map[np.setdiff1d(v, members_to_be_deleted)]
+                                 for k, v in self.member_tags.items()}
+
+    def get_number_of_members(self) -> int:
+        """
+        :return: the number of members in ``Structure``
+        """
+        return self.members.shape[1]
+
+    def get_member_tags(self, index: int) -> List[str]:
+        """
+        A list with the tags for the member with index ``index``
+
+        :param index: the index of the member
+        :return: list of tags
+        """
+        return [k for k, v in self.member_tags.items() if index in v]
+
+    def has_member_tag(self, index: int, tag: str) -> bool:
+        """
+        Return ``True`` if member with index ``index`` has tag ``tag``
+
+        :param index: the index of the member
+        :param tag: the tag
+        :return: ``True`` or ``False``
+        """
+        return tag in self.member_tags and index in self.member_tags[tag]
+
+    def get_members_by_tags(self, tags: Sequence[str]) -> npt.NDArray[np.uint64]:
+        """
+        Return a list of member indices that have tags in the sequence ``tags``
+
+        :param tags: the sequence of tags
+        :return: list of member indices
+        """
+        if len(tags) == 0:
+            return np.zeros((0,))
+        elif len(tags) == 1:
+            return self.member_tags.get(tags[0], np.zeros((0,)))
+        else:
+            return reduce(lambda a1, a2: np.intersect1d(a1, a2, assume_unique=True),
+                          [v for k, v in self.member_tags.items() if k in tags])
+
+    def get_number_of_members_by_tag(self, tag: str) -> int:
+        """
+        Return the number of members with tag ``tag``
+
+        :param tag: the tags
+        :return: the number of members
+        """
+        return len(self.member_tags.get(tag, []))
+
+    def delete_member_tag(self, tag: str) -> None:
+        """
+        Delete member tag ``tag``
+
+        :param tag: the member tag to be deleted
+        """
+        # delete member tag
+        del self.member_tags[tag]
+        if tag in self.member_defaults:
+            del self.member_defaults[tag]
+
+    def set_member_tag(self, tag: str, indices: npt.NDArray[np.uint64]) -> None:
+        """
+        Associate members with indices in ``indices`` to the new tag ``tag``
+
+        :param tag: the member tag
+        :param indices: the member indices
+        """
+        # set new member tag
+
+        # make sure tag is unique
+        assert tag not in self.member_tags, f"member tag '{tag}' already exists"
+
+        # normalize indices
+        v = np.unique(indices)
+
+        # make sure indices are valid
+        number_of_members = self.get_number_of_members()
+        assert np.amin(v) >= 0, \
+            'member tag index must be greater or equal than zero'
+        assert np.amax(v) < number_of_members, \
+            'member tag index must be less than number of members'
+
+        # set tag
+        self.member_tags[tag] = v
+
+    def add_member_tag(self, tag: str, indices: npt.NDArray[np.uint64]) -> None:
+        """
+        Add members with indices in ``indices`` to the existing member tag ``tag``
+
+        :param tag: the member tag
+        :param indices: the member indices
+        """
+
+        # make sure indices are valid
+        number_of_members = self.get_number_of_members()
+        assert np.amin(indices) >= 0, \
+            'member tag index must be greater or equal than zero'
+        assert np.amax(indices) < number_of_members, \
+            'member tag index must be less than number of members'
+
+        # set tag
+        self.member_tags[tag] = np.union1d(self.member_tags[tag], indices)
+
+    def remove_member_tag(self, tag: str, indices: npt.NDArray[np.uint64]) -> None:
+        """
+        Remove members with indices in ``indices`` from the existing member tag ``tag``
+
+        :param tag: the member tag
+        :param indices: the member indices
+        """
+        # remove indices from existing member tag
+
+        # set tag
+        self.member_tags[tag] = np.setdiff1d(self.member_tags[tag], indices)
+
+    def delete_node_tag(self, tag: str) -> None:
+        """
+        Delete node tag ``tag``
+
+        :param tag: the node tag to be deleted
+        """
+        del self.node_tags[tag]
+        if tag in self.node_defaults:
+            del self.node_defaults[tag]
+
+    def set_node_tag(self, tag: str, indices: npt.NDArray[np.uint64]) -> None:
+        """
+        Associate nodes with indices in ``indices`` to the new tag ``tag``
+
+        :param tag: the node tag
+        :param indices: the node indices
+        """
+
+        # make sure tag is unique
+        assert tag not in self.node_tags, f"node tag '{tag}' already exists"
+
+        # normalize indices
+        v = np.unique(indices)
+
+        # make sure indices are valid
+        assert np.amin(v) >= 0, \
+            'node tag index must be greater or equal than zero'
+        assert np.amax(v) < self.get_number_of_nodes(), \
+            'node tag index must be less than number of nodes'
+
+        # set tag
+        self.node_tags[tag] = v
+
+    def add_node_tag(self, tag: str, indices: npt.NDArray[np.uint64]) -> None:
+        """
+        Add nodes with indices in ``indices`` to the existing node tag ``tag``
+
+        :param tag: the node tag
+        :param indices: the node indices
+        """
+
+        # make sure indices are valid
+        assert np.amin(indices) >= 0, \
+            'node tag index must be greater or equal than zero'
+        assert np.amax(indices) < self.get_number_of_nodes(), \
+            'node tag index must be less than number of nodes'
+
+        # set tag
+        self.node_tags[tag] = np.union1d(self.node_tags[tag], indices)
+
+    def remove_node_tag(self, tag: str, indices: npt.NDArray[np.uint64]) -> None:
+        """
+        Remove nodes with indices in ``indices`` from the existing node tag ``tag``
+
+        :param tag: the node tag
+        :param indices: the node indices
+        """
+
+        # set tag
+        self.node_tags[tag] = np.setdiff1d(self.node_tags[tag], indices)
+
+    @staticmethod
+    def _set_dataframe(df: pd.DataFrame, index: Union[int, Sequence[int], slice], labels: Union[str, Sequence[str]],
+                       values: Any, wrap: bool = False, scalar: bool = True) -> None:
+        """
+        Auxiliary set method to wrap values when setting dataframe
+
+        :param df: the dataframe
+        :param index: the row index
+        :param labels: the column label(s)
+        :param values: the values to set to
+        :param wrap: if ``True``, wraps ``value`` in a ``Series`` or ``Dataframe`` before assignment
+        :param scalar: if ``True``, ``value`` is set to an array of len(index)
+
+        **Notes:**
+
+        1. This method is for convenience when assigning objects to dataframes.
+           See `this question <https://stackoverflow.com/questions/48000225/must-have-equal-len-keys-and-value-when-setting-with-an-iterable>`_
+           for details.
+        """
+        if wrap:
+            if isinstance(index, int):
+                idx = index = [index]
+                m = 1
+            else:
+                idx = df.index[index]
+                m = len(idx)
+            if scalar:
+                values = [values] * m
+            if isinstance(labels, str):
+                values = pd.Series(values, index=idx)
+            else:
+                values = pd.DataFrame(values, index=idx)
+        df.loc[index, labels] = values
+
+    def set_member_properties(self, index: Union[int, Sequence[int], slice], labels: Union[str, Sequence[str]],
+                              values: Any, wrap: bool = False, scalar: bool = True) -> None:
+        """
+        Set member properties
+
+        See :meth:`tnsgrt.structure.Structure._set_dataframe`
+
+        :param index: the element index
+        :param labels: the property label(s)
+        :param values: the values to set to
+        :param wrap: if ``True``, wraps ``value`` in a ``Series`` or ``Dataframe`` before assignment
+        :param scalar: if ``True``, ``value`` is set to an array of len(index)
+        """
+        Structure._set_dataframe(self.member_properties, index, labels, values, wrap, scalar)
+
+    def get_member_properties(self, index: Union[int, Sequence[int], slice], labels: Union[str, List[str]])\
+            -> pd.DataFrame:
+        """
+        Retrieve member properties
+
+        :param index: the member index
+        :param labels: the member property labels
+        :return: datafrome with the selected properties
+        """
+        return self.member_properties.loc[index, labels]
+
+    def set_node_properties(self, index: Union[int, Sequence[int], slice], labels: Union[str, Sequence[str]],
+                            values: Any, wrap: bool = False, scalar: bool = True) -> None:
+        """
+        Set node properties
+
+        See :meth:`tnsgrt.structure.Structure._set_dataframe`
+
+        :param index: the element index
+        :param labels: the property label(s)
+        :param values: the values to set to
+        :param wrap: if ``True``, wraps ``value`` in a ``Series`` or ``Dataframe`` before assignment
+        :param scalar: if ``True``, ``value`` is set to an array of len(index)
+        """
+        Structure._set_dataframe(self.node_properties, index, labels, values, wrap, scalar)
+
+    def get_node_properties(self, index: Union[int, Sequence[int], slice], labels: Union[str, List[str]])\
+            -> pd.DataFrame:
+        """
+        Retrieve node properties
+
+        :param index: the node index
+        :param labels: the node property labels
+        :return: datafrome with the selected properties
+        """
+        return self.node_properties.loc[index, labels]
+
+    def get_member_vectors(self) -> npt.NDArray[np.float_]:
+        """
+        :return: a 3 x m array with the ``Structure``'s members
+        """
+        return self.nodes[:, self.members[1, :]] - self.nodes[:, self.members[0, :]]
+
+    def get_member_length(self) -> npt.NDArray[np.float_]:
+        """
+        :return: an array with the ``Structure``'s member lengths
+        """
+        return np.linalg.norm(self.nodes[:, self.members[1, :]] - self.nodes[:, self.members[0, :]], axis=0)
+
+    def get_center_of_mass(self) -> npt.NDArray[np.float_]:
+        """
+        :return: the ``Structure``'s center of mass
+        """
+        # Computes the center of mass
+        mass = self.member_properties['mass'].values
+        return np.sum(mass * (self.nodes[:, self.members[0, :]] + self.nodes[:, self.members[1, :]])/2, axis=1) \
+            / np.sum(mass)
+
+    def get_centroid(self) -> npt.NDArray[np.float_]:
+        """
+        :return: the ``Structure``'s geometric center or centroid
+        """
+        # Computes the centroid (geometric center)
+        return np.sum(self.nodes, axis=1) / self.get_number_of_nodes()
+
+    def update_member_properties(self, property_name: Optional[Union[str, Iterable[str]]] = None) -> None:
+        """
+        Update ``Structure``'s member properties
+
+        If property_name is
+
+        - 'stiffness': calculate ``stiffness`` and ``rest_length`` based on ``modulus``, ``radius``, ``inner_radius``
+           and ``lambda_``
+        - 'mass': calculate ``mass`` and ``volume`` based on ``radius`` and ``density``
+        - 'force': calculate ``force`` based on ``lambda_``
+
+        :param property_name: the property name to update; if ``None``, update all properties
+        """
+
+        if isinstance(property_name, str):
+
+            # update stiffness and rest length
+            if property_name == 'stiffness':
+                member_length = self.get_member_length()
+                modulus_times_area = self.member_properties['modulus'].values * np.pi * \
+                    (self.member_properties['radius'].values ** 2 - self.member_properties['inner_radius'].values ** 2)
+                stiffness = modulus_times_area / member_length
+                if np.any(stiffness < 0):
+                    raise Exception(f'Structure::update_member_property: negative stiffness computed')
+                rest_length = member_length * (1 - self.member_properties['lambda_'].values / stiffness)
+                if np.any(rest_length < 0):
+                    raise Exception(f'Structure::update_member_property: negative rest_length computed')
+                self.member_properties['stiffness'] = stiffness
+                self.member_properties['rest_length'] = rest_length
+
+            # update mass and volume
+            elif property_name == 'mass':
+                member_length = self.get_member_length()
+                volume = np.pi * (self.member_properties['radius'] ** 2 -
+                                  self.member_properties['inner_radius'].values ** 2) * member_length
+                if np.any(volume < 0):
+                    raise Exception(f'Structure::update_member_property: negative volume computed')
+                mass = volume * self.member_properties['density']
+                if np.any(mass < 0):
+                    raise Exception(f'Structure::update_member_property: negative mass computed')
+                self.member_properties['volume'] = volume
+                self.member_properties['mass'] = mass
+
+            # update force
+            elif property_name == 'force':
+                self.member_properties['force'] = self.get_member_length() * self.member_properties['lambda_'].values
+
+            else:
+                raise Exception('Structure::update_member_property: '
+                                f'do not know how to update property {property_name}')
+
+        else:
+
+            # iterate all if None
+            if property_name is None:
+                property_name = ['mass', 'stiffness', 'force']
+
+            # iterate properties
+            for prop in property_name:
+                self.update_member_properties(prop)
+
+    def get_close_nodes(self, radius=1e-6) -> Tuple[Set[int], npt.NDArray]:
+        """
+        Returns the set of nodes that lie within ``radius`` distance to other nodes in ``Structure`` and the
+        corresponding map
+
+        For example, if::
+
+            close_nodes, close_nodes_map = s.get_close_nodes()
+
+        is such that::
+
+            close_nodes = {1, 3}
+            close_nodes_map = [0,0,2,2,4]
+
+        then node ``1`` is close to node ``0`` and node ``3`` is close to node ``2``.
+
+        :param radius: the proximity radius
+        :return: tuple with ``close_nodes`` and ``close_nodes_map``
+        """
+
+        tree = scipy.spatial.KDTree(self.nodes.transpose())
+        indices = tree.query_ball_tree(tree, r=radius)
+        close_nodes_map = np.arange(self.get_number_of_nodes())
+        close_nodes_set = set()
+        for i, neighbors in enumerate(indices):
+            for k in [j for j in neighbors if j > i]:
+                close_nodes_map[k] = i
+                close_nodes_set.add(k)
+        if close_nodes_set:
+            # apply map until no changes
+            while True:
+                last_merge_map = close_nodes_map.copy()
+                close_nodes_map = close_nodes_map[close_nodes_map]
+                if np.all(last_merge_map == close_nodes_map):
+                    break
+        return close_nodes_set, close_nodes_map
+
+    def merge_close_nodes(self, radius: float = 1e-6, verbose: bool = False) -> None:
+        """
+        Merge then remove all nodes in ``Structure`` which lie within ``radius``
+
+        :param radius: the proximity radius
+        :param verbose: if ``True`` issues a warning with number of nodes removed after the merge
+        """
+        # get close nodes
+        close_nodes_set, close_nodes_map = self.get_close_nodes(radius)
+        if close_nodes_set:
+            # list of nodes to be removed
+            nodes_to_be_removed = list(close_nodes_set)
+            # apply merge_map to members
+            self.members = close_nodes_map[self.members]
+            # remove nodes, to make sure the member node numbering is correct
+            self.remove_nodes(nodes_to_be_removed, verify_if_unused=False, verbose=verbose)
+
+    def merge(self, s: 'Structure', inplace=False) -> Optional['Structure']:
+        """
+        Return a new ``Structure`` in which the current `Structure`` and ``s`` are merged
+
+        :param s: the ``Structure`` to merge
+        :param inplace: if ``True`` merge is done in place without creating a copy
+        :return: the merged ``Structure``
+        """
+
+        if inplace:
+            target = self
+        else:
+            target = self.copy()
+
+        # offset members in s by number_of_members
+        number_of_members = self.get_number_of_members()
+        number_of_nodes = self.get_number_of_nodes()
+
+        # merge nodes
+        target.nodes = np.hstack((self.nodes, s.nodes))
+
+        # merge node tags
+        for k, v in s.node_tags.items():
+            # append or add
+            target.node_tags[k] = np.hstack((self.node_tags[k], number_of_nodes + v)) \
+                if k in self.node_tags \
+                else number_of_nodes + v
+
+        # merge node properties
+        target.node_properties = pd.concat((self.node_properties, s.node_properties), ignore_index=True)
+
+        # merge members, offset by number of nodes
+        target.members = np.hstack((self.members, number_of_nodes + s.members))
+
+        # merge member tags
+        for k, v in s.member_tags.items():
+            # append or add
+            target.member_tags[k] = np.hstack((self.member_tags[k], number_of_members + v)) \
+                if k in self.member_tags \
+                else number_of_members + v
+
+        # merge member properties
+        target.member_properties = pd.concat((self.member_properties, s.member_properties), ignore_index=True)
+
+        return target
+
+    def equilibrium(self, force: Optional[npt.ArrayLike] = None, lambda_bar: float = 1,
+                    equalities: Optional[list[npt.ArrayLike]] = None,
+                    epsilon: float = 1e-7) -> None:
+        """
+        Solves for the set of internal forces that ensures the equilibrium of the current ``Structure`` in response
+        to the vector of external forces ``forces``
+
+        Solve the force equilibrium equation
+
+        .. math::
+           A \\lambda = f
+
+        in which:
+
+        - :math:`A`: is a matrix representing the element vectors
+        - :math:`f`: is the vector of external forces
+        - :math:`\\lambda`: is the vector of resulting force coefficients
+
+        If the :math:`i` th element is a string then
+
+        .. math::
+            x_i \\geq 0
+
+        If no external force is given then the sum of the bar force coefficients equals ``lambda_bar``
+
+        All elements in the equalities are set equal. For example, if::
+
+            equalities = [[0, 1, 3], [2, 4]]
+
+        then the equilibrium is shought satisfying the constraints
+
+        .. math::
+            x_0 = x_1 = x_3, \\qquad x_2 = x_4
+
+        :param force: a 3 x n array of external forces; or zero if `None`
+        :param lambda_bar: the normalizing factor
+        :param equalities: a list of lists of member indices which are constrained to have the same force coefficient
+        :param epsilon: numerical accuracy
+        """
+
+        number_of_nodes = self.get_number_of_nodes()
+        number_of_strings = len(self.member_tags.get('string', []))
+        number_of_bars = len(self.member_tags.get('bar', []))
+        number_of_members = number_of_strings + number_of_bars
+
+        assert number_of_members == number_of_bars + number_of_strings, \
+            'number of members is not equal to the sum of number of bars and strings'
+
+        # member vectors
+        member_vectors = self.get_member_vectors()
+
+        # coefficient matrix
+        Aeq = np.zeros((3 * number_of_nodes, number_of_members))
+
+        # string coefficient
+        if number_of_strings:
+            for i in self.member_tags['string']:
+
+                ii = 3 * int(self.members[0, i])
+                Aeq[ii:ii+3, i] = -member_vectors[:, i]
+
+                jj = 3 * int(self.members[1, i])
+                Aeq[jj:jj+3, i] = member_vectors[:, i]
+
+        # bar coefficient
+        if number_of_bars:
+            for i in self.member_tags['bar']:
+
+                ii = 3 * int(self.members[0, i])
+                Aeq[ii:ii+3, i] = member_vectors[:, i]
+
+                jj = 3 * int(self.members[1, i])
+                Aeq[jj:jj+3, i] = -member_vectors[:, i]
+
+        A = Aeq
+        m = 3 * number_of_nodes
+
+        # external forces
+        if force is None:
+            A = np.vstack((A, np.ones((1, number_of_members))))
+            blo = bup = np.hstack((np.zeros((3 * number_of_nodes,)), 1))
+        else:
+            beq = np.array(force)
+            assert np.all(beq.shape == (3, number_of_nodes)), 'force must be a 3 x n matrix'
+            blo = bup = beq.flatten(order='F')
+
+        # For equilibrium: Aeq x = beq
+
+        # impose equalities
+        # indices in each row are set to be equal
+        if equalities is not None:
+            number_of_constraints = sum(map(len, equalities)) - len(equalities)
+            Aeq = np.zeros((number_of_constraints, number_of_members))
+            beq = np.zeros((number_of_constraints, ))
+            ii = 0
+            for eqs in equalities:
+                nn = len(eqs)
+                for jj in range(1, nn):
+                    Aeq[ii+jj-1, eqs[0]] = 1
+                    Aeq[ii+jj-1, eqs[jj]] = -1
+                ii += nn
+            A = np.vstack((A, Aeq))
+            blo = bup = np.hstack((blo, beq))
+
+        # enforce strings have positive force coefficients
+        # when there are no external forces set to one to avoid nontrivial solution
+        xup = None
+        if number_of_strings:
+            xlo = np.full((number_of_members, ), 0)
+            xlo[self.member_tags['string']] = 0
+        else:
+            xlo = None
+
+        # cost function
+        c = np.ones((number_of_members,))
+
+        # solve lp
+        cost, gamma, status = optim.lp(number_of_members, m, c, A, blo, bup, xlo, xup)
+
+        # if infeasible, throw error
+        if status == 'infeasible':
+            raise Exception('could not find equilibrium')
+
+        # flip sign for bars
+        lambda_ = gamma
+        if number_of_bars:
+            lambda_[self.member_tags['bar']] *= -1
+
+            if force is None:
+                # scale solution for bars
+                scale = -np.sum(lambda_[self.member_tags['bar']]) / number_of_bars
+                lambda_ *= np.abs(lambda_bar) / scale
+
+        # assign lambda
+        self.member_properties['lambda_'] = lambda_
+
+        # update force
+        self.update_member_properties('force')
+
+    def stiffness(self, epsilon: float = 1e-6, storage: str = 'sparse',
+                  apply_rigid_body_constraint: bool = False,
+                  apply_planar_constraint: bool = False):
+        """
+        Computes
+
+        - `normal`: potential energy (1 x 1)
+        - `F`: force vectors (3 x n)
+        - `K`: stiffness matrix (3 n x 3 n)
+        - `M`: mass matrix (n x 1)
+
+        for the current ``Structure``. The mass and stiffness matrices are returned in the form of an object of the
+        class :class:`tnsgrt.stiffness.Stiffness`
+
+        :param epsilon: numerical accuracy
+        :param storage: if ``sparse`` stores the resulting stiffeness and mass matrices in sparse csr format
+        :param apply_rigid_body_constraint: if ``True`` apply 3D rigid body constraints
+        :param apply_planar_constraint: if ``True`` apply 2D constraints
+        :return: tuple (`S`, `F`, `normal`)
+        """
+
+        number_of_nodes = self.get_number_of_nodes()
+        number_of_strings = len(self.member_tags.get('string', []))
+        number_of_bars = len(self.member_tags.get('bar', []))
+        number_of_members = number_of_strings + number_of_bars
+
+        assert number_of_members == number_of_bars + number_of_strings, \
+            'number of members is not equal to the sum of number of bars and strings'
+
+        if number_of_nodes <= 12 and storage == 'sparse':
+            storage = 'dense'
+            warnings.warn("number of nodes is small; storage set to 'dense'")
+
+        # member vectors
+        member_vectors = self.get_member_vectors()
+        member_length = self.get_member_length()
+
+        k = self.member_properties['stiffness'].values
+        lambda_ = self.member_properties['lambda_'].values
+        mass = self.member_properties['mass'].values
+
+        # compute potential
+        v = np.sum(((lambda_ * member_length) ** 2) / k / 2)
+
+        # Compute force and stiffness
+
+        # preallocate F
+        F = np.zeros((3, number_of_nodes))
+        # preallocate K
+        if storage == 'sparse':
+            # sparse storage
+            diag = np.unique(self.members)
+            diff = np.unique(self.members, axis=1)
+            row_col = np.hstack((np.vstack((diag, diag)), diff, np.flipud(diff)))
+            data = np.zeros((row_col.shape[1]))
+            K = scipy.sparse.kron(scipy.sparse.coo_matrix((data, row_col),
+                                                          shape=(number_of_nodes, number_of_nodes)),
+                                  np.ones((3, 3))).tocsr()
+        else:
+            # dense storage
+            K = np.zeros((3 * number_of_nodes, 3 * number_of_nodes))
+
+        lambda_ * member_vectors
+        # calculate stiffness and force
+        for i in range(number_of_members):
+
+            mij = member_vectors[:, i] / member_length[i]
+            fij = lambda_[i] * member_vectors[:, i]
+
+            mijmij = np.outer(mij, mij)
+            # kij = k[index] * Mij + lambda_[index] * (np.eye(3) - Mij)
+            kij = (k[i] - lambda_[i]) * mijmij + lambda_[i] * np.eye(3)
+
+            i, j = self.members[:, i].astype(dtype=np.int_)
+
+            F[:, i] += fij
+            F[:, j] -= fij
+
+            ii = 3 * i
+            jj = 3 * j
+
+            K[ii:ii+3, ii:ii+3] += kij
+            K[jj:jj+3, jj:jj+3] += kij
+            K[ii:ii+3, jj:jj+3] -= kij
+            K[jj:jj+3, ii:ii+3] -= kij
+
+        # Compute mass
+        M = np.zeros((number_of_nodes,))
+        M[self.members[0, :]] = mass / 2
+        M[self.members[1, :]] += mass / 2
+
+        diag = np.kron(M, np.ones((3,)))
+        if storage == 'sparse':
+            # sparse storage
+            M = scipy.sparse.diags(diag, format='csr')
+        else:
+            # dense storage
+            M = np.diag(np.kron(M, np.ones((3,))))
+
+        # Check forces
+        sum_of_forces = np.linalg.norm(F, ord='fro')
+        if sum_of_forces > epsilon:
+            warnings.warn(f'Structure::stiffness: force balance not satisfied, sum of forces = {sum_of_forces}')
+
+        # Build stiffness object
+        stiffness = Stiffness(K, M)
+
+        # node constraints
+        constraints = self.node_properties['constraint']
+        has_constraints = constraints.isna().sum() < self.get_number_of_nodes()
+        if has_constraints:
+            # apply node constraints
+            stiffness.apply_constraint(*NodeConstraint.node_constraint(self.nodes, constraints))
+        if apply_rigid_body_constraint:
+            # apply rigid body constraints
+            stiffness.apply_constraint(*NodeConstraint.rigid_body_constraint(self.nodes), local=False)
+        if apply_planar_constraint:
+            # apply planar constraints
+            stiffness.apply_constraint(*NodeConstraint.planar_constraint(self.nodes), local=False)
+
+        return stiffness, F, v
```

### Comparing `tnsgrt-0.3/src/tnsgrt/utils.py` & `tnsgrt-0.4/src/tnsgrt/utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-from enum import Enum
-from typing import Literal, Tuple, Union
-
-import numpy as np
-import numpy.typing as npt
-import scipy
-
-
-def rotation_2d(phi: float) -> npt.NDArray:
-    """
-    Return a 2D rotation matrix
-
-    :param phi: the rotation angle in radians
-    :return: the rotation matrix
-    """
-    return np.array([[np.cos(phi), -np.sin(phi)], [np.sin(phi), np.cos(phi)]])
-
-
-def rotation_3d(v: npt.NDArray) -> npt.NDArray:
-    """
-    Return a 3D rotation matrix
-
-    :param v: the vector around which to rotate; its norm is the angle to rotate
-    :return: the rotation matrix
-
-    **Notes:**
-
-    See :meth:`scipy.spatial.transform.Rotation.from_rotvec` for details
-    """
-    return scipy.spatial.transform.Rotation.from_rotvec(v).as_matrix()
-
-
-def orthogonalize(a: npt.NDArray, epsilon: float = 1e-8, mode: Literal['reduced', 'complete'] = 'reduced')\
-        -> Union[Tuple[int, npt.NDArray, npt.NDArray],Tuple[int, npt.NDArray]]:
-    """
-    Ortoghonalize the constraint
-
-    .. math::
-        A^T \\, x = 0
-
-    :param a: the coefficient array :math:`A`
-    :param epsilon: the accuracy with which to evaluate the rank
-    :param mode: 'complete' or 'reduced'
-    :return: tuple with rank, the orthogonalized coefficient array, and its null space if mode is 'complete'
-
-    **Notes:**
-
-        1. If ``mode = 'reduced'`` the constraint coefficient is normalized at the constructor by calculating
-           the *reduced* QR decomposition
-
-           .. math::
-               A = Q R, \\quad Q^T Q = I, \\quad R \\text{ is upper triangular}
-
-           Assuming that :math:`A` is full rank, the equivalent orthogonal constraint
-
-           .. math::
-               A^T x = R^T V^T x = 0 \\quad \\Leftrightarrow \\quad V^T x = 0
-
-           is obtained in which the coefficient is the orthogonal matrix :math:`V = Q`
-
-        2. If ``mode = 'complete'`` the constraint coefficient is normalized at the constructor by calculating
-           the *complete* QR decomposition
-
-           .. math::
-               A = Q R, \\quad Q^T Q = Q Q^T = I, \\quad R \\text{ is upper triangular}
-
-           Assuming that :math:`A` is full rank, partition
-
-           .. math::
-               \\begin{bmatrix} V & T \\end{bmatrix} = Q = \\begin{bmatrix} Q_1 & Q_2 \\end{bmatrix}, \\qquad R = \\begin{bmatrix} R_1 \\\\ 0 \\end{bmatrix}, \\quad R_1 \\text{ is upper triangular}
-
-           to obtain the equivalent orthogonal constraint and its solution
-
-           .. math::
-               A^T x = R_1^T V^T x = 0 \\quad \\Leftrightarrow \\quad V^T x = 0, \\qquad x = T y
-
-           The matrix :math:`T` is an orthogonal basis for the constraint null space
-
-        3. The above factorizations are modified to take into account the numerical rank of :math:`A` when it
-           is rank-deficient
-    """
-    assert a.shape[1] < a.shape[0], 'a must be tall'
-    # QR decomposition
-    if mode == 'complete':
-        q, r = np.linalg.qr(a, mode='complete')
-    else:
-        q, r = np.linalg.qr(a)
-    # check for rank
-    rank = np.count_nonzero(np.abs(np.diag(r)) > epsilon)
-    # return tuple
-    if mode == 'complete':
-        return rank, q[:, :rank], q[:, rank:]
-    else:
-        return rank, q[:, :rank]
-
-
-def norm(a: Union[npt.NDArray, scipy.sparse.csr_matrix]) -> float:
-    """
-    :param a: the array
-    :return: the 2-norm of the array
-    """
-    return np.linalg.norm(a.data) if scipy.sparse.issparse(a) else np.linalg.norm(a)
-
-
-class Colors(Enum):
-    """
-    Default colors
-    """
-
-    BLUE = (0, 0.4470, 0.7410)
-    """
-    """
-    ORANGE = (0.8500, 0.3250, 0.0980)
-    """
-    """
-    YELLOW = (0.9290, 0.6940, 0.1250)
-    """
-    """
-    PURPLE = (0.4940, 0.1840, 0.5560)
-    """
-    """
-    GREEN = (0.4660, 0.6740, 0.1880)
-    """
-    """
-    LIGHT_BLUE = (0.3010, 0.7450, 0.9330)
-    """
-    """
-    BROWN = (0.6350, 0.0780, 0.1840)
-    """
-    """
+from enum import Enum
+from typing import Literal, Tuple, Union
+
+import numpy as np
+import numpy.typing as npt
+import scipy
+
+
+def rotation_2d(phi: float) -> npt.NDArray:
+    """
+    Return a 2D rotation matrix
+
+    :param phi: the rotation angle in radians
+    :return: the rotation matrix
+    """
+    return np.array([[np.cos(phi), -np.sin(phi)], [np.sin(phi), np.cos(phi)]])
+
+
+def rotation_3d(v: npt.NDArray) -> npt.NDArray:
+    """
+    Return a 3D rotation matrix
+
+    :param v: the vector around which to rotate; its norm is the angle to rotate
+    :return: the rotation matrix
+
+    **Notes:**
+
+    See :meth:`scipy.spatial.transform.Rotation.from_rotvec` for details
+    """
+    return scipy.spatial.transform.Rotation.from_rotvec(v).as_matrix()
+
+
+def orthogonalize(a: npt.NDArray, epsilon: float = 1e-8, mode: Literal['reduced', 'complete'] = 'reduced')\
+        -> Union[Tuple[int, npt.NDArray, npt.NDArray],Tuple[int, npt.NDArray]]:
+    """
+    Ortoghonalize the constraint
+
+    .. math::
+        A^T \\, x = 0
+
+    :param a: the coefficient array :math:`A`
+    :param epsilon: the accuracy with which to evaluate the rank
+    :param mode: 'complete' or 'reduced'
+    :return: tuple with rank, the orthogonalized coefficient array, and its null space if mode is 'complete'
+
+    **Notes:**
+
+        1. If ``mode = 'reduced'`` the constraint coefficient is normalized at the constructor by calculating
+           the *reduced* QR decomposition
+
+           .. math::
+               A = Q R, \\quad Q^T Q = I, \\quad R \\text{ is upper triangular}
+
+           Assuming that :math:`A` is full rank, the equivalent orthogonal constraint
+
+           .. math::
+               A^T x = R^T V^T x = 0 \\quad \\Leftrightarrow \\quad V^T x = 0
+
+           is obtained in which the coefficient is the orthogonal matrix :math:`V = Q`
+
+        2. If ``mode = 'complete'`` the constraint coefficient is normalized at the constructor by calculating
+           the *complete* QR decomposition
+
+           .. math::
+               A = Q R, \\quad Q^T Q = Q Q^T = I, \\quad R \\text{ is upper triangular}
+
+           Assuming that :math:`A` is full rank, partition
+
+           .. math::
+               \\begin{bmatrix} V & T \\end{bmatrix} = Q = \\begin{bmatrix} Q_1 & Q_2 \\end{bmatrix}, \\qquad R = \\begin{bmatrix} R_1 \\\\ 0 \\end{bmatrix}, \\quad R_1 \\text{ is upper triangular}
+
+           to obtain the equivalent orthogonal constraint and its solution
+
+           .. math::
+               A^T x = R_1^T V^T x = 0 \\quad \\Leftrightarrow \\quad V^T x = 0, \\qquad x = T y
+
+           The matrix :math:`T` is an orthogonal basis for the constraint null space
+
+        3. The above factorizations are modified to take into account the numerical rank of :math:`A` when it
+           is rank-deficient
+    """
+    assert a.shape[1] < a.shape[0], 'a must be tall'
+    # QR decomposition
+    if mode == 'complete':
+        q, r = np.linalg.qr(a, mode='complete')
+    else:
+        q, r = np.linalg.qr(a)
+    # check for rank
+    rank = np.count_nonzero(np.abs(np.diag(r)) > epsilon)
+    # return tuple
+    if mode == 'complete':
+        return rank, q[:, :rank], q[:, rank:]
+    else:
+        return rank, q[:, :rank]
+
+
+def norm(a: Union[npt.NDArray, scipy.sparse.csr_matrix]) -> float:
+    """
+    :param a: the array
+    :return: the 2-norm of the array
+    """
+    return np.linalg.norm(a.data) if scipy.sparse.issparse(a) else np.linalg.norm(a)
+
+
+class Colors(Enum):
+    """
+    Default colors
+    """
+
+    BLUE = (0, 0.4470, 0.7410)
+    """
+    """
+    ORANGE = (0.8500, 0.3250, 0.0980)
+    """
+    """
+    YELLOW = (0.9290, 0.6940, 0.1250)
+    """
+    """
+    PURPLE = (0.4940, 0.1840, 0.5560)
+    """
+    """
+    GREEN = (0.4660, 0.6740, 0.1880)
+    """
+    """
+    LIGHT_BLUE = (0.3010, 0.7450, 0.9330)
+    """
+    """
+    BROWN = (0.6350, 0.0780, 0.1840)
+    """
+    """
```

### Comparing `tnsgrt-0.3/src/tnsgrt/plotter/plotter.py` & `tnsgrt-0.4/src/tnsgrt/plotter/plotter.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-from typing import Union, Sequence, Tuple
-
-import numpy as np
-import numpy.typing as npt
-from scipy.spatial.transform import Rotation
-
-from tnsgrt.structure import Structure
-
-
-class Plotter:
-    """
-    Base class for structure plotters
-    """
-
-    def plot(self, s: Union[Structure, Sequence[Structure]], **kwargs) -> None:
-        """
-        Plot structure
-
-        :param s: the structure or sequence of structures
-        :param \\**kwargs: additional keyword arguments
-        """
-        pass
-
-    @staticmethod
-    def unit_cylinder(n: int = 10, radius: float = 1, height: float = 1) \
-            -> tuple[npt.NDArray, npt.NDArray, npt.NDArray]:
-        """
-        Return xyz grid points for solid cylinder centered at the origin
-
-        :param n: number of sides
-        :param radius: radius of cylinder
-        :param height: height of cylinder
-        :return: tuple with x, y, and z points
-        """
-        z = np.linspace(0, height, 2)
-        theta = np.linspace(0, 2 * np.pi, n)
-        theta_grid, z_grid = np.meshgrid(theta, z)
-        x_grid = radius * np.cos(theta_grid)
-        y_grid = radius * np.sin(theta_grid)
-        return x_grid, y_grid, z_grid
-
-    @staticmethod
-    def cylinder(node1: npt.NDArray, node2: npt.NDArray,
-                 volume: float = 0., radius: float = 0.01, n: int = 12) \
-            -> Tuple[npt.NDArray, npt.NDArray, npt.NDArray]:
-        """
-        Return xyz grid points for cylinder with center aligned with the vector defined by ``node1`` and ``node2``
-
-        :param node1: center of the base of the cylinder
-        :param node2: center of the top of the cylinder
-        :param volume: volume of the cylinder, used to set the radius if positive
-        :param radius: radius of the cylinder, ignore if volume is positive
-        :param n: number of sides
-        :return: tuple with x, y, and z points
-        """
-        # rod vector length
-        rod = node2 - node1
-        length = np.linalg.norm(rod)
-        if volume > 0.:
-            radius = np.sqrt((volume / length) / np.pi)
-
-        # draw unit cylinder
-        x, y, z = Plotter.unit_cylinder(n, radius, length)
-
-        # rotation vector
-        rotation_vector = [-rod[1], rod[0], 0]
-
-        # rotation angle
-        angle = np.arccos(rod[2] / length)
-        if angle > 1e-4:
-
-            norm = np.linalg.norm(rotation_vector)
-            if norm < 1e-6:
-                rotation_vector = [1, 0, 0]
-            else:
-                rotation_vector /= norm
-
-            rotation_matrix = Rotation.from_rotvec(angle * rotation_vector)
-
-            # rotate
-            for i in range(x.shape[0]):
-                xyz = np.vstack((x[i, :], y[i, :], z[i, :]))
-                xyz = rotation_matrix.apply(xyz.transpose()).transpose()
-                x[i, :] = xyz[0, :]
-                y[i, :] = xyz[1, :]
-                z[i, :] = xyz[2, :]
-
-        # translate
-        x += node1[0]
-        y += node1[1]
-        z += node1[2]
-
-        return x, y, z
+from typing import Union, Sequence, Tuple
+
+import numpy as np
+import numpy.typing as npt
+from scipy.spatial.transform import Rotation
+
+from tnsgrt.structure import Structure
+
+
+class Plotter:
+    """
+    Base class for structure plotters
+    """
+
+    def plot(self, s: Union[Structure, Sequence[Structure]], **kwargs) -> None:
+        """
+        Plot structure
+
+        :param s: the structure or sequence of structures
+        :param \\**kwargs: additional keyword arguments
+        """
+        pass
+
+    @staticmethod
+    def unit_cylinder(n: int = 10, radius: float = 1, height: float = 1) \
+            -> tuple[npt.NDArray, npt.NDArray, npt.NDArray]:
+        """
+        Return xyz grid points for solid cylinder centered at the origin
+
+        :param n: number of sides
+        :param radius: radius of cylinder
+        :param height: height of cylinder
+        :return: tuple with x, y, and z points
+        """
+        z = np.linspace(0, height, 2)
+        theta = np.linspace(0, 2 * np.pi, n)
+        theta_grid, z_grid = np.meshgrid(theta, z)
+        x_grid = radius * np.cos(theta_grid)
+        y_grid = radius * np.sin(theta_grid)
+        return x_grid, y_grid, z_grid
+
+    @staticmethod
+    def cylinder(node1: npt.NDArray, node2: npt.NDArray,
+                 volume: float = 0., radius: float = 0.01, n: int = 12) \
+            -> Tuple[npt.NDArray, npt.NDArray, npt.NDArray]:
+        """
+        Return xyz grid points for cylinder with center aligned with the vector defined by ``node1`` and ``node2``
+
+        :param node1: center of the base of the cylinder
+        :param node2: center of the top of the cylinder
+        :param volume: volume of the cylinder, used to set the radius if positive
+        :param radius: radius of the cylinder, ignore if volume is positive
+        :param n: number of sides
+        :return: tuple with x, y, and z points
+        """
+        # rod vector length
+        rod = node2 - node1
+        length = np.linalg.norm(rod)
+        if volume > 0.:
+            radius = np.sqrt((volume / length) / np.pi)
+
+        # draw unit cylinder
+        x, y, z = Plotter.unit_cylinder(n, radius, length)
+
+        # rotation vector
+        rotation_vector = [-rod[1], rod[0], 0]
+
+        # rotation angle
+        angle = np.arccos(rod[2] / length)
+        if angle > 1e-4:
+
+            norm = np.linalg.norm(rotation_vector)
+            if norm < 1e-6:
+                rotation_vector = [1, 0, 0]
+            else:
+                rotation_vector /= norm
+
+            rotation_matrix = Rotation.from_rotvec(angle * rotation_vector)
+
+            # rotate
+            for i in range(x.shape[0]):
+                xyz = np.vstack((x[i, :], y[i, :], z[i, :]))
+                xyz = rotation_matrix.apply(xyz.transpose()).transpose()
+                x[i, :] = xyz[0, :]
+                y[i, :] = xyz[1, :]
+                z[i, :] = xyz[2, :]
+
+        # translate
+        x += node1[0]
+        y += node1[1]
+        z += node1[2]
+
+        return x, y, z
```

### Comparing `tnsgrt-0.3/src/tnsgrt/plotter/vispy.py` & `tnsgrt-0.4/src/tnsgrt/plotter/vispy.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-from typing import Sequence, Union
-
-from tnsgrt.structure import Structure
-from .plotter import Plotter
-
-from vispy import scene as vispyscene
-
-
-class VisPyPlotter(Plotter):
-    """
-    VisPy based structure plotter
-
-    :param camera: dict with camera settings
-    :param scene: dict with vispy scene settings
-    """
-
-    defaults = {
-        'plot_nodes': True,
-        'plot_members': True,
-        'node_marker': 'o',
-        'node_markersize': .05,
-        'node_linewidth': 2,
-        'node_linestyle': 'none',
-        'node_facecolor': (1, 1, 1),
-        'node_edgecolor': (1, 1, 1)
-    }
-
-    def __init__(self, camera=None, scene=None):
-
-        scene_kwargs = {
-            'keys': 'interactive',
-            'size': (600, 600)
-        }
-        if scene:
-            scene_kwargs.update(scene)
-
-        camera_kwargs = {
-            'fov': 0,
-            'scale_factor': 1
-        }
-        if camera:
-            camera_kwargs.update(camera if camera else {})
-
-        # Create canvas and view
-        self.canvas = vispyscene.SceneCanvas(**scene_kwargs)
-        self.view = self.canvas.central_widget.add_view()
-        self.view.camera = vispyscene.cameras.ArcballCamera(**camera_kwargs)
-
-    def get_canvas(self):
-        """
-        :return: vispy canvas 
-        """
-        return self.canvas
-
-    def plot(self, s: Union[Structure, Sequence[Structure]], **kwargs):
-
-        # loop if a sequence is given
-        if not isinstance(s, Structure):
-            for si in s:
-                self.plot(si, **kwargs)
-            return
-
-        # process options
-        defaults = VisPyPlotter.defaults.copy()
-        defaults.update(kwargs)
-
-        # plot nodes
-        nodes = s.nodes
-        if defaults['plot_nodes']:
-            # Create and show visual
-            vis = vispyscene.visuals.Markers(
-                pos=nodes.transpose(),
-                size=defaults['node_markersize'],
-                antialias=0,
-                face_color=defaults['node_facecolor'],
-                edge_color=defaults['node_edgecolor'],
-                edge_width=0,
-                scaling=True,
-                spherical=True,
-            )
-            vis.parent = self.view.scene
-
-        # plot members
-        members = s.members
-        if defaults['plot_members']:
-            for j in range(s.get_number_of_members()):
-                if s.member_properties.loc[j, 'visible']:
-                    if s.has_member_tag(j, 'string'):
-                        # plot strings as lines
-                        kwargs = s.get_member_properties(j, ['facecolor', 'linewidth']).to_dict()
-                        kwargs['color'] = kwargs['facecolor']
-                        del kwargs['facecolor']
-                        kwargs['width'] = kwargs['linewidth']
-                        del kwargs['linewidth']
-                        line = nodes[:, [members[0, j], members[1, j]]].transpose()
-                        vis = vispyscene.visuals.Line(line, **kwargs)
-                        vis.parent = self.view.scene
-                    else:
-                        # plot others as solid elements
-                        kwargs = s.get_member_properties(j, ['facecolor']).to_dict()
-                        kwargs['color'] = kwargs['facecolor']
-                        del kwargs['facecolor']
-                        line = nodes[:, [members[0, j], members[1, j]]].transpose()
-                        vis = vispyscene.visuals.Tube(line, radius=.025, **kwargs)
-                        vis.parent = self.view.scene
+from typing import Sequence, Union
+
+from tnsgrt.structure import Structure
+from .plotter import Plotter
+
+from vispy import scene as vispyscene
+
+
+class VisPyPlotter(Plotter):
+    """
+    VisPy based structure plotter
+
+    :param camera: dict with camera settings
+    :param scene: dict with vispy scene settings
+    """
+
+    defaults = {
+        'plot_nodes': True,
+        'plot_members': True,
+        'node_marker': 'o',
+        'node_markersize': .05,
+        'node_linewidth': 2,
+        'node_linestyle': 'none',
+        'node_facecolor': (1, 1, 1),
+        'node_edgecolor': (1, 1, 1)
+    }
+
+    def __init__(self, camera=None, scene=None):
+
+        scene_kwargs = {
+            'keys': 'interactive',
+            'size': (600, 600)
+        }
+        if scene:
+            scene_kwargs.update(scene)
+
+        camera_kwargs = {
+            'fov': 0,
+            'scale_factor': 1
+        }
+        if camera:
+            camera_kwargs.update(camera if camera else {})
+
+        # Create canvas and view
+        self.canvas = vispyscene.SceneCanvas(**scene_kwargs)
+        self.view = self.canvas.central_widget.add_view()
+        self.view.camera = vispyscene.cameras.ArcballCamera(**camera_kwargs)
+
+    def get_canvas(self):
+        """
+        :return: vispy canvas 
+        """
+        return self.canvas
+
+    def plot(self, s: Union[Structure, Sequence[Structure]], **kwargs):
+
+        # loop if a sequence is given
+        if not isinstance(s, Structure):
+            for si in s:
+                self.plot(si, **kwargs)
+            return
+
+        # process options
+        defaults = VisPyPlotter.defaults.copy()
+        defaults.update(kwargs)
+
+        # plot nodes
+        nodes = s.nodes
+        if defaults['plot_nodes']:
+            # Create and show visual
+            vis = vispyscene.visuals.Markers(
+                pos=nodes.transpose(),
+                size=defaults['node_markersize'],
+                antialias=0,
+                face_color=defaults['node_facecolor'],
+                edge_color=defaults['node_edgecolor'],
+                edge_width=0,
+                scaling=True,
+                spherical=True,
+            )
+            vis.parent = self.view.scene
+
+        # plot members
+        members = s.members
+        if defaults['plot_members']:
+            for j in range(s.get_number_of_members()):
+                if s.member_properties.loc[j, 'visible']:
+                    if s.has_member_tag(j, 'string'):
+                        # plot strings as lines
+                        kwargs = s.get_member_properties(j, ['facecolor', 'linewidth']).to_dict()
+                        kwargs['color'] = kwargs['facecolor']
+                        del kwargs['facecolor']
+                        kwargs['width'] = kwargs['linewidth']
+                        del kwargs['linewidth']
+                        line = nodes[:, [members[0, j], members[1, j]]].transpose()
+                        vis = vispyscene.visuals.Line(line, **kwargs)
+                        vis.parent = self.view.scene
+                    else:
+                        # plot others as solid elements
+                        kwargs = s.get_member_properties(j, ['facecolor']).to_dict()
+                        kwargs['color'] = kwargs['facecolor']
+                        del kwargs['facecolor']
+                        line = nodes[:, [members[0, j], members[1, j]]].transpose()
+                        vis = vispyscene.visuals.Tube(line, radius=.025, **kwargs)
+                        vis.parent = self.view.scene
```

### Comparing `tnsgrt-0.3/tests/test_michell.py` & `tnsgrt-0.4/tests/test_michell.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import unittest
-
-import itertools
-from parameterized import parameterized
-
-from tnsgrt.michell import Michell
-
-
-class TestMichell(unittest.TestCase):
-
-    @parameterized.expand(itertools.product([4, 6, 12], [3, 4, 10, 12]))
-    def test_michell(self, p, q):
-        s = Michell(p, q=q)
-        # print(f'p = {p}, q = {q}')
-        self.assertEqual(s.get_number_of_nodes(), p*q+1)
-        # self.assertEqual(s.get_number_of_members(), p*(q+1)+2*p)
-        # self.assertEqual(set(s.member_tags.keys()), {'bar', 'string', 'vertical', 'top', 'bottom'})
-        #
-        # rho = 1
-        # alpha = np.pi/2-np.pi/p
-        # lambda_ = np.hstack((
-        #     rho * np.cos(np.pi/p) / np.cos(alpha - np.pi/p) * np.ones((p,)),
-        #     (1/rho) * np.cos(np.pi / p) / np.cos(alpha - np.pi/p) * np.ones((p,)),
-        #     np.ones((p,)),
-        #     -np.ones((p,))
-        # ))
-        # np.testing.assert_allclose(s.member_properties['lambda_'], lambda_)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+import itertools
+from parameterized import parameterized
+
+from tnsgrt.michell import Michell
+
+
+class TestMichell(unittest.TestCase):
+
+    @parameterized.expand(itertools.product([4, 6, 12], [3, 4, 10, 12], [0.5, 1, 1.5]))
+    def test_michell(self, p, q, radius):
+        s = Michell(p, q=q, radius=radius)
+        # print(f'p = {p}, q = {q}')
+        self.assertEqual(s.get_number_of_nodes(), p*q+1)
+        # self.assertEqual(s.get_number_of_members(), p*(q+1)+2*p)
+        # self.assertEqual(set(s.member_tags.keys()), {'bar', 'string', 'vertical', 'top', 'bottom'})
+        #
+        # rho = 1
+        # alpha = np.pi/2-np.pi/p
+        # lambda_ = np.hstack((
+        #     rho * np.cos(np.pi/p) / np.cos(alpha - np.pi/p) * np.ones((p,)),
+        #     (1/rho) * np.cos(np.pi / p) / np.cos(alpha - np.pi/p) * np.ones((p,)),
+        #     np.ones((p,)),
+        #     -np.ones((p,))
+        # ))
+        # np.testing.assert_allclose(s.member_properties['lambda_'], lambda_)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `tnsgrt-0.3/tests/test_snelson.py` & `tnsgrt-0.4/tests/test_snelson.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import unittest
-
-import itertools
-from parameterized import parameterized
-import numpy as np
-
-from tnsgrt.prism import Prism
-
-
-class TestSnelson(unittest.TestCase):
-
-    @parameterized.expand(itertools.product([3, 4, 6, 12], ['lp', 'analytic']))
-    def test_regular_prism(self, p, method='analytic'):
-        s = Prism(p, equilibrium_method=method)
-        self.assertEqual(s.get_number_of_members(), 4*p)
-        self.assertEqual(s.get_number_of_nodes(), 2*p)
-        self.assertEqual(set(s.member_tags.keys()), {'bar', 'string', 'vertical', 'top', 'bottom'})
-
-        rho = 1
-        alpha = np.pi/2-np.pi/p
-        lambda_ = np.hstack((
-            rho * np.cos(np.pi/p) / np.cos(alpha - np.pi/p) * np.ones((p,)),
-            (1/rho) * np.cos(np.pi / p) / np.cos(alpha - np.pi/p) * np.ones((p,)),
-            np.ones((p,)),
-            -np.ones((p,))
-        ))
-        np.testing.assert_allclose(s.member_properties['lambda_'], lambda_)
-
-    @parameterized.expand(itertools.product([3, 4, 6, 12], [0, .25, .5, 1], ['lp', 'analytic'], [1, 0.8, 1.2]))
-    def test_diagonal_prism(self, p, lb=0, equilibrium_method='analytic', rho=1):
-        alpha = (1-lb) * (np.pi/2 - np.pi/p) + lb * np.pi/2
-        s = Prism(p, top_radius=rho, bottom_radius=1, alpha=alpha, diagonal=True,
-                  equilibrium_method=equilibrium_method)
-        self.assertEqual(s.get_number_of_members(), 5 * p)
-        self.assertEqual(s.get_number_of_nodes(), 2 * p)
-        self.assertEqual(set(s.member_tags.keys()), {'bar', 'string', 'vertical', 'top', 'bottom', 'diagonal'})
-
-        lambda_ = np.hstack((
-            rho * np.cos(np.pi / p) / np.cos(alpha - np.pi / p) * np.ones((p,)),
-            (1 / rho) * np.cos(np.pi / p) / np.cos(alpha - np.pi / p) * np.ones((p,)),
-            2 * np.cos(alpha) * np.cos(np.pi / p) / np.cos(alpha - np.pi / p) * np.ones((p,)),
-            -np.cos(alpha + np.pi / p) / np.cos(alpha - np.pi / p) * np.ones((p,)),
-            -np.ones((p,))
-        ))
-        np.testing.assert_allclose(s.member_properties['lambda_'], lambda_, atol=1e-6, rtol=0)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+import itertools
+from parameterized import parameterized
+import numpy as np
+
+from tnsgrt.prism import Prism
+
+
+class TestSnelson(unittest.TestCase):
+
+    @parameterized.expand(itertools.product([3, 4, 6, 12], ['lp', 'analytic']))
+    def test_regular_prism(self, p, method='analytic'):
+        s = Prism(p, equilibrium_method=method)
+        self.assertEqual(s.get_number_of_members(), 4*p)
+        self.assertEqual(s.get_number_of_nodes(), 2*p)
+        self.assertEqual(set(s.member_tags.keys()), {'bar', 'string', 'vertical', 'top', 'bottom'})
+
+        rho = 1
+        alpha = np.pi/2-np.pi/p
+        lambda_ = np.hstack((
+            rho * np.cos(np.pi/p) / np.cos(alpha - np.pi/p) * np.ones((p,)),
+            (1/rho) * np.cos(np.pi / p) / np.cos(alpha - np.pi/p) * np.ones((p,)),
+            np.ones((p,)),
+            -np.ones((p,))
+        ))
+        np.testing.assert_allclose(s.member_properties['lambda_'], lambda_)
+
+    @parameterized.expand(itertools.product([3, 4, 6, 12], [0, .25, .5, 1], ['lp', 'analytic'], [1, 0.8, 1.2]))
+    def test_diagonal_prism(self, p, lb=0, equilibrium_method='analytic', rho=1):
+        alpha = (1-lb) * (np.pi/2 - np.pi/p) + lb * np.pi/2
+        s = Prism(p, top_radius=rho, bottom_radius=1, alpha=alpha, diagonal=True,
+                  equilibrium_method=equilibrium_method)
+        self.assertEqual(s.get_number_of_members(), 5 * p)
+        self.assertEqual(s.get_number_of_nodes(), 2 * p)
+        self.assertEqual(set(s.member_tags.keys()), {'bar', 'string', 'vertical', 'top', 'bottom', 'diagonal'})
+
+        lambda_ = np.hstack((
+            rho * np.cos(np.pi / p) / np.cos(alpha - np.pi / p) * np.ones((p,)),
+            (1 / rho) * np.cos(np.pi / p) / np.cos(alpha - np.pi / p) * np.ones((p,)),
+            2 * np.cos(alpha) * np.cos(np.pi / p) / np.cos(alpha - np.pi / p) * np.ones((p,)),
+            -np.cos(alpha + np.pi / p) / np.cos(alpha - np.pi / p) * np.ones((p,)),
+            -np.ones((p,))
+        ))
+        np.testing.assert_allclose(s.member_properties['lambda_'], lambda_, atol=1e-6, rtol=0)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `tnsgrt-0.3/tests/test_stiffness.py` & `tnsgrt-0.4/tests/test_stiffness.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-import unittest
-from typing import Optional
-
-import numpy as np
-
-from tnsgrt.prism import Prism
-from tnsgrt.stiffness import NodeConstraint
-
-
-class TestStiffness(unittest.TestCase):
-
-    def test_stiffness(self):
-        s = Prism(3)
-        S, F, v = s.stiffness()
-        d = S.eigs()[0]
-        # 6 rigid body nodes
-        self.assertEqual(np.count_nonzero(d < 1e-3), 6)
-        # 6 rigid body nodes + 1 soft node
-        self.assertEqual(np.count_nonzero(d < 1e6), 7)
-
-    def test_rigid_body_1(self):
-        s = Prism(3)
-        # calculate stiffness
-        S, F, v = s.stiffness(apply_rigid_body_constraint=True)
-        # calculate eigenvalues
-        d = S.eigs(k=6)[0]
-        # no rigid body nodes
-        self.assertEqual(np.count_nonzero(d < 1e-3), 0)
-        # 1 soft node
-        self.assertEqual(np.count_nonzero(d < 1e6), 1)
-
-    def test_eigenmodes(self):
-        s = Prism(3)
-        # calculate stiffness
-        S, F, v = s.stiffness(apply_rigid_body_constraint=True)
-        # eigenmodes
-        d = S.modes(k=6)[0]
-        # no rigid body nodes
-        self.assertEqual(np.count_nonzero(d < 1e-3), 0)
-        # 1 soft node
-        self.assertEqual(np.count_nonzero(d < 1e2), 1)
-
-    def test_node_constraint(self):
-
-        c = NodeConstraint()
-        self.assertEqual(c.dof, 0)
-        np.testing.assert_allclose(c.normal, np.eye(3))
-        self.assertEqual(c.basis, None)
-
-        c = NodeConstraint(np.array([[1, 0, 0]]))
-        self.assertEqual(c.dof, 2)
-        np.testing.assert_allclose(c.normal, np.array([[1, 0, 0]]))
-        np.testing.assert_allclose(c.basis, [[0, 0], [1, 0], [0, 1]])
-
-        c = NodeConstraint(np.array([[1, 0, 0], [0, 1, 0]]))
-        self.assertEqual(c.dof, 1)
-        np.testing.assert_allclose(c.normal, np.array([[1, 0, 0], [0, 1, 0]]))
-        np.testing.assert_allclose(c.basis, [[0], [0], [1]])
-
-        c = NodeConstraint(np.array([[1, 1, 0]]))
-        self.assertEqual(c.dof, 2)
-        np.testing.assert_allclose(c.normal, np.array([[-np.sqrt(2) / 2, -np.sqrt(2) / 2, 0]]))
-        np.testing.assert_allclose(c.basis, [[-np.sqrt(2) / 2, 0], [np.sqrt(2) / 2, 0], [0, 1]])
-
-        nodes = np.array([[1, 0], [0, 1], [0, 0]])
-        constraints = [None]*2
-        constraints[0] = NodeConstraint(np.array(([[1, 1, 0]])))
-        constraints[1] = NodeConstraint()
-
-        R, T = NodeConstraint.node_constraint(nodes, constraints, storage='full')
-        self.assertEqual(R.shape, (4, 6))
-        self.assertEqual(T.shape, (6, 2))
-
-        Rs, Ts = NodeConstraint.node_constraint(nodes, constraints)
-        self.assertEqual(Rs.shape, (4, 6))
-        self.assertEqual(Ts.shape, (6, 2))
-
-        np.testing.assert_equal(R, Rs.toarray())
-        np.testing.assert_equal(T, Ts.toarray())
-
-        self.assertTrue(np.linalg.norm((Rs @ Ts).toarray()) < 1e-6)
-        self.assertTrue(np.linalg.norm(Rs @ Rs.transpose() - np.eye(4)) < 1e-6)
-        self.assertTrue(np.linalg.norm(Ts.transpose() @ Ts - np.eye(2)) < 1e-6)
-
-        nodes = np.array([[1, 0, 1], [0, 1, 1], [0, 0, 1]])
-        constraints: list[Optional[NodeConstraint]] = [None]*3
-        constraints[0] = NodeConstraint(np.array(([[1, 1, 0]])))
-        constraints[2] = NodeConstraint()
-
-        R, T = NodeConstraint.node_constraint(nodes, constraints, storage='full')
-        self.assertEqual(R.shape, (4, 9))
-        self.assertEqual(T.shape, (9, 5))
-
-        Rs, Ts = NodeConstraint.node_constraint(nodes, constraints)
-        self.assertEqual(Rs.shape, (4, 9))
-        self.assertEqual(Ts.shape, (9, 5))
-
-        np.testing.assert_equal(R, Rs.toarray())
-        np.testing.assert_equal(T, Ts.toarray())
-
-        self.assertTrue(np.linalg.norm((Rs @ Ts).toarray()) < 1e-6)
-        self.assertTrue(np.linalg.norm(Rs @ Rs.transpose() - np.eye(4)) < 1e-6)
-        self.assertTrue(np.linalg.norm(Ts.transpose() @ Ts - np.eye(5)) < 1e-6)
-
-        nodes = np.array([[1, 0, 0, 0, 1], [0, 1, 0, 1, 1], [0, 0, 2, 1, 3]])
-        constraints: list[Optional[NodeConstraint]] = [None]*5
-        constraints[0] = NodeConstraint(np.array(([[1, 1, 0]])))
-        constraints[2] = NodeConstraint()
-
-        R, T = NodeConstraint.node_constraint(nodes, constraints, storage='full')
-        self.assertEqual(R.shape, (4, 15))
-        self.assertEqual(T.shape, (15, 11))
-
-        Rs, Ts = NodeConstraint.node_constraint(nodes, constraints)
-        self.assertEqual(Rs.shape, (4, 15))
-        self.assertEqual(Ts.shape, (15, 11))
-
-        np.testing.assert_equal(R, Rs.toarray())
-        np.testing.assert_equal(T, Ts.toarray())
-
-        self.assertTrue(np.linalg.norm((Rs @ Ts).toarray()) < 1e-6)
-        self.assertTrue(np.linalg.norm(Rs @ Rs.transpose() - np.eye(4)) < 1e-6)
-        self.assertTrue(np.linalg.norm(Ts.transpose() @ Ts - np.eye(11)) < 1e-6)
-
-    def test_rigid_body_2(self):
-
-        nodes = np.matrix([[0, 0, 0], [1, 0, 0], [0, 1, 0]]).transpose()
-        constraints = NodeConstraint.rigid_body_three_point_constraint(nodes)
-        self.assertEqual(constraints[0].dof, 0)
-        self.assertEqual(constraints[1].dof, 1)
-        np.testing.assert_allclose(constraints[1].normal, np.array([[0, 0, -1], [0, 1, 0]]))
-        self.assertEqual(constraints[2].dof, 2)
-        np.testing.assert_allclose(constraints[2].normal, np.array([[0, 0, -1]]))
-
-        R, T = NodeConstraint.node_constraint(nodes, constraints, storage='full')
-        self.assertEqual(R.shape, (6, 9))
-        self.assertEqual(T.shape, (9, 3))
-
-        Rs, Ts = NodeConstraint.node_constraint(nodes, constraints)
-        self.assertEqual(Rs.shape, (6, 9))
-        self.assertEqual(Ts.shape, (9, 3))
-
-        np.testing.assert_equal(R, Rs.toarray())
-        np.testing.assert_equal(T, Ts.toarray())
-
-    def test_rigid_body_3(self):
-
-        # create 3 prism
-        s = Prism(3)
-        # set rigid body constraint on 3 bottom nodes
-        s.node_properties.loc[:2, 'constraint'] = NodeConstraint.rigid_body_three_point_constraint(s.nodes[:, :3])
-        # calculate stiffness
-        S, F, v = s.stiffness()
-        # calculate eigenvalues
-        d = S.eigs(k=6)[0]
-        # no rigid body nodes
-        self.assertEqual(np.count_nonzero(d < 1e-3), 0)
-        # 1 soft node
-        self.assertEqual(np.count_nonzero(d < 1e6), 1)
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from typing import Optional
+
+import numpy as np
+
+from tnsgrt.prism import Prism
+from tnsgrt.stiffness import NodeConstraint
+
+
+class TestStiffness(unittest.TestCase):
+
+    def test_stiffness(self):
+        s = Prism(3)
+        S, F, v = s.stiffness()
+        d = S.eigs()[0]
+        # 6 rigid body nodes
+        self.assertEqual(np.count_nonzero(d < 1e-3), 6)
+        # 6 rigid body nodes + 1 soft node
+        self.assertEqual(np.count_nonzero(d < 1e6), 7)
+
+    def test_rigid_body_1(self):
+        s = Prism(3)
+        # calculate stiffness
+        S, F, v = s.stiffness(apply_rigid_body_constraint=True)
+        # calculate eigenvalues
+        d = S.eigs(k=6)[0]
+        # no rigid body nodes
+        self.assertEqual(np.count_nonzero(d < 1e-3), 0)
+        # 1 soft node
+        self.assertEqual(np.count_nonzero(d < 1e6), 1)
+
+    def test_eigenmodes(self):
+        s = Prism(3)
+        # calculate stiffness
+        S, F, v = s.stiffness(apply_rigid_body_constraint=True)
+        # eigenmodes
+        d = S.modes(k=6)[0]
+        # no rigid body nodes
+        self.assertEqual(np.count_nonzero(d < 1e-3), 0)
+        # 1 soft node
+        self.assertEqual(np.count_nonzero(d < 1e2), 1)
+
+    def test_node_constraint(self):
+
+        c = NodeConstraint()
+        self.assertEqual(c.dof, 0)
+        np.testing.assert_allclose(c.normal, np.eye(3))
+        self.assertEqual(c.basis, None)
+
+        c = NodeConstraint(np.array([[1, 0, 0]]))
+        self.assertEqual(c.dof, 2)
+        np.testing.assert_allclose(c.normal, np.array([[1, 0, 0]]))
+        np.testing.assert_allclose(c.basis, [[0, 0], [1, 0], [0, 1]])
+
+        c = NodeConstraint(np.array([[1, 0, 0], [0, 1, 0]]))
+        self.assertEqual(c.dof, 1)
+        np.testing.assert_allclose(c.normal, np.array([[1, 0, 0], [0, 1, 0]]))
+        np.testing.assert_allclose(c.basis, [[0], [0], [1]])
+
+        c = NodeConstraint(np.array([[1, 1, 0]]))
+        self.assertEqual(c.dof, 2)
+        np.testing.assert_allclose(c.normal, np.array([[-np.sqrt(2) / 2, -np.sqrt(2) / 2, 0]]))
+        np.testing.assert_allclose(c.basis, [[-np.sqrt(2) / 2, 0], [np.sqrt(2) / 2, 0], [0, 1]])
+
+        nodes = np.array([[1, 0], [0, 1], [0, 0]])
+        constraints = [None]*2
+        constraints[0] = NodeConstraint(np.array(([[1, 1, 0]])))
+        constraints[1] = NodeConstraint()
+
+        R, T = NodeConstraint.node_constraint(nodes, constraints, storage='full')
+        self.assertEqual(R.shape, (4, 6))
+        self.assertEqual(T.shape, (6, 2))
+
+        Rs, Ts = NodeConstraint.node_constraint(nodes, constraints)
+        self.assertEqual(Rs.shape, (4, 6))
+        self.assertEqual(Ts.shape, (6, 2))
+
+        np.testing.assert_equal(R, Rs.toarray())
+        np.testing.assert_equal(T, Ts.toarray())
+
+        self.assertTrue(np.linalg.norm((Rs @ Ts).toarray()) < 1e-6)
+        self.assertTrue(np.linalg.norm(Rs @ Rs.transpose() - np.eye(4)) < 1e-6)
+        self.assertTrue(np.linalg.norm(Ts.transpose() @ Ts - np.eye(2)) < 1e-6)
+
+        nodes = np.array([[1, 0, 1], [0, 1, 1], [0, 0, 1]])
+        constraints: list[Optional[NodeConstraint]] = [None]*3
+        constraints[0] = NodeConstraint(np.array(([[1, 1, 0]])))
+        constraints[2] = NodeConstraint()
+
+        R, T = NodeConstraint.node_constraint(nodes, constraints, storage='full')
+        self.assertEqual(R.shape, (4, 9))
+        self.assertEqual(T.shape, (9, 5))
+
+        Rs, Ts = NodeConstraint.node_constraint(nodes, constraints)
+        self.assertEqual(Rs.shape, (4, 9))
+        self.assertEqual(Ts.shape, (9, 5))
+
+        np.testing.assert_equal(R, Rs.toarray())
+        np.testing.assert_equal(T, Ts.toarray())
+
+        self.assertTrue(np.linalg.norm((Rs @ Ts).toarray()) < 1e-6)
+        self.assertTrue(np.linalg.norm(Rs @ Rs.transpose() - np.eye(4)) < 1e-6)
+        self.assertTrue(np.linalg.norm(Ts.transpose() @ Ts - np.eye(5)) < 1e-6)
+
+        nodes = np.array([[1, 0, 0, 0, 1], [0, 1, 0, 1, 1], [0, 0, 2, 1, 3]])
+        constraints: list[Optional[NodeConstraint]] = [None]*5
+        constraints[0] = NodeConstraint(np.array(([[1, 1, 0]])))
+        constraints[2] = NodeConstraint()
+
+        R, T = NodeConstraint.node_constraint(nodes, constraints, storage='full')
+        self.assertEqual(R.shape, (4, 15))
+        self.assertEqual(T.shape, (15, 11))
+
+        Rs, Ts = NodeConstraint.node_constraint(nodes, constraints)
+        self.assertEqual(Rs.shape, (4, 15))
+        self.assertEqual(Ts.shape, (15, 11))
+
+        np.testing.assert_equal(R, Rs.toarray())
+        np.testing.assert_equal(T, Ts.toarray())
+
+        self.assertTrue(np.linalg.norm((Rs @ Ts).toarray()) < 1e-6)
+        self.assertTrue(np.linalg.norm(Rs @ Rs.transpose() - np.eye(4)) < 1e-6)
+        self.assertTrue(np.linalg.norm(Ts.transpose() @ Ts - np.eye(11)) < 1e-6)
+
+    def test_rigid_body_2(self):
+
+        nodes = np.matrix([[0, 0, 0], [1, 0, 0], [0, 1, 0]]).transpose()
+        constraints = NodeConstraint.rigid_body_three_point_constraint(nodes)
+        self.assertEqual(constraints[0].dof, 0)
+        self.assertEqual(constraints[1].dof, 1)
+        np.testing.assert_allclose(constraints[1].normal, np.array([[0, 0, -1], [0, 1, 0]]))
+        self.assertEqual(constraints[2].dof, 2)
+        np.testing.assert_allclose(constraints[2].normal, np.array([[0, 0, -1]]))
+
+        R, T = NodeConstraint.node_constraint(nodes, constraints, storage='full')
+        self.assertEqual(R.shape, (6, 9))
+        self.assertEqual(T.shape, (9, 3))
+
+        Rs, Ts = NodeConstraint.node_constraint(nodes, constraints)
+        self.assertEqual(Rs.shape, (6, 9))
+        self.assertEqual(Ts.shape, (9, 3))
+
+        np.testing.assert_equal(R, Rs.toarray())
+        np.testing.assert_equal(T, Ts.toarray())
+
+    def test_rigid_body_3(self):
+
+        # create 3 prism
+        s = Prism(3)
+        # set rigid body constraint on 3 bottom nodes
+        s.node_properties.loc[:2, 'constraint'] = NodeConstraint.rigid_body_three_point_constraint(s.nodes[:, :3])
+        # calculate stiffness
+        S, F, v = s.stiffness()
+        # calculate eigenvalues
+        d = S.eigs(k=6)[0]
+        # no rigid body nodes
+        self.assertEqual(np.count_nonzero(d < 1e-3), 0)
+        # 1 soft node
+        self.assertEqual(np.count_nonzero(d < 1e6), 1)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `tnsgrt-0.3/tests/test_structure.py` & `tnsgrt-0.4/tests/test_structure.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,779 +1,779 @@
-import unittest
-
-import numpy as np
-import pandas as pd
-import scipy
-
-from tnsgrt import utils
-from tnsgrt.stiffness import NodeConstraint
-from tnsgrt.structure import Structure
-
-
-class TestStructure(unittest.TestCase):
-
-    def test_constructor(self):
-
-        # empty structure
-        s = Structure()
-        self.assertEqual(s.label, None)
-        np.testing.assert_array_equal(s.nodes, np.zeros((3, 0), np.float_))
-        self.assertEqual(len(s.node_properties), 0)
-        self.assertEqual(s.get_number_of_nodes(), 0)
-        self.assertEqual(s.node_tags, {})
-        self.assertEqual(len(s.member_properties), 0)
-        self.assertEqual(s.get_number_of_members(), 0)
-        np.testing.assert_array_equal(s.members, np.zeros((2, 0), np.uint64))
-        np.testing.assert_array_equal(s.member_tags['bar'], np.zeros((0,), np.uint64))
-        np.testing.assert_array_equal(s.member_tags['string'], np.zeros((0,), np.uint64))
-
-        nodes = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
-        s = Structure(nodes, label='label')
-        self.assertEqual(s.label, 'label')
-        self.assertEqual(s.nodes.dtype, np.float_)
-        self.assertEqual(s.members.dtype, np.uint64)
-        np.testing.assert_array_equal(s.nodes, nodes)
-        self.assertEqual(len(s.node_properties), 3)
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        self.assertEqual(s.node_tags, {})
-        np.testing.assert_array_equal(s.members, np.zeros((2, 0), np.uint64))
-        np.testing.assert_array_equal(s.member_tags['bar'], np.zeros((0,), np.uint64))
-        np.testing.assert_array_equal(s.member_tags['string'], np.zeros((0,), np.uint64))
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        self.assertEqual(s.get_number_of_members(), 0)
-        self.assertEqual(len(s.member_properties), 0)
-
-        members = np.array([[0, 1, 2], [1, 2, 0]])
-        s = Structure(nodes, members, label='label')
-        self.assertEqual(s.label, 'label')
-        self.assertEqual(s.nodes.dtype, np.float_)
-        self.assertEqual(s.members.dtype, np.uint64)
-        np.testing.assert_array_equal(s.nodes, nodes)
-        self.assertEqual(len(s.node_properties), 3)
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        self.assertEqual(s.node_tags, {})
-        np.testing.assert_array_equal(s.members, members)
-        np.testing.assert_array_equal(s.member_tags['bar'], np.arange(0, 3, dtype=np.uint64))
-        np.testing.assert_array_equal(s.member_tags['string'], np.zeros((0,), np.uint64))
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        self.assertEqual(s.get_number_of_members(), 3)
-        self.assertEqual(len(s.member_properties), 3)
-
-        s = Structure(nodes, members, number_of_strings=1)
-        self.assertEqual(s.label, None)
-        self.assertEqual(s.nodes.dtype, np.float_)
-        self.assertEqual(s.members.dtype, np.uint64)
-        np.testing.assert_array_equal(s.nodes, nodes)
-        self.assertEqual(len(s.node_properties), 3)
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        self.assertEqual(s.node_tags, {})
-        np.testing.assert_array_equal(s.members, members)
-        np.testing.assert_array_equal(s.member_tags['bar'], np.arange(1, 3, dtype=np.uint64))
-        np.testing.assert_array_equal(s.member_tags['string'], np.arange(0, 1, dtype=np.uint64))
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        self.assertEqual(s.get_number_of_members(), 3)
-        self.assertEqual(len(s.member_properties), 3)
-
-        s = Structure(nodes, members, number_of_strings=2)
-        self.assertEqual(s.label, None)
-        self.assertEqual(s.nodes.dtype, np.float_)
-        self.assertEqual(s.members.dtype, np.uint64)
-        np.testing.assert_array_equal(s.nodes, nodes)
-        self.assertEqual(len(s.node_properties), 3)
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        self.assertEqual(s.node_tags, {})
-        np.testing.assert_array_equal(s.members, members)
-        np.testing.assert_array_equal(s.member_tags['bar'], np.arange(2, 3, dtype=np.uint64))
-        np.testing.assert_array_equal(s.member_tags['string'], np.arange(0, 2, dtype=np.uint64))
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        self.assertEqual(s.get_number_of_members(), 3)
-        self.assertEqual(len(s.member_properties), 3)
-
-        member_defaults = Structure.member_defaults.copy()
-        Structure.member_defaults['vertical'] = {'linewidth': 1001, 'volume': 2}
-        s = Structure(nodes, members,
-                      member_tags={
-                          'bar': np.arange(1, 3, dtype=np.uint64),
-                          'string': np.arange(0, 1, dtype=np.uint64),
-                          'vertical': np.arange(2, 3, dtype=np.uint64)
-                      },
-                      node_tags={
-                          'bottom': np.array([0, 1], dtype=np.uint64),
-                          'top': np.array([2], dtype=np.uint64)
-                      })
-        self.assertEqual(s.label, None)
-        self.assertEqual(s.nodes.dtype, np.float_)
-        self.assertEqual(s.members.dtype, np.uint64)
-        np.testing.assert_array_equal(s.nodes, nodes)
-        self.assertEqual(len(s.node_properties), 3)
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        self.assertEqual(set(s.node_tags.keys()), {'bottom', 'top'})
-        np.testing.assert_array_equal(s.node_tags['bottom'], np.array([0, 1], dtype=np.uint64))
-        np.testing.assert_array_equal(s.node_tags['top'], np.array([2], dtype=np.uint64))
-        np.testing.assert_array_equal(s.members, members)
-        np.testing.assert_array_equal(s.member_tags['bar'], np.arange(1, 3, dtype=np.uint64))
-        np.testing.assert_array_equal(s.member_tags['string'], np.arange(0, 1, dtype=np.uint64))
-        np.testing.assert_array_equal(s.member_tags['vertical'], np.arange(2, 3, dtype=np.uint64))
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        self.assertEqual(s.get_number_of_members(), 3)
-        self.assertEqual(s.get_member_tags(0), ['string'])
-        self.assertEqual(s.get_member_tags(1), ['bar'])
-        self.assertEqual(s.get_member_tags(2), ['bar', 'vertical'])
-        self.assertTrue(s.has_member_tag(2, 'bar'))
-        self.assertTrue(s.has_member_tag(2, 'vertical'))
-        self.assertFalse(s.has_member_tag(1, 'vertical'))
-        np.testing.assert_array_equal(s.get_members_by_tags(['bar']), [1, 2])
-        np.testing.assert_array_equal(s.get_members_by_tags(['bar', 'vertical']), [2])
-        self.assertEqual(len(s.member_properties), 3)
-        self.assertEqual(s.member_properties.loc[1, 'linewidth'], 2)
-        self.assertEqual(s.member_properties.loc[2, 'linewidth'], 1001)
-        self.assertEqual(s.get_member_properties([1, 2], ['volume', 'mass']).to_dict('index'),
-                         {1: {'volume': 0., 'mass': 1.}, 2: {'volume': 2., 'mass': 1.}})
-        self.assertEqual(s.get_member_properties(2, ['volume', 'mass']).to_dict(), {'volume': 2., 'mass': 1.})
-        Structure.member_defaults = member_defaults
-
-    def test_get_set_member_properties(self):
-
-        nodes = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
-        members = np.array([[0, 1, 2], [1, 2, 0]])
-        s = Structure(nodes, members,
-                      member_tags={
-                          'bar': np.arange(1, 3, dtype=np.uint64),
-                          'string': np.arange(0, 1, dtype=np.uint64),
-                          'vertical': np.arange(2, 3, dtype=np.uint64)
-                      },
-                      node_tags={
-                          'bottom': np.array([0, 1], dtype=np.uint64),
-                          'top': np.array([2], dtype=np.uint64)
-                      })
-
-        properties = s.get_member_properties([1, 2], 'volume')
-        self.assertIsInstance(properties, pd.Series)
-        self.assertEqual(len(properties), 2)
-        np.testing.assert_array_equal(properties.values, [0, 0])
-
-        properties = s.get_member_properties(slice(None), 'volume')
-        self.assertIsInstance(properties, pd.Series)
-        self.assertEqual(len(properties), 3)
-
-        properties = s.get_member_properties([1, 2], 'facecolor')
-        self.assertIsInstance(properties, pd.Series)
-        self.assertEqual(len(properties), 2)
-
-        properties = s.get_member_properties(slice(None), 'facecolor')
-        self.assertIsInstance(properties, pd.Series)
-        self.assertEqual(len(properties), 3)
-
-        properties = s.get_member_properties([1, 2], ['volume', 'facecolor'])
-        self.assertIsInstance(properties, pd.DataFrame)
-        self.assertEqual(len(properties), 2)
-
-        properties = s.get_member_properties(slice(None), ['volume', 'facecolor'])
-        self.assertIsInstance(properties, pd.DataFrame)
-        self.assertEqual(len(properties), 3)
-
-        s.set_member_properties(2, 'volume', 3)
-        np.testing.assert_array_equal(s.member_properties['volume'].values, [0, 0, 3])
-
-        s.set_member_properties([1, 2], 'volume', [1, 2])
-        np.testing.assert_array_equal(s.member_properties['volume'].values, [0, 1, 2])
-
-        s.set_member_properties([1, 2], 'volume', 3)
-        np.testing.assert_array_equal(s.member_properties['volume'].values, [0, 3, 3])
-
-        s.set_member_properties([1, 2], 'volume', 1, wrap=True)
-        np.testing.assert_array_equal(s.member_properties['volume'].values, [0, 1, 1])
-
-        s.set_member_properties(2, 'facecolor', utils.Colors.BROWN.value, wrap=True)
-        self.assertEqual(s.member_properties['facecolor'].tolist(),
-                         [utils.Colors.ORANGE.value, utils.Colors.BLUE.value, utils.Colors.BROWN.value])
-
-        s.set_member_properties([1, 2], 'facecolor', utils.Colors.GREEN.value, wrap=True)
-        self.assertEqual(s.member_properties['facecolor'].tolist(),
-                         [utils.Colors.ORANGE.value, utils.Colors.GREEN.value, utils.Colors.GREEN.value])
-
-        s.set_member_properties([1, 2], 'facecolor', [utils.Colors.BLUE.value, utils.Colors.ORANGE.value],
-                                wrap=True, scalar=False)
-        self.assertEqual(s.member_properties['facecolor'].tolist(),
-                         [utils.Colors.ORANGE.value, utils.Colors.BLUE.value, utils.Colors.ORANGE.value])
-
-
-    def test_add_members_and_add_nodes(self):
-
-        nodes1 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
-        members1 = np.array([[0, 1, 2], [1, 2, 0]])
-        s = Structure(nodes1, members1,
-                      member_tags={
-                          'bar': np.arange(1, 3, dtype=np.uint64),
-                          'string': np.arange(0, 1, dtype=np.uint64),
-                          'vertical': np.arange(2, 3, dtype=np.uint64)
-                      })
-        members2 = s.get_number_of_nodes() + np.array([[0], [1]])
-        nodes2 = np.array([[1, 0], [1, 1], [0, 1]])
-        s.add_nodes(nodes2, node_tags={
-            'bottom': np.array([0], dtype=np.uint64),
-            'top': np.array([1], dtype=np.uint64)
-        })
-        s.add_members(members2, number_of_strings=1)
-
-        self.assertEqual(s.get_number_of_nodes(), 5)
-        self.assertEqual(len(s.node_properties), 5)
-        self.assertEqual(set(s.node_tags.keys()), {'bottom', 'top'})
-        np.testing.assert_array_equal(s.node_tags['bottom'], np.array([3], dtype=np.uint64))
-        np.testing.assert_array_equal(s.node_tags['top'], np.array([4], dtype=np.uint64))
-        self.assertEqual(s.get_number_of_members(), 4)
-        self.assertEqual(set(s.member_tags.keys()), {'bar', 'string', 'vertical'})
-        np.testing.assert_array_equal(s.member_tags['bar'], [1, 2])
-        np.testing.assert_array_equal(s.member_tags['string'], [0, 3])
-        np.testing.assert_array_equal(s.member_tags['vertical'], [2])
-        np.testing.assert_array_equal(s.members, [[0, 1, 2, 3], [1, 2, 0, 4]])
-        np.testing.assert_array_equal(s.nodes, [[1, 0, 0, 1, 0], [0, 1, 0, 1, 1], [0, 0, 1, 0, 1]])
-        np.testing.assert_array_equal(s.member_properties.index, np.arange(4))
-
-    def test_copy(self):
-
-        nodes = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
-        members = np.array([[0, 1, 2], [1, 2, 0]])
-        member_defaults = Structure.member_defaults.copy()
-        Structure.member_defaults['vertical'] = {'linewidth': 1001, 'volume': 2}
-        s = Structure(nodes, members,
-                      member_tags={
-                          'bar': np.arange(1, 3, dtype=np.uint64),
-                          'string': np.arange(0, 1, dtype=np.uint64),
-                          'vertical': np.arange(2, 3, dtype=np.uint64)
-                      },
-                      node_tags={
-                          'bottom': np.array([0, 1], dtype=np.uint64),
-                          'top': np.array([2], dtype=np.uint64)
-                      }, label='label')
-
-        self.assertEqual(s.label, 'label')
-        self.assertEqual(s.nodes.dtype, np.float_)
-        self.assertEqual(s.members.dtype, np.uint64)
-        np.testing.assert_array_equal(s.nodes, nodes)
-        self.assertEqual(len(s.node_properties), 3)
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        self.assertEqual(set(s.node_tags.keys()), {'bottom', 'top'})
-        np.testing.assert_array_equal(s.node_tags['bottom'], np.array([0, 1], dtype=np.uint64))
-        np.testing.assert_array_equal(s.node_tags['top'], np.array([2], dtype=np.uint64))
-        np.testing.assert_array_equal(s.members, members)
-        np.testing.assert_array_equal(s.member_tags['bar'], np.arange(1, 3, dtype=np.uint64))
-        np.testing.assert_array_equal(s.member_tags['string'], np.arange(0, 1, dtype=np.uint64))
-        np.testing.assert_array_equal(s.member_tags['vertical'], np.arange(2, 3, dtype=np.uint64))
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        self.assertEqual(s.get_number_of_members(), 3)
-        self.assertEqual(s.get_member_tags(0), ['string'])
-        self.assertEqual(s.get_member_tags(1), ['bar'])
-        self.assertEqual(s.get_member_tags(2), ['bar', 'vertical'])
-        self.assertTrue(s.has_member_tag(2, 'bar'))
-        self.assertTrue(s.has_member_tag(2, 'vertical'))
-        self.assertFalse(s.has_member_tag(1, 'vertical'))
-        np.testing.assert_array_equal(s.get_members_by_tags(['bar']), [1, 2])
-        np.testing.assert_array_equal(s.get_members_by_tags(['bar', 'vertical']), [2])
-        self.assertEqual(len(s.member_properties), 3)
-        self.assertEqual(s.member_properties.loc[1, 'linewidth'], 2)
-        self.assertEqual(s.member_properties.loc[2, 'linewidth'], 1001)
-        self.assertEqual(s.get_member_properties([1, 2], ['volume', 'mass']).to_dict('index'),
-                         {1: {'volume': 0., 'mass': 1.}, 2: {'volume': 2., 'mass': 1.}})
-        self.assertEqual(s.get_member_properties(2, ['volume', 'mass']).to_dict(), {'volume': 2., 'mass': 1.})
-
-        copy = s.copy()
-
-        self.assertEqual(copy.label, 'label')
-        self.assertEqual(copy.nodes.dtype, np.float_)
-        self.assertEqual(copy.members.dtype, np.uint64)
-        np.testing.assert_array_equal(copy.nodes, nodes)
-        self.assertEqual(len(copy.node_properties), 3)
-        self.assertEqual(copy.get_number_of_nodes(), 3)
-        self.assertEqual(set(copy.node_tags.keys()), {'bottom', 'top'})
-        np.testing.assert_array_equal(copy.node_tags['bottom'], np.array([0, 1], dtype=np.uint64))
-        np.testing.assert_array_equal(copy.node_tags['top'], np.array([2], dtype=np.uint64))
-        np.testing.assert_array_equal(copy.members, members)
-        np.testing.assert_array_equal(copy.member_tags['bar'], np.arange(1, 3, dtype=np.uint64))
-        np.testing.assert_array_equal(copy.member_tags['string'], np.arange(0, 1, dtype=np.uint64))
-        np.testing.assert_array_equal(copy.member_tags['vertical'], np.arange(2, 3, dtype=np.uint64))
-        self.assertEqual(copy.get_number_of_nodes(), 3)
-        self.assertEqual(copy.get_number_of_members(), 3)
-        self.assertEqual(copy.get_member_tags(0), ['string'])
-        self.assertEqual(copy.get_member_tags(1), ['bar'])
-        self.assertEqual(copy.get_member_tags(2), ['bar', 'vertical'])
-        self.assertTrue(copy.has_member_tag(2, 'bar'))
-        self.assertTrue(copy.has_member_tag(2, 'vertical'))
-        self.assertFalse(copy.has_member_tag(1, 'vertical'))
-        np.testing.assert_array_equal(copy.get_members_by_tags(['bar']), [1, 2])
-        np.testing.assert_array_equal(copy.get_members_by_tags(['bar', 'vertical']), [2])
-        self.assertEqual(len(copy.member_properties), 3)
-        self.assertEqual(copy.member_properties.loc[1, 'linewidth'], 2)
-        self.assertEqual(copy.member_properties.loc[2, 'linewidth'], 1001)
-        self.assertEqual(copy.get_member_properties([1, 2], ['volume', 'mass']).to_dict('index'),
-                         {1: {'volume': 0., 'mass': 1.}, 2: {'volume': 2., 'mass': 1.}})
-        self.assertEqual(copy.get_member_properties(2, ['volume', 'mass']).to_dict(), {'volume': 2., 'mass': 1.})
-
-        Structure.member_defaults = member_defaults
-
-    def test_merge(self):
-
-        nodes1 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
-        members1 = np.array([[0, 1, 2], [1, 2, 0]])
-        s1 = Structure(nodes1, members1,
-                       member_tags={
-                           'bar': np.arange(1, 3, dtype=np.uint64),
-                           'string': np.arange(0, 1, dtype=np.uint64),
-                           'vertical': np.arange(2, 3, dtype=np.uint64)
-                       },
-                       node_tags={
-                           'bottom': np.array([0, 1], dtype=np.uint64),
-                           'top': np.array([2], dtype=np.uint64)
-                       })
-
-        nodes2 = np.array([[1, 0], [1, 1], [0, 1]])
-        members2 = np.array([[0], [1]])
-        s2 = Structure(nodes2, members2, number_of_strings=1)
-
-        s1.merge(s2, inplace=True)
-
-        self.assertEqual(s1.get_number_of_nodes(), 5)
-        self.assertEqual(len(s1.node_properties), 5)
-        self.assertEqual(set(s1.node_tags.keys()), {'bottom', 'top'})
-        np.testing.assert_array_equal(s1.node_tags['bottom'], np.array([0, 1], dtype=np.uint64))
-        np.testing.assert_array_equal(s1.node_tags['top'], np.array([2], dtype=np.uint64))
-        self.assertEqual(s1.get_number_of_members(), 4)
-        self.assertEqual(set(s1.member_tags.keys()), {'bar', 'string', 'vertical'})
-        np.testing.assert_array_equal(s1.member_tags['bar'], [1, 2])
-        np.testing.assert_array_equal(s1.member_tags['string'], [0, 3])
-        np.testing.assert_array_equal(s1.member_tags['vertical'], [2])
-        np.testing.assert_array_equal(s1.members, [[0, 1, 2, 3], [1, 2, 0, 4]])
-        np.testing.assert_array_equal(s1.nodes, [[1, 0, 0, 1, 0], [0, 1, 0, 1, 1], [0, 0, 1, 0, 1]])
-        np.testing.assert_array_equal(s1.member_properties.index, np.arange(4))
-
-        # nodes1 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
-        # members1 = np.array([[0, 1, 2], [1, 2, 0]])
-        s1 = Structure(nodes1, members1,
-                       member_tags={
-                           'bar': np.arange(1, 3, dtype=np.uint64),
-                           'string': np.arange(0, 1, dtype=np.uint64),
-                           'vertical': np.arange(2, 3, dtype=np.uint64)
-                       },
-                       node_tags={
-                           'bottom': np.array([0, 1], dtype=np.uint64),
-                           'top': np.array([2], dtype=np.uint64)
-                       })
-
-        # nodes2 = np.array([[1, 0], [1, 1], [0, 1]])
-        # members2 = np.array([[0], [1]])
-        s2 = Structure(nodes2, members2, number_of_strings=1)
-
-        s2.merge(s1, inplace=True)
-        self.assertEqual(s2.get_number_of_nodes(), 5)
-        self.assertEqual(len(s2.node_properties), 5)
-        self.assertEqual(set(s2.node_tags.keys()), {'bottom', 'top'})
-        np.testing.assert_array_equal(s2.node_tags['bottom'], np.array([2, 3], dtype=np.uint64))
-        np.testing.assert_array_equal(s2.node_tags['top'], np.array([4], dtype=np.uint64))
-        self.assertEqual(s2.get_number_of_members(), 4)
-        self.assertEqual(set(s2.member_tags.keys()), {'bar', 'string', 'vertical'})
-        np.testing.assert_array_equal(s2.member_tags['bar'], [2, 3])
-        np.testing.assert_array_equal(s2.member_tags['string'], [0, 1])
-        np.testing.assert_array_equal(s2.member_tags['vertical'], [3])
-        np.testing.assert_array_equal(s2.members, [[0, 2, 3, 4], [1, 3, 4, 2]])
-        np.testing.assert_array_equal(s2.nodes, [[1, 0, 1, 0, 0], [1, 1, 0, 1, 0], [0, 1, 0, 0, 1]])
-        np.testing.assert_array_equal(s2.member_properties.index, np.arange(4))
-
-        s1 = Structure(nodes1, members1,
-                       member_tags={
-                           'bar': np.arange(1, 3, dtype=np.uint64),
-                           'string': np.arange(0, 1, dtype=np.uint64),
-                           'vertical': np.arange(2, 3, dtype=np.uint64)
-                       },
-                       node_tags={
-                           'bottom': np.array([0, 1], dtype=np.uint64),
-                           'top': np.array([2], dtype=np.uint64)
-                       })
-
-        # nodes2 = np.array([[1, 0], [1, 1], [0, 1]])
-        # members2 = np.array([[0], [1]])
-        s2 = Structure(nodes2, members2, number_of_strings=1)
-
-        s = s1.merge(s2)
-
-        self.assertFalse(s is s1)
-        self.assertFalse(s is s2)
-        self.assertEqual(s.get_number_of_nodes(), 5)
-        self.assertEqual(len(s.node_properties), 5)
-        self.assertEqual(set(s.node_tags.keys()), {'bottom', 'top'})
-        np.testing.assert_array_equal(s.node_tags['bottom'], np.array([0, 1], dtype=np.uint64))
-        np.testing.assert_array_equal(s.node_tags['top'], np.array([2], dtype=np.uint64))
-        self.assertEqual(s.get_number_of_members(), 4)
-        self.assertEqual(set(s.member_tags.keys()), {'bar', 'string', 'vertical'})
-        np.testing.assert_array_equal(s.member_tags['bar'], [1, 2])
-        np.testing.assert_array_equal(s.member_tags['string'], [0, 3])
-        np.testing.assert_array_equal(s.member_tags['vertical'], [2])
-        np.testing.assert_array_equal(s.members, [[0, 1, 2, 3], [1, 2, 0, 4]])
-        np.testing.assert_array_equal(s.nodes, [[1, 0, 0, 1, 0], [0, 1, 0, 1, 1], [0, 0, 1, 0, 1]])
-        np.testing.assert_array_equal(s.member_properties.index, np.arange(4))
-
-    def test_length_com_cog_translate(self):
-
-        nodes1 = np.array([[1, 0, 0, 0], [0, 1, 0, 1], [0, 0, 2, 1]])
-        members1 = np.array([[0, 1, 2, 3], [1, 2, 0, 0]])
-        s = Structure(nodes1, members1, number_of_strings=2)
-
-        # test get member length
-        np.testing.assert_array_equal(s.get_member_length(),
-                                      [np.linalg.norm(nodes1[:, 1]-nodes1[:, 0]),
-                                       np.linalg.norm(nodes1[:, 2]-nodes1[:, 1]),
-                                       np.linalg.norm(nodes1[:, 0]-nodes1[:, 2]),
-                                       np.linalg.norm(nodes1[:, 3]-nodes1[:, 0])])
-
-        # test center of mass
-        np.testing.assert_array_equal(s.get_center_of_mass(),
-                                      (nodes1[:, 1] + nodes1[:, 0] + nodes1[:, 2] + nodes1[:, 1] +
-                                       nodes1[:, 0] + nodes1[:, 2] + nodes1[:, 3] + nodes1[:, 0])/8)
-
-        # test center of gravity
-        np.testing.assert_array_equal(s.get_centroid(),
-                                      (nodes1[:, 0] + nodes1[:, 1] + nodes1[:, 2] + nodes1[:, 3])/4)
-
-    def test_rotate(self):
-
-        nodes1 = np.array([[1, 0, 0, 0], [0, 1, 0, 1], [0, 0, 2, 1]])
-        members1 = np.array([[0, 1, 2, 3], [1, 2, 0, 0]])
-        s = Structure(nodes1, members1, number_of_strings=2)
-
-        v = np.array([1, 1, 1])
-        s.rotate(v)
-        R = scipy.spatial.transform.Rotation.from_rotvec(v)
-        np.testing.assert_array_equal(s.nodes, R.apply(nodes1.transpose()).transpose())
-
-    def test_reflect(self):
-
-        nodes1 = np.array([[1, 0, 0, 0], [0, 1, 0, 1], [0, 0, 2, 1]])
-        members1 = np.array([[0, 1, 2, 3], [1, 2, 0, 0]])
-        s = Structure(nodes1, members1, number_of_strings=2)
-
-        v = np.array([1, 1, 1])
-        s.reflect(v)
-        H = np.eye(3) - 2 * np.outer(v, v)/(np.linalg.norm(v)**2)
-        np.testing.assert_array_equal(s.nodes, H @ nodes1)
-
-        s.set_nodes(nodes1)
-        p = np.array([1, -1, 2])
-        s.reflect(v, p)
-        p = p.reshape((3, 1))
-        np.testing.assert_array_equal(s.nodes, (H @ (nodes1 - p)) + p)
-
-    def test_remove_nodes(self):
-
-        nodes1 = np.array([[1, 0, 0, 0], [0, 1, 0, 1], [0, 0, 2, 1]])
-        nodes1_tags = {'tags': np.array([0, 2, 3], dtype=np.uint64)}
-        members1 = np.array([[0, 1, 2], [1, 2, 0]])
-        s = Structure(nodes1, members1, number_of_strings=2, node_tags=nodes1_tags)
-
-        np.testing.assert_array_equal(s.get_unused_nodes(), [3])
-        self.assertTrue(s.has_unused_nodes())
-
-        s.remove_nodes([3])
-        np.testing.assert_array_equal(s.nodes, nodes1[:, :3])
-        self.assertEqual(len(s.node_properties), 3)
-        np.testing.assert_array_equal(s.node_properties.index, np.arange(3))
-        np.testing.assert_array_equal(s.members, members1)
-        np.testing.assert_array_equal(s.node_tags['tags'], [0, 2])
-        self.assertFalse(s.has_unused_nodes())
-
-        members2 = np.array([[0, 1, 3], [1, 3, 0]])
-        s = Structure(nodes1, members2, number_of_strings=2, node_tags=nodes1_tags)
-
-        np.testing.assert_array_equal(s.get_unused_nodes(), [2])
-        self.assertTrue(s.has_unused_nodes())
-
-        s.remove_nodes([2])
-        np.testing.assert_array_equal(s.nodes, nodes1[:, [0, 1, 3]])
-        self.assertEqual(len(s.node_properties), 3)
-        np.testing.assert_array_equal(s.node_properties.index, np.arange(3))
-        np.testing.assert_array_equal(s.node_tags['tags'], [0, 2])
-        np.testing.assert_array_equal(s.members, members1)
-
-        members3 = np.array([[0, 3], [3, 0]])
-        s = Structure(nodes1, members3, number_of_strings=2, node_tags=nodes1_tags)
-
-        np.testing.assert_array_equal(s.get_unused_nodes(), [1, 2])
-        self.assertTrue(s.has_unused_nodes())
-
-        s.remove_nodes([1, 2])
-        np.testing.assert_array_equal(s.nodes, nodes1[:, [0, 3]])
-        np.testing.assert_array_equal(s.members, np.array([[0, 1], [1, 0]]))
-        np.testing.assert_array_equal(s.node_tags['tags'], [0, 1])
-        self.assertFalse(s.has_unused_nodes())
-
-        members4 = np.array([[1, 3], [3, 1]])
-        s = Structure(nodes1, members4, number_of_strings=2, node_tags=nodes1_tags)
-
-        np.testing.assert_array_equal(s.get_unused_nodes(), [0, 2])
-        self.assertTrue(s.has_unused_nodes())
-
-        s.remove_nodes([0, 2])
-        np.testing.assert_array_equal(s.nodes, nodes1[:, [1, 3]])
-        self.assertEqual(len(s.node_properties), 2)
-        np.testing.assert_array_equal(s.node_properties.index, np.arange(2))
-        np.testing.assert_array_equal(s.members, np.array([[0, 1], [1, 0]]))
-        np.testing.assert_array_equal(s.node_tags['tags'], [1])
-        self.assertFalse(s.has_unused_nodes())
-
-        # has used nodes
-        s = Structure(nodes1, members1, number_of_strings=2, node_tags=nodes1_tags)
-
-        np.testing.assert_array_equal(s.get_unused_nodes(), [3])
-        self.assertTrue(s.has_unused_nodes())
-
-        with self.assertWarns(Warning):
-            s.remove_nodes([2, 3])
-
-        np.testing.assert_array_equal(s.nodes, nodes1[:, :3])
-        self.assertEqual(len(s.node_properties), 3)
-        np.testing.assert_array_equal(s.node_properties.index, np.arange(3))
-        np.testing.assert_array_equal(s.members, members1)
-        np.testing.assert_array_equal(s.node_tags['tags'], [0, 2])
-        self.assertFalse(s.has_unused_nodes())
-
-        s = Structure(nodes1, members1, number_of_strings=2, node_tags=nodes1_tags)
-
-        np.testing.assert_array_equal(s.get_unused_nodes(), [3])
-        self.assertTrue(s.has_unused_nodes())
-
-        with self.assertWarns(Warning):
-            s.remove_nodes([1, 2])
-
-        np.testing.assert_array_equal(s.nodes, nodes1)
-        self.assertEqual(len(s.node_properties), 4)
-        np.testing.assert_array_equal(s.node_properties.index, np.arange(4))
-        np.testing.assert_array_equal(s.members, members1)
-        np.testing.assert_array_equal(s.node_tags['tags'], [0, 2, 3])
-        self.assertTrue(s.has_unused_nodes())
-
-        # None as parameter
-
-        members3 = np.array([[0, 3], [3, 0]])
-        s = Structure(nodes1, members3, number_of_strings=2, node_tags=nodes1_tags)
-
-        np.testing.assert_array_equal(s.get_unused_nodes(), [1, 2])
-        self.assertTrue(s.has_unused_nodes())
-
-        s.remove_nodes()
-        np.testing.assert_array_equal(s.nodes, nodes1[:, [0, 3]])
-        self.assertEqual(len(s.node_properties), 2)
-        np.testing.assert_array_equal(s.node_properties.index, np.arange(2))
-        np.testing.assert_array_equal(s.members, np.array([[0, 1], [1, 0]]))
-        np.testing.assert_array_equal(s.node_tags['tags'], [0, 1])
-        self.assertFalse(s.has_unused_nodes())
-
-    def test_remove_members(self):
-
-        nodes = np.array([[1, 0, 0, 0], [0, 1, 0, 1], [0, 0, 2, 1]])
-        nodes_tags = {'tags': np.array([0, 2, 3], dtype=np.uint64)}
-        members = np.array([[0, 1, 2], [1, 2, 0]])
-        members_tag = {'mtag': np.array([0, 2], dtype=np.uint64)}
-
-        s = Structure(nodes, members, number_of_strings=2, node_tags=nodes_tags, member_tags=members_tag)
-
-        s.remove_members([2])
-        np.testing.assert_array_equal(s.nodes, nodes)
-        self.assertEqual(len(s.node_properties), 4)
-        np.testing.assert_array_equal(s.members, members[:, :2])
-        np.testing.assert_array_equal(s.member_tags['mtag'], [0])
-
-        s = Structure(nodes, members, number_of_strings=2, node_tags=nodes_tags, member_tags=members_tag)
-
-        s.remove_members([0, 1])
-        np.testing.assert_array_equal(s.nodes, nodes)
-        self.assertEqual(len(s.node_properties), 4)
-        np.testing.assert_array_equal(s.members, members[:, [2]])
-        np.testing.assert_array_equal(s.member_tags['mtag'], [0])
-
-        s = Structure(nodes, members, number_of_strings=2, node_tags=nodes_tags, member_tags=members_tag)
-
-        s.remove_members([1, 2])
-        np.testing.assert_array_equal(s.nodes, nodes)
-        self.assertEqual(len(s.node_properties), 4)
-        np.testing.assert_array_equal(s.members, members[:, [0]])
-        np.testing.assert_array_equal(s.member_tags['mtag'], [0])
-
-    def test_close_node(self):
-
-        nodes1 = np.array([[1, 0, 0, 0], [0, 1, 0, 1], [0, 0, 2, 1]])
-        members1 = np.array([[0, 1, 2], [1, 2, 0]])
-        s = Structure(nodes1, members1, number_of_strings=2)
-        merge, merge_map = s.get_close_nodes()
-        self.assertFalse(merge)
-
-        s.merge_close_nodes()
-        self.assertEqual(s.get_number_of_nodes(), 4)
-        np.testing.assert_array_equal(s.nodes, nodes1)
-        np.testing.assert_array_equal(s.members, members1)
-
-        nodes1 = np.array([[1, 0, 0, 1], [0, 1, 0, 0], [0, 0, 2, 0]])
-        members1 = np.array([[0, 1, 2, 3], [1, 2, 0, 1]])
-        s = Structure(nodes1, members1, number_of_strings=2)
-        merge, merge_map = s.get_close_nodes()
-        self.assertEqual(merge, {3})
-        np.testing.assert_array_equal(merge_map, [0, 1, 2, 0])
-
-        s.merge_close_nodes()
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        np.testing.assert_array_equal(s.nodes, nodes1[:, :3])
-        np.testing.assert_array_equal(s.members, np.array([[0, 1, 2, 0], [1, 2, 0, 1]]))
-
-        nodes1 = np.array([[1, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 2]])
-        members1 = np.array([[0, 1, 2, 3], [1, 2, 0, 1]])
-        s = Structure(nodes1, members1, number_of_strings=2)
-        merge, merge_map = s.get_close_nodes()
-        self.assertEqual(merge, {2})
-        np.testing.assert_array_equal(merge_map, [0, 1, 0, 3])
-
-        s.merge_close_nodes()
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        np.testing.assert_array_equal(s.nodes, nodes1[:, [0, 1, 3]])
-        np.testing.assert_array_equal(s.members, np.array([[0, 1, 0, 2], [1, 0, 0, 1]]))
-
-        radius = 0.1
-        nodes1 = np.array([[1, 0, 0, 1, 1], [0, 1, 0, 0, 0], [0, 0, 2, .9*radius, 1.8*radius]])
-        members1 = np.array([[0, 1, 2, 3, 2], [1, 2, 0, 1, 4]])
-        s = Structure(nodes1, members1, number_of_strings=2)
-        merge, merge_map = s.get_close_nodes(radius)
-        self.assertEqual(merge, {3, 4})
-        np.testing.assert_array_equal(merge_map, [0, 1, 2, 0, 0])
-
-        s.merge_close_nodes(radius)
-        self.assertEqual(s.get_number_of_nodes(), 3)
-        np.testing.assert_array_equal(s.nodes, nodes1[:, :3])
-        np.testing.assert_array_equal(s.members, np.array([[0, 1, 2, 0, 2], [1, 2, 0, 1, 0]]))
-
-    def test_equilibrium_update_member_properties(self):
-
-        nodes = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0]])
-        members = np.array([[0, 1], [1, 2], [2, 0], [0, 3], [1, 3], [2, 3]]).transpose()
-        s0 = Structure(nodes, members)
-
-        center = s0.get_centroid()
-        s0.add_nodes(center.reshape((3, 1)))
-
-        s1 = s0.copy()
-
-        members = np.array([[0, 4], [1, 4], [2, 4]]).transpose()
-        s1.add_members(members, number_of_strings=3)
-
-        # won't be in equilibrium with only three strings
-        self.assertRaises(Exception, s1.equilibrium)
-
-        s1 = s0.copy()
-
-        members = np.array([[0, 4], [1, 4], [2, 4], [3, 4]]).transpose()
-        s1.add_members(members, number_of_strings=4)
-
-        # equilibrium
-        s1.equilibrium()
-
-        # set properties
-        s1.update_member_properties()
-
-        # forces
-        force = np.hstack((np.kron(np.array([-np.sqrt(2), -1, np.sqrt(11)]), np.ones((3,))), [np.sqrt(3)]))
-        np.testing.assert_allclose(s1.member_properties['force'], force)
-
-        lambda_ = np.hstack((np.kron(np.array([-1, -1, 4]), np.ones((3,))), [4]))
-        np.testing.assert_allclose(s1.member_properties['lambda_'], lambda_)
-
-        mass = np.hstack((157./200. * np.ones((6,)), 157./200./4 * np.ones((4,))))
-        np.testing.assert_allclose(s1.member_properties['mass'] / s1.get_member_length() / np.pi,
-                                   mass)
-
-        volume = np.hstack((np.ones((6,)), 1/4 * np.ones((4,))))
-        np.testing.assert_allclose(10000 * s1.member_properties['volume'] / s1.get_member_length() / np.pi,
-                                   volume)
-
-        np.testing.assert_allclose(s1.member_properties['stiffness'],
-                                   np.pi * s1.member_properties['modulus'] * (s1.member_properties['radius']**2 -
-                                                                              s1.member_properties['inner_radius']**2)
-                                   / s1.get_member_length())
-
-        np.testing.assert_allclose(s1.member_properties['rest_length'],
-                                   s1.get_member_length() * (1 - s1.member_properties['lambda_'].values
-                                                             / s1.member_properties['stiffness']))
-
-    def test_node_tags(self):
-
-        nodes = np.array([[1, 0, 0, 0, 1], [0, 1, 0, 1, 1], [0, 0, 2, 1, 3]])
-        nodes_tags = {
-            'nags0': np.array([0, 3], dtype=np.uint64),
-            'nags1': np.array([1, 2], dtype=np.uint64)
-        }
-        members = np.array([[0, 1, 2, 3], [1, 2, 0, 4]])
-        members_tag = {
-            'mags0': np.array([0], dtype=np.uint64),
-            'mags1': np.array([1, 2], dtype=np.uint64)
-        }
-        s = Structure(nodes, members, number_of_strings=2, node_tags=nodes_tags, member_tags=members_tag)
-
-        s.set_node_tag('nags2', [0, 3])
-        np.testing.assert_array_equal(s.node_tags['nags2'], [0, 3])
-
-        s.add_node_tag('nags1', [3])
-        np.testing.assert_array_equal(s.node_tags['nags1'], [1, 2, 3])
-
-        s.remove_node_tag('nags1', [2])
-        np.testing.assert_array_equal(s.node_tags['nags1'], [1, 3])
-
-        s.delete_node_tag('nags1')
-        self.assertFalse('nags1' in s.node_tags)
-
-    def test_member_tags(self):
-
-        nodes = np.array([[1, 0, 0, 0, 1], [0, 1, 0, 1, 1], [0, 0, 2, 1, 3]])
-        nodes_tags = {
-            'nags0': np.array([0, 3], dtype=np.uint64),
-            'nags1': np.array([1, 2], dtype=np.uint64)
-        }
-        members = np.array([[0, 1, 2, 3], [1, 2, 0, 4]])
-        members_tag = {
-            'mags0': np.array([0], dtype=np.uint64),
-            'mags1': np.array([1, 2], dtype=np.uint64)
-        }
-        s = Structure(nodes, members, number_of_strings=2, node_tags=nodes_tags, member_tags=members_tag)
-
-        s.set_member_tag('mags2', [0, 3])
-        np.testing.assert_array_equal(s.member_tags['mags2'], [0, 3])
-
-        s.add_member_tag('mags1', [3])
-        np.testing.assert_array_equal(s.member_tags['mags1'], [1, 2, 3])
-
-        s.remove_member_tag('mags1', [2])
-        np.testing.assert_array_equal(s.member_tags['mags1'], [1, 3])
-
-        s.delete_member_tag('mags1')
-        self.assertFalse('mags1' in s.member_tags)
-
-    def test_node_constraint(self):
-
-        nodes = np.array([[1, 0, 0, 0, 1], [0, 1, 0, 1, 1], [0, 0, 2, 1, 3]])
-        nodes_tags = {
-            'nags0': np.array([0, 3], dtype=np.uint64),
-            'nags1': np.array([1, 2], dtype=np.uint64)
-        }
-        members = np.array([[0, 1, 2, 3], [1, 2, 0, 4]])
-        members_tag = {
-            'mags0': np.array([0], dtype=np.uint64),
-            'mags1': np.array([1, 2], dtype=np.uint64)
-        }
-        s = Structure(nodes, members, number_of_strings=2, node_tags=nodes_tags, member_tags=members_tag)
-        s.node_properties.loc[2, 'constraint'] = NodeConstraint()
-        s.node_properties.loc[0, 'constraint'] = NodeConstraint(np.array(([[1, 1, 0]])))
-
-        # print(s.node_properties.loc[2, 'constraint'])
-        # print(s.node_properties.loc[2, 'constraint'].__class__)
-        # print(s.node_properties.loc[0, 'constraint'])
-        # print(s.node_properties.loc[0, 'constraint'].__class__)
-
-        R, T = NodeConstraint.node_constraint(s.nodes, s.node_properties['constraint'])
-        self.assertEqual(R.shape, (4, 15))
-        self.assertEqual(T.shape, (15, 11))
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+import numpy as np
+import pandas as pd
+import scipy
+
+from tnsgrt import utils
+from tnsgrt.stiffness import NodeConstraint
+from tnsgrt.structure import Structure
+
+
+class TestStructure(unittest.TestCase):
+
+    def test_constructor(self):
+
+        # empty structure
+        s = Structure()
+        self.assertEqual(s.label, None)
+        np.testing.assert_array_equal(s.nodes, np.zeros((3, 0), np.float_))
+        self.assertEqual(len(s.node_properties), 0)
+        self.assertEqual(s.get_number_of_nodes(), 0)
+        self.assertEqual(s.node_tags, {})
+        self.assertEqual(len(s.member_properties), 0)
+        self.assertEqual(s.get_number_of_members(), 0)
+        np.testing.assert_array_equal(s.members, np.zeros((2, 0), np.uint64))
+        np.testing.assert_array_equal(s.member_tags['bar'], np.zeros((0,), np.uint64))
+        np.testing.assert_array_equal(s.member_tags['string'], np.zeros((0,), np.uint64))
+
+        nodes = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
+        s = Structure(nodes, label='label')
+        self.assertEqual(s.label, 'label')
+        self.assertEqual(s.nodes.dtype, np.float_)
+        self.assertEqual(s.members.dtype, np.uint64)
+        np.testing.assert_array_equal(s.nodes, nodes)
+        self.assertEqual(len(s.node_properties), 3)
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        self.assertEqual(s.node_tags, {})
+        np.testing.assert_array_equal(s.members, np.zeros((2, 0), np.uint64))
+        np.testing.assert_array_equal(s.member_tags['bar'], np.zeros((0,), np.uint64))
+        np.testing.assert_array_equal(s.member_tags['string'], np.zeros((0,), np.uint64))
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        self.assertEqual(s.get_number_of_members(), 0)
+        self.assertEqual(len(s.member_properties), 0)
+
+        members = np.array([[0, 1, 2], [1, 2, 0]])
+        s = Structure(nodes, members, label='label')
+        self.assertEqual(s.label, 'label')
+        self.assertEqual(s.nodes.dtype, np.float_)
+        self.assertEqual(s.members.dtype, np.uint64)
+        np.testing.assert_array_equal(s.nodes, nodes)
+        self.assertEqual(len(s.node_properties), 3)
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        self.assertEqual(s.node_tags, {})
+        np.testing.assert_array_equal(s.members, members)
+        np.testing.assert_array_equal(s.member_tags['bar'], np.arange(0, 3, dtype=np.uint64))
+        np.testing.assert_array_equal(s.member_tags['string'], np.zeros((0,), np.uint64))
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        self.assertEqual(s.get_number_of_members(), 3)
+        self.assertEqual(len(s.member_properties), 3)
+
+        s = Structure(nodes, members, number_of_strings=1)
+        self.assertEqual(s.label, None)
+        self.assertEqual(s.nodes.dtype, np.float_)
+        self.assertEqual(s.members.dtype, np.uint64)
+        np.testing.assert_array_equal(s.nodes, nodes)
+        self.assertEqual(len(s.node_properties), 3)
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        self.assertEqual(s.node_tags, {})
+        np.testing.assert_array_equal(s.members, members)
+        np.testing.assert_array_equal(s.member_tags['bar'], np.arange(1, 3, dtype=np.uint64))
+        np.testing.assert_array_equal(s.member_tags['string'], np.arange(0, 1, dtype=np.uint64))
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        self.assertEqual(s.get_number_of_members(), 3)
+        self.assertEqual(len(s.member_properties), 3)
+
+        s = Structure(nodes, members, number_of_strings=2)
+        self.assertEqual(s.label, None)
+        self.assertEqual(s.nodes.dtype, np.float_)
+        self.assertEqual(s.members.dtype, np.uint64)
+        np.testing.assert_array_equal(s.nodes, nodes)
+        self.assertEqual(len(s.node_properties), 3)
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        self.assertEqual(s.node_tags, {})
+        np.testing.assert_array_equal(s.members, members)
+        np.testing.assert_array_equal(s.member_tags['bar'], np.arange(2, 3, dtype=np.uint64))
+        np.testing.assert_array_equal(s.member_tags['string'], np.arange(0, 2, dtype=np.uint64))
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        self.assertEqual(s.get_number_of_members(), 3)
+        self.assertEqual(len(s.member_properties), 3)
+
+        member_defaults = Structure.member_defaults.copy()
+        Structure.member_defaults['vertical'] = {'linewidth': 1001, 'volume': 2}
+        s = Structure(nodes, members,
+                      member_tags={
+                          'bar': np.arange(1, 3, dtype=np.uint64),
+                          'string': np.arange(0, 1, dtype=np.uint64),
+                          'vertical': np.arange(2, 3, dtype=np.uint64)
+                      },
+                      node_tags={
+                          'bottom': np.array([0, 1], dtype=np.uint64),
+                          'top': np.array([2], dtype=np.uint64)
+                      })
+        self.assertEqual(s.label, None)
+        self.assertEqual(s.nodes.dtype, np.float_)
+        self.assertEqual(s.members.dtype, np.uint64)
+        np.testing.assert_array_equal(s.nodes, nodes)
+        self.assertEqual(len(s.node_properties), 3)
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        self.assertEqual(set(s.node_tags.keys()), {'bottom', 'top'})
+        np.testing.assert_array_equal(s.node_tags['bottom'], np.array([0, 1], dtype=np.uint64))
+        np.testing.assert_array_equal(s.node_tags['top'], np.array([2], dtype=np.uint64))
+        np.testing.assert_array_equal(s.members, members)
+        np.testing.assert_array_equal(s.member_tags['bar'], np.arange(1, 3, dtype=np.uint64))
+        np.testing.assert_array_equal(s.member_tags['string'], np.arange(0, 1, dtype=np.uint64))
+        np.testing.assert_array_equal(s.member_tags['vertical'], np.arange(2, 3, dtype=np.uint64))
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        self.assertEqual(s.get_number_of_members(), 3)
+        self.assertEqual(s.get_member_tags(0), ['string'])
+        self.assertEqual(s.get_member_tags(1), ['bar'])
+        self.assertEqual(s.get_member_tags(2), ['bar', 'vertical'])
+        self.assertTrue(s.has_member_tag(2, 'bar'))
+        self.assertTrue(s.has_member_tag(2, 'vertical'))
+        self.assertFalse(s.has_member_tag(1, 'vertical'))
+        np.testing.assert_array_equal(s.get_members_by_tags(['bar']), [1, 2])
+        np.testing.assert_array_equal(s.get_members_by_tags(['bar', 'vertical']), [2])
+        self.assertEqual(len(s.member_properties), 3)
+        self.assertEqual(s.member_properties.loc[1, 'linewidth'], 2)
+        self.assertEqual(s.member_properties.loc[2, 'linewidth'], 1001)
+        self.assertEqual(s.get_member_properties([1, 2], ['volume', 'mass']).to_dict('index'),
+                         {1: {'volume': 0., 'mass': 1.}, 2: {'volume': 2., 'mass': 1.}})
+        self.assertEqual(s.get_member_properties(2, ['volume', 'mass']).to_dict(), {'volume': 2., 'mass': 1.})
+        Structure.member_defaults = member_defaults
+
+    def test_get_set_member_properties(self):
+
+        nodes = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
+        members = np.array([[0, 1, 2], [1, 2, 0]])
+        s = Structure(nodes, members,
+                      member_tags={
+                          'bar': np.arange(1, 3, dtype=np.uint64),
+                          'string': np.arange(0, 1, dtype=np.uint64),
+                          'vertical': np.arange(2, 3, dtype=np.uint64)
+                      },
+                      node_tags={
+                          'bottom': np.array([0, 1], dtype=np.uint64),
+                          'top': np.array([2], dtype=np.uint64)
+                      })
+
+        properties = s.get_member_properties([1, 2], 'volume')
+        self.assertIsInstance(properties, pd.Series)
+        self.assertEqual(len(properties), 2)
+        np.testing.assert_array_equal(properties.values, [0, 0])
+
+        properties = s.get_member_properties(slice(None), 'volume')
+        self.assertIsInstance(properties, pd.Series)
+        self.assertEqual(len(properties), 3)
+
+        properties = s.get_member_properties([1, 2], 'facecolor')
+        self.assertIsInstance(properties, pd.Series)
+        self.assertEqual(len(properties), 2)
+
+        properties = s.get_member_properties(slice(None), 'facecolor')
+        self.assertIsInstance(properties, pd.Series)
+        self.assertEqual(len(properties), 3)
+
+        properties = s.get_member_properties([1, 2], ['volume', 'facecolor'])
+        self.assertIsInstance(properties, pd.DataFrame)
+        self.assertEqual(len(properties), 2)
+
+        properties = s.get_member_properties(slice(None), ['volume', 'facecolor'])
+        self.assertIsInstance(properties, pd.DataFrame)
+        self.assertEqual(len(properties), 3)
+
+        s.set_member_properties(2, 'volume', 3)
+        np.testing.assert_array_equal(s.member_properties['volume'].values, [0, 0, 3])
+
+        s.set_member_properties([1, 2], 'volume', [1, 2])
+        np.testing.assert_array_equal(s.member_properties['volume'].values, [0, 1, 2])
+
+        s.set_member_properties([1, 2], 'volume', 3)
+        np.testing.assert_array_equal(s.member_properties['volume'].values, [0, 3, 3])
+
+        s.set_member_properties([1, 2], 'volume', 1, wrap=True)
+        np.testing.assert_array_equal(s.member_properties['volume'].values, [0, 1, 1])
+
+        s.set_member_properties(2, 'facecolor', utils.Colors.BROWN.value, wrap=True)
+        self.assertEqual(s.member_properties['facecolor'].tolist(),
+                         [utils.Colors.ORANGE.value, utils.Colors.BLUE.value, utils.Colors.BROWN.value])
+
+        s.set_member_properties([1, 2], 'facecolor', utils.Colors.GREEN.value, wrap=True)
+        self.assertEqual(s.member_properties['facecolor'].tolist(),
+                         [utils.Colors.ORANGE.value, utils.Colors.GREEN.value, utils.Colors.GREEN.value])
+
+        s.set_member_properties([1, 2], 'facecolor', [utils.Colors.BLUE.value, utils.Colors.ORANGE.value],
+                                wrap=True, scalar=False)
+        self.assertEqual(s.member_properties['facecolor'].tolist(),
+                         [utils.Colors.ORANGE.value, utils.Colors.BLUE.value, utils.Colors.ORANGE.value])
+
+
+    def test_add_members_and_add_nodes(self):
+
+        nodes1 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
+        members1 = np.array([[0, 1, 2], [1, 2, 0]])
+        s = Structure(nodes1, members1,
+                      member_tags={
+                          'bar': np.arange(1, 3, dtype=np.uint64),
+                          'string': np.arange(0, 1, dtype=np.uint64),
+                          'vertical': np.arange(2, 3, dtype=np.uint64)
+                      })
+        members2 = s.get_number_of_nodes() + np.array([[0], [1]])
+        nodes2 = np.array([[1, 0], [1, 1], [0, 1]])
+        s.add_nodes(nodes2, node_tags={
+            'bottom': np.array([0], dtype=np.uint64),
+            'top': np.array([1], dtype=np.uint64)
+        })
+        s.add_members(members2, number_of_strings=1)
+
+        self.assertEqual(s.get_number_of_nodes(), 5)
+        self.assertEqual(len(s.node_properties), 5)
+        self.assertEqual(set(s.node_tags.keys()), {'bottom', 'top'})
+        np.testing.assert_array_equal(s.node_tags['bottom'], np.array([3], dtype=np.uint64))
+        np.testing.assert_array_equal(s.node_tags['top'], np.array([4], dtype=np.uint64))
+        self.assertEqual(s.get_number_of_members(), 4)
+        self.assertEqual(set(s.member_tags.keys()), {'bar', 'string', 'vertical'})
+        np.testing.assert_array_equal(s.member_tags['bar'], [1, 2])
+        np.testing.assert_array_equal(s.member_tags['string'], [0, 3])
+        np.testing.assert_array_equal(s.member_tags['vertical'], [2])
+        np.testing.assert_array_equal(s.members, [[0, 1, 2, 3], [1, 2, 0, 4]])
+        np.testing.assert_array_equal(s.nodes, [[1, 0, 0, 1, 0], [0, 1, 0, 1, 1], [0, 0, 1, 0, 1]])
+        np.testing.assert_array_equal(s.member_properties.index, np.arange(4))
+
+    def test_copy(self):
+
+        nodes = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
+        members = np.array([[0, 1, 2], [1, 2, 0]])
+        member_defaults = Structure.member_defaults.copy()
+        Structure.member_defaults['vertical'] = {'linewidth': 1001, 'volume': 2}
+        s = Structure(nodes, members,
+                      member_tags={
+                          'bar': np.arange(1, 3, dtype=np.uint64),
+                          'string': np.arange(0, 1, dtype=np.uint64),
+                          'vertical': np.arange(2, 3, dtype=np.uint64)
+                      },
+                      node_tags={
+                          'bottom': np.array([0, 1], dtype=np.uint64),
+                          'top': np.array([2], dtype=np.uint64)
+                      }, label='label')
+
+        self.assertEqual(s.label, 'label')
+        self.assertEqual(s.nodes.dtype, np.float_)
+        self.assertEqual(s.members.dtype, np.uint64)
+        np.testing.assert_array_equal(s.nodes, nodes)
+        self.assertEqual(len(s.node_properties), 3)
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        self.assertEqual(set(s.node_tags.keys()), {'bottom', 'top'})
+        np.testing.assert_array_equal(s.node_tags['bottom'], np.array([0, 1], dtype=np.uint64))
+        np.testing.assert_array_equal(s.node_tags['top'], np.array([2], dtype=np.uint64))
+        np.testing.assert_array_equal(s.members, members)
+        np.testing.assert_array_equal(s.member_tags['bar'], np.arange(1, 3, dtype=np.uint64))
+        np.testing.assert_array_equal(s.member_tags['string'], np.arange(0, 1, dtype=np.uint64))
+        np.testing.assert_array_equal(s.member_tags['vertical'], np.arange(2, 3, dtype=np.uint64))
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        self.assertEqual(s.get_number_of_members(), 3)
+        self.assertEqual(s.get_member_tags(0), ['string'])
+        self.assertEqual(s.get_member_tags(1), ['bar'])
+        self.assertEqual(s.get_member_tags(2), ['bar', 'vertical'])
+        self.assertTrue(s.has_member_tag(2, 'bar'))
+        self.assertTrue(s.has_member_tag(2, 'vertical'))
+        self.assertFalse(s.has_member_tag(1, 'vertical'))
+        np.testing.assert_array_equal(s.get_members_by_tags(['bar']), [1, 2])
+        np.testing.assert_array_equal(s.get_members_by_tags(['bar', 'vertical']), [2])
+        self.assertEqual(len(s.member_properties), 3)
+        self.assertEqual(s.member_properties.loc[1, 'linewidth'], 2)
+        self.assertEqual(s.member_properties.loc[2, 'linewidth'], 1001)
+        self.assertEqual(s.get_member_properties([1, 2], ['volume', 'mass']).to_dict('index'),
+                         {1: {'volume': 0., 'mass': 1.}, 2: {'volume': 2., 'mass': 1.}})
+        self.assertEqual(s.get_member_properties(2, ['volume', 'mass']).to_dict(), {'volume': 2., 'mass': 1.})
+
+        copy = s.copy()
+
+        self.assertEqual(copy.label, 'label')
+        self.assertEqual(copy.nodes.dtype, np.float_)
+        self.assertEqual(copy.members.dtype, np.uint64)
+        np.testing.assert_array_equal(copy.nodes, nodes)
+        self.assertEqual(len(copy.node_properties), 3)
+        self.assertEqual(copy.get_number_of_nodes(), 3)
+        self.assertEqual(set(copy.node_tags.keys()), {'bottom', 'top'})
+        np.testing.assert_array_equal(copy.node_tags['bottom'], np.array([0, 1], dtype=np.uint64))
+        np.testing.assert_array_equal(copy.node_tags['top'], np.array([2], dtype=np.uint64))
+        np.testing.assert_array_equal(copy.members, members)
+        np.testing.assert_array_equal(copy.member_tags['bar'], np.arange(1, 3, dtype=np.uint64))
+        np.testing.assert_array_equal(copy.member_tags['string'], np.arange(0, 1, dtype=np.uint64))
+        np.testing.assert_array_equal(copy.member_tags['vertical'], np.arange(2, 3, dtype=np.uint64))
+        self.assertEqual(copy.get_number_of_nodes(), 3)
+        self.assertEqual(copy.get_number_of_members(), 3)
+        self.assertEqual(copy.get_member_tags(0), ['string'])
+        self.assertEqual(copy.get_member_tags(1), ['bar'])
+        self.assertEqual(copy.get_member_tags(2), ['bar', 'vertical'])
+        self.assertTrue(copy.has_member_tag(2, 'bar'))
+        self.assertTrue(copy.has_member_tag(2, 'vertical'))
+        self.assertFalse(copy.has_member_tag(1, 'vertical'))
+        np.testing.assert_array_equal(copy.get_members_by_tags(['bar']), [1, 2])
+        np.testing.assert_array_equal(copy.get_members_by_tags(['bar', 'vertical']), [2])
+        self.assertEqual(len(copy.member_properties), 3)
+        self.assertEqual(copy.member_properties.loc[1, 'linewidth'], 2)
+        self.assertEqual(copy.member_properties.loc[2, 'linewidth'], 1001)
+        self.assertEqual(copy.get_member_properties([1, 2], ['volume', 'mass']).to_dict('index'),
+                         {1: {'volume': 0., 'mass': 1.}, 2: {'volume': 2., 'mass': 1.}})
+        self.assertEqual(copy.get_member_properties(2, ['volume', 'mass']).to_dict(), {'volume': 2., 'mass': 1.})
+
+        Structure.member_defaults = member_defaults
+
+    def test_merge(self):
+
+        nodes1 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
+        members1 = np.array([[0, 1, 2], [1, 2, 0]])
+        s1 = Structure(nodes1, members1,
+                       member_tags={
+                           'bar': np.arange(1, 3, dtype=np.uint64),
+                           'string': np.arange(0, 1, dtype=np.uint64),
+                           'vertical': np.arange(2, 3, dtype=np.uint64)
+                       },
+                       node_tags={
+                           'bottom': np.array([0, 1], dtype=np.uint64),
+                           'top': np.array([2], dtype=np.uint64)
+                       })
+
+        nodes2 = np.array([[1, 0], [1, 1], [0, 1]])
+        members2 = np.array([[0], [1]])
+        s2 = Structure(nodes2, members2, number_of_strings=1)
+
+        s1.merge(s2, inplace=True)
+
+        self.assertEqual(s1.get_number_of_nodes(), 5)
+        self.assertEqual(len(s1.node_properties), 5)
+        self.assertEqual(set(s1.node_tags.keys()), {'bottom', 'top'})
+        np.testing.assert_array_equal(s1.node_tags['bottom'], np.array([0, 1], dtype=np.uint64))
+        np.testing.assert_array_equal(s1.node_tags['top'], np.array([2], dtype=np.uint64))
+        self.assertEqual(s1.get_number_of_members(), 4)
+        self.assertEqual(set(s1.member_tags.keys()), {'bar', 'string', 'vertical'})
+        np.testing.assert_array_equal(s1.member_tags['bar'], [1, 2])
+        np.testing.assert_array_equal(s1.member_tags['string'], [0, 3])
+        np.testing.assert_array_equal(s1.member_tags['vertical'], [2])
+        np.testing.assert_array_equal(s1.members, [[0, 1, 2, 3], [1, 2, 0, 4]])
+        np.testing.assert_array_equal(s1.nodes, [[1, 0, 0, 1, 0], [0, 1, 0, 1, 1], [0, 0, 1, 0, 1]])
+        np.testing.assert_array_equal(s1.member_properties.index, np.arange(4))
+
+        # nodes1 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]])
+        # members1 = np.array([[0, 1, 2], [1, 2, 0]])
+        s1 = Structure(nodes1, members1,
+                       member_tags={
+                           'bar': np.arange(1, 3, dtype=np.uint64),
+                           'string': np.arange(0, 1, dtype=np.uint64),
+                           'vertical': np.arange(2, 3, dtype=np.uint64)
+                       },
+                       node_tags={
+                           'bottom': np.array([0, 1], dtype=np.uint64),
+                           'top': np.array([2], dtype=np.uint64)
+                       })
+
+        # nodes2 = np.array([[1, 0], [1, 1], [0, 1]])
+        # members2 = np.array([[0], [1]])
+        s2 = Structure(nodes2, members2, number_of_strings=1)
+
+        s2.merge(s1, inplace=True)
+        self.assertEqual(s2.get_number_of_nodes(), 5)
+        self.assertEqual(len(s2.node_properties), 5)
+        self.assertEqual(set(s2.node_tags.keys()), {'bottom', 'top'})
+        np.testing.assert_array_equal(s2.node_tags['bottom'], np.array([2, 3], dtype=np.uint64))
+        np.testing.assert_array_equal(s2.node_tags['top'], np.array([4], dtype=np.uint64))
+        self.assertEqual(s2.get_number_of_members(), 4)
+        self.assertEqual(set(s2.member_tags.keys()), {'bar', 'string', 'vertical'})
+        np.testing.assert_array_equal(s2.member_tags['bar'], [2, 3])
+        np.testing.assert_array_equal(s2.member_tags['string'], [0, 1])
+        np.testing.assert_array_equal(s2.member_tags['vertical'], [3])
+        np.testing.assert_array_equal(s2.members, [[0, 2, 3, 4], [1, 3, 4, 2]])
+        np.testing.assert_array_equal(s2.nodes, [[1, 0, 1, 0, 0], [1, 1, 0, 1, 0], [0, 1, 0, 0, 1]])
+        np.testing.assert_array_equal(s2.member_properties.index, np.arange(4))
+
+        s1 = Structure(nodes1, members1,
+                       member_tags={
+                           'bar': np.arange(1, 3, dtype=np.uint64),
+                           'string': np.arange(0, 1, dtype=np.uint64),
+                           'vertical': np.arange(2, 3, dtype=np.uint64)
+                       },
+                       node_tags={
+                           'bottom': np.array([0, 1], dtype=np.uint64),
+                           'top': np.array([2], dtype=np.uint64)
+                       })
+
+        # nodes2 = np.array([[1, 0], [1, 1], [0, 1]])
+        # members2 = np.array([[0], [1]])
+        s2 = Structure(nodes2, members2, number_of_strings=1)
+
+        s = s1.merge(s2)
+
+        self.assertFalse(s is s1)
+        self.assertFalse(s is s2)
+        self.assertEqual(s.get_number_of_nodes(), 5)
+        self.assertEqual(len(s.node_properties), 5)
+        self.assertEqual(set(s.node_tags.keys()), {'bottom', 'top'})
+        np.testing.assert_array_equal(s.node_tags['bottom'], np.array([0, 1], dtype=np.uint64))
+        np.testing.assert_array_equal(s.node_tags['top'], np.array([2], dtype=np.uint64))
+        self.assertEqual(s.get_number_of_members(), 4)
+        self.assertEqual(set(s.member_tags.keys()), {'bar', 'string', 'vertical'})
+        np.testing.assert_array_equal(s.member_tags['bar'], [1, 2])
+        np.testing.assert_array_equal(s.member_tags['string'], [0, 3])
+        np.testing.assert_array_equal(s.member_tags['vertical'], [2])
+        np.testing.assert_array_equal(s.members, [[0, 1, 2, 3], [1, 2, 0, 4]])
+        np.testing.assert_array_equal(s.nodes, [[1, 0, 0, 1, 0], [0, 1, 0, 1, 1], [0, 0, 1, 0, 1]])
+        np.testing.assert_array_equal(s.member_properties.index, np.arange(4))
+
+    def test_length_com_cog_translate(self):
+
+        nodes1 = np.array([[1, 0, 0, 0], [0, 1, 0, 1], [0, 0, 2, 1]])
+        members1 = np.array([[0, 1, 2, 3], [1, 2, 0, 0]])
+        s = Structure(nodes1, members1, number_of_strings=2)
+
+        # test get member length
+        np.testing.assert_array_equal(s.get_member_length(),
+                                      [np.linalg.norm(nodes1[:, 1]-nodes1[:, 0]),
+                                       np.linalg.norm(nodes1[:, 2]-nodes1[:, 1]),
+                                       np.linalg.norm(nodes1[:, 0]-nodes1[:, 2]),
+                                       np.linalg.norm(nodes1[:, 3]-nodes1[:, 0])])
+
+        # test center of mass
+        np.testing.assert_array_equal(s.get_center_of_mass(),
+                                      (nodes1[:, 1] + nodes1[:, 0] + nodes1[:, 2] + nodes1[:, 1] +
+                                       nodes1[:, 0] + nodes1[:, 2] + nodes1[:, 3] + nodes1[:, 0])/8)
+
+        # test center of gravity
+        np.testing.assert_array_equal(s.get_centroid(),
+                                      (nodes1[:, 0] + nodes1[:, 1] + nodes1[:, 2] + nodes1[:, 3])/4)
+
+    def test_rotate(self):
+
+        nodes1 = np.array([[1, 0, 0, 0], [0, 1, 0, 1], [0, 0, 2, 1]])
+        members1 = np.array([[0, 1, 2, 3], [1, 2, 0, 0]])
+        s = Structure(nodes1, members1, number_of_strings=2)
+
+        v = np.array([1, 1, 1])
+        s.rotate(v)
+        R = scipy.spatial.transform.Rotation.from_rotvec(v)
+        np.testing.assert_array_equal(s.nodes, R.apply(nodes1.transpose()).transpose())
+
+    def test_reflect(self):
+
+        nodes1 = np.array([[1, 0, 0, 0], [0, 1, 0, 1], [0, 0, 2, 1]])
+        members1 = np.array([[0, 1, 2, 3], [1, 2, 0, 0]])
+        s = Structure(nodes1, members1, number_of_strings=2)
+
+        v = np.array([1, 1, 1])
+        s.reflect(v)
+        H = np.eye(3) - 2 * np.outer(v, v)/(np.linalg.norm(v)**2)
+        np.testing.assert_array_equal(s.nodes, H @ nodes1)
+
+        s.set_nodes(nodes1)
+        p = np.array([1, -1, 2])
+        s.reflect(v, p)
+        p = p.reshape((3, 1))
+        np.testing.assert_array_equal(s.nodes, (H @ (nodes1 - p)) + p)
+
+    def test_remove_nodes(self):
+
+        nodes1 = np.array([[1, 0, 0, 0], [0, 1, 0, 1], [0, 0, 2, 1]])
+        nodes1_tags = {'tags': np.array([0, 2, 3], dtype=np.uint64)}
+        members1 = np.array([[0, 1, 2], [1, 2, 0]])
+        s = Structure(nodes1, members1, number_of_strings=2, node_tags=nodes1_tags)
+
+        np.testing.assert_array_equal(s.get_unused_nodes(), [3])
+        self.assertTrue(s.has_unused_nodes())
+
+        s.remove_nodes([3])
+        np.testing.assert_array_equal(s.nodes, nodes1[:, :3])
+        self.assertEqual(len(s.node_properties), 3)
+        np.testing.assert_array_equal(s.node_properties.index, np.arange(3))
+        np.testing.assert_array_equal(s.members, members1)
+        np.testing.assert_array_equal(s.node_tags['tags'], [0, 2])
+        self.assertFalse(s.has_unused_nodes())
+
+        members2 = np.array([[0, 1, 3], [1, 3, 0]])
+        s = Structure(nodes1, members2, number_of_strings=2, node_tags=nodes1_tags)
+
+        np.testing.assert_array_equal(s.get_unused_nodes(), [2])
+        self.assertTrue(s.has_unused_nodes())
+
+        s.remove_nodes([2])
+        np.testing.assert_array_equal(s.nodes, nodes1[:, [0, 1, 3]])
+        self.assertEqual(len(s.node_properties), 3)
+        np.testing.assert_array_equal(s.node_properties.index, np.arange(3))
+        np.testing.assert_array_equal(s.node_tags['tags'], [0, 2])
+        np.testing.assert_array_equal(s.members, members1)
+
+        members3 = np.array([[0, 3], [3, 0]])
+        s = Structure(nodes1, members3, number_of_strings=2, node_tags=nodes1_tags)
+
+        np.testing.assert_array_equal(s.get_unused_nodes(), [1, 2])
+        self.assertTrue(s.has_unused_nodes())
+
+        s.remove_nodes([1, 2])
+        np.testing.assert_array_equal(s.nodes, nodes1[:, [0, 3]])
+        np.testing.assert_array_equal(s.members, np.array([[0, 1], [1, 0]]))
+        np.testing.assert_array_equal(s.node_tags['tags'], [0, 1])
+        self.assertFalse(s.has_unused_nodes())
+
+        members4 = np.array([[1, 3], [3, 1]])
+        s = Structure(nodes1, members4, number_of_strings=2, node_tags=nodes1_tags)
+
+        np.testing.assert_array_equal(s.get_unused_nodes(), [0, 2])
+        self.assertTrue(s.has_unused_nodes())
+
+        s.remove_nodes([0, 2])
+        np.testing.assert_array_equal(s.nodes, nodes1[:, [1, 3]])
+        self.assertEqual(len(s.node_properties), 2)
+        np.testing.assert_array_equal(s.node_properties.index, np.arange(2))
+        np.testing.assert_array_equal(s.members, np.array([[0, 1], [1, 0]]))
+        np.testing.assert_array_equal(s.node_tags['tags'], [1])
+        self.assertFalse(s.has_unused_nodes())
+
+        # has used nodes
+        s = Structure(nodes1, members1, number_of_strings=2, node_tags=nodes1_tags)
+
+        np.testing.assert_array_equal(s.get_unused_nodes(), [3])
+        self.assertTrue(s.has_unused_nodes())
+
+        with self.assertWarns(Warning):
+            s.remove_nodes([2, 3])
+
+        np.testing.assert_array_equal(s.nodes, nodes1[:, :3])
+        self.assertEqual(len(s.node_properties), 3)
+        np.testing.assert_array_equal(s.node_properties.index, np.arange(3))
+        np.testing.assert_array_equal(s.members, members1)
+        np.testing.assert_array_equal(s.node_tags['tags'], [0, 2])
+        self.assertFalse(s.has_unused_nodes())
+
+        s = Structure(nodes1, members1, number_of_strings=2, node_tags=nodes1_tags)
+
+        np.testing.assert_array_equal(s.get_unused_nodes(), [3])
+        self.assertTrue(s.has_unused_nodes())
+
+        with self.assertWarns(Warning):
+            s.remove_nodes([1, 2])
+
+        np.testing.assert_array_equal(s.nodes, nodes1)
+        self.assertEqual(len(s.node_properties), 4)
+        np.testing.assert_array_equal(s.node_properties.index, np.arange(4))
+        np.testing.assert_array_equal(s.members, members1)
+        np.testing.assert_array_equal(s.node_tags['tags'], [0, 2, 3])
+        self.assertTrue(s.has_unused_nodes())
+
+        # None as parameter
+
+        members3 = np.array([[0, 3], [3, 0]])
+        s = Structure(nodes1, members3, number_of_strings=2, node_tags=nodes1_tags)
+
+        np.testing.assert_array_equal(s.get_unused_nodes(), [1, 2])
+        self.assertTrue(s.has_unused_nodes())
+
+        s.remove_nodes()
+        np.testing.assert_array_equal(s.nodes, nodes1[:, [0, 3]])
+        self.assertEqual(len(s.node_properties), 2)
+        np.testing.assert_array_equal(s.node_properties.index, np.arange(2))
+        np.testing.assert_array_equal(s.members, np.array([[0, 1], [1, 0]]))
+        np.testing.assert_array_equal(s.node_tags['tags'], [0, 1])
+        self.assertFalse(s.has_unused_nodes())
+
+    def test_remove_members(self):
+
+        nodes = np.array([[1, 0, 0, 0], [0, 1, 0, 1], [0, 0, 2, 1]])
+        nodes_tags = {'tags': np.array([0, 2, 3], dtype=np.uint64)}
+        members = np.array([[0, 1, 2], [1, 2, 0]])
+        members_tag = {'mtag': np.array([0, 2], dtype=np.uint64)}
+
+        s = Structure(nodes, members, number_of_strings=2, node_tags=nodes_tags, member_tags=members_tag)
+
+        s.remove_members([2])
+        np.testing.assert_array_equal(s.nodes, nodes)
+        self.assertEqual(len(s.node_properties), 4)
+        np.testing.assert_array_equal(s.members, members[:, :2])
+        np.testing.assert_array_equal(s.member_tags['mtag'], [0])
+
+        s = Structure(nodes, members, number_of_strings=2, node_tags=nodes_tags, member_tags=members_tag)
+
+        s.remove_members([0, 1])
+        np.testing.assert_array_equal(s.nodes, nodes)
+        self.assertEqual(len(s.node_properties), 4)
+        np.testing.assert_array_equal(s.members, members[:, [2]])
+        np.testing.assert_array_equal(s.member_tags['mtag'], [0])
+
+        s = Structure(nodes, members, number_of_strings=2, node_tags=nodes_tags, member_tags=members_tag)
+
+        s.remove_members([1, 2])
+        np.testing.assert_array_equal(s.nodes, nodes)
+        self.assertEqual(len(s.node_properties), 4)
+        np.testing.assert_array_equal(s.members, members[:, [0]])
+        np.testing.assert_array_equal(s.member_tags['mtag'], [0])
+
+    def test_close_node(self):
+
+        nodes1 = np.array([[1, 0, 0, 0], [0, 1, 0, 1], [0, 0, 2, 1]])
+        members1 = np.array([[0, 1, 2], [1, 2, 0]])
+        s = Structure(nodes1, members1, number_of_strings=2)
+        merge, merge_map = s.get_close_nodes()
+        self.assertFalse(merge)
+
+        s.merge_close_nodes()
+        self.assertEqual(s.get_number_of_nodes(), 4)
+        np.testing.assert_array_equal(s.nodes, nodes1)
+        np.testing.assert_array_equal(s.members, members1)
+
+        nodes1 = np.array([[1, 0, 0, 1], [0, 1, 0, 0], [0, 0, 2, 0]])
+        members1 = np.array([[0, 1, 2, 3], [1, 2, 0, 1]])
+        s = Structure(nodes1, members1, number_of_strings=2)
+        merge, merge_map = s.get_close_nodes()
+        self.assertEqual(merge, {3})
+        np.testing.assert_array_equal(merge_map, [0, 1, 2, 0])
+
+        s.merge_close_nodes()
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        np.testing.assert_array_equal(s.nodes, nodes1[:, :3])
+        np.testing.assert_array_equal(s.members, np.array([[0, 1, 2, 0], [1, 2, 0, 1]]))
+
+        nodes1 = np.array([[1, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 2]])
+        members1 = np.array([[0, 1, 2, 3], [1, 2, 0, 1]])
+        s = Structure(nodes1, members1, number_of_strings=2)
+        merge, merge_map = s.get_close_nodes()
+        self.assertEqual(merge, {2})
+        np.testing.assert_array_equal(merge_map, [0, 1, 0, 3])
+
+        s.merge_close_nodes()
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        np.testing.assert_array_equal(s.nodes, nodes1[:, [0, 1, 3]])
+        np.testing.assert_array_equal(s.members, np.array([[0, 1, 0, 2], [1, 0, 0, 1]]))
+
+        radius = 0.1
+        nodes1 = np.array([[1, 0, 0, 1, 1], [0, 1, 0, 0, 0], [0, 0, 2, .9*radius, 1.8*radius]])
+        members1 = np.array([[0, 1, 2, 3, 2], [1, 2, 0, 1, 4]])
+        s = Structure(nodes1, members1, number_of_strings=2)
+        merge, merge_map = s.get_close_nodes(radius)
+        self.assertEqual(merge, {3, 4})
+        np.testing.assert_array_equal(merge_map, [0, 1, 2, 0, 0])
+
+        s.merge_close_nodes(radius)
+        self.assertEqual(s.get_number_of_nodes(), 3)
+        np.testing.assert_array_equal(s.nodes, nodes1[:, :3])
+        np.testing.assert_array_equal(s.members, np.array([[0, 1, 2, 0, 2], [1, 2, 0, 1, 0]]))
+
+    def test_equilibrium_update_member_properties(self):
+
+        nodes = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0]])
+        members = np.array([[0, 1], [1, 2], [2, 0], [0, 3], [1, 3], [2, 3]]).transpose()
+        s0 = Structure(nodes, members)
+
+        center = s0.get_centroid()
+        s0.add_nodes(center.reshape((3, 1)))
+
+        s1 = s0.copy()
+
+        members = np.array([[0, 4], [1, 4], [2, 4]]).transpose()
+        s1.add_members(members, number_of_strings=3)
+
+        # won't be in equilibrium with only three strings
+        self.assertRaises(Exception, s1.equilibrium)
+
+        s1 = s0.copy()
+
+        members = np.array([[0, 4], [1, 4], [2, 4], [3, 4]]).transpose()
+        s1.add_members(members, number_of_strings=4)
+
+        # equilibrium
+        s1.equilibrium()
+
+        # set properties
+        s1.update_member_properties()
+
+        # forces
+        force = np.hstack((np.kron(np.array([-np.sqrt(2), -1, np.sqrt(11)]), np.ones((3,))), [np.sqrt(3)]))
+        np.testing.assert_allclose(s1.member_properties['force'], force)
+
+        lambda_ = np.hstack((np.kron(np.array([-1, -1, 4]), np.ones((3,))), [4]))
+        np.testing.assert_allclose(s1.member_properties['lambda_'], lambda_)
+
+        mass = np.hstack((157./200. * np.ones((6,)), 157./200./4 * np.ones((4,))))
+        np.testing.assert_allclose(s1.member_properties['mass'] / s1.get_member_length() / np.pi,
+                                   mass)
+
+        volume = np.hstack((np.ones((6,)), 1/4 * np.ones((4,))))
+        np.testing.assert_allclose(10000 * s1.member_properties['volume'] / s1.get_member_length() / np.pi,
+                                   volume)
+
+        np.testing.assert_allclose(s1.member_properties['stiffness'],
+                                   np.pi * s1.member_properties['modulus'] * (s1.member_properties['radius']**2 -
+                                                                              s1.member_properties['inner_radius']**2)
+                                   / s1.get_member_length())
+
+        np.testing.assert_allclose(s1.member_properties['rest_length'],
+                                   s1.get_member_length() * (1 - s1.member_properties['lambda_'].values
+                                                             / s1.member_properties['stiffness']))
+
+    def test_node_tags(self):
+
+        nodes = np.array([[1, 0, 0, 0, 1], [0, 1, 0, 1, 1], [0, 0, 2, 1, 3]])
+        nodes_tags = {
+            'nags0': np.array([0, 3], dtype=np.uint64),
+            'nags1': np.array([1, 2], dtype=np.uint64)
+        }
+        members = np.array([[0, 1, 2, 3], [1, 2, 0, 4]])
+        members_tag = {
+            'mags0': np.array([0], dtype=np.uint64),
+            'mags1': np.array([1, 2], dtype=np.uint64)
+        }
+        s = Structure(nodes, members, number_of_strings=2, node_tags=nodes_tags, member_tags=members_tag)
+
+        s.set_node_tag('nags2', [0, 3])
+        np.testing.assert_array_equal(s.node_tags['nags2'], [0, 3])
+
+        s.add_node_tag('nags1', [3])
+        np.testing.assert_array_equal(s.node_tags['nags1'], [1, 2, 3])
+
+        s.remove_node_tag('nags1', [2])
+        np.testing.assert_array_equal(s.node_tags['nags1'], [1, 3])
+
+        s.delete_node_tag('nags1')
+        self.assertFalse('nags1' in s.node_tags)
+
+    def test_member_tags(self):
+
+        nodes = np.array([[1, 0, 0, 0, 1], [0, 1, 0, 1, 1], [0, 0, 2, 1, 3]])
+        nodes_tags = {
+            'nags0': np.array([0, 3], dtype=np.uint64),
+            'nags1': np.array([1, 2], dtype=np.uint64)
+        }
+        members = np.array([[0, 1, 2, 3], [1, 2, 0, 4]])
+        members_tag = {
+            'mags0': np.array([0], dtype=np.uint64),
+            'mags1': np.array([1, 2], dtype=np.uint64)
+        }
+        s = Structure(nodes, members, number_of_strings=2, node_tags=nodes_tags, member_tags=members_tag)
+
+        s.set_member_tag('mags2', [0, 3])
+        np.testing.assert_array_equal(s.member_tags['mags2'], [0, 3])
+
+        s.add_member_tag('mags1', [3])
+        np.testing.assert_array_equal(s.member_tags['mags1'], [1, 2, 3])
+
+        s.remove_member_tag('mags1', [2])
+        np.testing.assert_array_equal(s.member_tags['mags1'], [1, 3])
+
+        s.delete_member_tag('mags1')
+        self.assertFalse('mags1' in s.member_tags)
+
+    def test_node_constraint(self):
+
+        nodes = np.array([[1, 0, 0, 0, 1], [0, 1, 0, 1, 1], [0, 0, 2, 1, 3]])
+        nodes_tags = {
+            'nags0': np.array([0, 3], dtype=np.uint64),
+            'nags1': np.array([1, 2], dtype=np.uint64)
+        }
+        members = np.array([[0, 1, 2, 3], [1, 2, 0, 4]])
+        members_tag = {
+            'mags0': np.array([0], dtype=np.uint64),
+            'mags1': np.array([1, 2], dtype=np.uint64)
+        }
+        s = Structure(nodes, members, number_of_strings=2, node_tags=nodes_tags, member_tags=members_tag)
+        s.node_properties.loc[2, 'constraint'] = NodeConstraint()
+        s.node_properties.loc[0, 'constraint'] = NodeConstraint(np.array(([[1, 1, 0]])))
+
+        # print(s.node_properties.loc[2, 'constraint'])
+        # print(s.node_properties.loc[2, 'constraint'].__class__)
+        # print(s.node_properties.loc[0, 'constraint'])
+        # print(s.node_properties.loc[0, 'constraint'].__class__)
+
+        R, T = NodeConstraint.node_constraint(s.nodes, s.node_properties['constraint'])
+        self.assertEqual(R.shape, (4, 15))
+        self.assertEqual(T.shape, (15, 11))
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `tnsgrt-0.3/LICENSE` & `tnsgrt-0.4/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Mauricio de Oliveira
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Mauricio de Oliveira
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `tnsgrt-0.3/pyproject.toml` & `tnsgrt-0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "tnsgrt"
-version = "0.3"
-authors = [
-    { name = "Mauricio C. de Oliveira", email = "mcdeoliveira@duck.com" }
-]
-description = "Python library with support for analysis and design of Tensegrity structures"
-readme = "README.md"
-license = {file = "LICENSE"}
-keywords = ["Tensegrity", "structures", "trusses"]
-
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Other Audience",
-    "Topic :: Scientific/Engineering",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.7",
-]
-
-dependencies = [
-    "numpy",
-    "matplotlib",
-    "pandas",
-    "scipy",
-    "cvxpy",
-    "vispy",
-    "parameterized"
-]
-
-[project.urls]
-"Homepage" = "https://github.com/mcdeoliveira/tensegrity"
-
-[tool.setuptools]
-py-modules = []
-
-[tool.pytest.ini_options]
-pythonpath = [
-  "src"
-]
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "tnsgrt"
+version = "0.4"
+authors = [
+    { name = "Mauricio C. de Oliveira", email = "mcdeoliveira@duck.com" }
+]
+description = "Python library with support for analysis and design of Tensegrity structures"
+readme = "README.md"
+license = {file = "LICENSE"}
+keywords = ["Tensegrity", "structures", "trusses"]
+requires-python = ">3.7"
+
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Other Audience",
+    "Topic :: Scientific/Engineering",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.7",
+]
+
+dependencies = [
+    "numpy",
+    "matplotlib",
+    "pandas",
+    "scipy",
+    "cvxpy",
+    "vispy",
+    "parameterized"
+]
+
+[project.urls]
+"Homepage" = "https://github.com/mcdeoliveira/tensegrity"
+
+[tool.setuptools]
+py-modules = []
+
+[tool.pytest.ini_options]
+pythonpath = [
+  "src"
+]
```

### Comparing `tnsgrt-0.3/PKG-INFO` & `tnsgrt-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tnsgrt
-Version: 0.3
+Version: 0.4
 Summary: Python library with support for analysis and design of Tensegrity structures
 Project-URL: Homepage, https://github.com/mcdeoliveira/tensegrity
 Author-email: "Mauricio C. de Oliveira" <mcdeoliveira@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Mauricio de Oliveira
         
@@ -28,14 +28,15 @@
 License-File: LICENSE
 Keywords: Tensegrity,structures,trusses
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >3.7
 Requires-Dist: cvxpy
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: parameterized
 Requires-Dist: scipy
 Requires-Dist: vispy
```

