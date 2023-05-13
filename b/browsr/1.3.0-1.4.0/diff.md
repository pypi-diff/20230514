# Comparing `tmp/browsr-1.3.0.tar.gz` & `tmp/browsr-1.4.0.tar.gz`

## Comparing `browsr-1.3.0.tar` & `browsr-1.4.0.tar`

### file list

```diff
@@ -1,34 +1,41 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.3.0/.releaserc.js
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 browsr-1.3.0/mkdocs.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/__init__.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/__main__.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/_base.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/_config.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/_utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/_version.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/browsr.css
--rw-r--r--   0        0        0    10712 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/browsr.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 browsr-1.3.0/docs/api_documentation.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.3.0/docs/cli.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.3.0/docs/contributing.md
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 browsr-1.3.0/docs/index.md
--rw-r--r--   0        0        0   118212 2020-02-02 00:00:00.000000 browsr-1.3.0/requirements/requirements-dev.txt
--rw-r--r--   0        0        0    82526 2020-02-02 00:00:00.000000 browsr-1.3.0/requirements/requirements-prod.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 browsr-1.3.0/tests/test_cli.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.3.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 browsr-1.3.0/README.md
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 browsr-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 browsr-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.4.0/.releaserc.js
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 browsr-1.4.0/mkdocs.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.4.0/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/__main__.py
+-rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/_base.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/_cli.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/_config.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/_utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/_version.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/browsr.css
+-rw-r--r--   0        0        0    12920 2020-02-02 00:00:00.000000 browsr-1.4.0/browsr/browsr.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/cli.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/contributing.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/index.md
+-rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/_static/browsr.png
+-rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/_static/browsr_no_label.png
+-rw-r--r--   0        0        0  1112808 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/_static/screenshot_datatable.png
+-rw-r--r--   0        0        0   838657 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/_static/screenshot_markdown.png
+-rw-r--r--   0        0        0  1550033 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/_static/screenshot_mona_lisa.png
+-rw-r--r--   0        0        0  1031902 2020-02-02 00:00:00.000000 browsr-1.4.0/docs/_static/screenshot_utils.png
+-rw-r--r--   0        0        0   118970 2020-02-02 00:00:00.000000 browsr-1.4.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0    82526 2020-02-02 00:00:00.000000 browsr-1.4.0/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.4.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 browsr-1.4.0/README.md
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 browsr-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 browsr-1.4.0/PKG-INFO
```

### Comparing `browsr-1.3.0/.pre-commit-config.yaml` & `browsr-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/.releaserc.js` & `browsr-1.4.0/.releaserc.js`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/mkdocs.yaml` & `browsr-1.4.0/mkdocs.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # schema: https://squidfunk.github.io/mkdocs-material/schema.json
 
 site_name: browsr
 nav:
     - index.md
     - Command Line Interface ⌨️: cli.md
     - Contributing 🤝: contributing.md
-    - API Documentation 🤖: api_documentation.md
+    - API Documentation 🤖: reference/
 theme:
-    favicon: https://raw.githubusercontent.com/juftin/juftin/main/static/juftin.png
-    logo: https://i.imgur.com/QiAXcEm.png
+    favicon: _static/browsr_no_label.png
+    logo: _static/browsr_no_label.png
     name: material
     features:
         - navigation.tracking
         - content.code.annotate
         - content.code.copy
-        - navigation.indexes
     palette:
         - media: "(prefers-color-scheme: light)"
           scheme: default
           accent: purple
           toggle:
               icon: material/weather-sunny
               name: Switch to dark mode
@@ -53,14 +52,20 @@
           custom_checkbox: true
     - pymdownx.tilde
     - admonition
     - pymdownx.details
     - mkdocs-click
 plugins:
     - search
+    - gen-files:
+          scripts:
+              - docs/gen_ref_pages.py
+    - literate-nav:
+          nav_file: SUMMARY.md
+    - section-index:
     - mkdocstrings:
           handlers:
               python:
                   import:
                       - https://docs.python.org/3/objects.inv
                       - https://numpy.org/doc/stable/objects.inv
                       - https://pandas.pydata.org/docs/objects.inv
```

### Comparing `browsr-1.3.0/.github/semantic_release/package-lock.json` & `browsr-1.4.0/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/.github/semantic_release/release_notes.hbs` & `browsr-1.4.0/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/.github/workflows/lint.yaml` & `browsr-1.4.0/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/.github/workflows/publish.yaml` & `browsr-1.4.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/.github/workflows/release.yaml` & `browsr-1.4.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/.github/workflows/tests.yaml` & `browsr-1.4.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/browsr/_config.py` & `browsr-1.4.0/browsr/_config.py`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/browsr/browsr.py` & `browsr-1.4.0/browsr/browsr.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,81 +3,87 @@
 
 This module contains the code browser app for the browsr package.
 This app was inspired by the CodeBrowser example from textual
 """
 
 import json
 import pathlib
+import shutil
+from textwrap import dedent
 from typing import TYPE_CHECKING, Any, Iterable, Optional, Union
 
-import click
 import pandas as pd
-import rich_click
 import upath
 from art import text2art  # type: ignore[import]
-from rich import traceback
 from rich.markdown import Markdown
 from rich.syntax import Syntax
 from rich.traceback import Traceback
 from rich_pixels import Pixels
-from textual.containers import Container, VerticalScroll
+from textual.binding import Binding
+from textual.containers import Container, Horizontal, VerticalScroll
 from textual.reactive import var
 from textual.widget import Widget
 from textual.widgets import DataTable, DirectoryTree, Footer, Header, Static
 from upath.implementations.cloud import CloudPath
 
 from browsr._base import (
-    BrowsrClickContext,
     BrowsrTextualApp,
+    ConfirmationPopUp,
+    CurrentFileInfoBar,
     FileSizeError,
     TextualAppContext,
     UniversalDirectoryTree,
-    debug_option,
 )
 from browsr._config import favorite_themes, image_file_extensions
-from browsr._utils import open_image
-from browsr._version import __application__, __version__
+from browsr._utils import (
+    FileInfo,
+    get_file_info,
+    handle_duplicate_filenames,
+    open_image,
+)
+from browsr._version import __application__
 
 
-class CodeBrowser(BrowsrTextualApp):
+class Browsr(BrowsrTextualApp):
     """
     Textual code browser app.
     """
 
     TITLE = __application__
     CSS_PATH = "browsr.css"
     BINDINGS = [
-        ("q", "quit", "Quit"),
-        ("f", "toggle_files", "Toggle Files"),
-        ("t", "theme", "Toggle Theme"),
-        ("n", "linenos", "Toggle Line Numbers"),
-        ("d", "toggle_dark", "Toggle dark mode"),
+        Binding("q", "quit", "Quit"),
+        Binding("f", "toggle_files", "Toggle Files"),
+        Binding("t", "theme", "Toggle Theme"),
+        Binding("n", "linenos", "Toggle Line Numbers"),
+        Binding("d", "toggle_dark", "Toggle Dark Mode"),
     ]
 
     show_tree = var(True)
     theme_index = var(0)
     linenos = var(False)
     rich_themes = favorite_themes
     selected_file_path: Union[upath.UPath, pathlib.Path, None, var[None]] = var(None)
     force_show_tree = var(False)
-
-    traceback.install(show_locals=True)
+    hidden_table_view = var(False)
 
     def watch_show_tree(self, show_tree: bool) -> None:
         """
         Called when show_tree is modified.
         """
         self.set_class(show_tree, "-show-tree")
 
     def compose(self) -> Iterable[Widget]:
         """
         Compose our UI.
         """
         assert isinstance(self.config_object, TextualAppContext)
         file_path = self.config_object.path
+        if isinstance(file_path, CloudPath):
+            self.bind("x", "download_file", description="Download File", show=True)
         if file_path.is_file():
             self.selected_file_path = file_path
             file_path = file_path.parent
         elif file_path.is_dir() and file_path.joinpath("README.md").exists():
             if TYPE_CHECKING:
                 assert isinstance(file_path, pathlib.Path)
             self.selected_file_path = file_path.joinpath("README.md")
@@ -86,16 +92,36 @@
         yield self.header
         self.directory_tree = UniversalDirectoryTree(str(file_path), id="tree-view")
         self.code_view = VerticalScroll(Static(id="code", expand=True), id="code-view")
         self.table_view: DataTable[str] = DataTable(
             zebra_stripes=True, show_header=True, show_cursor=True, id="table-view"
         )
         self.table_view.display = False
-        self.container = Container(self.directory_tree, self.code_view, self.table_view)
+        self.confirmation = ConfirmationPopUp()
+        self.confirmation_window = Container(
+            self.confirmation, id="confirmation-container"
+        )
+        self.confirmation_window.display = False
+        self.container = Container(
+            self.directory_tree,
+            self.code_view,
+            self.table_view,
+            self.confirmation_window,
+        )
         yield self.container
+        self.file_information = CurrentFileInfoBar()
+        self.info_bar = Horizontal(
+            self.file_information,
+            id="file-info-bar",
+        )
+        if self.selected_file_path is not None:
+            self.file_information.file_info = get_file_info(
+                file_path=self.selected_file_path
+            )
+        yield self.info_bar
         self.footer = Footer()
         yield self.footer
 
     def render_document(
         self,
         document: pathlib.Path,
     ) -> Union[Syntax, Markdown, DataTable[str], Pixels]:
@@ -124,17 +150,20 @@
             df = pd.read_parquet(document)[:500]
             return self.df_to_table(pandas_dataframe=df, table=self.table_view)
         elif document.suffix.lower() in image_file_extensions:
             screen_width = self.app.size.width / 4
             content = open_image(document=document, screen_width=screen_width)
             return content
         elif document.suffix.lower() in [".json"]:
-            code_str = document.read_text()
-            code_obj = json.loads(code_str)
-            code_lines = json.dumps(code_obj, indent=2).splitlines()
+            code_str = document.read_text(encoding="utf-8", errors="replace")
+            try:
+                code_obj = json.loads(code_str)
+                code_lines = json.dumps(code_obj, indent=2).splitlines()
+            except json.JSONDecodeError:
+                code_lines = code_str.splitlines()
         else:
             code_lines = document.read_text(
                 encoding="utf-8", errors="replace"
             ).splitlines()
         code = "\n".join(code_lines[:1000])
         lexer = Syntax.guess_lexer(str(document), code=code)
         return Syntax(
@@ -142,30 +171,24 @@
             lexer=lexer,
             line_numbers=self.linenos,
             word_wrap=False,
             indent_guides=False,
             theme=self.rich_themes[self.theme_index],
         )
 
-    @classmethod
-    def _handle_file_size(cls, file_path: pathlib.Path) -> None:
+    def _handle_file_size(self, file_info: FileInfo) -> None:
         """
         Handle a File Size
         """
-        stat = file_path.stat()
-        if isinstance(stat, dict):
-            file_size = {key.lower(): value for key, value in stat.items()}["size"]
-            file_size_mb = file_size / 1000 / 1000
-        else:
-            file_size_mb = stat.st_size / 1000 / 1000
-        max_file_size = 8
-        too_large = file_size_mb >= max_file_size
+        file_size_mb = file_info.size / 1000 / 1000
+        too_large = file_size_mb >= self.config_object.max_file_size  # type: ignore[union-attr]
         exception = (
             True
-            if not isinstance(file_path, CloudPath) and ".csv" in file_path.suffixes
+            if not isinstance(file_info.file, CloudPath)
+            and ".csv" in file_info.file.suffixes
             else False
         )
         if too_large is True and exception is not True:
             raise FileSizeError("File too large")
 
     def render_code_page(
         self,
@@ -178,16 +201,17 @@
         """
         code_view = self.query_one("#code", Static)
         font = "univers"
         if content is not None:
             code_view.update(text2art(content, font=font))
             return
         try:
-            self._handle_file_size(file_path=file_path)
-            element = self.render_document(document=file_path)
+            file_info = get_file_info(file_path=file_path)
+            self._handle_file_size(file_info=file_info)
+            element = self.render_document(document=file_info.file)
         except FileSizeError:
             self.table_view.display = False
             self.code_view.display = True
             code_view.update(
                 text2art("FILE TOO", font=font) + "\n\n" + text2art("LARGE", font=font)
             )
             self.sub_title = f"ERROR [{self.rich_themes[self.theme_index]}]"
@@ -244,15 +268,17 @@
     def on_directory_tree_file_selected(
         self, event: DirectoryTree.FileSelected
     ) -> None:
         """
         Called when the user click a file in the directory tree.
         """
         self.selected_file_path = upath.UPath(event.path)
+        file_info = get_file_info(file_path=self.selected_file_path)
         self.render_code_page(file_path=upath.UPath(event.path))
+        self.file_information.file_info = file_info
 
     def action_toggle_files(self) -> None:
         """
         Called in response to key binding.
         """
         self.show_tree = not self.show_tree
 
@@ -273,34 +299,58 @@
         An action to toggle line numbers.
         """
         if self.selected_file_path is None:
             return
         self.linenos = not self.linenos
         self.render_code_page(file_path=self.selected_file_path, scroll_home=False)
 
+    def _get_download_file_name(self) -> pathlib.Path:
+        """
+        Get the download file name.
+        """
+        download_dir = pathlib.Path.home() / "Downloads"
+        if not download_dir.exists():
+            raise FileNotFoundError(f"Download directory {download_dir} not found")
+        download_path = download_dir / self.selected_file_path.name  # type: ignore[union-attr]
+        handled_download_path = handle_duplicate_filenames(file_path=download_path)
+        return handled_download_path
 
-@click.command(name="browsr", cls=rich_click.rich_command.RichCommand)
-@click.argument("path", default=None, required=False, metavar="PATH")
-@click.version_option(version=__version__, prog_name=__application__)
-@click.pass_obj
-@debug_option
-def browsr(
-    context: Optional[BrowsrClickContext], path: Optional[str], debug: bool
-) -> None:
-    """
-    Start the TUI File Browser
+    def download_selected_file(self) -> None:
+        """
+        Download the selected file.
+        """
+        if self.selected_file_path is None:
+            return
+        elif self.selected_file_path.is_dir():
+            return
+        elif isinstance(self.selected_file_path, CloudPath):
+            handled_download_path = self._get_download_file_name()
+            with self.selected_file_path.open("rb") as file_handle:
+                with handled_download_path.open("wb") as download_handle:
+                    shutil.copyfileobj(file_handle, download_handle)
 
-    This utility displays a TUI (textual user interface) application. The application
-    allows you to visually browse through a repository and display the contents of its
-    files
-    """
-    if context is None:
-        context = BrowsrClickContext(debug=debug)
-    elif context.debug is False:
-        context.debug = debug
-    config = TextualAppContext(file_path=path, debug=context.debug)
-    app = CodeBrowser(config_object=config)
-    app.run()
+    def action_download_file(self) -> None:
+        """
+        Download the selected file.
+        """
+        if self.selected_file_path is None:
+            return
+        elif self.selected_file_path.is_dir():
+            return
+        elif isinstance(self.selected_file_path, CloudPath):
+            handled_download_path = self._get_download_file_name()
+            prompt_message: str = dedent(
+                f"""
+                ## File Download
 
+                **Are you sure you want to download that file?**
 
-if __name__ == "__main__":
-    browsr()
+                **File:** `{self.selected_file_path}`
+
+                **Path:** `{handled_download_path}`
+                """
+            )
+            self.confirmation.download_message.update(Markdown(prompt_message))
+            self.confirmation.refresh()
+            self.hidden_table_view = self.table_view.display
+            self.table_view.display = False
+            self.confirmation_window.display = True
```

### Comparing `browsr-1.3.0/docs/contributing.md` & `browsr-1.4.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/docs/index.md` & `browsr-1.4.0/docs/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,59 @@
 # browsr
 
 <div align="center">
 <a href="https://github.com/juftin/browsr">
-  <img src=https://i.imgur.com/QiAXcEm.png
+  <img src=_static/browsr.png
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
 
----
-
-**Table of Contents**
-
--   [Installation](#installation)
-    -   [Extra Installation](#extra-installation)
--   [Usage](#usage)
--   [License](#license)
-
 <body>
 <div style="display: grid; grid-template-columns: repeat(2, 1fr); grid-gap: 10px;">
-  <img src="https://i.imgur.com/6apkI2Q.png" alt="Image 1">
-  <img src="https://i.imgur.com/y7ZLRTX.png" alt="Image 2">
-  <img src="https://i.imgur.com/oRBJ0vj.png" alt="Image 3">
-  <img src="https://i.imgur.com/HWSjWCY.png" alt="Image 4">
+  <img src="_static/screenshot_utils.png" alt="Image 1">
+  <img src="_static/screenshot_datatable.png" alt="Image 2">
+  <img src="_static/screenshot_mona_lisa.png" alt="Image 3">
+  <img src="_static/screenshot_markdown.png" alt="Image 4">
 </div>
 </body>
 
 ## Installation
 
 The below command recommends [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx` installs the package in
 an isolated environment and makes it easy to uninstall. If you'd like to use `pip` instead, just replace `pipx`
 with `pip` in the below command.
 
-```console
+```shell
 pipx install browsr
 ```
 
 ## Extra Installation
 
 If you're looking to use `browsr` on remote file systems, like AWS S3, you'll need to install the `remote` extra.
 If you'd like to browse parquet files, you'll need to install the `parquet` extra. Or, even simpler,
 you can install the `all` extra to get all the extras.
 
-```console
+```shell
 pipx install "browsr[all]"
 ```
 
 ## Usage
 
-```console
+```shell
 browsr ~/Downloads/
 ```
 
 Simply give `browsr` a path to a file/directory and it will open a browser window
 with a file browser. You can also give it a URL to a remote file system, like AWS S3.
 
-```console
+```shell
 browsr s3://my-bucket/my-file.parquet
 ```
-
-## License
-
-`browsr` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

#### html2text {}

```diff
@@ -6,25 +6,21 @@
 browsr/) [![Testing Status](https://github.com/juftin/browsr/actions/workflows/
 tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/
 workflows/tests.yaml?query=branch%3Amain) [![GitHub License](https://
 img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://
 github.com/juftin/browsr/blob/main/LICENSE) **`browsr`** is a TUI (text-based
 user interface) file browser for your terminal. It's a simple way to browse
 your files and take a peek at their contents. Plus it works on local and remote
-file systems. --- **Table of Contents** - [Installation](#installation) -
-[Extra Installation](#extra-installation) - [Usage](#usage) - [License]
-(#license)
+file systems.
 [Image 1] [Image 2] [Image 3] [Image 4]
 ## Installation The below command recommends [pipx](https://pypa.github.io/
 pipx/) instead of pip. `pipx` installs the package in an isolated environment
 and makes it easy to uninstall. If you'd like to use `pip` instead, just
-replace `pipx` with `pip` in the below command. ```console pipx install browsr
+replace `pipx` with `pip` in the below command. ```shell pipx install browsr
 ``` ## Extra Installation If you're looking to use `browsr` on remote file
 systems, like AWS S3, you'll need to install the `remote` extra. If you'd like
 to browse parquet files, you'll need to install the `parquet` extra. Or, even
-simpler, you can install the `all` extra to get all the extras. ```console pipx
-install "browsr[all]" ``` ## Usage ```console browsr ~/Downloads/ ``` Simply
-give `browsr` a path to a file/directory and it will open a browser window with
-a file browser. You can also give it a URL to a remote file system, like AWS
-S3. ```console browsr s3://my-bucket/my-file.parquet ``` ## License `browsr` is
-distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html)
-license.
+simpler, you can install the `all` extra to get all the extras. ```shell pipx
+install "browsr[all]" ``` ## Usage ```shell browsr ~/Downloads/ ``` Simply give
+`browsr` a path to a file/directory and it will open a browser window with a
+file browser. You can also give it a URL to a remote file system, like AWS S3.
+```shell browsr s3://my-bucket/my-file.parquet ```
```

### Comparing `browsr-1.3.0/requirements/requirements-dev.txt` & `browsr-1.4.0/requirements/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -767,32 +767,47 @@
     # via mkdocs
 mkdocs==1.4.3 \
     --hash=sha256:5955093bbd4dd2e9403c5afaf57324ad8b04f16886512a3ee6ef828956481c57 \
     --hash=sha256:6ee46d309bda331aac915cd24aab882c179a933bd9e77b80ce7d2eaaa3f689dd
     # via
     #   -r requirements.in
     #   mkdocs-autorefs
+    #   mkdocs-gen-files
+    #   mkdocs-literate-nav
     #   mkdocs-material
+    #   mkdocs-section-index
     #   mkdocstrings
 mkdocs-autorefs==0.4.1 \
     --hash=sha256:70748a7bd025f9ecd6d6feeba8ba63f8e891a1af55f48e366d6d6e78493aba84 \
     --hash=sha256:a2248a9501b29dc0cc8ba4c09f4f47ff121945f6ce33d760f145d6f89d313f5b
     # via mkdocstrings
 mkdocs-click==0.8.0 \
     --hash=sha256:965f38231eb04d8c980406c5ab4becf7303ef3ffc68fdb29be91927eff1adfbe \
     --hash=sha256:f9c26d4abd505bca4113d1529d03d1ae709a68a82fc364db289634788d029353
     # via -r requirements.in
+mkdocs-gen-files==0.4.0 \
+    --hash=sha256:3241a4c947ecd11763ca77cc645015305bf71a0e1b9b886801c114fcf9971e71 \
+    --hash=sha256:377bff8ee8e93515916689f483d971643f83a94eed7e92318854da8f344f0163
+    # via -r requirements.in
+mkdocs-literate-nav==0.6.0 \
+    --hash=sha256:81ccbea18163ae8e10bd0bd39237fe70c32a1f2dff6c170779f5d52dd98a0470 \
+    --hash=sha256:8c1b84714e5974da5e44e011ec0069275ae7647270c13a679662cf6ffce675a4
+    # via -r requirements.in
 mkdocs-material==9.1.9 \
     --hash=sha256:74d8da1371ab3a326868fe47bae3cbc4aa22e93c048b4ca5117e6817b88bd734 \
     --hash=sha256:7db24261cb17400e132c46d17eea712bfe71056d892a9beba32cf68210297141
     # via -r requirements.in
 mkdocs-material-extensions==1.1.1 \
     --hash=sha256:9c003da71e2cc2493d910237448c672e00cefc800d3d6ae93d2fc69979e3bd93 \
     --hash=sha256:e41d9f38e4798b6617ad98ca8f7f1157b1e4385ac1459ca1e4ea219b556df945
     # via mkdocs-material
+mkdocs-section-index==0.3.5 \
+    --hash=sha256:1f6359287b0a823d6297cf1cb6c0a49ed75851d0d1cea8b425b207a45ce10141 \
+    --hash=sha256:fa8b1ce0649326b1873c6460c1df2bb0c4825fd21e3dd416f13ec212d31edf12
+    # via -r requirements.in
 mkdocstrings[python]==0.21.2 \
     --hash=sha256:304e56a2e90595708a38a13a278e538a67ad82052dd5c8b71f77a604a4f3d911 \
     --hash=sha256:949ef8da92df9d692ca07be50616459a6b536083a25520fd54b00e8814ce019b
     # via
     #   -r requirements.in
     #   mkdocstrings-python
 mkdocstrings-python==0.9.0 \
```

### Comparing `browsr-1.3.0/requirements/requirements-prod.txt` & `browsr-1.4.0/requirements/requirements-prod.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/.gitignore` & `browsr-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/LICENSE.txt` & `browsr-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `browsr-1.3.0/README.md` & `browsr-1.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 # browsr
 
 <div align="center">
 <a href="https://github.com/juftin/browsr">
-  <img src=https://i.imgur.com/QiAXcEm.png
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
 
----
+<details open></summary></summary>
 
 <body>
 <div style="display: grid; grid-template-columns: repeat(2, 1fr); grid-gap: 10px;">
-  <img src="https://i.imgur.com/6apkI2Q.png" alt="Image 1">
-  <img src="https://i.imgur.com/y7ZLRTX.png" alt="Image 2">
-  <img src="https://i.imgur.com/oRBJ0vj.png" alt="Image 3">
-  <img src="https://i.imgur.com/HWSjWCY.png" alt="Image 4">
+  <img src="docs/_static/screenshot_utils.png" alt="Image 1">
+  <img src="docs/_static/screenshot_datatable.png" alt="Image 2">
+  <img src="docs/_static/screenshot_mona_lisa.png" alt="Image 3">
+  <img src="docs/_static/screenshot_markdown.png" alt="Image 4">
 </div>
 </body>
 
+</details>
+
 ## Installation
 
 The below command recommends [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx` installs the package in
 an isolated environment and makes it easy to uninstall. If you'd like to use `pip` instead, just replace `pipx`
 with `pip` in the below command.
 
-```console
+```shell
 pipx install browsr
 ```
 
 ## Extra Installation
 
 If you're looking to use `browsr` on remote file systems, like AWS S3, you'll need to install the `remote` extra.
 If you'd like to browse parquet files, you'll need to install the `parquet` extra. Or, even simpler,
 you can install the `all` extra to get all the extras.
 
-```console
+```shell
 pipx install "browsr[all]"
 ```
 
 ## Usage
 
-```console
+```shell
 browsr ~/Downloads/
 ```
 
 Simply give `browsr` a path to a file/directory and it will open a browser window
 with a file browser. You can also give it a URL to a remote file system, like AWS S3.
 
-```console
+```shell
 browsr s3://my-bucket/my-file.parquet
 ```
 
 ## License
 
-`browsr` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+**`browsr`** is distributed under the terms of the [MIT license](LICENSE).
```

#### html2text {}

```diff
@@ -6,23 +6,22 @@
 browsr/) [![Testing Status](https://github.com/juftin/browsr/actions/workflows/
 tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/
 workflows/tests.yaml?query=branch%3Amain) [![GitHub License](https://
 img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://
 github.com/juftin/browsr/blob/main/LICENSE) **`browsr`** is a TUI (text-based
 user interface) file browser for your terminal. It's a simple way to browse
 your files and take a peek at their contents. Plus it works on local and remote
-file systems. ---
+file systems.
 [Image 1] [Image 2] [Image 3] [Image 4]
-## Installation The below command recommends [pipx](https://pypa.github.io/
+ ## Installation The below command recommends [pipx](https://pypa.github.io/
 pipx/) instead of pip. `pipx` installs the package in an isolated environment
 and makes it easy to uninstall. If you'd like to use `pip` instead, just
-replace `pipx` with `pip` in the below command. ```console pipx install browsr
+replace `pipx` with `pip` in the below command. ```shell pipx install browsr
 ``` ## Extra Installation If you're looking to use `browsr` on remote file
 systems, like AWS S3, you'll need to install the `remote` extra. If you'd like
 to browse parquet files, you'll need to install the `parquet` extra. Or, even
-simpler, you can install the `all` extra to get all the extras. ```console pipx
-install "browsr[all]" ``` ## Usage ```console browsr ~/Downloads/ ``` Simply
-give `browsr` a path to a file/directory and it will open a browser window with
-a file browser. You can also give it a URL to a remote file system, like AWS
-S3. ```console browsr s3://my-bucket/my-file.parquet ``` ## License `browsr` is
-distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html)
-license.
+simpler, you can install the `all` extra to get all the extras. ```shell pipx
+install "browsr[all]" ``` ## Usage ```shell browsr ~/Downloads/ ``` Simply give
+`browsr` a path to a file/directory and it will open a browser window with a
+file browser. You can also give it a URL to a remote file system, like AWS S3.
+```shell browsr s3://my-bucket/my-file.parquet ``` ## License **`browsr`** is
+distributed under the terms of the [MIT license](LICENSE).
```

### Comparing `browsr-1.3.0/pyproject.toml` & `browsr-1.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,17 @@
   "pytest~=7.3.1",
   "pytest-cov~=4.0.0",
   "pytest-mock~=3.10.0",
   "mkdocs~=1.4.2",
   "mkdocs-material~=9.1.6",
   "mkdocs-click~=0.8.0",
   "mkdocstrings[python]~=0.21.2",
+  "mkdocs-gen-files~=0.4.0",
+  "mkdocs-literate-nav~=0.6.0",
+  "mkdocs-section-index~=0.3.5",
   "black~=23.3.0",
   "ruff~=0.0.261",
   "mypy~=1.2.0",
   "pandas-stubs~=2.0.0.230412",
   "pip-tools~=6.13.0"
 ]
 features = ["all"]
```

### Comparing `browsr-1.3.0/PKG-INFO` & `browsr-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: browsr
-Version: 1.3.0
+Version: 1.4.0
 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme
 Project-URL: Issues, https://github.com/juftin/browsr/issues
 Project-URL: Source, https://github.com/juftin/browsr
 Author-email: Justin Flannery <justin.flannery@juftin.com>
 License-Expression: MIT
-License-File: LICENSE.txt
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <4.0,>=3.8
@@ -43,68 +43,70 @@
 Requires-Dist: s3fs~=2023.1.0; extra == 'remote'
 Description-Content-Type: text/markdown
 
 # browsr
 
 <div align="center">
 <a href="https://github.com/juftin/browsr">
-  <img src=https://i.imgur.com/QiAXcEm.png
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
 
----
+<details open></summary></summary>
 
 <body>
 <div style="display: grid; grid-template-columns: repeat(2, 1fr); grid-gap: 10px;">
-  <img src="https://i.imgur.com/6apkI2Q.png" alt="Image 1">
-  <img src="https://i.imgur.com/y7ZLRTX.png" alt="Image 2">
-  <img src="https://i.imgur.com/oRBJ0vj.png" alt="Image 3">
-  <img src="https://i.imgur.com/HWSjWCY.png" alt="Image 4">
+  <img src="docs/_static/screenshot_utils.png" alt="Image 1">
+  <img src="docs/_static/screenshot_datatable.png" alt="Image 2">
+  <img src="docs/_static/screenshot_mona_lisa.png" alt="Image 3">
+  <img src="docs/_static/screenshot_markdown.png" alt="Image 4">
 </div>
 </body>
 
+</details>
+
 ## Installation
 
 The below command recommends [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx` installs the package in
 an isolated environment and makes it easy to uninstall. If you'd like to use `pip` instead, just replace `pipx`
 with `pip` in the below command.
 
-```console
+```shell
 pipx install browsr
 ```
 
 ## Extra Installation
 
 If you're looking to use `browsr` on remote file systems, like AWS S3, you'll need to install the `remote` extra.
 If you'd like to browse parquet files, you'll need to install the `parquet` extra. Or, even simpler,
 you can install the `all` extra to get all the extras.
 
-```console
+```shell
 pipx install "browsr[all]"
 ```
 
 ## Usage
 
-```console
+```shell
 browsr ~/Downloads/
 ```
 
 Simply give `browsr` a path to a file/directory and it will open a browser window
 with a file browser. You can also give it a URL to a remote file system, like AWS S3.
 
-```console
+```shell
 browsr s3://my-bucket/my-file.parquet
 ```
 
 ## License
 
-`browsr` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+**`browsr`** is distributed under the terms of the [MIT license](LICENSE).
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: browsr Version: 1.3.0 Summary: TUI File Browser App
+Metadata-Version: 2.1 Name: browsr Version: 1.4.0 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme Project-
 URL: Issues, https://github.com/juftin/browsr/issues Project-URL: Source,
 https://github.com/juftin/browsr Author-email: Justin Flannery
-flannery@juftin.com> License-Expression: MIT License-File: LICENSE.txt
-Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Python: <4.0,>=3.8 Requires-Dist: art~=5.7 Requires-Dist: click~=8.1.3
-Requires-Dist: fsspec~=2023.1.0 Requires-Dist: pandas~=1.5.2 Requires-Dist:
-pillow>=9.1.0 Requires-Dist: pymupdf~=1.22.3 Requires-Dist: rich-click~=1.5.2
-Requires-Dist: rich-pixels~=2.1.1 Requires-Dist: rich~=13.3.5 Requires-Dist:
-textual~=0.22.3 Requires-Dist: universal-pathlib~=0.0.21 Provides-Extra: all
-Requires-Dist: adlfs~=2023.1.0; extra == 'all' Requires-Dist: aiohttp~=3.8.3;
-extra == 'all' Requires-Dist: gcsfs~=2023.1.0; extra == 'all' Requires-Dist:
-pyarrow~=10.0.0; extra == 'all' Requires-Dist: requests~=2.28.2; extra == 'all'
-Requires-Dist: s3fs~=2023.1.0; extra == 'all' Provides-Extra: parquet Requires-
-Dist: pyarrow~=10.0.0; extra == 'parquet' Provides-Extra: remote Requires-Dist:
+flannery@juftin.com> License-Expression: MIT License-File: LICENSE Classifier:
+Development Status :: 4 - Beta Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: <4.0,>=3.8
+Requires-Dist: art~=5.7 Requires-Dist: click~=8.1.3 Requires-Dist:
+fsspec~=2023.1.0 Requires-Dist: pandas~=1.5.2 Requires-Dist: pillow>=9.1.0
+Requires-Dist: pymupdf~=1.22.3 Requires-Dist: rich-click~=1.5.2 Requires-Dist:
+rich-pixels~=2.1.1 Requires-Dist: rich~=13.3.5 Requires-Dist: textual~=0.22.3
+Requires-Dist: universal-pathlib~=0.0.21 Provides-Extra: all Requires-Dist:
+adlfs~=2023.1.0; extra == 'all' Requires-Dist: aiohttp~=3.8.3; extra == 'all'
+Requires-Dist: gcsfs~=2023.1.0; extra == 'all' Requires-Dist: pyarrow~=10.0.0;
+extra == 'all' Requires-Dist: requests~=2.28.2; extra == 'all' Requires-Dist:
+s3fs~=2023.1.0; extra == 'all' Provides-Extra: parquet Requires-Dist:
+pyarrow~=10.0.0; extra == 'parquet' Provides-Extra: remote Requires-Dist:
 adlfs~=2023.1.0; extra == 'remote' Requires-Dist: aiohttp~=3.8.3; extra ==
 'remote' Requires-Dist: gcsfs~=2023.1.0; extra == 'remote' Requires-Dist:
 requests~=2.28.2; extra == 'remote' Requires-Dist: s3fs~=2023.1.0; extra ==
 'remote' Description-Content-Type: text/markdown # browsr
                                    [browsr]
 [![browsr Version](https://img.shields.io/pypi/v/
 browsr?color=blue&label=browsr)](https://github.com/juftin/browsr) [![PyPI]
@@ -28,23 +28,22 @@
 browsr/) [![Testing Status](https://github.com/juftin/browsr/actions/workflows/
 tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/
 workflows/tests.yaml?query=branch%3Amain) [![GitHub License](https://
 img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://
 github.com/juftin/browsr/blob/main/LICENSE) **`browsr`** is a TUI (text-based
 user interface) file browser for your terminal. It's a simple way to browse
 your files and take a peek at their contents. Plus it works on local and remote
-file systems. ---
+file systems.
 [Image 1] [Image 2] [Image 3] [Image 4]
-## Installation The below command recommends [pipx](https://pypa.github.io/
+ ## Installation The below command recommends [pipx](https://pypa.github.io/
 pipx/) instead of pip. `pipx` installs the package in an isolated environment
 and makes it easy to uninstall. If you'd like to use `pip` instead, just
-replace `pipx` with `pip` in the below command. ```console pipx install browsr
+replace `pipx` with `pip` in the below command. ```shell pipx install browsr
 ``` ## Extra Installation If you're looking to use `browsr` on remote file
 systems, like AWS S3, you'll need to install the `remote` extra. If you'd like
 to browse parquet files, you'll need to install the `parquet` extra. Or, even
-simpler, you can install the `all` extra to get all the extras. ```console pipx
-install "browsr[all]" ``` ## Usage ```console browsr ~/Downloads/ ``` Simply
-give `browsr` a path to a file/directory and it will open a browser window with
-a file browser. You can also give it a URL to a remote file system, like AWS
-S3. ```console browsr s3://my-bucket/my-file.parquet ``` ## License `browsr` is
-distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html)
-license.
+simpler, you can install the `all` extra to get all the extras. ```shell pipx
+install "browsr[all]" ``` ## Usage ```shell browsr ~/Downloads/ ``` Simply give
+`browsr` a path to a file/directory and it will open a browser window with a
+file browser. You can also give it a URL to a remote file system, like AWS S3.
+```shell browsr s3://my-bucket/my-file.parquet ``` ## License **`browsr`** is
+distributed under the terms of the [MIT license](LICENSE).
```

