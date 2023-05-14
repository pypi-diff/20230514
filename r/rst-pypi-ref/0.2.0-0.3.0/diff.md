# Comparing `tmp/rst-pypi-ref-0.2.0.tar.gz` & `tmp/rst_pypi_ref-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rst-pypi-ref-0.2.0.tar", last modified: Sun Apr  9 02:38:32 2023, max compression
+gzip compressed data, was "rst_pypi_ref-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rst-pypi-ref-0.2.0.tar` & `rst_pypi_ref-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      560 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/.editorconfig
--rw-r--r--   0        0        0      792 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     1863 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     3278 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/.gitignore
--rw-r--r--   0        0        0      492 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      382 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/CHANGES.rst
--rw-r--r--   0        0        0     9161 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/LICENSE
--rw-r--r--   0        0        0     1061 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/README.rst
--rw-r--r--   0        0        0     1386 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       78 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/rst_pypi_ref/__init__.py
--rwxr-xr-x   0        0        0      204 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/rst_pypi_ref/cli.py
--rw-r--r--   0        0        0      926 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/rst_pypi_ref/core.py
--rw-r--r--   0        0        0      384 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/rst_pypi_ref/sphinx.py
--rw-r--r--   0        0        0      741 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/setup.cfg
--rw-r--r--   0        0        0      317 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0       65 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/tests/roots/test-default/conf.py
--rw-r--r--   0        0        0      100 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/tests/roots/test-default/index.rst
--rw-r--r--   0        0        0      612 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/tests/test_it.py
--rw-r--r--   0        0        0      355 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/tests/test_sphinx.py
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 rst-pypi-ref-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      560 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/.editorconfig
+-rw-r--r--   0        0        0      792 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1863 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3278 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/.gitignore
+-rw-r--r--   0        0        0      492 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      497 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/CHANGES.rst
+-rw-r--r--   0        0        0     9161 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1309 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/README.rst
+-rw-r--r--   0        0        0     1386 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/rst_pypi_ref/__init__.py
+-rwxr-xr-x   0        0        0      204 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/rst_pypi_ref/cli.py
+-rw-r--r--   0        0        0     1127 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/rst_pypi_ref/core.py
+-rw-r--r--   0        0        0      384 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/rst_pypi_ref/sphinx.py
+-rw-r--r--   0        0        0      741 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/setup.cfg
+-rw-r--r--   0        0        0      317 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0       65 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/tests/roots/test-default/conf.py
+-rw-r--r--   0        0        0      100 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/tests/roots/test-default/index.rst
+-rw-r--r--   0        0        0      975 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/tests/test_it.py
+-rw-r--r--   0        0        0      355 2023-05-14 19:02:59.563869 rst_pypi_ref-0.3.0/tests/test_sphinx.py
+-rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 rst_pypi_ref-0.3.0/PKG-INFO
```

### Comparing `rst-pypi-ref-0.2.0/.editorconfig` & `rst_pypi_ref-0.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `rst-pypi-ref-0.2.0/.github/workflows/main.yml` & `rst_pypi_ref-0.3.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `rst-pypi-ref-0.2.0/.github/workflows/release.yml` & `rst_pypi_ref-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rst-pypi-ref-0.2.0/.gitignore` & `rst_pypi_ref-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rst-pypi-ref-0.2.0/LICENSE` & `rst_pypi_ref-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rst-pypi-ref-0.2.0/README.rst` & `rst_pypi_ref-0.3.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,23 @@
 
 Usage
 =====
 
 When you write ``:pypi:`rst-pypi-ref``` into reStructuredText source,
 this appends ref to PyPI URL for ``rst-pypi-ref``.
 
+Supporting syntax
+-----------------
+
+* Package name only: ``:pypi:`rst-pypi-ref```
+* Explicit version: ``:pypi:`rst-pypi-ref==0.2.0```
+* Change display text: ``:pypi:`PyPI Link <rst-pypi-ref>```
+
+  * There package name in between ``<`` and ``>``.
+
 Simple usage
 ------------
 
 .. code-block:: console
 
    $ echo ':pypi:`rst-pypi-ref`' | python -m rst_pypi_ref.cli
    <document source="<stdin>">
```

### Comparing `rst-pypi-ref-0.2.0/pyproject.toml` & `rst_pypi_ref-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rst-pypi-ref-0.2.0/rst_pypi_ref/core.py` & `rst_pypi_ref-0.3.0/rst_pypi_ref/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Core module."""
+import re
 from typing import List, Optional
 
 from docutils import nodes
 from docutils.parsers.rst import roles
 from docutils.parsers.rst.states import Inliner
 
 
@@ -24,13 +25,18 @@
     inliner: Inliner,
     options: Optional[dict] = None,
     content: Optional[List[str]] = None,
 ):
     """Parse ``pypi`` role."""
     options = roles.normalized_role_options(options)
     messages = []
-    url = build_package_url(text)
-    return [nodes.reference(rawtext, text, refuri=url, **options)], messages
+    title = target = text
+    matched = re.match(r"^(?P<title>.+) <(?P<target>.+)>$", text)
+    if matched:
+        title = matched.group("title")
+        target = matched.group("target")
+    url = build_package_url(target)
+    return [nodes.reference(rawtext, title, refuri=url, **options)], messages
 
 
 def bootstrap():
     roles.register_canonical_role("pypi", pypi_reference_role)
```

### Comparing `rst-pypi-ref-0.2.0/setup.cfg` & `rst_pypi_ref-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.3.0
 commit = True
 tag = False
 message = release: Bump version {current_version} -> {new_version}
 
 [bumpversion:file:rst_pypi_ref/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `rst-pypi-ref-0.2.0/tests/test_it.py` & `rst_pypi_ref-0.3.0/tests/test_it.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from rst_pypi_ref import core
 
 
-def test_pypi_reference_role():
-    nodes, messages = core.pypi_reference_role(
-        "pypi", ":pypi:`docutils`", "docutils", 0, None
-    )
-    assert len(nodes) == 1
-    node = nodes[0]
-    assert node["refuri"] == "https://pypi.org/project/docutils/"
+class TestForPyPiReferenceRole:
+    def test_name_only(self):
+        nodes, messages = core.pypi_reference_role(
+            "pypi", ":pypi:`docutils`", "docutils", 0, None
+        )
+        assert len(nodes) == 1
+        node = nodes[0]
+        assert node["refuri"] == "https://pypi.org/project/docutils/"
+
+    def test_title_and_target(self):
+        nodes, messages = core.pypi_reference_role(
+            "pypi", ":pypi:`PyPI Link <docutils>`", "PyPI Link <docutils>", 0, None
+        )
+        assert len(nodes) == 1
+        node = nodes[0]
+        assert node["refuri"] == "https://pypi.org/project/docutils/"
 
 
 class TestForBuildPackageUrl:
     def test_name_only(self):
         url = core.build_package_url("docutils")
         assert url == "https://pypi.org/project/docutils/"
```

### Comparing `rst-pypi-ref-0.2.0/PKG-INFO` & `rst_pypi_ref-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rst-pypi-ref
-Version: 0.2.0
+Version: 0.3.0
 Summary: reStructuredText custom role to add ref to PyPI.
 Author-email: Kazuya Takei <myself@attakei.net>
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -55,14 +55,23 @@
 
 Usage
 =====
 
 When you write ``:pypi:`rst-pypi-ref``` into reStructuredText source,
 this appends ref to PyPI URL for ``rst-pypi-ref``.
 
+Supporting syntax
+-----------------
+
+* Package name only: ``:pypi:`rst-pypi-ref```
+* Explicit version: ``:pypi:`rst-pypi-ref==0.2.0```
+* Change display text: ``:pypi:`PyPI Link <rst-pypi-ref>```
+
+  * There package name in between ``<`` and ``>``.
+
 Simple usage
 ------------
 
 .. code-block:: console
 
    $ echo ':pypi:`rst-pypi-ref`' | python -m rst_pypi_ref.cli
    <document source="<stdin>">
```

