# Comparing `tmp/browsr-1.4.0.tar.gz` & `tmp/browsr-1.5.0.tar.gz`

## Comparing `browsr-1.4.0.tar` & `browsr-1.5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.4.0/.releaserc.js
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 browsr-1.4.0/mkdocs.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/__main__.py
--rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/_base.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/_cli.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/_config.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/_utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/_version.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/browsr.css
--rw-r--r--   0        0        0    12920 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/browsr.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/cli.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/contributing.md
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/index.md
--rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/_static/browsr.png
--rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/_static/browsr_no_label.png
--rw-r--r--   0        0        0  1112808 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/_static/screenshot_datatable.png
--rw-r--r--   0        0        0   838657 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/_static/screenshot_markdown.png
--rw-r--r--   0        0        0  1550033 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/_static/screenshot_mona_lisa.png
--rw-r--r--   0        0        0  1031902 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/_static/screenshot_utils.png
--rw-r--r--   0        0        0   118970 2020-02-02 00:00:00.000000 browsr-1.4.0/requirements/requirements-dev.txt
--rw-r--r--   0        0        0    82526 2020-02-02 00:00:00.000000 browsr-1.4.0/requirements/requirements-prod.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.4.0/tests/conftest.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.4.0/tests/test_cli.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.4.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.4.0/LICENSE
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 browsr-1.4.0/README.md
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 browsr-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 browsr-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.5.0/.releaserc.js
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 browsr-1.5.0/mkdocs.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/__main__.py
+-rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/_base.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/_cli.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/_config.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/_utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/_version.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/browsr.css
+-rw-r--r--   0        0        0    12920 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/browsr.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/cli.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/contributing.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/index.md
+-rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/_static/browsr.png
+-rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/_static/browsr_no_label.png
+-rw-r--r--   0        0        0  1112808 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/_static/screenshot_datatable.png
+-rw-r--r--   0        0        0   838657 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/_static/screenshot_markdown.png
+-rw-r--r--   0        0        0  1550033 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/_static/screenshot_mona_lisa.png
+-rw-r--r--   0        0        0  1031902 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/_static/screenshot_utils.png
+-rw-r--r--   0        0        0   118970 2020-02-02 00:00:00.000000 browsr-1.5.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0    82526 2020-02-02 00:00:00.000000 browsr-1.5.0/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.5.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 browsr-1.5.0/README.md
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 browsr-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 browsr-1.5.0/PKG-INFO
```

### Comparing `browsr-1.4.0/.pre-commit-config.yaml` & `browsr-1.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/.releaserc.js` & `browsr-1.5.0/.releaserc.js`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/mkdocs.yaml` & `browsr-1.5.0/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/.github/semantic_release/package-lock.json` & `browsr-1.5.0/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/.github/semantic_release/release_notes.hbs` & `browsr-1.5.0/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/.github/workflows/lint.yaml` & `browsr-1.5.0/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/.github/workflows/publish.yaml` & `browsr-1.5.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/.github/workflows/release.yaml` & `browsr-1.5.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/.github/workflows/tests.yaml` & `browsr-1.5.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/browsr/_base.py` & `browsr-1.5.0/browsr/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
 
 class UniversalDirectoryTree(DirectoryTree):
     """
     A Universal DirectoryTree supporting different filesystems
     """
 
-    def load_directory(self, node: TreeNode[DirEntry]) -> None:
+    def _load_directory(self, node: TreeNode[DirEntry]) -> None:
         """
         Load Directory Using Universal Pathlib
         """
         assert node.data is not None
         dir_path = UPath(node.data.path)
         node.data.loaded = True
         top_level_buckets = self._handle_top_level_bucket(dir_path=dir_path)
@@ -152,19 +152,32 @@
         for path in top_level_buckets or directory:
             if top_level_buckets is None:
                 path_name = path.name
             else:
                 path_name = str(path).replace("s3://", "").rstrip("/")
             node.add(
                 path_name,
-                data=DirEntry(str(path), path.is_dir()),
+                data=DirEntry(path),
                 allow_expand=path.is_dir(),
             )
         node.expand()
 
+    def reload(self) -> None:
+        """
+        Reload the `DirectoryTree` contents.
+        """
+        self.reset(str(self.path), DirEntry(UPath(self.path)))
+        self._load_directory(self.root)
+
+    def validate_path(self, path: Union[str, UPath]) -> UPath:  # type: ignore[override]
+        """
+        Ensure that the path is of the `UPath` type.
+        """
+        return UPath(path)
+
     def _handle_top_level_bucket(self, dir_path: UPath) -> Optional[Iterable[UPath]]:
         """
         Handle scenarios when someone wants to browse all of s3
 
         This is because S3FS handles the root directory differently than other filesystems
         """
         if str(dir_path) == "s3:/":
```

### Comparing `browsr-1.4.0/browsr/_cli.py` & `browsr-1.5.0/browsr/_cli.py`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/browsr/_config.py` & `browsr-1.5.0/browsr/_config.py`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/browsr/_utils.py` & `browsr-1.5.0/browsr/_utils.py`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/browsr/browsr.css` & `browsr-1.5.0/browsr/browsr.css`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/browsr/browsr.py` & `browsr-1.5.0/browsr/browsr.py`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/docs/contributing.md` & `browsr-1.5.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/docs/gen_ref_pages.py` & `browsr-1.5.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/docs/index.md` & `browsr-1.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 # browsr
 
 <div align="center">
 <a href="https://github.com/juftin/browsr">
-  <img src=_static/browsr.png
+  <img src=docs/_static/browsr.png
     width="400" alt="browsr">
 </a>
 </div>
 
 [![browsr Version](https://img.shields.io/pypi/v/browsr?color=blue&label=browsr)](https://github.com/juftin/browsr)
 [![PyPI](https://img.shields.io/pypi/pyversions/browsr)](https://pypi.python.org/pypi/browsr/)
 [![Testing Status](https://github.com/juftin/browsr/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/workflows/tests.yaml?query=branch%3Amain)
 [![GitHub License](https://img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://github.com/juftin/browsr/blob/main/LICENSE)
 
 **`browsr`** is a TUI (text-based user interface) file browser for your terminal.
 It's a simple way to browse your files and take a peek at their contents. Plus it
 works on local and remote file systems.
 
+<details open></summary></summary>
+
 <body>
 <div style="display: grid; grid-template-columns: repeat(2, 1fr); grid-gap: 10px;">
-  <img src="_static/screenshot_utils.png" alt="Image 1">
-  <img src="_static/screenshot_datatable.png" alt="Image 2">
-  <img src="_static/screenshot_mona_lisa.png" alt="Image 3">
-  <img src="_static/screenshot_markdown.png" alt="Image 4">
+    <picture>
+        <img src="docs/_static/screenshot_utils.png" alt="Image 1" href="">
+    </picture>
+    <picture>
+        <img src="docs/_static/screenshot_datatable.png" alt="Image 2" href="">
+    </picture>
+    <picture>
+        <img src="docs/_static/screenshot_mona_lisa.png" alt="Image 3" href="">
+    </picture>
+    <picture>
+        <img src="docs/_static/screenshot_markdown.png" alt="Image 4" href="">
+    </picture>
 </div>
 </body>
 
+</details>
+
 ## Installation
 
 The below command recommends [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx` installs the package in
 an isolated environment and makes it easy to uninstall. If you'd like to use `pip` instead, just replace `pipx`
 with `pip` in the below command.
 
 ```shell
@@ -53,7 +65,13 @@
 
 Simply give `browsr` a path to a file/directory and it will open a browser window
 with a file browser. You can also give it a URL to a remote file system, like AWS S3.
 
 ```shell
 browsr s3://my-bucket/my-file.parquet
 ```
+
+### [Check out the Documentation](https://juftin.com/browsr/) for more
+
+## License
+
+**`browsr`** is distributed under the terms of the [MIT license](LICENSE).
```

#### html2text {}

```diff
@@ -7,20 +7,22 @@
 tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/
 workflows/tests.yaml?query=branch%3Amain) [![GitHub License](https://
 img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://
 github.com/juftin/browsr/blob/main/LICENSE) **`browsr`** is a TUI (text-based
 user interface) file browser for your terminal. It's a simple way to browse
 your files and take a peek at their contents. Plus it works on local and remote
 file systems.
-[Image 1] [Image 2] [Image 3] [Image 4]
-## Installation The below command recommends [pipx](https://pypa.github.io/
+ [Image 1]   [Image 2]   [Image 3]   [Image 4]
+ ## Installation The below command recommends [pipx](https://pypa.github.io/
 pipx/) instead of pip. `pipx` installs the package in an isolated environment
 and makes it easy to uninstall. If you'd like to use `pip` instead, just
 replace `pipx` with `pip` in the below command. ```shell pipx install browsr
 ``` ## Extra Installation If you're looking to use `browsr` on remote file
 systems, like AWS S3, you'll need to install the `remote` extra. If you'd like
 to browse parquet files, you'll need to install the `parquet` extra. Or, even
 simpler, you can install the `all` extra to get all the extras. ```shell pipx
 install "browsr[all]" ``` ## Usage ```shell browsr ~/Downloads/ ``` Simply give
 `browsr` a path to a file/directory and it will open a browser window with a
 file browser. You can also give it a URL to a remote file system, like AWS S3.
-```shell browsr s3://my-bucket/my-file.parquet ```
+```shell browsr s3://my-bucket/my-file.parquet ``` ### [Check out the
+Documentation](https://juftin.com/browsr/) for more ## License **`browsr`** is
+distributed under the terms of the [MIT license](LICENSE).
```

### Comparing `browsr-1.4.0/docs/_static/browsr.png` & `browsr-1.5.0/docs/_static/browsr.png`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/docs/_static/browsr_no_label.png` & `browsr-1.5.0/docs/_static/browsr_no_label.png`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/docs/_static/screenshot_datatable.png` & `browsr-1.5.0/docs/_static/screenshot_datatable.png`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/docs/_static/screenshot_markdown.png` & `browsr-1.5.0/docs/_static/screenshot_markdown.png`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/docs/_static/screenshot_mona_lisa.png` & `browsr-1.5.0/docs/_static/screenshot_mona_lisa.png`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/docs/_static/screenshot_utils.png` & `browsr-1.5.0/docs/_static/screenshot_utils.png`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/requirements/requirements-dev.txt` & `browsr-1.5.0/requirements/requirements-dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1447,17 +1447,17 @@
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via
     #   azure-core
     #   azure-identity
     #   google-auth
     #   isodate
     #   python-dateutil
-textual==0.22.3 \
-    --hash=sha256:1ef6457b9d8b727a67d2344bf2d0b530dce1afab55e1bf4e964e430929301baa \
-    --hash=sha256:a68172f7797e9f269270491e039f1e48096530dff64dbfe893e8477f2d4e200c
+textual==0.24.1 \
+    --hash=sha256:4c7e1f4ed12b9615c63fa3eb7cb9df68d29e0ae5b2352997958cd7ee5533f926 \
+    --hash=sha256:a7deb7ac5a1502424c754fe165ae13cb3890e47ddc514d3f089cb2984c336d1d
     # via -r requirements.in
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   black
     #   build
```

### Comparing `browsr-1.4.0/requirements/requirements-prod.txt` & `browsr-1.5.0/requirements/requirements-prod.txt`

 * *Files 0% similar despite different names*

```diff
@@ -961,17 +961,17 @@
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via
     #   azure-core
     #   azure-identity
     #   google-auth
     #   isodate
     #   python-dateutil
-textual==0.22.3 \
-    --hash=sha256:1ef6457b9d8b727a67d2344bf2d0b530dce1afab55e1bf4e964e430929301baa \
-    --hash=sha256:a68172f7797e9f269270491e039f1e48096530dff64dbfe893e8477f2d4e200c
+textual==0.24.1 \
+    --hash=sha256:4c7e1f4ed12b9615c63fa3eb7cb9df68d29e0ae5b2352997958cd7ee5533f926 \
+    --hash=sha256:a7deb7ac5a1502424c754fe165ae13cb3890e47ddc514d3f089cb2984c336d1d
     # via -r requirements.in
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
     # via
     #   aioitertools
     #   azure-core
```

### Comparing `browsr-1.4.0/.gitignore` & `browsr-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/LICENSE` & `browsr-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `browsr-1.4.0/pyproject.toml` & `browsr-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "art~=5.7",
   "click~=8.1.3",
   "fsspec~=2023.1.0",
   "pandas~=1.5.2",
   "rich~=13.3.5",
   "rich-click~=1.5.2",
   "rich-pixels~=2.1.1",
-  "textual~=0.22.3",
+  "textual~=0.24.1",
   "universal-pathlib~=0.0.21",
   "Pillow>=9.1.0",
   "PyMuPDF~=1.22.3"
 ]
 description = "TUI File Browser App"
 dynamic = ["version"]
 keywords = []
```

### Comparing `browsr-1.4.0/PKG-INFO` & `browsr-1.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browsr
-Version: 1.4.0
+Version: 1.5.0
 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme
 Project-URL: Issues, https://github.com/juftin/browsr/issues
 Project-URL: Source, https://github.com/juftin/browsr
 Author-email: Justin Flannery <justin.flannery@juftin.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -20,15 +20,15 @@
 Requires-Dist: fsspec~=2023.1.0
 Requires-Dist: pandas~=1.5.2
 Requires-Dist: pillow>=9.1.0
 Requires-Dist: pymupdf~=1.22.3
 Requires-Dist: rich-click~=1.5.2
 Requires-Dist: rich-pixels~=2.1.1
 Requires-Dist: rich~=13.3.5
-Requires-Dist: textual~=0.22.3
+Requires-Dist: textual~=0.24.1
 Requires-Dist: universal-pathlib~=0.0.21
 Provides-Extra: all
 Requires-Dist: adlfs~=2023.1.0; extra == 'all'
 Requires-Dist: aiohttp~=3.8.3; extra == 'all'
 Requires-Dist: gcsfs~=2023.1.0; extra == 'all'
 Requires-Dist: pyarrow~=10.0.0; extra == 'all'
 Requires-Dist: requests~=2.28.2; extra == 'all'
@@ -61,18 +61,26 @@
 It's a simple way to browse your files and take a peek at their contents. Plus it
 works on local and remote file systems.
 
 <details open></summary></summary>
 
 <body>
 <div style="display: grid; grid-template-columns: repeat(2, 1fr); grid-gap: 10px;">
-  <img src="docs/_static/screenshot_utils.png" alt="Image 1">
-  <img src="docs/_static/screenshot_datatable.png" alt="Image 2">
-  <img src="docs/_static/screenshot_mona_lisa.png" alt="Image 3">
-  <img src="docs/_static/screenshot_markdown.png" alt="Image 4">
+    <picture>
+        <img src="docs/_static/screenshot_utils.png" alt="Image 1" href="">
+    </picture>
+    <picture>
+        <img src="docs/_static/screenshot_datatable.png" alt="Image 2" href="">
+    </picture>
+    <picture>
+        <img src="docs/_static/screenshot_mona_lisa.png" alt="Image 3" href="">
+    </picture>
+    <picture>
+        <img src="docs/_static/screenshot_markdown.png" alt="Image 4" href="">
+    </picture>
 </div>
 </body>
 
 </details>
 
 ## Installation
 
@@ -103,10 +111,12 @@
 Simply give `browsr` a path to a file/directory and it will open a browser window
 with a file browser. You can also give it a URL to a remote file system, like AWS S3.
 
 ```shell
 browsr s3://my-bucket/my-file.parquet
 ```
 
+### [Check out the Documentation](https://juftin.com/browsr/) for more
+
 ## License
 
 **`browsr`** is distributed under the terms of the [MIT license](LICENSE).
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: browsr Version: 1.4.0 Summary: TUI File Browser App
+Metadata-Version: 2.1 Name: browsr Version: 1.5.0 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme Project-
 URL: Issues, https://github.com/juftin/browsr/issues Project-URL: Source,
 https://github.com/juftin/browsr Author-email: Justin Flannery
 flannery@juftin.com> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: <4.0,>=3.8
 Requires-Dist: art~=5.7 Requires-Dist: click~=8.1.3 Requires-Dist:
 fsspec~=2023.1.0 Requires-Dist: pandas~=1.5.2 Requires-Dist: pillow>=9.1.0
 Requires-Dist: pymupdf~=1.22.3 Requires-Dist: rich-click~=1.5.2 Requires-Dist:
-rich-pixels~=2.1.1 Requires-Dist: rich~=13.3.5 Requires-Dist: textual~=0.22.3
+rich-pixels~=2.1.1 Requires-Dist: rich~=13.3.5 Requires-Dist: textual~=0.24.1
 Requires-Dist: universal-pathlib~=0.0.21 Provides-Extra: all Requires-Dist:
 adlfs~=2023.1.0; extra == 'all' Requires-Dist: aiohttp~=3.8.3; extra == 'all'
 Requires-Dist: gcsfs~=2023.1.0; extra == 'all' Requires-Dist: pyarrow~=10.0.0;
 extra == 'all' Requires-Dist: requests~=2.28.2; extra == 'all' Requires-Dist:
 s3fs~=2023.1.0; extra == 'all' Provides-Extra: parquet Requires-Dist:
 pyarrow~=10.0.0; extra == 'parquet' Provides-Extra: remote Requires-Dist:
 adlfs~=2023.1.0; extra == 'remote' Requires-Dist: aiohttp~=3.8.3; extra ==
@@ -29,21 +29,22 @@
 tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/
 workflows/tests.yaml?query=branch%3Amain) [![GitHub License](https://
 img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://
 github.com/juftin/browsr/blob/main/LICENSE) **`browsr`** is a TUI (text-based
 user interface) file browser for your terminal. It's a simple way to browse
 your files and take a peek at their contents. Plus it works on local and remote
 file systems.
-[Image 1] [Image 2] [Image 3] [Image 4]
+ [Image 1]   [Image 2]   [Image 3]   [Image 4]
  ## Installation The below command recommends [pipx](https://pypa.github.io/
 pipx/) instead of pip. `pipx` installs the package in an isolated environment
 and makes it easy to uninstall. If you'd like to use `pip` instead, just
 replace `pipx` with `pip` in the below command. ```shell pipx install browsr
 ``` ## Extra Installation If you're looking to use `browsr` on remote file
 systems, like AWS S3, you'll need to install the `remote` extra. If you'd like
 to browse parquet files, you'll need to install the `parquet` extra. Or, even
 simpler, you can install the `all` extra to get all the extras. ```shell pipx
 install "browsr[all]" ``` ## Usage ```shell browsr ~/Downloads/ ``` Simply give
 `browsr` a path to a file/directory and it will open a browser window with a
 file browser. You can also give it a URL to a remote file system, like AWS S3.
-```shell browsr s3://my-bucket/my-file.parquet ``` ## License **`browsr`** is
+```shell browsr s3://my-bucket/my-file.parquet ``` ### [Check out the
+Documentation](https://juftin.com/browsr/) for more ## License **`browsr`** is
 distributed under the terms of the [MIT license](LICENSE).
```

