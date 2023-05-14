# Comparing `tmp/data2latex-0.0.1.tar.gz` & `tmp/data2latex-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2latex-0.0.1.tar", last modified: Sun May 14 11:11:45 2023, max compression
+gzip compressed data, was "data2latex-1.0.0.tar", last modified: Sun May 14 12:37:41 2023, max compression
```

## Comparing `data2latex-0.0.1.tar` & `data2latex-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 11:11:45.461240 data2latex-0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-05-14 10:51:18.000000 data2latex-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3808 2023-05-14 11:11:45.460239 data2latex-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1430 2023-05-06 16:07:16.000000 data2latex-0.0.1/README.md
--rw-rw-rw-   0        0        0     1801 2023-05-14 11:09:56.000000 data2latex-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 11:11:45.461240 data2latex-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 11:11:45.428240 data2latex-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 11:11:45.443237 data2latex-0.0.1/src/data2latex/
--rw-rw-rw-   0        0        0      266 2023-05-11 19:09:04.000000 data2latex-0.0.1/src/data2latex/__init__.py
--rw-rw-rw-   0        0        0     8211 2023-05-11 23:03:20.000000 data2latex-0.0.1/src/data2latex/dm.py
--rw-rw-rw-   0        0        0     7300 2023-05-07 19:42:55.000000 data2latex-0.0.1/src/data2latex/environments.py
--rw-rw-rw-   0        0        0    10015 2023-05-13 22:01:26.000000 data2latex-0.0.1/src/data2latex/features.py
--rw-rw-rw-   0        0        0     7369 2023-05-10 13:28:58.000000 data2latex-0.0.1/src/data2latex/iter_protocols.py
--rw-rw-rw-   0        0        0    30923 2023-05-13 22:38:12.000000 data2latex-0.0.1/src/data2latex/plot.py
--rw-rw-rw-   0        0        0    18502 2023-05-13 21:52:50.000000 data2latex-0.0.1/src/data2latex/table.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:11:45.459238 data2latex-0.0.1/src/data2latex.egg-info/
--rw-rw-rw-   0        0        0     3808 2023-05-14 11:11:45.000000 data2latex-0.0.1/src/data2latex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-05-14 11:11:45.000000 data2latex-0.0.1/src/data2latex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 11:11:45.000000 data2latex-0.0.1/src/data2latex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-05-14 11:11:45.000000 data2latex-0.0.1/src/data2latex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-14 11:11:45.000000 data2latex-0.0.1/src/data2latex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 12:37:41.202202 data2latex-1.0.0/
+-rw-rw-rw-   0        0        0     1094 2023-05-14 10:51:18.000000 data2latex-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4898 2023-05-14 12:37:41.201202 data2latex-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2023-05-14 11:48:20.000000 data2latex-1.0.0/README.md
+-rw-rw-rw-   0        0        0     1814 2023-05-14 12:35:58.000000 data2latex-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 12:37:41.202202 data2latex-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 12:37:41.175202 data2latex-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 12:37:41.191269 data2latex-1.0.0/src/data2latex/
+-rw-rw-rw-   0        0        0      266 2023-05-11 19:09:04.000000 data2latex-1.0.0/src/data2latex/__init__.py
+-rw-rw-rw-   0        0        0     8211 2023-05-11 23:03:20.000000 data2latex-1.0.0/src/data2latex/dm.py
+-rw-rw-rw-   0        0        0     7300 2023-05-07 19:42:55.000000 data2latex-1.0.0/src/data2latex/environments.py
+-rw-rw-rw-   0        0        0    10015 2023-05-13 22:01:26.000000 data2latex-1.0.0/src/data2latex/features.py
+-rw-rw-rw-   0        0        0     7369 2023-05-10 13:28:58.000000 data2latex-1.0.0/src/data2latex/iter_protocols.py
+-rw-rw-rw-   0        0        0    30923 2023-05-13 22:38:12.000000 data2latex-1.0.0/src/data2latex/plot.py
+-rw-rw-rw-   0        0        0    18502 2023-05-13 21:52:50.000000 data2latex-1.0.0/src/data2latex/table.py
+drwxrwxrwx   0        0        0        0 2023-05-14 12:37:41.200205 data2latex-1.0.0/src/data2latex.egg-info/
+-rw-rw-rw-   0        0        0     4898 2023-05-14 12:37:41.000000 data2latex-1.0.0/src/data2latex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-05-14 12:37:41.000000 data2latex-1.0.0/src/data2latex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 12:37:41.000000 data2latex-1.0.0/src/data2latex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-05-14 12:37:41.000000 data2latex-1.0.0/src/data2latex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-14 12:37:41.000000 data2latex-1.0.0/src/data2latex.egg-info/top_level.txt
```

### Comparing `data2latex-0.0.1/LICENSE` & `data2latex-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data2latex-0.0.1/PKG-INFO` & `data2latex-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: data2latex
-Version: 0.0.1
-Summary: Prototype for simple generation of LaTeX tables and plots from scientific data for use in papers.
+Version: 1.0.0
+Summary: Package prototype for simple generation of LaTeX tables and plots from scientific data for use in any document.
 Author-email: Richard Kokštein <richard.Kokstein@fs.cvut.cz>
 License: MIT License
         
         Copyright (c) 2023 Richard Kokstein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -27,53 +27,82 @@
         
 Project-URL: homepage, https://github.com/Trolobezka/data2latex
 Project-URL: documentation, https://github.com/Trolobezka/data2latex
 Project-URL: repository, https://github.com/Trolobezka/data2latex
 Project-URL: Bug Tracker, https://github.com/Trolobezka/data2latex/issues
 Keywords: generation,latex,table,plot,graph,array,datatable
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# data2latex
+# Data2LaTeX
 
-This project is part of my bachelor thesis which deals with data representation using Python and LaTeX.
+![Data2LaTeX logo](docs/_static/img/logo.png)
 
-The idea behind this package prototype is that generating LaTeX documents containing scientific data from Python should not be difficult and require many steps. Currently the package supports the creation of simple tables and two types of plots: scatter plot and line plot. The package uses the PyLaTeX package to handle the document creation and compilation process. The main data sources are arrays and data tables from the popular Numpy, SciPy and Pandas packages. A major inspiration for the package syntax is the Matplotlib.Pyplot package, which allows plots to be created in a few lines of code. This package allows the user to choose a backend for plotting: Matplotlib in Python or pgfplots in LaTeX.
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+This project is part of my bachelor thesis which deals with data representation using **Python** and **LaTeX**. You can find the source code on my [GitHub](https://github.com/Trolobezka/data2latex).
+
+The idea behind this package prototype is that generating LaTeX documents containing scientific data from Python should not be difficult and require many steps. Currently the package supports the creation of simple tables and two types of plots: scatter plots and line plots. The package uses the [PyLaTeX](https://github.com/JelteF/PyLaTeX) package to handle the document creation and compilation process. The main data sources are arrays and data tables from the popular `numpy` and `pandas` packages. A major inspiration for the module syntax is the `matplotlib.pyplot` module, which allows plots to be created in a few lines of code. The tables are created using `tblr` environment from `tabularray` package. The plots are created using `tikzpicture` / `axis` environment from `tikz` / `pgfplots` package.
 
 ## Examples
 
+Examples with results can be found in the [documentation](https://trolobezka.github.io/data2latex-docs).
+
+### Simple features
+
+```python
+import data2latex as dtol
+dtol.section("Data2LaTeX")
+dtol.text("This project is part of my bachelor thesis which deals with data representation using Python and LaTeX")
+dtol.finish("simple_features")
+```
+
+### Simple table
+
 ```python
-print("Hello World!")
+import data2latex as dtol
+data = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
+dtol.table(data)
+dtol.finish("simple_table")
+```
+
+### Simple plot
+
+```python
+port data2latex as dtol
+X = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+Y = [84, 13, 94, 37, 80, 89, 90, 45, 55, 26, 92]
+dtol.plot(X, Y, line="-", mark="*")
+dtol.finish("simple_plot")
 ```
 
 ## Installation
 
 ```bash
 python -m pip install --upgrade pip
 python -m pip install --upgrade data2latex
 ```
 
-## Developing
+## Development
 
 ```bash
 python -m venv .venv
 ./.venv/Scripts/activate
 python -m pip install --upgrade pip
-python -m pip install .
 python -m pip install .[dev]
 ```
 
 ## Generating documentation
 
 ```bash
 sphinx-apidoc -o docs src/data2latex
@@ -82,9 +111,15 @@
 
 ## Packaging
 
 ```bash
 python clear.py
 python -m pip install --upgrade build
 python -m build
-python -m pip install ./dist/data2latex-?.whl
+```
+
+## Publishing
+
+```bash
+python -m pip install --upgrade twine
+python -m twine upload dist/*
 ```
```

### Comparing `data2latex-0.0.1/pyproject.toml` & `data2latex-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "data2latex"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name="Richard Kokštein", email="richard.Kokstein@fs.cvut.cz" },
 ]
-description = "Prototype for simple generation of LaTeX tables and plots from scientific data for use in papers."
+description = "Package prototype for simple generation of LaTeX tables and plots from scientific data for use in any document."
 keywords = ["generation", "latex", "table", "plot", "graph", "array", "datatable"]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Intended Audience :: Science/Research",
     "Topic :: Utilities",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Visualization",
```

### Comparing `data2latex-0.0.1/src/data2latex/dm.py` & `data2latex-1.0.0/src/data2latex/dm.py`

 * *Files identical despite different names*

### Comparing `data2latex-0.0.1/src/data2latex/environments.py` & `data2latex-1.0.0/src/data2latex/environments.py`

 * *Files identical despite different names*

### Comparing `data2latex-0.0.1/src/data2latex/features.py` & `data2latex-1.0.0/src/data2latex/features.py`

 * *Files identical despite different names*

### Comparing `data2latex-0.0.1/src/data2latex/iter_protocols.py` & `data2latex-1.0.0/src/data2latex/iter_protocols.py`

 * *Files identical despite different names*

### Comparing `data2latex-0.0.1/src/data2latex/plot.py` & `data2latex-1.0.0/src/data2latex/plot.py`

 * *Files identical despite different names*

### Comparing `data2latex-0.0.1/src/data2latex/table.py` & `data2latex-1.0.0/src/data2latex/table.py`

 * *Files identical despite different names*

### Comparing `data2latex-0.0.1/src/data2latex.egg-info/PKG-INFO` & `data2latex-1.0.0/src/data2latex.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: data2latex
-Version: 0.0.1
-Summary: Prototype for simple generation of LaTeX tables and plots from scientific data for use in papers.
+Version: 1.0.0
+Summary: Package prototype for simple generation of LaTeX tables and plots from scientific data for use in any document.
 Author-email: Richard Kokštein <richard.Kokstein@fs.cvut.cz>
 License: MIT License
         
         Copyright (c) 2023 Richard Kokstein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -27,53 +27,82 @@
         
 Project-URL: homepage, https://github.com/Trolobezka/data2latex
 Project-URL: documentation, https://github.com/Trolobezka/data2latex
 Project-URL: repository, https://github.com/Trolobezka/data2latex
 Project-URL: Bug Tracker, https://github.com/Trolobezka/data2latex/issues
 Keywords: generation,latex,table,plot,graph,array,datatable
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# data2latex
+# Data2LaTeX
 
-This project is part of my bachelor thesis which deals with data representation using Python and LaTeX.
+![Data2LaTeX logo](docs/_static/img/logo.png)
 
-The idea behind this package prototype is that generating LaTeX documents containing scientific data from Python should not be difficult and require many steps. Currently the package supports the creation of simple tables and two types of plots: scatter plot and line plot. The package uses the PyLaTeX package to handle the document creation and compilation process. The main data sources are arrays and data tables from the popular Numpy, SciPy and Pandas packages. A major inspiration for the package syntax is the Matplotlib.Pyplot package, which allows plots to be created in a few lines of code. This package allows the user to choose a backend for plotting: Matplotlib in Python or pgfplots in LaTeX.
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+This project is part of my bachelor thesis which deals with data representation using **Python** and **LaTeX**. You can find the source code on my [GitHub](https://github.com/Trolobezka/data2latex).
+
+The idea behind this package prototype is that generating LaTeX documents containing scientific data from Python should not be difficult and require many steps. Currently the package supports the creation of simple tables and two types of plots: scatter plots and line plots. The package uses the [PyLaTeX](https://github.com/JelteF/PyLaTeX) package to handle the document creation and compilation process. The main data sources are arrays and data tables from the popular `numpy` and `pandas` packages. A major inspiration for the module syntax is the `matplotlib.pyplot` module, which allows plots to be created in a few lines of code. The tables are created using `tblr` environment from `tabularray` package. The plots are created using `tikzpicture` / `axis` environment from `tikz` / `pgfplots` package.
 
 ## Examples
 
+Examples with results can be found in the [documentation](https://trolobezka.github.io/data2latex-docs).
+
+### Simple features
+
+```python
+import data2latex as dtol
+dtol.section("Data2LaTeX")
+dtol.text("This project is part of my bachelor thesis which deals with data representation using Python and LaTeX")
+dtol.finish("simple_features")
+```
+
+### Simple table
+
 ```python
-print("Hello World!")
+import data2latex as dtol
+data = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
+dtol.table(data)
+dtol.finish("simple_table")
+```
+
+### Simple plot
+
+```python
+port data2latex as dtol
+X = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+Y = [84, 13, 94, 37, 80, 89, 90, 45, 55, 26, 92]
+dtol.plot(X, Y, line="-", mark="*")
+dtol.finish("simple_plot")
 ```
 
 ## Installation
 
 ```bash
 python -m pip install --upgrade pip
 python -m pip install --upgrade data2latex
 ```
 
-## Developing
+## Development
 
 ```bash
 python -m venv .venv
 ./.venv/Scripts/activate
 python -m pip install --upgrade pip
-python -m pip install .
 python -m pip install .[dev]
 ```
 
 ## Generating documentation
 
 ```bash
 sphinx-apidoc -o docs src/data2latex
@@ -82,9 +111,15 @@
 
 ## Packaging
 
 ```bash
 python clear.py
 python -m pip install --upgrade build
 python -m build
-python -m pip install ./dist/data2latex-?.whl
+```
+
+## Publishing
+
+```bash
+python -m pip install --upgrade twine
+python -m twine upload dist/*
 ```
```

