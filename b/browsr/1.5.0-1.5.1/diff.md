# Comparing `tmp/browsr-1.5.0.tar.gz` & `tmp/browsr-1.5.1.tar.gz`

## Comparing `browsr-1.5.0.tar` & `browsr-1.5.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.5.0/.releaserc.js
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 browsr-1.5.0/mkdocs.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.5.0/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/__main__.py
--rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/_base.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/_cli.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/_config.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/_utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/_version.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/browsr.css
--rw-r--r--   0        0        0    12920 2020-02-02 00:00:00.000000 browsr-1.5.0/browsr/browsr.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/cli.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/contributing.md
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/index.md
--rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/_static/browsr.png
--rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/_static/browsr_no_label.png
--rw-r--r--   0        0        0  1112808 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/_static/screenshot_datatable.png
--rw-r--r--   0        0        0   838657 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/_static/screenshot_markdown.png
--rw-r--r--   0        0        0  1550033 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/_static/screenshot_mona_lisa.png
--rw-r--r--   0        0        0  1031902 2020-02-02 00:00:00.000000 browsr-1.5.0/docs/_static/screenshot_utils.png
--rw-r--r--   0        0        0   118970 2020-02-02 00:00:00.000000 browsr-1.5.0/requirements/requirements-dev.txt
--rw-r--r--   0        0        0    82526 2020-02-02 00:00:00.000000 browsr-1.5.0/requirements/requirements-prod.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.5.0/tests/conftest.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.5.0/tests/test_cli.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.5.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.5.0/LICENSE
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 browsr-1.5.0/README.md
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 browsr-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 browsr-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.5.1/.releaserc.js
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 browsr-1.5.1/mkdocs.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/__main__.py
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/_base.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/_cli.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/_config.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/_utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/_version.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/browsr.css
+-rw-r--r--   0        0        0    12920 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/browsr.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/cli.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/contributing.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/index.md
+-rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/_static/browsr.png
+-rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/_static/browsr_no_label.png
+-rw-r--r--   0        0        0  1112808 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/_static/screenshot_datatable.png
+-rw-r--r--   0        0        0   838657 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/_static/screenshot_markdown.png
+-rw-r--r--   0        0        0  1550033 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/_static/screenshot_mona_lisa.png
+-rw-r--r--   0        0        0  1031902 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/_static/screenshot_utils.png
+-rw-r--r--   0        0        0   124300 2020-02-02 00:00:00.000000 browsr-1.5.1/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0    82506 2020-02-02 00:00:00.000000 browsr-1.5.1/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.5.1/tests/conftest.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.5.1/tests/test_cli.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.5.1/LICENSE
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 browsr-1.5.1/README.md
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 browsr-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 browsr-1.5.1/PKG-INFO
```

### Comparing `browsr-1.5.0/.pre-commit-config.yaml` & `browsr-1.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/.releaserc.js` & `browsr-1.5.1/.releaserc.js`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/mkdocs.yaml` & `browsr-1.5.1/mkdocs.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 site_name: browsr
 nav:
     - index.md
     - Command Line Interface ⌨️: cli.md
     - Contributing 🤝: contributing.md
     - API Documentation 🤖: reference/
 theme:
-    favicon: _static/browsr_no_label.png
-    logo: _static/browsr_no_label.png
+    favicon: https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/browsr_no_label.png
+    logo: https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/browsr_no_label.png
     name: material
     features:
         - navigation.tracking
         - content.code.annotate
         - content.code.copy
     palette:
         - media: "(prefers-color-scheme: light)"
```

### Comparing `browsr-1.5.0/.github/semantic_release/package-lock.json` & `browsr-1.5.1/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/.github/semantic_release/release_notes.hbs` & `browsr-1.5.1/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/.github/workflows/lint.yaml` & `browsr-1.5.1/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/.github/workflows/publish.yaml` & `browsr-1.5.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/.github/workflows/release.yaml` & `browsr-1.5.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/.github/workflows/tests.yaml` & `browsr-1.5.1/.github/workflows/tests.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,13 @@
               uses: actions/setup-python@v4
               with:
                   python-version: ${{ matrix.python }}
             - name: Install Hatch
               run: |
                   python -m pip install --upgrade pip
                   python -m pip install -q hatch
-                  hatch env create
                   hatch --version
             - name: Test Suite
               run: |
                   echo "::add-matcher::.github/workflows/matchers/python.json"
-                  hatch run test
+                  hatch run +py="${{ matrix.python }}" test:matrix
                   echo "::remove-matcher owner=python::"
```

### Comparing `browsr-1.5.0/browsr/_base.py` & `browsr-1.5.1/browsr/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 Extension Classes
 """
 
 from __future__ import annotations
 
 import math
 import pathlib
-import stat
 from dataclasses import dataclass
 from textwrap import dedent
-from typing import Any, Dict, Iterable, List, Optional, Union
+from typing import Any, Dict, Iterable, Optional, Union
 
 import numpy as np
-import rich_click as click
 import upath
 from pandas import DataFrame
 from rich import traceback
 from rich.console import RenderableType
 from rich.markdown import Markdown
 from rich.text import Text
 from textual.app import App, ComposeResult
@@ -27,18 +25,14 @@
 from textual.widgets._directory_tree import DirEntry
 from textual.widgets._tree import TreeNode
 from upath import UPath
 
 from browsr._config import favorite_themes
 from browsr._utils import FileInfo
 
-debug_option = click.option(
-    "--debug/--no-debug", default=False, help="Enable extra debugging output"
-)
-
 
 @dataclass
 class TextualAppContext:
     """
     App Context Object
     """
 
@@ -132,15 +126,15 @@
 
 
 class UniversalDirectoryTree(DirectoryTree):
     """
     A Universal DirectoryTree supporting different filesystems
     """
 
-    def _load_directory(self, node: TreeNode[DirEntry]) -> None:
+    def load_directory(self, node: TreeNode[DirEntry]) -> None:
         """
         Load Directory Using Universal Pathlib
         """
         assert node.data is not None
         dir_path = UPath(node.data.path)
         node.data.loaded = True
         top_level_buckets = self._handle_top_level_bucket(dir_path=dir_path)
@@ -152,32 +146,19 @@
         for path in top_level_buckets or directory:
             if top_level_buckets is None:
                 path_name = path.name
             else:
                 path_name = str(path).replace("s3://", "").rstrip("/")
             node.add(
                 path_name,
-                data=DirEntry(path),
+                data=DirEntry(str(path), path.is_dir()),
                 allow_expand=path.is_dir(),
             )
         node.expand()
 
-    def reload(self) -> None:
-        """
-        Reload the `DirectoryTree` contents.
-        """
-        self.reset(str(self.path), DirEntry(UPath(self.path)))
-        self._load_directory(self.root)
-
-    def validate_path(self, path: Union[str, UPath]) -> UPath:  # type: ignore[override]
-        """
-        Ensure that the path is of the `UPath` type.
-        """
-        return UPath(path)
-
     def _handle_top_level_bucket(self, dir_path: UPath) -> Optional[Iterable[UPath]]:
         """
         Handle scenarios when someone wants to browse all of s3
 
         This is because S3FS handles the root directory differently than other filesystems
         """
         if str(dir_path) == "s3:/":
@@ -201,83 +182,67 @@
     Thanks, Kupo. https://github.com/darrenburns/kupo
     """
 
     file_info: Union[FileInfo, var[None]] = reactive(None)  # type: ignore[assignment]
 
     def watch_file_info(self, new_file: Union[FileInfo, None]) -> None:
         """
-        Watch the file property for changes
+        Watch the file_info property for changes
         """
         if new_file is None:
             self.display = False
         else:
             self.display = True
 
     @classmethod
     def _convert_size(cls, size_bytes: int) -> str:
         """
         Convert Bytes to Human Readable String
         """
         if size_bytes == 0:
-            return " 0[dim]B"
-        size_name = ("B", "K", "M", "G", "T", "P", "E", "Z", "Y")
+            return " 0B"
+        size_name = ("B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB")
         index = int(math.floor(math.log(size_bytes, 1024)))
         p = math.pow(1024, index)
         number = round(size_bytes / p, 2)
         unit = size_name[index]
-        return f"{number:.0f}[dim]{unit}[/]"
-
-    @classmethod
-    def _render_mode_string(cls, file_info: FileInfo) -> List[Any]:
-        """
-        Render the Mode String for the Current File Info Bar
-        """
-        if file_info.is_local is False:
-            return [("----------", "dim"), (" ╲ ", "dim cyan")]
-        perm_string = stat.filemode(file_info.stat.st_mode)  # type: ignore[union-attr]
-        perm_string = Text.assemble(  # type: ignore[assignment]
-            (perm_string[0], "b dim"),
-            (perm_string[1], "yellow b" if perm_string[1] == "r" else "dim"),
-            (perm_string[2], "red b" if perm_string[2] == "w" else "dim"),
-            (perm_string[3], "green b" if perm_string[3] == "x" else "dim"),
-            (perm_string[4], "yellow b" if perm_string[4] == "r" else "dim"),
-            (perm_string[5], "red b" if perm_string[5] == "w" else "dim"),
-            (perm_string[6], "green b" if perm_string[6] == "x" else "dim"),
-            (perm_string[7], "b yellow" if perm_string[7] == "r" else "dim"),
-            (perm_string[8], "b red" if perm_string[8] == "w" else "dim"),
-            (perm_string[9], "b green" if perm_string[9] == "x" else "dim"),
-        )
-        assembled = [
-            perm_string,
-            (" ╲ ", "dim cyan"),
-        ]
-        return assembled
+        return f"{round(number, 0)}{unit}"
 
     def render(self) -> RenderableType:
         """
         Render the Current File Info Bar
         """
-        if self.file_info is None:
+        if self.file_info is None or not self.file_info.is_file:
             return Text("")
-        modify_time = self.file_info.last_modified.strftime("%-d %b %y %H:%M")
-        assembled = self._render_mode_string(file_info=self.file_info)
-        if self.file_info.is_file:
+        modify_time = self.file_info.last_modified.strftime("%b, %-d %Y %I:%M %p")
+        assembled = [
+            "🗄️️️  ",
+            self._convert_size(self.file_info.size),
+            "   📅️  ",
+            modify_time,
+            "  💾  ",
+            self.file_info.file.name,
+            "  📂  ",
+            self.file_info.file.parent.name,
+        ]
+        if self.file_info.owner not in ["", None]:
+            assembled += [
+                "  👤  ",
+                self.file_info.owner,
+            ]
+        if self.file_info.group.strip() not in ["", None]:
             assembled += [
-                Text.from_markup(self._convert_size(self.file_info.size)),
-                (" ╲ ", "dim cyan"),
+                "  🏠  ",
+                self.file_info.group,
             ]
         assembled += [
-            modify_time,
-            (" ╲ ", "dim cyan"),
-            self.file_info.owner,
-            (" ╲ ", "dim cyan"),
-            self.file_info.group,
+            "  ∙ ",
         ]
-
-        return Text.assemble(*assembled)
+        dim_text = [Text(item, style="dim") for item in assembled]
+        return Text.assemble(*dim_text)
 
 
 class ConfirmationPopUp(Container):
     """
     A Pop Up that asks for confirmation
     """
```

### Comparing `browsr-1.5.0/browsr/_cli.py` & `browsr-1.5.1/browsr/_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,30 +45,30 @@
 )
 def browsr(
     path: Optional[str],
     debug: bool,
     max_file_size: int,
 ) -> None:
     """
-    browsr is a file browser TUI (textual user interface) application. The application
+    **`browsr`** is a file browser TUI (textual user interface) application. The application
     allows you to visually browse through a directory (local or cloud) and display the
     contents of its files
 
     \f
 
-    ![browsr](_static/screenshot_utils.png)
+    ![browsr](https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_utils.png)
 
     ## Installation
 
-    It's recommended to install browsr via [pipx](https://pypa.github.io/pipx/)
-    with **all** optional dependencies, this enables **browsr** to access
+    It's recommended to install **`browsr`** via [pipx](https://pypa.github.io/pipx/)
+    with **`all`** optional dependencies, this enables **`browsr`** to access
     remote cloud storage buckets and open parquet files.
 
-    ```bash
-    pipx install browsr
+    ```shell
+    pipx install "browsr[all]"
     ```
 
     ## Usage Examples
 
     - Load your current working directory: **`browsr`**
     - Load a specific directory: **`browsr /path/to/directory`**
     - Load an S3 bucket: **`browsr s3://bucket-name`**
```

### Comparing `browsr-1.5.0/browsr/_config.py` & `browsr-1.5.1/browsr/_config.py`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/browsr/_utils.py` & `browsr-1.5.1/browsr/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,14 @@
     is_cloudpath = isinstance(file_path, CloudPath)
     if isinstance(stat, dict):
         # raise ValueError(json.dumps(stat, indent=4))
         lower_dict = {key.lower(): value for key, value in stat.items()}
         file_size = lower_dict["size"]
         last_modified = lower_dict.get("lastmodified") or lower_dict.get("updated")
         if isinstance(last_modified, str):
-            # 2023-05-12T21:25:17.050Z
             last_modified = datetime.datetime.fromisoformat(last_modified[:-1])
         return FileInfo(
             file=file_path,
             size=file_size,
             last_modified=last_modified,
             stat=stat,
             is_local=False,
```

### Comparing `browsr-1.5.0/browsr/browsr.css` & `browsr-1.5.1/browsr/browsr.css`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/browsr/browsr.py` & `browsr-1.5.1/browsr/browsr.py`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/docs/contributing.md` & `browsr-1.5.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/docs/gen_ref_pages.py` & `browsr-1.5.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/docs/index.md` & `browsr-1.5.1/docs/index.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # browsr
 
 <div align="center">
-<a href="https://github.com/juftin/browsr">
-  <img src=_static/browsr.png
-    width="400" alt="browsr">
-</a>
+    <picture>
+        <img src=https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/browsr.png
+             width="400" alt="browsr">
+    </picture>
 </div>
 
 [![browsr Version](https://img.shields.io/pypi/v/browsr?color=blue&label=browsr)](https://github.com/juftin/browsr)
 [![PyPI](https://img.shields.io/pypi/pyversions/browsr)](https://pypi.python.org/pypi/browsr/)
 [![Testing Status](https://github.com/juftin/browsr/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/workflows/tests.yaml?query=branch%3Amain)
 [![GitHub License](https://img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://github.com/juftin/browsr/blob/main/LICENSE)
 
@@ -44,24 +44,24 @@
     object-fit: contain;
   }
 </style>
 
 <body>
   <div class="grid" style="display: grid; grid-template-columns: repeat(2, 1fr); grid-gap: 10px;">
     <div class="grid-item">
-      <img src="_static/screenshot_utils.png" alt="Image 1">
+      <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_utils.png" alt="Image 1">
     </div>
     <div class="grid-item">
-      <img src="_static/screenshot_datatable.png" alt="Image 2">
+      <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_datatable.png" alt="Image 2">
     </div>
     <div class="grid-item">
-      <img src="_static/screenshot_mona_lisa.png" alt="Image 3">
+      <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_mona_lisa.png" alt="Image 3">
     </div>
     <div class="grid-item">
-      <img src="_static/screenshot_markdown.png" alt="Image 4">
+      <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_markdown.png" alt="Image 4">
     </div>
   </div>
 
   <div class="expanded" style="display: none;">
     <img src="">
   </div>
 
@@ -81,27 +81,27 @@
 
 ```shell
 pipx install browsr
 ```
 
 ## Extra Installation
 
-If you're looking to use `browsr` on remote file systems, like AWS S3, you'll need to install the `remote` extra.
+If you're looking to use **`browsr`** on remote file systems, like AWS S3, you'll need to install the `remote` extra.
 If you'd like to browse parquet files, you'll need to install the `parquet` extra. Or, even simpler,
 you can install the `all` extra to get all the extras.
 
 ```shell
 pipx install "browsr[all]"
 ```
 
 ## Usage
 
 ```shell
 browsr ~/Downloads/
 ```
 
-Simply give `browsr` a path to a file/directory and it will open a browser window
+Simply give **`browsr`** a path to a file/directory and it will open a browser window
 with a file browser. You can also give it a URL to a remote file system, like AWS S3.
 
 ```shell
 browsr s3://my-bucket/my-file.parquet
 ```
```

#### html2text {}

```diff
@@ -16,15 +16,15 @@
 [Image 3]
 [Image 4]
 [Image]
 ## Installation The below command recommends [pipx](https://pypa.github.io/
 pipx/) instead of pip. `pipx` installs the package in an isolated environment
 and makes it easy to uninstall. If you'd like to use `pip` instead, just
 replace `pipx` with `pip` in the below command. ```shell pipx install browsr
-``` ## Extra Installation If you're looking to use `browsr` on remote file
+``` ## Extra Installation If you're looking to use **`browsr`** on remote file
 systems, like AWS S3, you'll need to install the `remote` extra. If you'd like
 to browse parquet files, you'll need to install the `parquet` extra. Or, even
 simpler, you can install the `all` extra to get all the extras. ```shell pipx
 install "browsr[all]" ``` ## Usage ```shell browsr ~/Downloads/ ``` Simply give
-`browsr` a path to a file/directory and it will open a browser window with a
-file browser. You can also give it a URL to a remote file system, like AWS S3.
-```shell browsr s3://my-bucket/my-file.parquet ```
+**`browsr`** a path to a file/directory and it will open a browser window with
+a file browser. You can also give it a URL to a remote file system, like AWS
+S3. ```shell browsr s3://my-bucket/my-file.parquet ```
```

### Comparing `browsr-1.5.0/docs/_static/browsr.png` & `browsr-1.5.1/docs/_static/browsr.png`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/docs/_static/browsr_no_label.png` & `browsr-1.5.1/docs/_static/browsr_no_label.png`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/docs/_static/screenshot_datatable.png` & `browsr-1.5.1/docs/_static/screenshot_datatable.png`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/docs/_static/screenshot_markdown.png` & `browsr-1.5.1/docs/_static/screenshot_markdown.png`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/docs/_static/screenshot_mona_lisa.png` & `browsr-1.5.1/docs/_static/screenshot_mona_lisa.png`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/docs/_static/screenshot_utils.png` & `browsr-1.5.1/docs/_static/screenshot_utils.png`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/requirements/requirements-dev.txt` & `browsr-1.5.1/requirements/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --generate-hashes --output-file=requirements/requirements-dev.txt --resolver=backtracking requirements.in
 #
 adal==1.2.7 \
     --hash=sha256:2a7451ed7441ddbc57703042204a3e30ef747478eea022c70f789fc7f084bc3d \
     --hash=sha256:d74f45b81317454d96e982fd1c50e6fb5c99ac2223728aea8764433a39f566f1
@@ -106,14 +106,15 @@
     --hash=sha256:fe7ba4a51f33ab275515f66b0a236bcde4fb5561498fe8f898d4e549b2e4509f
     # via
     #   -r requirements.in
     #   adlfs
     #   aiobotocore
     #   gcsfs
     #   s3fs
+    #   textual
 aioitertools==0.11.0 \
     --hash=sha256:04b95e3dab25b449def24d7df809411c10e62aab0cbe31a50ca4e68748c43394 \
     --hash=sha256:42c68b8dd3a69c2bf7f2233bf7df4bb58b557bca5252ac02ed5187bbc67d6831
     # via aiobotocore
 aiosignal==1.3.1 \
     --hash=sha256:54cd96e15e1649b75d6c87526a6ff0b6c1b0dd3459f43d9ca11d48c339b68cfc \
     --hash=sha256:f8376fb07dd1e86a584e4fcdec80b36b7f81aac666ebc724e2c090300dd83b17
@@ -345,14 +346,15 @@
     # via
     #   -r requirements.in
     #   black
     #   mkdocs
     #   mkdocs-click
     #   pip-tools
     #   rich-click
+    #   textual
 colorama==0.4.6 \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
     # via
     #   griffe
     #   mkdocs-material
 coverage[toml]==7.2.5 \
@@ -651,18 +653,15 @@
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via
     #   requests
     #   yarl
 importlib-metadata==6.6.0 \
     --hash=sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed \
     --hash=sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705
-    # via
-    #   markdown
-    #   mkdocs
-    #   textual
+    # via textual
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 isodate==0.6.1 \
     --hash=sha256:0751eece944162659049d35f4f549ed815792b38793f07cf73381c1c87cbed96 \
     --hash=sha256:48c5881de7e8b0a0d648cb024c8062dc84e7b840ed81e864c7614fd3c127bde9
@@ -820,14 +819,79 @@
     # via
     #   azure-identity
     #   msal-extensions
 msal-extensions==1.0.0 \
     --hash=sha256:91e3db9620b822d0ed2b4d1850056a0f133cba04455e62f11612e40f5502f2ee \
     --hash=sha256:c676aba56b0cce3783de1b5c5ecfe828db998167875126ca4b47dc6436451354
     # via azure-identity
+msgpack==1.0.5 \
+    --hash=sha256:06f5174b5f8ed0ed919da0e62cbd4ffde676a374aba4020034da05fab67b9164 \
+    --hash=sha256:0c05a4a96585525916b109bb85f8cb6511db1c6f5b9d9cbcbc940dc6b4be944b \
+    --hash=sha256:137850656634abddfb88236008339fdaba3178f4751b28f270d2ebe77a563b6c \
+    --hash=sha256:17358523b85973e5f242ad74aa4712b7ee560715562554aa2134d96e7aa4cbbf \
+    --hash=sha256:18334484eafc2b1aa47a6d42427da7fa8f2ab3d60b674120bce7a895a0a85bdd \
+    --hash=sha256:1835c84d65f46900920b3708f5ba829fb19b1096c1800ad60bae8418652a951d \
+    --hash=sha256:1967f6129fc50a43bfe0951c35acbb729be89a55d849fab7686004da85103f1c \
+    --hash=sha256:1ab2f3331cb1b54165976a9d976cb251a83183631c88076613c6c780f0d6e45a \
+    --hash=sha256:1c0f7c47f0087ffda62961d425e4407961a7ffd2aa004c81b9c07d9269512f6e \
+    --hash=sha256:20a97bf595a232c3ee6d57ddaadd5453d174a52594bf9c21d10407e2a2d9b3bd \
+    --hash=sha256:20c784e66b613c7f16f632e7b5e8a1651aa5702463d61394671ba07b2fc9e025 \
+    --hash=sha256:266fa4202c0eb94d26822d9bfd7af25d1e2c088927fe8de9033d929dd5ba24c5 \
+    --hash=sha256:28592e20bbb1620848256ebc105fc420436af59515793ed27d5c77a217477705 \
+    --hash=sha256:288e32b47e67f7b171f86b030e527e302c91bd3f40fd9033483f2cacc37f327a \
+    --hash=sha256:3055b0455e45810820db1f29d900bf39466df96ddca11dfa6d074fa47054376d \
+    --hash=sha256:332360ff25469c346a1c5e47cbe2a725517919892eda5cfaffe6046656f0b7bb \
+    --hash=sha256:362d9655cd369b08fda06b6657a303eb7172d5279997abe094512e919cf74b11 \
+    --hash=sha256:366c9a7b9057e1547f4ad51d8facad8b406bab69c7d72c0eb6f529cf76d4b85f \
+    --hash=sha256:36961b0568c36027c76e2ae3ca1132e35123dcec0706c4b7992683cc26c1320c \
+    --hash=sha256:379026812e49258016dd84ad79ac8446922234d498058ae1d415f04b522d5b2d \
+    --hash=sha256:382b2c77589331f2cb80b67cc058c00f225e19827dbc818d700f61513ab47bea \
+    --hash=sha256:476a8fe8fae289fdf273d6d2a6cb6e35b5a58541693e8f9f019bfe990a51e4ba \
+    --hash=sha256:48296af57cdb1d885843afd73c4656be5c76c0c6328db3440c9601a98f303d87 \
+    --hash=sha256:4867aa2df9e2a5fa5f76d7d5565d25ec76e84c106b55509e78c1ede0f152659a \
+    --hash=sha256:4c075728a1095efd0634a7dccb06204919a2f67d1893b6aa8e00497258bf926c \
+    --hash=sha256:4f837b93669ce4336e24d08286c38761132bc7ab29782727f8557e1eb21b2080 \
+    --hash=sha256:4f8d8b3bf1ff2672567d6b5c725a1b347fe838b912772aa8ae2bf70338d5a198 \
+    --hash=sha256:525228efd79bb831cf6830a732e2e80bc1b05436b086d4264814b4b2955b2fa9 \
+    --hash=sha256:5494ea30d517a3576749cad32fa27f7585c65f5f38309c88c6d137877fa28a5a \
+    --hash=sha256:55b56a24893105dc52c1253649b60f475f36b3aa0fc66115bffafb624d7cb30b \
+    --hash=sha256:56a62ec00b636583e5cb6ad313bbed36bb7ead5fa3a3e38938503142c72cba4f \
+    --hash=sha256:57e1f3528bd95cc44684beda696f74d3aaa8a5e58c816214b9046512240ef437 \
+    --hash=sha256:586d0d636f9a628ddc6a17bfd45aa5b5efaf1606d2b60fa5d87b8986326e933f \
+    --hash=sha256:5cb47c21a8a65b165ce29f2bec852790cbc04936f502966768e4aae9fa763cb7 \
+    --hash=sha256:6c4c68d87497f66f96d50142a2b73b97972130d93677ce930718f68828b382e2 \
+    --hash=sha256:821c7e677cc6acf0fd3f7ac664c98803827ae6de594a9f99563e48c5a2f27eb0 \
+    --hash=sha256:916723458c25dfb77ff07f4c66aed34e47503b2eb3188b3adbec8d8aa6e00f48 \
+    --hash=sha256:9e6ca5d5699bcd89ae605c150aee83b5321f2115695e741b99618f4856c50898 \
+    --hash=sha256:9f5ae84c5c8a857ec44dc180a8b0cc08238e021f57abdf51a8182e915e6299f0 \
+    --hash=sha256:a2b031c2e9b9af485d5e3c4520f4220d74f4d222a5b8dc8c1a3ab9448ca79c57 \
+    --hash=sha256:a61215eac016f391129a013c9e46f3ab308db5f5ec9f25811e811f96962599a8 \
+    --hash=sha256:a740fa0e4087a734455f0fc3abf5e746004c9da72fbd541e9b113013c8dc3282 \
+    --hash=sha256:a9985b214f33311df47e274eb788a5893a761d025e2b92c723ba4c63936b69b1 \
+    --hash=sha256:ab31e908d8424d55601ad7075e471b7d0140d4d3dd3272daf39c5c19d936bd82 \
+    --hash=sha256:ac9dd47af78cae935901a9a500104e2dea2e253207c924cc95de149606dc43cc \
+    --hash=sha256:addab7e2e1fcc04bd08e4eb631c2a90960c340e40dfc4a5e24d2ff0d5a3b3edb \
+    --hash=sha256:b1d46dfe3832660f53b13b925d4e0fa1432b00f5f7210eb3ad3bb9a13c6204a6 \
+    --hash=sha256:b2de4c1c0538dcb7010902a2b97f4e00fc4ddf2c8cda9749af0e594d3b7fa3d7 \
+    --hash=sha256:b5ef2f015b95f912c2fcab19c36814963b5463f1fb9049846994b007962743e9 \
+    --hash=sha256:b72d0698f86e8d9ddf9442bdedec15b71df3598199ba33322d9711a19f08145c \
+    --hash=sha256:bae7de2026cbfe3782c8b78b0db9cbfc5455e079f1937cb0ab8d133496ac55e1 \
+    --hash=sha256:bf22a83f973b50f9d38e55c6aade04c41ddda19b00c4ebc558930d78eecc64ed \
+    --hash=sha256:c075544284eadc5cddc70f4757331d99dcbc16b2bbd4849d15f8aae4cf36d31c \
+    --hash=sha256:c396e2cc213d12ce017b686e0f53497f94f8ba2b24799c25d913d46c08ec422c \
+    --hash=sha256:cb5aaa8c17760909ec6cb15e744c3ebc2ca8918e727216e79607b7bbce9c8f77 \
+    --hash=sha256:cdc793c50be3f01106245a61b739328f7dccc2c648b501e237f0699fe1395b81 \
+    --hash=sha256:d25dd59bbbbb996eacf7be6b4ad082ed7eacc4e8f3d2df1ba43822da9bfa122a \
+    --hash=sha256:e42b9594cc3bf4d838d67d6ed62b9e59e201862a25e9a157019e171fbe672dd3 \
+    --hash=sha256:e57916ef1bd0fee4f21c4600e9d1da352d8816b52a599c46460e93a6e9f17086 \
+    --hash=sha256:ed40e926fa2f297e8a653c954b732f125ef97bdd4c889f243182299de27e2aa9 \
+    --hash=sha256:ef8108f8dedf204bb7b42994abf93882da1159728a2d4c5e82012edd92c9da9f \
+    --hash=sha256:f933bbda5a3ee63b8834179096923b094b76f0c7a73c1cfe8f07ad608c58844b \
+    --hash=sha256:fe5c63197c55bce6385d9aee16c4d0641684628f63ace85f73571e65ad1c1e8d
+    # via textual
 multidict==6.0.4 \
     --hash=sha256:01a3a55bd90018c9c080fbb0b9f4891db37d148a0a18722b42f94694f8b6d4c9 \
     --hash=sha256:0b1a97283e0c85772d613878028fec909f003993e1007eafa715b24b377cb9b8 \
     --hash=sha256:0dfad7a5a1e39c53ed00d2dd0c2e36aed4650936dc18fd9a1826a5ae1cad6f03 \
     --hash=sha256:11bdf3f5e1518b24530b8241529d2050014c884cf18b6fc69c0c2b30ca248710 \
     --hash=sha256:1502e24330eb681bdaa3eb70d6358e818e8e8f908a22a1851dfd4e15bc2f8161 \
     --hash=sha256:16ab77bbeb596e14212e7bab8429f24c1579234a3a462105cda4a66904998664 \
@@ -1447,17 +1511,17 @@
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via
     #   azure-core
     #   azure-identity
     #   google-auth
     #   isodate
     #   python-dateutil
-textual==0.24.1 \
-    --hash=sha256:4c7e1f4ed12b9615c63fa3eb7cb9df68d29e0ae5b2352997958cd7ee5533f926 \
-    --hash=sha256:a7deb7ac5a1502424c754fe165ae13cb3890e47ddc514d3f089cb2984c336d1d
+textual[dev]==0.22.3 \
+    --hash=sha256:1ef6457b9d8b727a67d2344bf2d0b530dce1afab55e1bf4e964e430929301baa \
+    --hash=sha256:a68172f7797e9f269270491e039f1e48096530dff64dbfe893e8477f2d4e200c
     # via -r requirements.in
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   black
     #   build
@@ -1469,19 +1533,16 @@
     --hash=sha256:4fc2a7fbbc315f0b6630e0b899fd6c743705abe1094d007b0e612d10da15e0f3 \
     --hash=sha256:ecdc70d543aaf3616a7e48631543a884f74205f284cefd6649ddf44c6a820aac
     # via pandas-stubs
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
     # via
-    #   aioitertools
     #   azure-core
     #   azure-storage-blob
-    #   black
-    #   mkdocstrings
     #   mypy
     #   textual
 uc-micro-py==1.0.2 \
     --hash=sha256:30ae2ac9c49f39ac6dce743bd187fcd2b574b16ca095fa74cd9396795c954c54 \
     --hash=sha256:8c9110c309db9d9e87302e2f4ad2c3152770930d88ab385cd544e7a7e75f3de0
     # via linkify-it-py
 universal-pathlib==0.0.23 \
```

### Comparing `browsr-1.5.0/requirements/requirements-prod.txt` & `browsr-1.5.1/requirements/requirements-prod.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --generate-hashes --output-file=requirements/requirements-prod.txt --resolver=backtracking requirements.in
 #
 adal==1.2.7 \
     --hash=sha256:2a7451ed7441ddbc57703042204a3e30ef747478eea022c70f789fc7f084bc3d \
     --hash=sha256:d74f45b81317454d96e982fd1c50e6fb5c99ac2223728aea8764433a39f566f1
@@ -961,23 +961,22 @@
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via
     #   azure-core
     #   azure-identity
     #   google-auth
     #   isodate
     #   python-dateutil
-textual==0.24.1 \
-    --hash=sha256:4c7e1f4ed12b9615c63fa3eb7cb9df68d29e0ae5b2352997958cd7ee5533f926 \
-    --hash=sha256:a7deb7ac5a1502424c754fe165ae13cb3890e47ddc514d3f089cb2984c336d1d
+textual==0.22.3 \
+    --hash=sha256:1ef6457b9d8b727a67d2344bf2d0b530dce1afab55e1bf4e964e430929301baa \
+    --hash=sha256:a68172f7797e9f269270491e039f1e48096530dff64dbfe893e8477f2d4e200c
     # via -r requirements.in
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
     # via
-    #   aioitertools
     #   azure-core
     #   azure-storage-blob
     #   textual
 uc-micro-py==1.0.2 \
     --hash=sha256:30ae2ac9c49f39ac6dce743bd187fcd2b574b16ca095fa74cd9396795c954c54 \
     --hash=sha256:8c9110c309db9d9e87302e2f4ad2c3152770930d88ab385cd544e7a7e75f3de0
     # via linkify-it-py
```

### Comparing `browsr-1.5.0/.gitignore` & `browsr-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/LICENSE` & `browsr-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `browsr-1.5.0/README.md` & `browsr-1.5.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,161 +1,175 @@
 00000000: 2320 6272 6f77 7372 0a0a 3c64 6976 2061  # browsr..<div a
-00000010: 6c69 676e 3d22 6365 6e74 6572 223e 0a3c  lign="center">.<
-00000020: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000030: 6769 7468 7562 2e63 6f6d 2f6a 7566 7469  github.com/jufti
-00000040: 6e2f 6272 6f77 7372 223e 0a20 203c 696d  n/browsr">.  <im
-00000050: 6720 7372 633d 646f 6373 2f5f 7374 6174  g src=docs/_stat
-00000060: 6963 2f62 726f 7773 722e 706e 670a 2020  ic/browsr.png.  
-00000070: 2020 7769 6474 683d 2234 3030 2220 616c    width="400" al
-00000080: 743d 2262 726f 7773 7222 3e0a 3c2f 613e  t="browsr">.</a>
-00000090: 0a3c 2f64 6976 3e0a 0a5b 215b 6272 6f77  .</div>..[![brow
-000000a0: 7372 2056 6572 7369 6f6e 5d28 6874 7470  sr Version](http
-000000b0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000000c0: 696f 2f70 7970 692f 762f 6272 6f77 7372  io/pypi/v/browsr
-000000d0: 3f63 6f6c 6f72 3d62 6c75 6526 6c61 6265  ?color=blue&labe
-000000e0: 6c3d 6272 6f77 7372 295d 2868 7474 7073  l=browsr)](https
-000000f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00000100: 6674 696e 2f62 726f 7773 7229 0a5b 215b  ftin/browsr).[![
-00000110: 5079 5049 5d28 6874 7470 733a 2f2f 696d  PyPI](https://im
-00000120: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000130: 692f 7079 7665 7273 696f 6e73 2f62 726f  i/pyversions/bro
-00000140: 7773 7229 5d28 6874 7470 733a 2f2f 7079  wsr)](https://py
-00000150: 7069 2e70 7974 686f 6e2e 6f72 672f 7079  pi.python.org/py
-00000160: 7069 2f62 726f 7773 722f 290a 5b21 5b54  pi/browsr/).[![T
-00000170: 6573 7469 6e67 2053 7461 7475 735d 2868  esting Status](h
-00000180: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000190: 6d2f 6a75 6674 696e 2f62 726f 7773 722f  m/juftin/browsr/
-000001a0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-000001b0: 732f 7465 7374 732e 7961 6d6c 2f62 6164  s/tests.yaml/bad
-000001c0: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
-000001d0: 696e 295d 2868 7474 7073 3a2f 2f67 6974  in)](https://git
-000001e0: 6875 622e 636f 6d2f 6a75 6674 696e 2f62  hub.com/juftin/b
-000001f0: 726f 7773 722f 6163 7469 6f6e 732f 776f  rowsr/actions/wo
-00000200: 726b 666c 6f77 732f 7465 7374 732e 7961  rkflows/tests.ya
-00000210: 6d6c 3f71 7565 7279 3d62 7261 6e63 6825  ml?query=branch%
-00000220: 3341 6d61 696e 290a 5b21 5b47 6974 4875  3Amain).[![GitHu
-00000230: 6220 4c69 6365 6e73 655d 2868 7474 7073  b License](https
-00000240: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000250: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
-00000260: 2f6a 7566 7469 6e2f 6272 6f77 7372 3f63  /juftin/browsr?c
-00000270: 6f6c 6f72 3d62 6c75 6526 6c61 6265 6c3d  olor=blue&label=
-00000280: 4c69 6365 6e73 6529 5d28 6874 7470 733a  License)](https:
-00000290: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7566  //github.com/juf
-000002a0: 7469 6e2f 6272 6f77 7372 2f62 6c6f 622f  tin/browsr/blob/
-000002b0: 6d61 696e 2f4c 4943 454e 5345 290a 0a2a  main/LICENSE)..*
-000002c0: 2a60 6272 6f77 7372 602a 2a20 6973 2061  *`browsr`** is a
-000002d0: 2054 5549 2028 7465 7874 2d62 6173 6564   TUI (text-based
-000002e0: 2075 7365 7220 696e 7465 7266 6163 6529   user interface)
-000002f0: 2066 696c 6520 6272 6f77 7365 7220 666f   file browser fo
-00000300: 7220 796f 7572 2074 6572 6d69 6e61 6c2e  r your terminal.
-00000310: 0a49 7427 7320 6120 7369 6d70 6c65 2077  .It's a simple w
-00000320: 6179 2074 6f20 6272 6f77 7365 2079 6f75  ay to browse you
-00000330: 7220 6669 6c65 7320 616e 6420 7461 6b65  r files and take
-00000340: 2061 2070 6565 6b20 6174 2074 6865 6972   a peek at their
-00000350: 2063 6f6e 7465 6e74 732e 2050 6c75 7320   contents. Plus 
-00000360: 6974 0a77 6f72 6b73 206f 6e20 6c6f 6361  it.works on loca
-00000370: 6c20 616e 6420 7265 6d6f 7465 2066 696c  l and remote fil
-00000380: 6520 7379 7374 656d 732e 0a0a 3c64 6574  e systems...<det
-00000390: 6169 6c73 206f 7065 6e3e 3c2f 7375 6d6d  ails open></summ
-000003a0: 6172 793e 3c2f 7375 6d6d 6172 793e 0a0a  ary></summary>..
-000003b0: 3c62 6f64 793e 0a3c 6469 7620 7374 796c  <body>.<div styl
-000003c0: 653d 2264 6973 706c 6179 3a20 6772 6964  e="display: grid
-000003d0: 3b20 6772 6964 2d74 656d 706c 6174 652d  ; grid-template-
-000003e0: 636f 6c75 6d6e 733a 2072 6570 6561 7428  columns: repeat(
-000003f0: 322c 2031 6672 293b 2067 7269 642d 6761  2, 1fr); grid-ga
-00000400: 703a 2031 3070 783b 223e 0a20 2020 203c  p: 10px;">.    <
-00000410: 7069 6374 7572 653e 0a20 2020 2020 2020  picture>.       
-00000420: 203c 696d 6720 7372 633d 2264 6f63 732f   <img src="docs/
-00000430: 5f73 7461 7469 632f 7363 7265 656e 7368  _static/screensh
-00000440: 6f74 5f75 7469 6c73 2e70 6e67 2220 616c  ot_utils.png" al
-00000450: 743d 2249 6d61 6765 2031 2220 6872 6566  t="Image 1" href
-00000460: 3d22 223e 0a20 2020 203c 2f70 6963 7475  ="">.    </pictu
-00000470: 7265 3e0a 2020 2020 3c70 6963 7475 7265  re>.    <picture
-00000480: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
-00000490: 7263 3d22 646f 6373 2f5f 7374 6174 6963  rc="docs/_static
-000004a0: 2f73 6372 6565 6e73 686f 745f 6461 7461  /screenshot_data
-000004b0: 7461 626c 652e 706e 6722 2061 6c74 3d22  table.png" alt="
-000004c0: 496d 6167 6520 3222 2068 7265 663d 2222  Image 2" href=""
-000004d0: 3e0a 2020 2020 3c2f 7069 6374 7572 653e  >.    </picture>
-000004e0: 0a20 2020 203c 7069 6374 7572 653e 0a20  .    <picture>. 
-000004f0: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
-00000500: 2264 6f63 732f 5f73 7461 7469 632f 7363  "docs/_static/sc
-00000510: 7265 656e 7368 6f74 5f6d 6f6e 615f 6c69  reenshot_mona_li
-00000520: 7361 2e70 6e67 2220 616c 743d 2249 6d61  sa.png" alt="Ima
-00000530: 6765 2033 2220 6872 6566 3d22 223e 0a20  ge 3" href="">. 
-00000540: 2020 203c 2f70 6963 7475 7265 3e0a 2020     </picture>.  
-00000550: 2020 3c70 6963 7475 7265 3e0a 2020 2020    <picture>.    
-00000560: 2020 2020 3c69 6d67 2073 7263 3d22 646f      <img src="do
-00000570: 6373 2f5f 7374 6174 6963 2f73 6372 6565  cs/_static/scree
-00000580: 6e73 686f 745f 6d61 726b 646f 776e 2e70  nshot_markdown.p
-00000590: 6e67 2220 616c 743d 2249 6d61 6765 2034  ng" alt="Image 4
-000005a0: 2220 6872 6566 3d22 223e 0a20 2020 203c  " href="">.    <
-000005b0: 2f70 6963 7475 7265 3e0a 3c2f 6469 763e  /picture>.</div>
-000005c0: 0a3c 2f62 6f64 793e 0a0a 3c2f 6465 7461  .</body>..</deta
-000005d0: 696c 733e 0a0a 2323 2049 6e73 7461 6c6c  ils>..## Install
-000005e0: 6174 696f 6e0a 0a54 6865 2062 656c 6f77  ation..The below
-000005f0: 2063 6f6d 6d61 6e64 2072 6563 6f6d 6d65   command recomme
-00000600: 6e64 7320 5b70 6970 785d 2868 7474 7073  nds [pipx](https
-00000610: 3a2f 2f70 7970 612e 6769 7468 7562 2e69  ://pypa.github.i
-00000620: 6f2f 7069 7078 2f29 2069 6e73 7465 6164  o/pipx/) instead
-00000630: 206f 6620 7069 702e 2060 7069 7078 6020   of pip. `pipx` 
-00000640: 696e 7374 616c 6c73 2074 6865 2070 6163  installs the pac
-00000650: 6b61 6765 2069 6e0a 616e 2069 736f 6c61  kage in.an isola
-00000660: 7465 6420 656e 7669 726f 6e6d 656e 7420  ted environment 
-00000670: 616e 6420 6d61 6b65 7320 6974 2065 6173  and makes it eas
-00000680: 7920 746f 2075 6e69 6e73 7461 6c6c 2e20  y to uninstall. 
-00000690: 4966 2079 6f75 2764 206c 696b 6520 746f  If you'd like to
-000006a0: 2075 7365 2060 7069 7060 2069 6e73 7465   use `pip` inste
-000006b0: 6164 2c20 6a75 7374 2072 6570 6c61 6365  ad, just replace
-000006c0: 2060 7069 7078 600a 7769 7468 2060 7069   `pipx`.with `pi
-000006d0: 7060 2069 6e20 7468 6520 6265 6c6f 7720  p` in the below 
-000006e0: 636f 6d6d 616e 642e 0a0a 6060 6073 6865  command...```she
-000006f0: 6c6c 0a70 6970 7820 696e 7374 616c 6c20  ll.pipx install 
-00000700: 6272 6f77 7372 0a60 6060 0a0a 2323 2045  browsr.```..## E
-00000710: 7874 7261 2049 6e73 7461 6c6c 6174 696f  xtra Installatio
-00000720: 6e0a 0a49 6620 796f 7527 7265 206c 6f6f  n..If you're loo
-00000730: 6b69 6e67 2074 6f20 7573 6520 6062 726f  king to use `bro
-00000740: 7773 7260 206f 6e20 7265 6d6f 7465 2066  wsr` on remote f
-00000750: 696c 6520 7379 7374 656d 732c 206c 696b  ile systems, lik
-00000760: 6520 4157 5320 5333 2c20 796f 7527 6c6c  e AWS S3, you'll
-00000770: 206e 6565 6420 746f 2069 6e73 7461 6c6c   need to install
-00000780: 2074 6865 2060 7265 6d6f 7465 6020 6578   the `remote` ex
-00000790: 7472 612e 0a49 6620 796f 7527 6420 6c69  tra..If you'd li
-000007a0: 6b65 2074 6f20 6272 6f77 7365 2070 6172  ke to browse par
-000007b0: 7175 6574 2066 696c 6573 2c20 796f 7527  quet files, you'
-000007c0: 6c6c 206e 6565 6420 746f 2069 6e73 7461  ll need to insta
-000007d0: 6c6c 2074 6865 2060 7061 7271 7565 7460  ll the `parquet`
-000007e0: 2065 7874 7261 2e20 4f72 2c20 6576 656e   extra. Or, even
-000007f0: 2073 696d 706c 6572 2c0a 796f 7520 6361   simpler,.you ca
-00000800: 6e20 696e 7374 616c 6c20 7468 6520 6061  n install the `a
-00000810: 6c6c 6020 6578 7472 6120 746f 2067 6574  ll` extra to get
-00000820: 2061 6c6c 2074 6865 2065 7874 7261 732e   all the extras.
-00000830: 0a0a 6060 6073 6865 6c6c 0a70 6970 7820  ..```shell.pipx 
-00000840: 696e 7374 616c 6c20 2262 726f 7773 725b  install "browsr[
-00000850: 616c 6c5d 220a 6060 600a 0a23 2320 5573  all]".```..## Us
-00000860: 6167 650a 0a60 6060 7368 656c 6c0a 6272  age..```shell.br
-00000870: 6f77 7372 207e 2f44 6f77 6e6c 6f61 6473  owsr ~/Downloads
-00000880: 2f0a 6060 600a 0a53 696d 706c 7920 6769  /.```..Simply gi
-00000890: 7665 2060 6272 6f77 7372 6020 6120 7061  ve `browsr` a pa
-000008a0: 7468 2074 6f20 6120 6669 6c65 2f64 6972  th to a file/dir
-000008b0: 6563 746f 7279 2061 6e64 2069 7420 7769  ectory and it wi
-000008c0: 6c6c 206f 7065 6e20 6120 6272 6f77 7365  ll open a browse
-000008d0: 7220 7769 6e64 6f77 0a77 6974 6820 6120  r window.with a 
-000008e0: 6669 6c65 2062 726f 7773 6572 2e20 596f  file browser. Yo
-000008f0: 7520 6361 6e20 616c 736f 2067 6976 6520  u can also give 
-00000900: 6974 2061 2055 524c 2074 6f20 6120 7265  it a URL to a re
-00000910: 6d6f 7465 2066 696c 6520 7379 7374 656d  mote file system
-00000920: 2c20 6c69 6b65 2041 5753 2053 332e 0a0a  , like AWS S3...
-00000930: 6060 6073 6865 6c6c 0a62 726f 7773 7220  ```shell.browsr 
-00000940: 7333 3a2f 2f6d 792d 6275 636b 6574 2f6d  s3://my-bucket/m
-00000950: 792d 6669 6c65 2e70 6172 7175 6574 0a60  y-file.parquet.`
-00000960: 6060 0a0a 2323 2320 5b43 6865 636b 206f  ``..### [Check o
-00000970: 7574 2074 6865 2044 6f63 756d 656e 7461  ut the Documenta
-00000980: 7469 6f6e 5d28 6874 7470 733a 2f2f 6a75  tion](https://ju
-00000990: 6674 696e 2e63 6f6d 2f62 726f 7773 722f  ftin.com/browsr/
-000009a0: 2920 666f 7220 6d6f 7265 0a0a 2323 204c  ) for more..## L
-000009b0: 6963 656e 7365 0a0a 2a2a 6062 726f 7773  icense..**`brows
-000009c0: 7260 2a2a 2069 7320 6469 7374 7269 6275  r`** is distribu
-000009d0: 7465 6420 756e 6465 7220 7468 6520 7465  ted under the te
-000009e0: 726d 7320 6f66 2074 6865 205b 4d49 5420  rms of the [MIT 
-000009f0: 6c69 6365 6e73 655d 284c 4943 454e 5345  license](LICENSE
-00000a00: 292e 0a                                  )..
+00000010: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+00000020: 2020 203c 7069 6374 7572 653e 0a20 2020     <picture>.   
+00000030: 2020 2020 203c 696d 6720 7372 633d 6874       <img src=ht
+00000040: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000050: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000060: 6a75 6674 696e 2f62 726f 7773 722f 6d61  juftin/browsr/ma
+00000070: 696e 2f64 6f63 732f 5f73 7461 7469 632f  in/docs/_static/
+00000080: 6272 6f77 7372 2e70 6e67 0a20 2020 2020  browsr.png.     
+00000090: 2020 2020 2020 2020 7769 6474 683d 2234          width="4
+000000a0: 3030 2220 616c 743d 2262 726f 7773 7222  00" alt="browsr"
+000000b0: 3e0a 2020 2020 3c2f 7069 6374 7572 653e  >.    </picture>
+000000c0: 0a3c 2f64 6976 3e0a 0a5b 215b 6272 6f77  .</div>..[![brow
+000000d0: 7372 2056 6572 7369 6f6e 5d28 6874 7470  sr Version](http
+000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000000f0: 696f 2f70 7970 692f 762f 6272 6f77 7372  io/pypi/v/browsr
+00000100: 3f63 6f6c 6f72 3d62 6c75 6526 6c61 6265  ?color=blue&labe
+00000110: 6c3d 6272 6f77 7372 295d 2868 7474 7073  l=browsr)](https
+00000120: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00000130: 6674 696e 2f62 726f 7773 7229 0a5b 215b  ftin/browsr).[![
+00000140: 5079 5049 5d28 6874 7470 733a 2f2f 696d  PyPI](https://im
+00000150: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000160: 692f 7079 7665 7273 696f 6e73 2f62 726f  i/pyversions/bro
+00000170: 7773 7229 5d28 6874 7470 733a 2f2f 7079  wsr)](https://py
+00000180: 7069 2e70 7974 686f 6e2e 6f72 672f 7079  pi.python.org/py
+00000190: 7069 2f62 726f 7773 722f 290a 5b21 5b54  pi/browsr/).[![T
+000001a0: 6573 7469 6e67 2053 7461 7475 735d 2868  esting Status](h
+000001b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001c0: 6d2f 6a75 6674 696e 2f62 726f 7773 722f  m/juftin/browsr/
+000001d0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+000001e0: 732f 7465 7374 732e 7961 6d6c 2f62 6164  s/tests.yaml/bad
+000001f0: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
+00000200: 696e 295d 2868 7474 7073 3a2f 2f67 6974  in)](https://git
+00000210: 6875 622e 636f 6d2f 6a75 6674 696e 2f62  hub.com/juftin/b
+00000220: 726f 7773 722f 6163 7469 6f6e 732f 776f  rowsr/actions/wo
+00000230: 726b 666c 6f77 732f 7465 7374 732e 7961  rkflows/tests.ya
+00000240: 6d6c 3f71 7565 7279 3d62 7261 6e63 6825  ml?query=branch%
+00000250: 3341 6d61 696e 290a 5b21 5b47 6974 4875  3Amain).[![GitHu
+00000260: 6220 4c69 6365 6e73 655d 2868 7474 7073  b License](https
+00000270: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000280: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
+00000290: 2f6a 7566 7469 6e2f 6272 6f77 7372 3f63  /juftin/browsr?c
+000002a0: 6f6c 6f72 3d62 6c75 6526 6c61 6265 6c3d  olor=blue&label=
+000002b0: 4c69 6365 6e73 6529 5d28 6874 7470 733a  License)](https:
+000002c0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 7566  //github.com/juf
+000002d0: 7469 6e2f 6272 6f77 7372 2f62 6c6f 622f  tin/browsr/blob/
+000002e0: 6d61 696e 2f4c 4943 454e 5345 290a 0a2a  main/LICENSE)..*
+000002f0: 2a60 6272 6f77 7372 602a 2a20 6973 2061  *`browsr`** is a
+00000300: 2054 5549 2028 7465 7874 2d62 6173 6564   TUI (text-based
+00000310: 2075 7365 7220 696e 7465 7266 6163 6529   user interface)
+00000320: 2066 696c 6520 6272 6f77 7365 7220 666f   file browser fo
+00000330: 7220 796f 7572 2074 6572 6d69 6e61 6c2e  r your terminal.
+00000340: 0a49 7427 7320 6120 7369 6d70 6c65 2077  .It's a simple w
+00000350: 6179 2074 6f20 6272 6f77 7365 2079 6f75  ay to browse you
+00000360: 7220 6669 6c65 7320 616e 6420 7461 6b65  r files and take
+00000370: 2061 2070 6565 6b20 6174 2074 6865 6972   a peek at their
+00000380: 2063 6f6e 7465 6e74 732e 2050 6c75 7320   contents. Plus 
+00000390: 6974 0a77 6f72 6b73 206f 6e20 6c6f 6361  it.works on loca
+000003a0: 6c20 616e 6420 7265 6d6f 7465 2066 696c  l and remote fil
+000003b0: 6520 7379 7374 656d 732e 0a0a 3c64 6574  e systems...<det
+000003c0: 6169 6c73 206f 7065 6e3e 3c2f 7375 6d6d  ails open></summ
+000003d0: 6172 793e 3c2f 7375 6d6d 6172 793e 0a0a  ary></summary>..
+000003e0: 3c62 6f64 793e 0a3c 6469 7620 7374 796c  <body>.<div styl
+000003f0: 653d 2264 6973 706c 6179 3a20 6772 6964  e="display: grid
+00000400: 3b20 6772 6964 2d74 656d 706c 6174 652d  ; grid-template-
+00000410: 636f 6c75 6d6e 733a 2072 6570 6561 7428  columns: repeat(
+00000420: 322c 2031 6672 293b 2067 7269 642d 6761  2, 1fr); grid-ga
+00000430: 703a 2031 3070 783b 223e 0a20 2020 203c  p: 10px;">.    <
+00000440: 7069 6374 7572 653e 0a20 2020 2020 2020  picture>.       
+00000450: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000460: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000470: 7263 6f6e 7465 6e74 2e63 6f6d 2f6a 7566  rcontent.com/juf
+00000480: 7469 6e2f 6272 6f77 7372 2f6d 6169 6e2f  tin/browsr/main/
+00000490: 646f 6373 2f5f 7374 6174 6963 2f73 6372  docs/_static/scr
+000004a0: 6565 6e73 686f 745f 7574 696c 732e 706e  eenshot_utils.pn
+000004b0: 6722 2061 6c74 3d22 496d 6167 6520 3122  g" alt="Image 1"
+000004c0: 3e0a 2020 2020 3c2f 7069 6374 7572 653e  >.    </picture>
+000004d0: 0a20 2020 203c 7069 6374 7572 653e 0a20  .    <picture>. 
+000004e0: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+000004f0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00000500: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000510: 6f6d 2f6a 7566 7469 6e2f 6272 6f77 7372  om/juftin/browsr
+00000520: 2f6d 6169 6e2f 646f 6373 2f5f 7374 6174  /main/docs/_stat
+00000530: 6963 2f73 6372 6565 6e73 686f 745f 6461  ic/screenshot_da
+00000540: 7461 7461 626c 652e 706e 6722 2061 6c74  tatable.png" alt
+00000550: 3d22 496d 6167 6520 3222 3e0a 2020 2020  ="Image 2">.    
+00000560: 3c2f 7069 6374 7572 653e 0a20 2020 203c  </picture>.    <
+00000570: 7069 6374 7572 653e 0a20 2020 2020 2020  picture>.       
+00000580: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000590: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000005a0: 7263 6f6e 7465 6e74 2e63 6f6d 2f6a 7566  rcontent.com/juf
+000005b0: 7469 6e2f 6272 6f77 7372 2f6d 6169 6e2f  tin/browsr/main/
+000005c0: 646f 6373 2f5f 7374 6174 6963 2f73 6372  docs/_static/scr
+000005d0: 6565 6e73 686f 745f 6d6f 6e61 5f6c 6973  eenshot_mona_lis
+000005e0: 612e 706e 6722 2061 6c74 3d22 496d 6167  a.png" alt="Imag
+000005f0: 6520 3322 3e0a 2020 2020 3c2f 7069 6374  e 3">.    </pict
+00000600: 7572 653e 0a20 2020 203c 7069 6374 7572  ure>.    <pictur
+00000610: 653e 0a20 2020 2020 2020 203c 696d 6720  e>.        <img 
+00000620: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00000630: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000640: 6e74 2e63 6f6d 2f6a 7566 7469 6e2f 6272  nt.com/juftin/br
+00000650: 6f77 7372 2f6d 6169 6e2f 646f 6373 2f5f  owsr/main/docs/_
+00000660: 7374 6174 6963 2f73 6372 6565 6e73 686f  static/screensho
+00000670: 745f 6d61 726b 646f 776e 2e70 6e67 2220  t_markdown.png" 
+00000680: 616c 743d 2249 6d61 6765 2034 223e 0a20  alt="Image 4">. 
+00000690: 2020 203c 2f70 6963 7475 7265 3e0a 3c2f     </picture>.</
+000006a0: 6469 763e 0a3c 2f62 6f64 793e 0a0a 3c2f  div>.</body>..</
+000006b0: 6465 7461 696c 733e 0a0a 2323 2049 6e73  details>..## Ins
+000006c0: 7461 6c6c 6174 696f 6e0a 0a54 6865 2062  tallation..The b
+000006d0: 656c 6f77 2063 6f6d 6d61 6e64 2072 6563  elow command rec
+000006e0: 6f6d 6d65 6e64 7320 5b70 6970 785d 2868  ommends [pipx](h
+000006f0: 7474 7073 3a2f 2f70 7970 612e 6769 7468  ttps://pypa.gith
+00000700: 7562 2e69 6f2f 7069 7078 2f29 2069 6e73  ub.io/pipx/) ins
+00000710: 7465 6164 206f 6620 7069 702e 2060 7069  tead of pip. `pi
+00000720: 7078 6020 696e 7374 616c 6c73 2074 6865  px` installs the
+00000730: 2070 6163 6b61 6765 2069 6e0a 616e 2069   package in.an i
+00000740: 736f 6c61 7465 6420 656e 7669 726f 6e6d  solated environm
+00000750: 656e 7420 616e 6420 6d61 6b65 7320 6974  ent and makes it
+00000760: 2065 6173 7920 746f 2075 6e69 6e73 7461   easy to uninsta
+00000770: 6c6c 2e20 4966 2079 6f75 2764 206c 696b  ll. If you'd lik
+00000780: 6520 746f 2075 7365 2060 7069 7060 2069  e to use `pip` i
+00000790: 6e73 7465 6164 2c20 6a75 7374 2072 6570  nstead, just rep
+000007a0: 6c61 6365 2060 7069 7078 600a 7769 7468  lace `pipx`.with
+000007b0: 2060 7069 7060 2069 6e20 7468 6520 6265   `pip` in the be
+000007c0: 6c6f 7720 636f 6d6d 616e 642e 0a0a 6060  low command...``
+000007d0: 6073 6865 6c6c 0a70 6970 7820 696e 7374  `shell.pipx inst
+000007e0: 616c 6c20 6272 6f77 7372 0a60 6060 0a0a  all browsr.```..
+000007f0: 2323 2045 7874 7261 2049 6e73 7461 6c6c  ## Extra Install
+00000800: 6174 696f 6e0a 0a49 6620 796f 7527 7265  ation..If you're
+00000810: 206c 6f6f 6b69 6e67 2074 6f20 7573 6520   looking to use 
+00000820: 2a2a 6062 726f 7773 7260 2a2a 206f 6e20  **`browsr`** on 
+00000830: 7265 6d6f 7465 2066 696c 6520 7379 7374  remote file syst
+00000840: 656d 732c 206c 696b 6520 4157 5320 5333  ems, like AWS S3
+00000850: 2c20 796f 7527 6c6c 206e 6565 6420 746f  , you'll need to
+00000860: 2069 6e73 7461 6c6c 2074 6865 2060 7265   install the `re
+00000870: 6d6f 7465 6020 6578 7472 612e 0a49 6620  mote` extra..If 
+00000880: 796f 7527 6420 6c69 6b65 2074 6f20 6272  you'd like to br
+00000890: 6f77 7365 2070 6172 7175 6574 2066 696c  owse parquet fil
+000008a0: 6573 2c20 796f 7527 6c6c 206e 6565 6420  es, you'll need 
+000008b0: 746f 2069 6e73 7461 6c6c 2074 6865 2060  to install the `
+000008c0: 7061 7271 7565 7460 2065 7874 7261 2e20  parquet` extra. 
+000008d0: 4f72 2c20 6576 656e 2073 696d 706c 6572  Or, even simpler
+000008e0: 2c0a 796f 7520 6361 6e20 696e 7374 616c  ,.you can instal
+000008f0: 6c20 7468 6520 6061 6c6c 6020 6578 7472  l the `all` extr
+00000900: 6120 746f 2067 6574 2061 6c6c 2074 6865  a to get all the
+00000910: 2065 7874 7261 732e 0a0a 6060 6073 6865   extras...```she
+00000920: 6c6c 0a70 6970 7820 696e 7374 616c 6c20  ll.pipx install 
+00000930: 2262 726f 7773 725b 616c 6c5d 220a 6060  "browsr[all]".``
+00000940: 600a 0a23 2320 5573 6167 650a 0a60 6060  `..## Usage..```
+00000950: 7368 656c 6c0a 6272 6f77 7372 207e 2f44  shell.browsr ~/D
+00000960: 6f77 6e6c 6f61 6473 2f0a 6060 600a 0a53  ownloads/.```..S
+00000970: 696d 706c 7920 6769 7665 202a 2a60 6272  imply give **`br
+00000980: 6f77 7372 602a 2a20 6120 7061 7468 2074  owsr`** a path t
+00000990: 6f20 6120 6669 6c65 2f64 6972 6563 746f  o a file/directo
+000009a0: 7279 2061 6e64 2069 7420 7769 6c6c 206f  ry and it will o
+000009b0: 7065 6e20 6120 6272 6f77 7365 7220 7769  pen a browser wi
+000009c0: 6e64 6f77 0a77 6974 6820 6120 6669 6c65  ndow.with a file
+000009d0: 2062 726f 7773 6572 2e20 596f 7520 6361   browser. You ca
+000009e0: 6e20 616c 736f 2067 6976 6520 6974 2061  n also give it a
+000009f0: 2055 524c 2074 6f20 6120 7265 6d6f 7465   URL to a remote
+00000a00: 2066 696c 6520 7379 7374 656d 2c20 6c69   file system, li
+00000a10: 6b65 2041 5753 2053 332e 0a0a 6060 6073  ke AWS S3...```s
+00000a20: 6865 6c6c 0a62 726f 7773 7220 7333 3a2f  hell.browsr s3:/
+00000a30: 2f6d 792d 6275 636b 6574 2f6d 792d 6669  /my-bucket/my-fi
+00000a40: 6c65 2e70 6172 7175 6574 0a60 6060 0a0a  le.parquet.```..
+00000a50: 2323 2320 5b43 6865 636b 206f 7574 2074  ### [Check out t
+00000a60: 6865 2044 6f63 756d 656e 7461 7469 6f6e  he Documentation
+00000a70: 5d28 6874 7470 733a 2f2f 6a75 6674 696e  ](https://juftin
+00000a80: 2e63 6f6d 2f62 726f 7773 722f 2920 666f  .com/browsr/) fo
+00000a90: 7220 6d6f 7265 0a0a 2323 204c 6963 656e  r more..## Licen
+00000aa0: 7365 0a0a 2a2a 6062 726f 7773 7260 2a2a  se..**`browsr`**
+00000ab0: 2069 7320 6469 7374 7269 6275 7465 6420   is distributed 
+00000ac0: 756e 6465 7220 7468 6520 7465 726d 7320  under the terms 
+00000ad0: 6f66 2074 6865 205b 4d49 5420 6c69 6365  of the [MIT lice
+00000ae0: 6e73 655d 284c 4943 454e 5345 292e 0a    nse](LICENSE)..
```

### Comparing `browsr-1.5.0/pyproject.toml` & `browsr-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "art~=5.7",
   "click~=8.1.3",
   "fsspec~=2023.1.0",
   "pandas~=1.5.2",
   "rich~=13.3.5",
   "rich-click~=1.5.2",
   "rich-pixels~=2.1.1",
-  "textual~=0.24.1",
+  "textual~=0.22.3",
   "universal-pathlib~=0.0.21",
   "Pillow>=9.1.0",
   "PyMuPDF~=1.22.3"
 ]
 description = "TUI File Browser App"
 dynamic = ["version"]
 keywords = []
@@ -82,18 +82,20 @@
   "mkdocs-gen-files~=0.4.0",
   "mkdocs-literate-nav~=0.6.0",
   "mkdocs-section-index~=0.3.5",
   "black~=23.3.0",
   "ruff~=0.0.261",
   "mypy~=1.2.0",
   "pandas-stubs~=2.0.0.230412",
-  "pip-tools~=6.13.0"
+  "pip-tools~=6.13.0",
+  "textual[dev]~=0.22.3"
 ]
 features = ["all"]
 pre-install-commands = ["pip install -U --no-deps -r requirements/requirements-dev.txt"]
+python = "3.10"
 
 [tool.hatch.envs.default.scripts]
 _pip_compile = "pip-compile --resolver=backtracking --generate-hashes requirements.in"
 all = ["format", "lint", "check", "test"]
 check = [
   "mypy --install-types --strict-optional --non-interactive {args:browsr/ tests/}"
 ]
```

### Comparing `browsr-1.5.0/PKG-INFO` & `browsr-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6272 6f77  : 2.1.Name: brow
 00000020: 7372 0a56 6572 7369 6f6e 3a20 312e 352e  sr.Version: 1.5.
-00000030: 300a 5375 6d6d 6172 793a 2054 5549 2046  0.Summary: TUI F
+00000030: 310a 5375 6d6d 6172 793a 2054 5549 2046  1.Summary: TUI F
 00000040: 696c 6520 4272 6f77 7365 7220 4170 700a  ile Browser App.
 00000050: 5072 6f6a 6563 742d 5552 4c3a 2044 6f63  Project-URL: Doc
 00000060: 756d 656e 7461 7469 6f6e 2c20 6874 7470  umentation, http
 00000070: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
 00000080: 7566 7469 6e2f 6272 6f77 7372 2372 6561  uftin/browsr#rea
 00000090: 646d 650a 5072 6f6a 6563 742d 5552 4c3a  dme.Project-URL:
 000000a0: 2049 7373 7565 732c 2068 7474 7073 3a2f   Issues, https:/
@@ -55,15 +55,15 @@
 00000360: 732d 4469 7374 3a20 7269 6368 2d63 6c69  s-Dist: rich-cli
 00000370: 636b 7e3d 312e 352e 320a 5265 7175 6972  ck~=1.5.2.Requir
 00000380: 6573 2d44 6973 743a 2072 6963 682d 7069  es-Dist: rich-pi
 00000390: 7865 6c73 7e3d 322e 312e 310a 5265 7175  xels~=2.1.1.Requ
 000003a0: 6972 6573 2d44 6973 743a 2072 6963 687e  ires-Dist: rich~
 000003b0: 3d31 332e 332e 350a 5265 7175 6972 6573  =13.3.5.Requires
 000003c0: 2d44 6973 743a 2074 6578 7475 616c 7e3d  -Dist: textual~=
-000003d0: 302e 3234 2e31 0a52 6571 7569 7265 732d  0.24.1.Requires-
+000003d0: 302e 3232 2e33 0a52 6571 7569 7265 732d  0.22.3.Requires-
 000003e0: 4469 7374 3a20 756e 6976 6572 7361 6c2d  Dist: universal-
 000003f0: 7061 7468 6c69 627e 3d30 2e30 2e32 310a  pathlib~=0.0.21.
 00000400: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
 00000410: 616c 6c0a 5265 7175 6972 6573 2d44 6973  all.Requires-Dis
 00000420: 743a 2061 646c 6673 7e3d 3230 3233 2e31  t: adlfs~=2023.1
 00000430: 2e30 3b20 6578 7472 6120 3d3d 2027 616c  .0; extra == 'al
 00000440: 6c27 0a52 6571 7569 7265 732d 4469 7374  l'.Requires-Dist
@@ -103,166 +103,180 @@
 00000660: 4469 7374 3a20 7333 6673 7e3d 3230 3233  Dist: s3fs~=2023
 00000670: 2e31 2e30 3b20 6578 7472 6120 3d3d 2027  .1.0; extra == '
 00000680: 7265 6d6f 7465 270a 4465 7363 7269 7074  remote'.Descript
 00000690: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
 000006a0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
 000006b0: 0a23 2062 726f 7773 720a 0a3c 6469 7620  .# browsr..<div 
 000006c0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-000006d0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000006e0: 2f67 6974 6875 622e 636f 6d2f 6a75 6674  /github.com/juft
-000006f0: 696e 2f62 726f 7773 7222 3e0a 2020 3c69  in/browsr">.  <i
-00000700: 6d67 2073 7263 3d64 6f63 732f 5f73 7461  mg src=docs/_sta
-00000710: 7469 632f 6272 6f77 7372 2e70 6e67 0a20  tic/browsr.png. 
-00000720: 2020 2077 6964 7468 3d22 3430 3022 2061     width="400" a
-00000730: 6c74 3d22 6272 6f77 7372 223e 0a3c 2f61  lt="browsr">.</a
-00000740: 3e0a 3c2f 6469 763e 0a0a 5b21 5b62 726f  >.</div>..[![bro
-00000750: 7773 7220 5665 7273 696f 6e5d 2868 7474  wsr Version](htt
-00000760: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000770: 2e69 6f2f 7079 7069 2f76 2f62 726f 7773  .io/pypi/v/brows
-00000780: 723f 636f 6c6f 723d 626c 7565 266c 6162  r?color=blue&lab
-00000790: 656c 3d62 726f 7773 7229 5d28 6874 7470  el=browsr)](http
-000007a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000007b0: 7566 7469 6e2f 6272 6f77 7372 290a 5b21  uftin/browsr).[!
-000007c0: 5b50 7950 495d 2868 7474 7073 3a2f 2f69  [PyPI](https://i
-000007d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000007e0: 7069 2f70 7976 6572 7369 6f6e 732f 6272  pi/pyversions/br
-000007f0: 6f77 7372 295d 2868 7474 7073 3a2f 2f70  owsr)](https://p
-00000800: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
-00000810: 7970 692f 6272 6f77 7372 2f29 0a5b 215b  ypi/browsr/).[![
-00000820: 5465 7374 696e 6720 5374 6174 7573 5d28  Testing Status](
-00000830: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000840: 6f6d 2f6a 7566 7469 6e2f 6272 6f77 7372  om/juftin/browsr
-00000850: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000860: 7773 2f74 6573 7473 2e79 616d 6c2f 6261  ws/tests.yaml/ba
-00000870: 6467 652e 7376 673f 6272 616e 6368 3d6d  dge.svg?branch=m
-00000880: 6169 6e29 5d28 6874 7470 733a 2f2f 6769  ain)](https://gi
-00000890: 7468 7562 2e63 6f6d 2f6a 7566 7469 6e2f  thub.com/juftin/
-000008a0: 6272 6f77 7372 2f61 6374 696f 6e73 2f77  browsr/actions/w
-000008b0: 6f72 6b66 6c6f 7773 2f74 6573 7473 2e79  orkflows/tests.y
-000008c0: 616d 6c3f 7175 6572 793d 6272 616e 6368  aml?query=branch
-000008d0: 2533 416d 6169 6e29 0a5b 215b 4769 7448  %3Amain).[![GitH
-000008e0: 7562 204c 6963 656e 7365 5d28 6874 7470  ub License](http
-000008f0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000900: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
-00000910: 652f 6a75 6674 696e 2f62 726f 7773 723f  e/juftin/browsr?
-00000920: 636f 6c6f 723d 626c 7565 266c 6162 656c  color=blue&label
-00000930: 3d4c 6963 656e 7365 295d 2868 7474 7073  =License)](https
-00000940: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00000950: 6674 696e 2f62 726f 7773 722f 626c 6f62  ftin/browsr/blob
-00000960: 2f6d 6169 6e2f 4c49 4345 4e53 4529 0a0a  /main/LICENSE)..
-00000970: 2a2a 6062 726f 7773 7260 2a2a 2069 7320  **`browsr`** is 
-00000980: 6120 5455 4920 2874 6578 742d 6261 7365  a TUI (text-base
-00000990: 6420 7573 6572 2069 6e74 6572 6661 6365  d user interface
-000009a0: 2920 6669 6c65 2062 726f 7773 6572 2066  ) file browser f
-000009b0: 6f72 2079 6f75 7220 7465 726d 696e 616c  or your terminal
-000009c0: 2e0a 4974 2773 2061 2073 696d 706c 6520  ..It's a simple 
-000009d0: 7761 7920 746f 2062 726f 7773 6520 796f  way to browse yo
-000009e0: 7572 2066 696c 6573 2061 6e64 2074 616b  ur files and tak
-000009f0: 6520 6120 7065 656b 2061 7420 7468 6569  e a peek at thei
-00000a00: 7220 636f 6e74 656e 7473 2e20 506c 7573  r contents. Plus
-00000a10: 2069 740a 776f 726b 7320 6f6e 206c 6f63   it.works on loc
-00000a20: 616c 2061 6e64 2072 656d 6f74 6520 6669  al and remote fi
-00000a30: 6c65 2073 7973 7465 6d73 2e0a 0a3c 6465  le systems...<de
-00000a40: 7461 696c 7320 6f70 656e 3e3c 2f73 756d  tails open></sum
-00000a50: 6d61 7279 3e3c 2f73 756d 6d61 7279 3e0a  mary></summary>.
-00000a60: 0a3c 626f 6479 3e0a 3c64 6976 2073 7479  .<body>.<div sty
-00000a70: 6c65 3d22 6469 7370 6c61 793a 2067 7269  le="display: gri
-00000a80: 643b 2067 7269 642d 7465 6d70 6c61 7465  d; grid-template
-00000a90: 2d63 6f6c 756d 6e73 3a20 7265 7065 6174  -columns: repeat
-00000aa0: 2832 2c20 3166 7229 3b20 6772 6964 2d67  (2, 1fr); grid-g
-00000ab0: 6170 3a20 3130 7078 3b22 3e0a 2020 2020  ap: 10px;">.    
-00000ac0: 3c70 6963 7475 7265 3e0a 2020 2020 2020  <picture>.      
-00000ad0: 2020 3c69 6d67 2073 7263 3d22 646f 6373    <img src="docs
-00000ae0: 2f5f 7374 6174 6963 2f73 6372 6565 6e73  /_static/screens
-00000af0: 686f 745f 7574 696c 732e 706e 6722 2061  hot_utils.png" a
-00000b00: 6c74 3d22 496d 6167 6520 3122 2068 7265  lt="Image 1" hre
-00000b10: 663d 2222 3e0a 2020 2020 3c2f 7069 6374  f="">.    </pict
-00000b20: 7572 653e 0a20 2020 203c 7069 6374 7572  ure>.    <pictur
-00000b30: 653e 0a20 2020 2020 2020 203c 696d 6720  e>.        <img 
-00000b40: 7372 633d 2264 6f63 732f 5f73 7461 7469  src="docs/_stati
-00000b50: 632f 7363 7265 656e 7368 6f74 5f64 6174  c/screenshot_dat
-00000b60: 6174 6162 6c65 2e70 6e67 2220 616c 743d  atable.png" alt=
-00000b70: 2249 6d61 6765 2032 2220 6872 6566 3d22  "Image 2" href="
-00000b80: 223e 0a20 2020 203c 2f70 6963 7475 7265  ">.    </picture
-00000b90: 3e0a 2020 2020 3c70 6963 7475 7265 3e0a  >.    <picture>.
-00000ba0: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
-00000bb0: 3d22 646f 6373 2f5f 7374 6174 6963 2f73  ="docs/_static/s
-00000bc0: 6372 6565 6e73 686f 745f 6d6f 6e61 5f6c  creenshot_mona_l
-00000bd0: 6973 612e 706e 6722 2061 6c74 3d22 496d  isa.png" alt="Im
-00000be0: 6167 6520 3322 2068 7265 663d 2222 3e0a  age 3" href="">.
-00000bf0: 2020 2020 3c2f 7069 6374 7572 653e 0a20      </picture>. 
-00000c00: 2020 203c 7069 6374 7572 653e 0a20 2020     <picture>.   
-00000c10: 2020 2020 203c 696d 6720 7372 633d 2264       <img src="d
-00000c20: 6f63 732f 5f73 7461 7469 632f 7363 7265  ocs/_static/scre
-00000c30: 656e 7368 6f74 5f6d 6172 6b64 6f77 6e2e  enshot_markdown.
-00000c40: 706e 6722 2061 6c74 3d22 496d 6167 6520  png" alt="Image 
-00000c50: 3422 2068 7265 663d 2222 3e0a 2020 2020  4" href="">.    
-00000c60: 3c2f 7069 6374 7572 653e 0a3c 2f64 6976  </picture>.</div
-00000c70: 3e0a 3c2f 626f 6479 3e0a 0a3c 2f64 6574  >.</body>..</det
-00000c80: 6169 6c73 3e0a 0a23 2320 496e 7374 616c  ails>..## Instal
-00000c90: 6c61 7469 6f6e 0a0a 5468 6520 6265 6c6f  lation..The belo
-00000ca0: 7720 636f 6d6d 616e 6420 7265 636f 6d6d  w command recomm
-00000cb0: 656e 6473 205b 7069 7078 5d28 6874 7470  ends [pipx](http
-00000cc0: 733a 2f2f 7079 7061 2e67 6974 6875 622e  s://pypa.github.
-00000cd0: 696f 2f70 6970 782f 2920 696e 7374 6561  io/pipx/) instea
-00000ce0: 6420 6f66 2070 6970 2e20 6070 6970 7860  d of pip. `pipx`
-00000cf0: 2069 6e73 7461 6c6c 7320 7468 6520 7061   installs the pa
-00000d00: 636b 6167 6520 696e 0a61 6e20 6973 6f6c  ckage in.an isol
-00000d10: 6174 6564 2065 6e76 6972 6f6e 6d65 6e74  ated environment
-00000d20: 2061 6e64 206d 616b 6573 2069 7420 6561   and makes it ea
-00000d30: 7379 2074 6f20 756e 696e 7374 616c 6c2e  sy to uninstall.
-00000d40: 2049 6620 796f 7527 6420 6c69 6b65 2074   If you'd like t
-00000d50: 6f20 7573 6520 6070 6970 6020 696e 7374  o use `pip` inst
-00000d60: 6561 642c 206a 7573 7420 7265 706c 6163  ead, just replac
-00000d70: 6520 6070 6970 7860 0a77 6974 6820 6070  e `pipx`.with `p
-00000d80: 6970 6020 696e 2074 6865 2062 656c 6f77  ip` in the below
-00000d90: 2063 6f6d 6d61 6e64 2e0a 0a60 6060 7368   command...```sh
-00000da0: 656c 6c0a 7069 7078 2069 6e73 7461 6c6c  ell.pipx install
-00000db0: 2062 726f 7773 720a 6060 600a 0a23 2320   browsr.```..## 
-00000dc0: 4578 7472 6120 496e 7374 616c 6c61 7469  Extra Installati
-00000dd0: 6f6e 0a0a 4966 2079 6f75 2772 6520 6c6f  on..If you're lo
-00000de0: 6f6b 696e 6720 746f 2075 7365 2060 6272  oking to use `br
-00000df0: 6f77 7372 6020 6f6e 2072 656d 6f74 6520  owsr` on remote 
-00000e00: 6669 6c65 2073 7973 7465 6d73 2c20 6c69  file systems, li
-00000e10: 6b65 2041 5753 2053 332c 2079 6f75 276c  ke AWS S3, you'l
-00000e20: 6c20 6e65 6564 2074 6f20 696e 7374 616c  l need to instal
-00000e30: 6c20 7468 6520 6072 656d 6f74 6560 2065  l the `remote` e
-00000e40: 7874 7261 2e0a 4966 2079 6f75 2764 206c  xtra..If you'd l
-00000e50: 696b 6520 746f 2062 726f 7773 6520 7061  ike to browse pa
-00000e60: 7271 7565 7420 6669 6c65 732c 2079 6f75  rquet files, you
-00000e70: 276c 6c20 6e65 6564 2074 6f20 696e 7374  'll need to inst
-00000e80: 616c 6c20 7468 6520 6070 6172 7175 6574  all the `parquet
-00000e90: 6020 6578 7472 612e 204f 722c 2065 7665  ` extra. Or, eve
-00000ea0: 6e20 7369 6d70 6c65 722c 0a79 6f75 2063  n simpler,.you c
-00000eb0: 616e 2069 6e73 7461 6c6c 2074 6865 2060  an install the `
-00000ec0: 616c 6c60 2065 7874 7261 2074 6f20 6765  all` extra to ge
-00000ed0: 7420 616c 6c20 7468 6520 6578 7472 6173  t all the extras
-00000ee0: 2e0a 0a60 6060 7368 656c 6c0a 7069 7078  ...```shell.pipx
-00000ef0: 2069 6e73 7461 6c6c 2022 6272 6f77 7372   install "browsr
-00000f00: 5b61 6c6c 5d22 0a60 6060 0a0a 2323 2055  [all]".```..## U
-00000f10: 7361 6765 0a0a 6060 6073 6865 6c6c 0a62  sage..```shell.b
-00000f20: 726f 7773 7220 7e2f 446f 776e 6c6f 6164  rowsr ~/Download
-00000f30: 732f 0a60 6060 0a0a 5369 6d70 6c79 2067  s/.```..Simply g
-00000f40: 6976 6520 6062 726f 7773 7260 2061 2070  ive `browsr` a p
-00000f50: 6174 6820 746f 2061 2066 696c 652f 6469  ath to a file/di
-00000f60: 7265 6374 6f72 7920 616e 6420 6974 2077  rectory and it w
-00000f70: 696c 6c20 6f70 656e 2061 2062 726f 7773  ill open a brows
-00000f80: 6572 2077 696e 646f 770a 7769 7468 2061  er window.with a
-00000f90: 2066 696c 6520 6272 6f77 7365 722e 2059   file browser. Y
-00000fa0: 6f75 2063 616e 2061 6c73 6f20 6769 7665  ou can also give
-00000fb0: 2069 7420 6120 5552 4c20 746f 2061 2072   it a URL to a r
-00000fc0: 656d 6f74 6520 6669 6c65 2073 7973 7465  emote file syste
-00000fd0: 6d2c 206c 696b 6520 4157 5320 5333 2e0a  m, like AWS S3..
-00000fe0: 0a60 6060 7368 656c 6c0a 6272 6f77 7372  .```shell.browsr
-00000ff0: 2073 333a 2f2f 6d79 2d62 7563 6b65 742f   s3://my-bucket/
-00001000: 6d79 2d66 696c 652e 7061 7271 7565 740a  my-file.parquet.
-00001010: 6060 600a 0a23 2323 205b 4368 6563 6b20  ```..### [Check 
-00001020: 6f75 7420 7468 6520 446f 6375 6d65 6e74  out the Document
-00001030: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6a  ation](https://j
-00001040: 7566 7469 6e2e 636f 6d2f 6272 6f77 7372  uftin.com/browsr
-00001050: 2f29 2066 6f72 206d 6f72 650a 0a23 2320  /) for more..## 
-00001060: 4c69 6365 6e73 650a 0a2a 2a60 6272 6f77  License..**`brow
-00001070: 7372 602a 2a20 6973 2064 6973 7472 6962  sr`** is distrib
-00001080: 7574 6564 2075 6e64 6572 2074 6865 2074  uted under the t
-00001090: 6572 6d73 206f 6620 7468 6520 5b4d 4954  erms of the [MIT
-000010a0: 206c 6963 656e 7365 5d28 4c49 4345 4e53   license](LICENS
-000010b0: 4529 2e0a                                E)..
+000006d0: 2020 2020 3c70 6963 7475 7265 3e0a 2020      <picture>.  
+000006e0: 2020 2020 2020 3c69 6d67 2073 7263 3d68        <img src=h
+000006f0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000700: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000710: 2f6a 7566 7469 6e2f 6272 6f77 7372 2f6d  /juftin/browsr/m
+00000720: 6169 6e2f 646f 6373 2f5f 7374 6174 6963  ain/docs/_static
+00000730: 2f62 726f 7773 722e 706e 670a 2020 2020  /browsr.png.    
+00000740: 2020 2020 2020 2020 2077 6964 7468 3d22           width="
+00000750: 3430 3022 2061 6c74 3d22 6272 6f77 7372  400" alt="browsr
+00000760: 223e 0a20 2020 203c 2f70 6963 7475 7265  ">.    </picture
+00000770: 3e0a 3c2f 6469 763e 0a0a 5b21 5b62 726f  >.</div>..[![bro
+00000780: 7773 7220 5665 7273 696f 6e5d 2868 7474  wsr Version](htt
+00000790: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000007a0: 2e69 6f2f 7079 7069 2f76 2f62 726f 7773  .io/pypi/v/brows
+000007b0: 723f 636f 6c6f 723d 626c 7565 266c 6162  r?color=blue&lab
+000007c0: 656c 3d62 726f 7773 7229 5d28 6874 7470  el=browsr)](http
+000007d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+000007e0: 7566 7469 6e2f 6272 6f77 7372 290a 5b21  uftin/browsr).[!
+000007f0: 5b50 7950 495d 2868 7474 7073 3a2f 2f69  [PyPI](https://i
+00000800: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000810: 7069 2f70 7976 6572 7369 6f6e 732f 6272  pi/pyversions/br
+00000820: 6f77 7372 295d 2868 7474 7073 3a2f 2f70  owsr)](https://p
+00000830: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
+00000840: 7970 692f 6272 6f77 7372 2f29 0a5b 215b  ypi/browsr/).[![
+00000850: 5465 7374 696e 6720 5374 6174 7573 5d28  Testing Status](
+00000860: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000870: 6f6d 2f6a 7566 7469 6e2f 6272 6f77 7372  om/juftin/browsr
+00000880: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000890: 7773 2f74 6573 7473 2e79 616d 6c2f 6261  ws/tests.yaml/ba
+000008a0: 6467 652e 7376 673f 6272 616e 6368 3d6d  dge.svg?branch=m
+000008b0: 6169 6e29 5d28 6874 7470 733a 2f2f 6769  ain)](https://gi
+000008c0: 7468 7562 2e63 6f6d 2f6a 7566 7469 6e2f  thub.com/juftin/
+000008d0: 6272 6f77 7372 2f61 6374 696f 6e73 2f77  browsr/actions/w
+000008e0: 6f72 6b66 6c6f 7773 2f74 6573 7473 2e79  orkflows/tests.y
+000008f0: 616d 6c3f 7175 6572 793d 6272 616e 6368  aml?query=branch
+00000900: 2533 416d 6169 6e29 0a5b 215b 4769 7448  %3Amain).[![GitH
+00000910: 7562 204c 6963 656e 7365 5d28 6874 7470  ub License](http
+00000920: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000930: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
+00000940: 652f 6a75 6674 696e 2f62 726f 7773 723f  e/juftin/browsr?
+00000950: 636f 6c6f 723d 626c 7565 266c 6162 656c  color=blue&label
+00000960: 3d4c 6963 656e 7365 295d 2868 7474 7073  =License)](https
+00000970: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
+00000980: 6674 696e 2f62 726f 7773 722f 626c 6f62  ftin/browsr/blob
+00000990: 2f6d 6169 6e2f 4c49 4345 4e53 4529 0a0a  /main/LICENSE)..
+000009a0: 2a2a 6062 726f 7773 7260 2a2a 2069 7320  **`browsr`** is 
+000009b0: 6120 5455 4920 2874 6578 742d 6261 7365  a TUI (text-base
+000009c0: 6420 7573 6572 2069 6e74 6572 6661 6365  d user interface
+000009d0: 2920 6669 6c65 2062 726f 7773 6572 2066  ) file browser f
+000009e0: 6f72 2079 6f75 7220 7465 726d 696e 616c  or your terminal
+000009f0: 2e0a 4974 2773 2061 2073 696d 706c 6520  ..It's a simple 
+00000a00: 7761 7920 746f 2062 726f 7773 6520 796f  way to browse yo
+00000a10: 7572 2066 696c 6573 2061 6e64 2074 616b  ur files and tak
+00000a20: 6520 6120 7065 656b 2061 7420 7468 6569  e a peek at thei
+00000a30: 7220 636f 6e74 656e 7473 2e20 506c 7573  r contents. Plus
+00000a40: 2069 740a 776f 726b 7320 6f6e 206c 6f63   it.works on loc
+00000a50: 616c 2061 6e64 2072 656d 6f74 6520 6669  al and remote fi
+00000a60: 6c65 2073 7973 7465 6d73 2e0a 0a3c 6465  le systems...<de
+00000a70: 7461 696c 7320 6f70 656e 3e3c 2f73 756d  tails open></sum
+00000a80: 6d61 7279 3e3c 2f73 756d 6d61 7279 3e0a  mary></summary>.
+00000a90: 0a3c 626f 6479 3e0a 3c64 6976 2073 7479  .<body>.<div sty
+00000aa0: 6c65 3d22 6469 7370 6c61 793a 2067 7269  le="display: gri
+00000ab0: 643b 2067 7269 642d 7465 6d70 6c61 7465  d; grid-template
+00000ac0: 2d63 6f6c 756d 6e73 3a20 7265 7065 6174  -columns: repeat
+00000ad0: 2832 2c20 3166 7229 3b20 6772 6964 2d67  (2, 1fr); grid-g
+00000ae0: 6170 3a20 3130 7078 3b22 3e0a 2020 2020  ap: 10px;">.    
+00000af0: 3c70 6963 7475 7265 3e0a 2020 2020 2020  <picture>.      
+00000b00: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000b10: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000b20: 6572 636f 6e74 656e 742e 636f 6d2f 6a75  ercontent.com/ju
+00000b30: 6674 696e 2f62 726f 7773 722f 6d61 696e  ftin/browsr/main
+00000b40: 2f64 6f63 732f 5f73 7461 7469 632f 7363  /docs/_static/sc
+00000b50: 7265 656e 7368 6f74 5f75 7469 6c73 2e70  reenshot_utils.p
+00000b60: 6e67 2220 616c 743d 2249 6d61 6765 2031  ng" alt="Image 1
+00000b70: 223e 0a20 2020 203c 2f70 6963 7475 7265  ">.    </picture
+00000b80: 3e0a 2020 2020 3c70 6963 7475 7265 3e0a  >.    <picture>.
+00000b90: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000ba0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+00000bb0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000bc0: 636f 6d2f 6a75 6674 696e 2f62 726f 7773  com/juftin/brows
+00000bd0: 722f 6d61 696e 2f64 6f63 732f 5f73 7461  r/main/docs/_sta
+00000be0: 7469 632f 7363 7265 656e 7368 6f74 5f64  tic/screenshot_d
+00000bf0: 6174 6174 6162 6c65 2e70 6e67 2220 616c  atatable.png" al
+00000c00: 743d 2249 6d61 6765 2032 223e 0a20 2020  t="Image 2">.   
+00000c10: 203c 2f70 6963 7475 7265 3e0a 2020 2020   </picture>.    
+00000c20: 3c70 6963 7475 7265 3e0a 2020 2020 2020  <picture>.      
+00000c30: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000c40: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000c50: 6572 636f 6e74 656e 742e 636f 6d2f 6a75  ercontent.com/ju
+00000c60: 6674 696e 2f62 726f 7773 722f 6d61 696e  ftin/browsr/main
+00000c70: 2f64 6f63 732f 5f73 7461 7469 632f 7363  /docs/_static/sc
+00000c80: 7265 656e 7368 6f74 5f6d 6f6e 615f 6c69  reenshot_mona_li
+00000c90: 7361 2e70 6e67 2220 616c 743d 2249 6d61  sa.png" alt="Ima
+00000ca0: 6765 2033 223e 0a20 2020 203c 2f70 6963  ge 3">.    </pic
+00000cb0: 7475 7265 3e0a 2020 2020 3c70 6963 7475  ture>.    <pictu
+00000cc0: 7265 3e0a 2020 2020 2020 2020 3c69 6d67  re>.        <img
+00000cd0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00000ce0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00000cf0: 656e 742e 636f 6d2f 6a75 6674 696e 2f62  ent.com/juftin/b
+00000d00: 726f 7773 722f 6d61 696e 2f64 6f63 732f  rowsr/main/docs/
+00000d10: 5f73 7461 7469 632f 7363 7265 656e 7368  _static/screensh
+00000d20: 6f74 5f6d 6172 6b64 6f77 6e2e 706e 6722  ot_markdown.png"
+00000d30: 2061 6c74 3d22 496d 6167 6520 3422 3e0a   alt="Image 4">.
+00000d40: 2020 2020 3c2f 7069 6374 7572 653e 0a3c      </picture>.<
+00000d50: 2f64 6976 3e0a 3c2f 626f 6479 3e0a 0a3c  /div>.</body>..<
+00000d60: 2f64 6574 6169 6c73 3e0a 0a23 2320 496e  /details>..## In
+00000d70: 7374 616c 6c61 7469 6f6e 0a0a 5468 6520  stallation..The 
+00000d80: 6265 6c6f 7720 636f 6d6d 616e 6420 7265  below command re
+00000d90: 636f 6d6d 656e 6473 205b 7069 7078 5d28  commends [pipx](
+00000da0: 6874 7470 733a 2f2f 7079 7061 2e67 6974  https://pypa.git
+00000db0: 6875 622e 696f 2f70 6970 782f 2920 696e  hub.io/pipx/) in
+00000dc0: 7374 6561 6420 6f66 2070 6970 2e20 6070  stead of pip. `p
+00000dd0: 6970 7860 2069 6e73 7461 6c6c 7320 7468  ipx` installs th
+00000de0: 6520 7061 636b 6167 6520 696e 0a61 6e20  e package in.an 
+00000df0: 6973 6f6c 6174 6564 2065 6e76 6972 6f6e  isolated environ
+00000e00: 6d65 6e74 2061 6e64 206d 616b 6573 2069  ment and makes i
+00000e10: 7420 6561 7379 2074 6f20 756e 696e 7374  t easy to uninst
+00000e20: 616c 6c2e 2049 6620 796f 7527 6420 6c69  all. If you'd li
+00000e30: 6b65 2074 6f20 7573 6520 6070 6970 6020  ke to use `pip` 
+00000e40: 696e 7374 6561 642c 206a 7573 7420 7265  instead, just re
+00000e50: 706c 6163 6520 6070 6970 7860 0a77 6974  place `pipx`.wit
+00000e60: 6820 6070 6970 6020 696e 2074 6865 2062  h `pip` in the b
+00000e70: 656c 6f77 2063 6f6d 6d61 6e64 2e0a 0a60  elow command...`
+00000e80: 6060 7368 656c 6c0a 7069 7078 2069 6e73  ``shell.pipx ins
+00000e90: 7461 6c6c 2062 726f 7773 720a 6060 600a  tall browsr.```.
+00000ea0: 0a23 2320 4578 7472 6120 496e 7374 616c  .## Extra Instal
+00000eb0: 6c61 7469 6f6e 0a0a 4966 2079 6f75 2772  lation..If you'r
+00000ec0: 6520 6c6f 6f6b 696e 6720 746f 2075 7365  e looking to use
+00000ed0: 202a 2a60 6272 6f77 7372 602a 2a20 6f6e   **`browsr`** on
+00000ee0: 2072 656d 6f74 6520 6669 6c65 2073 7973   remote file sys
+00000ef0: 7465 6d73 2c20 6c69 6b65 2041 5753 2053  tems, like AWS S
+00000f00: 332c 2079 6f75 276c 6c20 6e65 6564 2074  3, you'll need t
+00000f10: 6f20 696e 7374 616c 6c20 7468 6520 6072  o install the `r
+00000f20: 656d 6f74 6560 2065 7874 7261 2e0a 4966  emote` extra..If
+00000f30: 2079 6f75 2764 206c 696b 6520 746f 2062   you'd like to b
+00000f40: 726f 7773 6520 7061 7271 7565 7420 6669  rowse parquet fi
+00000f50: 6c65 732c 2079 6f75 276c 6c20 6e65 6564  les, you'll need
+00000f60: 2074 6f20 696e 7374 616c 6c20 7468 6520   to install the 
+00000f70: 6070 6172 7175 6574 6020 6578 7472 612e  `parquet` extra.
+00000f80: 204f 722c 2065 7665 6e20 7369 6d70 6c65   Or, even simple
+00000f90: 722c 0a79 6f75 2063 616e 2069 6e73 7461  r,.you can insta
+00000fa0: 6c6c 2074 6865 2060 616c 6c60 2065 7874  ll the `all` ext
+00000fb0: 7261 2074 6f20 6765 7420 616c 6c20 7468  ra to get all th
+00000fc0: 6520 6578 7472 6173 2e0a 0a60 6060 7368  e extras...```sh
+00000fd0: 656c 6c0a 7069 7078 2069 6e73 7461 6c6c  ell.pipx install
+00000fe0: 2022 6272 6f77 7372 5b61 6c6c 5d22 0a60   "browsr[all]".`
+00000ff0: 6060 0a0a 2323 2055 7361 6765 0a0a 6060  ``..## Usage..``
+00001000: 6073 6865 6c6c 0a62 726f 7773 7220 7e2f  `shell.browsr ~/
+00001010: 446f 776e 6c6f 6164 732f 0a60 6060 0a0a  Downloads/.```..
+00001020: 5369 6d70 6c79 2067 6976 6520 2a2a 6062  Simply give **`b
+00001030: 726f 7773 7260 2a2a 2061 2070 6174 6820  rowsr`** a path 
+00001040: 746f 2061 2066 696c 652f 6469 7265 6374  to a file/direct
+00001050: 6f72 7920 616e 6420 6974 2077 696c 6c20  ory and it will 
+00001060: 6f70 656e 2061 2062 726f 7773 6572 2077  open a browser w
+00001070: 696e 646f 770a 7769 7468 2061 2066 696c  indow.with a fil
+00001080: 6520 6272 6f77 7365 722e 2059 6f75 2063  e browser. You c
+00001090: 616e 2061 6c73 6f20 6769 7665 2069 7420  an also give it 
+000010a0: 6120 5552 4c20 746f 2061 2072 656d 6f74  a URL to a remot
+000010b0: 6520 6669 6c65 2073 7973 7465 6d2c 206c  e file system, l
+000010c0: 696b 6520 4157 5320 5333 2e0a 0a60 6060  ike AWS S3...```
+000010d0: 7368 656c 6c0a 6272 6f77 7372 2073 333a  shell.browsr s3:
+000010e0: 2f2f 6d79 2d62 7563 6b65 742f 6d79 2d66  //my-bucket/my-f
+000010f0: 696c 652e 7061 7271 7565 740a 6060 600a  ile.parquet.```.
+00001100: 0a23 2323 205b 4368 6563 6b20 6f75 7420  .### [Check out 
+00001110: 7468 6520 446f 6375 6d65 6e74 6174 696f  the Documentatio
+00001120: 6e5d 2868 7474 7073 3a2f 2f6a 7566 7469  n](https://jufti
+00001130: 6e2e 636f 6d2f 6272 6f77 7372 2f29 2066  n.com/browsr/) f
+00001140: 6f72 206d 6f72 650a 0a23 2320 4c69 6365  or more..## Lice
+00001150: 6e73 650a 0a2a 2a60 6272 6f77 7372 602a  nse..**`browsr`*
+00001160: 2a20 6973 2064 6973 7472 6962 7574 6564  * is distributed
+00001170: 2075 6e64 6572 2074 6865 2074 6572 6d73   under the terms
+00001180: 206f 6620 7468 6520 5b4d 4954 206c 6963   of the [MIT lic
+00001190: 656e 7365 5d28 4c49 4345 4e53 4529 2e0a  ense](LICENSE)..
```

