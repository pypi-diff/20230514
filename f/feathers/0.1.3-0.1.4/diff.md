# Comparing `tmp/feathers-0.1.3.tar.gz` & `tmp/feathers-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feathers-0.1.3.tar", max compression
+gzip compressed data, was "feathers-0.1.4.tar", max compression
```

## Comparing `feathers-0.1.3.tar` & `feathers-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       29 2023-05-13 06:59:34.277125 feathers-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/__init__.py
--rw-r--r--   0        0        0       53 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/__main__.py
--rw-r--r--   0        0        0     5996 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/cache.py
--rw-r--r--   0        0        0      161 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/demo.py
--rw-r--r--   0        0        0       71 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/renderables/__init__.py
--rw-r--r--   0        0        0     3187 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/renderables/_divider.py
--rw-r--r--   0        0        0       64 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/utils/__init__.py
--rw-r--r--   0        0        0      763 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/utils/_errors.py
--rw-r--r--   0        0        0      202 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/widgets/__init__.py
--rw-r--r--   0        0        0     5932 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/widgets/_cached_view.py
--rw-r--r--   0        0        0     9016 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/widgets/_nav_view.py
--rw-r--r--   0        0        0      146 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/widgets/chat/__init__.py
--rw-r--r--   0        0        0     2445 2023-05-13 06:59:34.277125 feathers-0.1.3/feathers/widgets/chat/_chat.py
--rw-r--r--   0        0        0     1113 2023-05-13 06:59:34.281126 feathers-0.1.3/feathers/widgets/chat/_models.py
--rw-r--r--   0        0        0     2193 2023-05-13 06:59:34.281126 feathers-0.1.3/feathers/widgets/chat/_renderers.py
--rw-r--r--   0        0        0      118 2023-05-13 06:59:34.281126 feathers-0.1.3/feathers/widgets/help/__init__.py
--rw-r--r--   0        0        0     1125 2023-05-13 06:59:34.281126 feathers-0.1.3/feathers/widgets/help/_base.py
--rw-r--r--   0        0        0     3684 2023-05-13 06:59:34.281126 feathers-0.1.3/feathers/widgets/help/_help.py
--rw-r--r--   0        0        0     5784 2023-05-13 06:59:34.281126 feathers-0.1.3/feathers/widgets/help/_long_help.py
--rw-r--r--   0        0        0      714 2023-05-13 06:59:34.281126 feathers-0.1.3/feathers/widgets/help/_models.py
--rw-r--r--   0        0        0     3999 2023-05-13 06:59:34.281126 feathers-0.1.3/feathers/widgets/help/_short_help.py
--rw-r--r--   0        0        0     1307 2023-05-13 06:59:34.281126 feathers-0.1.3/feathers/widgets/help/_utils.py
--rw-r--r--   0        0        0      907 2023-05-13 06:59:34.281126 feathers-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 feathers-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-05-14 10:38:47.181382 feathers-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/__main__.py
+-rw-r--r--   0        0        0     6502 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/cache.py
+-rw-r--r--   0        0        0      161 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/demo.py
+-rw-r--r--   0        0        0       71 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/renderables/__init__.py
+-rw-r--r--   0        0        0     3187 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/renderables/_divider.py
+-rw-r--r--   0        0        0       64 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/utils/__init__.py
+-rw-r--r--   0        0        0      763 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/utils/_errors.py
+-rw-r--r--   0        0        0      202 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/widgets/__init__.py
+-rw-r--r--   0        0        0     6561 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/widgets/_cached_view.py
+-rw-r--r--   0        0        0     9016 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/widgets/_nav_view.py
+-rw-r--r--   0        0        0      146 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/widgets/chat/__init__.py
+-rw-r--r--   0        0        0     2451 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/widgets/chat/_chat.py
+-rw-r--r--   0        0        0     1113 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/widgets/chat/_models.py
+-rw-r--r--   0        0        0     2193 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/widgets/chat/_renderers.py
+-rw-r--r--   0        0        0      118 2023-05-14 10:38:47.181382 feathers-0.1.4/feathers/widgets/help/__init__.py
+-rw-r--r--   0        0        0     1125 2023-05-14 10:38:47.185382 feathers-0.1.4/feathers/widgets/help/_base.py
+-rw-r--r--   0        0        0     3684 2023-05-14 10:38:47.185382 feathers-0.1.4/feathers/widgets/help/_help.py
+-rw-r--r--   0        0        0     5784 2023-05-14 10:38:47.185382 feathers-0.1.4/feathers/widgets/help/_long_help.py
+-rw-r--r--   0        0        0      714 2023-05-14 10:38:47.185382 feathers-0.1.4/feathers/widgets/help/_models.py
+-rw-r--r--   0        0        0     3999 2023-05-14 10:38:47.185382 feathers-0.1.4/feathers/widgets/help/_short_help.py
+-rw-r--r--   0        0        0     1307 2023-05-14 10:38:47.185382 feathers-0.1.4/feathers/widgets/help/_utils.py
+-rw-r--r--   0        0        0      907 2023-05-14 10:38:47.185382 feathers-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 feathers-0.1.4/PKG-INFO
```

### Comparing `feathers-0.1.3/feathers/cache.py` & `feathers-0.1.4/feathers/cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from __future__ import annotations
 
 from collections import OrderedDict
 from dataclasses import dataclass
+from typing import NewType
 
 from rich.console import Console, ConsoleOptions, RenderableType
 from rich.measure import Measurement
 from rich.segment import Segment
 from rich.text import Text
 from textual.geometry import Size
 from textual.strip import Strip
 
 
 class CacheListener:
     def on_cache_update(self):
         pass
 
 
+CacheId = NewType("CacheId", str)
+
+
 @dataclass
 class RenderableWithOptions:
     renderableType: RenderableType
+    id: str | None = None
     width: int | None = None
     expand: bool | None = False
     strink: bool | None = True
     wrap: bool = False
 
 
 class RenderablesCache:
@@ -36,18 +41,18 @@
     def __init__(
         self, console: Console, options: ConsoleOptions | None = None, listener: CacheListener | None = None
     ) -> None:
         self._console = console
         self._options = options if options is not None else console.options
         self._listener = listener
 
-        self._all_renderables: OrderedDict[int, RenderableWithOptions] = OrderedDict()
-        self._renderables_added: list[int] = []
-        self._renderables_removed: list[int] = []
-        self._cache: list[tuple[int, Strip]] = []
+        self._all_renderables: OrderedDict[CacheId, RenderableWithOptions] = OrderedDict()
+        self._renderables_added: list[CacheId] = []
+        self._renderables_removed: list[CacheId] = []
+        self._cache: list[tuple[CacheId, Strip]] = []
         self._virtual_size: Size = Size(0, 0)
 
         self._content_width: int | None = None
 
     @property
     def virtual_size(self) -> Size:
         return self._virtual_size
@@ -59,29 +64,34 @@
     @content_width.setter
     def content_width(self, value: int) -> None:
         if value != self._content_width:
             self._content_width = value
             self.refresh()
 
     def strip_at(self, index: int) -> Strip | None:
+        """Get the strip at given index from cache"""
         if index >= len(self._cache):
             return None
         return self._cache[index][1]
 
     def add(self, renderable: RenderableWithOptions):
-        renderable_id = id(renderable)
-        self._all_renderables[renderable_id] = renderable
-        self._renderables_added.append(renderable_id)
-        self._update_cache()
-
-    def remove(self, renderable: RenderableWithOptions):
-        renderable_id = id(renderable)
-        self._renderables_removed.append(renderable_id)
-        self._all_renderables.pop(renderable_id)
-        self._update_cache()
+        """Add a new renderable. Pass the id in renderable if you intend to update or remove it later"""
+        renderable_id = CacheId(renderable.id) if renderable.id else CacheId(str(id(renderable)))
+        if renderable_id not in self._all_renderables:
+            self._all_renderables[renderable_id] = renderable
+            self._renderables_added.append(renderable_id)
+            self._update_cache()
+
+    def remove(self, id: str):
+        """Remove the renderable from cache. If missing, the operation is ignored"""
+        renderable_id = CacheId(id)
+        if id in self._all_renderables:
+            self._renderables_removed.append(renderable_id)
+            self._all_renderables.pop(renderable_id)
+            self._update_cache()
 
     def refresh(self) -> None:
         self._cache.clear()
         self._renderables_added.clear()
         self._renderables_removed.clear()
         for id in self._all_renderables.keys():
             self._renderables_added.append(id)
@@ -106,22 +116,22 @@
             is_updated = True
             self._remove_from_cache(id)
         self._renderables_removed.clear()
 
         if is_updated and self._listener is not None:
             self._listener.on_cache_update()
 
-    def _add_to_cache(self, id: int, renderable: RenderableWithOptions) -> None:
+    def _add_to_cache(self, id: CacheId, renderable: RenderableWithOptions) -> None:
         strips = self._extract_lines(renderable)
         if strips is None:
             return
         for strip in strips:
             self._cache.append((id, strip))
 
-    def _remove_from_cache(self, id: int) -> None:
+    def _remove_from_cache(self, id: CacheId) -> None:
         # By iterating over the list in reverse order, we can safely remove items without changing
         # the indices of the remaining items in the list. This approach can be more memory-efficient
         # than making a copy of the list to iterate over, especially for large lists, since we only need
         # to keep track of the current index and don't need to create a copy of the list.
         for i in range(len(self._cache) - 1, -1, -1):
             if id in self._cache[i]:
                 self._cache.pop(i)
```

### Comparing `feathers-0.1.3/feathers/renderables/_divider.py` & `feathers-0.1.4/feathers/renderables/_divider.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.3/feathers/utils/_errors.py` & `feathers-0.1.4/feathers/utils/_errors.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.3/feathers/widgets/_cached_view.py` & `feathers-0.1.4/feathers/widgets/_cached_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,15 +73,20 @@
 
         self._renderables_cache: RenderablesCache = RenderablesCache(self.app.console, listener=self)
 
     def notify_style_update(self) -> None:
         self._renderables_cache.refresh()
 
     def _extract_renderable(
-        self, content: RenderableType | object, width: int | None, expand: bool | None, shrink: bool | None
+        self,
+        content: RenderableType | object,
+        id: str | None,
+        width: int | None = None,
+        expand: bool | None = None,
+        shrink: bool | None = None,
     ) -> RenderableWithOptions:
         renderable: RenderableType
         if not is_renderable(content):
             renderable = Pretty(content)
         else:
             if isinstance(content, str):
                 if self.markup:
@@ -89,58 +94,74 @@
                 else:
                     renderable = Text(content)
                 if self.highlighter is not None:
                     renderable = self.highlighter(renderable)
             else:
                 renderable = cast(RenderableType, content)
 
-        return RenderableWithOptions(renderable, width, expand, shrink, self.wrap)
+        return RenderableWithOptions(renderable, id, width, expand, shrink, self.wrap)
 
-    def add(
+    def add_entry(
         self,
         content: RenderableType | object,
+        id: str | None = None,
+        *,
         width: int | None = None,
         expand: bool = False,
         shrink: bool = True,
         scroll_end: bool | None = None,
     ) -> CachedView:
         """Write text or a rich renderable.
 
         Args:
             content: Rich renderable (or text).
-            width: Width to render or `None` to use optimal width.
-                Only used if either or both expand and shrink are True.
+            id: The renderable id which can later be used to remove or update the renderable. Can be missing if no
+            update or remove is intended
+            width: Width to render or `None` to use optimal width. Only used if either or both expand and shrink are
+            True.
             expand: Enable expand to widget width, or `False` to use `width`.
             shrink: Enable shrinking of content to fit width.
             scroll_end: Enable automatic scroll to end, or `None` to use `self.auto_scroll`.
 
         Returns:
-            The `TextLog` instance.
+            The `CachedView` instance.
         """
 
         width = width or self.max_width
-        renderable = self._extract_renderable(content, width, expand, shrink)
+        renderable = self._extract_renderable(content, id, width, expand, shrink)
         self._renderables_cache.add(renderable)
 
         auto_scroll = self.auto_scroll if scroll_end is None else scroll_end
         if auto_scroll:
             self.scroll_end(animate=False)
 
         return self
 
-    def on_resize(self):
-        self._renderables_cache.content_width = self.scrollable_content_region.width
+    def remove_entry(self, id: str) -> CachedView:
+        """Remove a renderable from cache.
+
+        Args:
+            id: The id of the renderable to remove. If id is not found, the operation is ignored.
+
+        Returns:
+            The `CachedView` instance.
+        """
+        self._renderables_cache.remove(id)
+        return self
 
     def clear(self) -> CachedView:
         self._renderables_cache.clear()
         self.max_width = 0
         self.virtual_size = Size(0, 0)
         self.refresh()
         return self
 
+    def on_resize(self):
+        self._renderables_cache.content_width = self.scrollable_content_region.width
+
     def on_cache_update(self):
         self.virtual_size = self._renderables_cache.virtual_size
         if self.auto_scroll:
             self.scroll_end(animate=False)
 
     def line_count(self) -> int:
         return len(self._renderables_cache)
```

### Comparing `feathers-0.1.3/feathers/widgets/_nav_view.py` & `feathers-0.1.4/feathers/widgets/_nav_view.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.3/feathers/widgets/chat/_chat.py` & `feathers-0.1.4/feathers/widgets/chat/_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         if chat_style not in _VALID_CHAT_STYLES:
             raise InvalidChatStyle(f"Valid chat styles are {friendly_list(_VALID_CHAT_STYLES)}")
         return chat_style
 
     def add_chat(self, entry: ChatEntry) -> None:
         self._entries.append(entry)
         renderable = ChatRenderable(self._renderer, entry)
-        self.add(renderable)
+        self.add_entry(renderable)
 
     def get_entries(self) -> list[ChatEntry]:
         return self._entries
 
     def clear_all_chats(self) -> None:
         self._entries.clear()
         self.clear()
```

### Comparing `feathers-0.1.3/feathers/widgets/chat/_models.py` & `feathers-0.1.4/feathers/widgets/chat/_models.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.3/feathers/widgets/chat/_renderers.py` & `feathers-0.1.4/feathers/widgets/chat/_renderers.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.3/feathers/widgets/help/_base.py` & `feathers-0.1.4/feathers/widgets/help/_base.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.3/feathers/widgets/help/_help.py` & `feathers-0.1.4/feathers/widgets/help/_help.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.3/feathers/widgets/help/_long_help.py` & `feathers-0.1.4/feathers/widgets/help/_long_help.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.3/feathers/widgets/help/_models.py` & `feathers-0.1.4/feathers/widgets/help/_models.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.3/feathers/widgets/help/_short_help.py` & `feathers-0.1.4/feathers/widgets/help/_short_help.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.3/feathers/widgets/help/_utils.py` & `feathers-0.1.4/feathers/widgets/help/_utils.py`

 * *Files identical despite different names*

### Comparing `feathers-0.1.3/pyproject.toml` & `feathers-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feathers"
-version = "0.1.3"
+version = "0.1.4"
 description = "Beautiful TUI components written on top of Textual"
 authors = ["Shashank Tomar <shashank004@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "feathers"}]
 repository = "https://github.com/shashanktomar/feathers"
 keywords = ["textual", "terminal", "TUI"]
```

### Comparing `feathers-0.1.3/PKG-INFO` & `feathers-0.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feathers
-Version: 0.1.3
+Version: 0.1.4
 Summary: Beautiful TUI components written on top of Textual
 Home-page: https://github.com/shashanktomar/feathers
 License: MIT
 Keywords: textual,terminal,TUI
 Author: Shashank Tomar
 Author-email: shashank004@gmail.com
 Requires-Python: >=3.8,<4.0
```

