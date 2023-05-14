# Comparing `tmp/sphinxext_altair-0.1.0.tar.gz` & `tmp/sphinxext_altair-0.1.1.tar.gz`

## Comparing `sphinxext_altair-0.1.0.tar` & `sphinxext_altair-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.0/sphinxext_altair/__init__.py
--rw-r--r--   0        0        0    12510 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.0/sphinxext_altair/altairplot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.0/sphinxext_altair/py.typed
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.0/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.0/LICENSE
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.0/README.md
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.1/sphinxext_altair/__init__.py
+-rw-r--r--   0        0        0    12510 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.1/sphinxext_altair/altairplot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.1/sphinxext_altair/py.typed
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.1/README.md
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 sphinxext_altair-0.1.1/PKG-INFO
```

### Comparing `sphinxext_altair-0.1.0/sphinxext_altair/altairplot.py` & `sphinxext_altair-0.1.1/sphinxext_altair/altairplot.py`

 * *Files identical despite different names*

### Comparing `sphinxext_altair-0.1.0/.gitignore` & `sphinxext_altair-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinxext_altair-0.1.0/LICENSE` & `sphinxext_altair-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxext_altair-0.1.0/README.md` & `sphinxext_altair-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,27 +13,33 @@
             x='Horsepower',
             y='Miles_per_Gallon',
             color='Origin',
             shape='Origin'
         )
 ```
 
-<img src="images/example_screenshot.png"  width="70%">
+<img src="https://raw.githubusercontent.com/altair-viz/sphinxext-altair/main/images/example_screenshot.png"  width="70%">
 
 You can enable the extension by adding it to your `conf.py`:
 
 ```python
 extensions = [
     ...
     "sphinxext_altair.altairplot",
     ...
 ]
 ```
 
-You can find all available options in the docstring of `sphinxext_altair/altairplot.py`. For more examples on how to use this extension, see the test Sphinx documentation in `tests/roots/test-altairplot` or the official [Altair documentation](https://github.com/altair-viz/altair/tree/master/doc)
+You can find all available options in the docstring of `sphinxext_altair/altairplot.py`. For more examples on how to use this extension, see the test Sphinx documentation in `tests/roots/test-altairplot` or the official [Altair documentation](https://github.com/altair-viz/altair/tree/master/doc).
+
+You can install the extension with:
+
+```bash
+pip install sphinxext-altair
+```
 
 
 # Contributing
 It's recommended to use a virtual environment for development:
 
 ```bash
 python -m venv .venv
```

### Comparing `sphinxext_altair-0.1.0/pyproject.toml` & `sphinxext_altair-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,15 @@
 path = "sphinxext_altair/__init__.py"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build]
 include = [
-    "/sphinxext_altair",
-    "README.md",
-    "LICENSE",
-    "pyproject.toml"
+    "/sphinxext_altair"
 ]
 
 [tool.hatch.envs.default]
 features = ["dev"]
 
 [tool.hatch.envs.default.scripts]
 test = [
```

### Comparing `sphinxext_altair-0.1.0/PKG-INFO` & `sphinxext_altair-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxext-altair
-Version: 0.1.0
+Version: 0.1.1
 Summary: sphinxext-altair: Sphinx extension for embedding Altair charts
 Project-URL: Source, https://github.com/altair-viz/sphinxext-altair
 Author: sphinxext-altair Contributors
 License-File: LICENSE
 Keywords: altair,sphinxext
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -47,27 +47,33 @@
             x='Horsepower',
             y='Miles_per_Gallon',
             color='Origin',
             shape='Origin'
         )
 ```
 
-<img src="images/example_screenshot.png"  width="70%">
+<img src="https://raw.githubusercontent.com/altair-viz/sphinxext-altair/main/images/example_screenshot.png"  width="70%">
 
 You can enable the extension by adding it to your `conf.py`:
 
 ```python
 extensions = [
     ...
     "sphinxext_altair.altairplot",
     ...
 ]
 ```
 
-You can find all available options in the docstring of `sphinxext_altair/altairplot.py`. For more examples on how to use this extension, see the test Sphinx documentation in `tests/roots/test-altairplot` or the official [Altair documentation](https://github.com/altair-viz/altair/tree/master/doc)
+You can find all available options in the docstring of `sphinxext_altair/altairplot.py`. For more examples on how to use this extension, see the test Sphinx documentation in `tests/roots/test-altairplot` or the official [Altair documentation](https://github.com/altair-viz/altair/tree/master/doc).
+
+You can install the extension with:
+
+```bash
+pip install sphinxext-altair
+```
 
 
 # Contributing
 It's recommended to use a virtual environment for development:
 
 ```bash
 python -m venv .venv
```

