# Comparing `tmp/docstruct-1.0.8.tar.gz` & `tmp/docstruct-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docstruct-1.0.8.tar", last modified: Mon Feb  6 14:12:04 2023, max compression
+gzip compressed data, was "docstruct-1.0.9.tar", last modified: Wed Feb  8 14:03:17 2023, max compression
```

## Comparing `docstruct-1.0.8.tar` & `docstruct-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-02-06 14:12:04.169346 docstruct-1.0.8/
--rw-r--r--   0 moran      (501) staff       (20)      403 2023-02-06 14:12:04.169075 docstruct-1.0.8/PKG-INFO
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-02-06 14:12:04.166092 docstruct-1.0.8/docstruct/
--rw-r--r--   0 moran      (501) staff       (20)      496 2023-02-05 15:39:51.000000 docstruct-1.0.8/docstruct/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)     6261 2023-02-01 16:30:22.000000 docstruct-1.0.8/docstruct/bounding_box.py
--rw-r--r--   0 moran      (501) staff       (20)      427 2023-02-01 07:14:44.000000 docstruct-1.0.8/docstruct/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     1390 2023-01-23 06:22:03.000000 docstruct-1.0.8/docstruct/graph.py
--rw-r--r--   0 moran      (501) staff       (20)     4654 2023-01-29 13:14:13.000000 docstruct-1.0.8/docstruct/hocr_parser.py
--rw-r--r--   0 moran      (501) staff       (20)     1876 2023-01-23 06:25:49.000000 docstruct-1.0.8/docstruct/ligatures.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-02-06 14:12:04.168789 docstruct-1.0.8/docstruct/paragraph_detection/
--rw-r--r--   0 moran      (501) staff       (20)        0 2023-01-17 08:52:54.000000 docstruct-1.0.8/docstruct/paragraph_detection/__init__.py
--rw-r--r--   0 moran      (501) staff       (20)      175 2023-01-17 10:37:46.000000 docstruct-1.0.8/docstruct/paragraph_detection/constants.py
--rw-r--r--   0 moran      (501) staff       (20)     4929 2023-01-24 07:20:21.000000 docstruct-1.0.8/docstruct/paragraph_detection/paragraph_extractor.py
--rw-r--r--   0 moran      (501) staff       (20)     3068 2023-01-18 12:50:41.000000 docstruct-1.0.8/docstruct/paragraph_detection/paragraph_sorter.py
--rw-r--r--   0 moran      (501) staff       (20)     2703 2023-02-02 08:56:14.000000 docstruct-1.0.8/docstruct/paragraph_detection/two_columns.py
--rw-r--r--   0 moran      (501) staff       (20)     1884 2023-02-02 09:17:13.000000 docstruct-1.0.8/docstruct/point.py
--rw-r--r--   0 moran      (501) staff       (20)     1935 2023-02-05 14:35:55.000000 docstruct-1.0.8/docstruct/searchable_pdf.py
--rw-r--r--   0 moran      (501) staff       (20)     2675 2023-02-02 09:07:22.000000 docstruct-1.0.8/docstruct/segment.py
--rw-r--r--   0 moran      (501) staff       (20)      829 2023-02-01 08:28:07.000000 docstruct-1.0.8/docstruct/space_partitioning.py
--rw-r--r--   0 moran      (501) staff       (20)    14436 2023-02-06 12:46:32.000000 docstruct-1.0.8/docstruct/text_block.py
--rw-r--r--   0 moran      (501) staff       (20)     3404 2023-02-05 14:34:26.000000 docstruct-1.0.8/docstruct/text_block_drawer.py
--rw-r--r--   0 moran      (501) staff       (20)     2995 2023-02-01 11:45:10.000000 docstruct-1.0.8/docstruct/text_block_splitter.py
--rw-r--r--   0 moran      (501) staff       (20)     4562 2023-02-05 14:33:32.000000 docstruct-1.0.8/docstruct/textract_parser.py
--rw-r--r--   0 moran      (501) staff       (20)      753 2023-01-29 15:19:18.000000 docstruct-1.0.8/docstruct/tree_traversals.py
-drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-02-06 14:12:04.167426 docstruct-1.0.8/docstruct.egg-info/
--rw-r--r--   0 moran      (501) staff       (20)      403 2023-02-06 14:12:04.000000 docstruct-1.0.8/docstruct.egg-info/PKG-INFO
--rw-r--r--   0 moran      (501) staff       (20)      789 2023-02-06 14:12:04.000000 docstruct-1.0.8/docstruct.egg-info/SOURCES.txt
--rw-r--r--   0 moran      (501) staff       (20)        1 2023-02-06 14:12:04.000000 docstruct-1.0.8/docstruct.egg-info/dependency_links.txt
--rw-r--r--   0 moran      (501) staff       (20)       98 2023-02-06 14:12:04.000000 docstruct-1.0.8/docstruct.egg-info/requires.txt
--rw-r--r--   0 moran      (501) staff       (20)       10 2023-02-06 14:12:04.000000 docstruct-1.0.8/docstruct.egg-info/top_level.txt
--rw-r--r--   0 moran      (501) staff       (20)       38 2023-02-06 14:12:04.169392 docstruct-1.0.8/setup.cfg
--rw-r--r--   0 moran      (501) staff       (20)      758 2023-02-06 12:35:22.000000 docstruct-1.0.8/setup.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-02-08 14:03:17.730759 docstruct-1.0.9/
+-rw-r--r--   0 moran      (501) staff       (20)      432 2023-02-08 14:03:17.730425 docstruct-1.0.9/PKG-INFO
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-02-08 14:03:17.726683 docstruct-1.0.9/docstruct/
+-rw-r--r--   0 moran      (501) staff       (20)      496 2023-02-08 11:41:35.000000 docstruct-1.0.9/docstruct/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)     6261 2023-02-08 08:24:52.000000 docstruct-1.0.9/docstruct/bounding_box.py
+-rw-r--r--   0 moran      (501) staff       (20)      602 2023-02-08 08:24:11.000000 docstruct-1.0.9/docstruct/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     1390 2023-02-08 08:31:34.000000 docstruct-1.0.9/docstruct/graph.py
+-rw-r--r--   0 moran      (501) staff       (20)     4654 2023-01-29 13:14:13.000000 docstruct-1.0.9/docstruct/hocr_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)     1876 2023-01-23 06:25:49.000000 docstruct-1.0.9/docstruct/ligatures.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-02-08 14:03:17.729948 docstruct-1.0.9/docstruct/paragraph_detection/
+-rw-r--r--   0 moran      (501) staff       (20)        0 2023-01-17 08:52:54.000000 docstruct-1.0.9/docstruct/paragraph_detection/__init__.py
+-rw-r--r--   0 moran      (501) staff       (20)      175 2023-01-17 10:37:46.000000 docstruct-1.0.9/docstruct/paragraph_detection/constants.py
+-rw-r--r--   0 moran      (501) staff       (20)     4929 2023-01-24 07:20:21.000000 docstruct-1.0.9/docstruct/paragraph_detection/paragraph_extractor.py
+-rw-r--r--   0 moran      (501) staff       (20)     3068 2023-01-18 12:50:41.000000 docstruct-1.0.9/docstruct/paragraph_detection/paragraph_sorter.py
+-rw-r--r--   0 moran      (501) staff       (20)     2703 2023-02-02 08:56:14.000000 docstruct-1.0.9/docstruct/paragraph_detection/two_columns.py
+-rw-r--r--   0 moran      (501) staff       (20)     2339 2023-02-08 04:54:35.000000 docstruct-1.0.9/docstruct/point.py
+-rw-r--r--   0 moran      (501) staff       (20)     1935 2023-02-05 14:35:55.000000 docstruct-1.0.9/docstruct/searchable_pdf.py
+-rw-r--r--   0 moran      (501) staff       (20)     2723 2023-02-08 09:35:12.000000 docstruct-1.0.9/docstruct/segment.py
+-rw-r--r--   0 moran      (501) staff       (20)      829 2023-02-01 08:28:07.000000 docstruct-1.0.9/docstruct/space_partitioning.py
+-rw-r--r--   0 moran      (501) staff       (20)    17499 2023-02-08 11:20:37.000000 docstruct-1.0.9/docstruct/text_block.py
+-rw-r--r--   0 moran      (501) staff       (20)     3408 2023-02-08 04:57:07.000000 docstruct-1.0.9/docstruct/text_block_drawer.py
+-rw-r--r--   0 moran      (501) staff       (20)     2995 2023-02-01 11:45:10.000000 docstruct-1.0.9/docstruct/text_block_splitter.py
+-rw-r--r--   0 moran      (501) staff       (20)     4562 2023-02-05 14:33:32.000000 docstruct-1.0.9/docstruct/textract_parser.py
+-rw-r--r--   0 moran      (501) staff       (20)      753 2023-02-08 05:18:17.000000 docstruct-1.0.9/docstruct/tree_traversals.py
+drwxr-xr-x   0 moran      (501) staff       (20)        0 2023-02-08 14:03:17.728187 docstruct-1.0.9/docstruct.egg-info/
+-rw-r--r--   0 moran      (501) staff       (20)      432 2023-02-08 14:03:17.000000 docstruct-1.0.9/docstruct.egg-info/PKG-INFO
+-rw-r--r--   0 moran      (501) staff       (20)      789 2023-02-08 14:03:17.000000 docstruct-1.0.9/docstruct.egg-info/SOURCES.txt
+-rw-r--r--   0 moran      (501) staff       (20)        1 2023-02-08 14:03:17.000000 docstruct-1.0.9/docstruct.egg-info/dependency_links.txt
+-rw-r--r--   0 moran      (501) staff       (20)       98 2023-02-08 14:03:17.000000 docstruct-1.0.9/docstruct.egg-info/requires.txt
+-rw-r--r--   0 moran      (501) staff       (20)       10 2023-02-08 14:03:17.000000 docstruct-1.0.9/docstruct.egg-info/top_level.txt
+-rw-r--r--   0 moran      (501) staff       (20)       38 2023-02-08 14:03:17.730809 docstruct-1.0.9/setup.cfg
+-rw-r--r--   0 moran      (501) staff       (20)      809 2023-02-08 14:02:50.000000 docstruct-1.0.9/setup.py
```

### Comparing `docstruct-1.0.8/docstruct/bounding_box.py` & `docstruct-1.0.9/docstruct/bounding_box.py`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/docstruct/graph.py` & `docstruct-1.0.9/docstruct/graph.py`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/docstruct/hocr_parser.py` & `docstruct-1.0.9/docstruct/hocr_parser.py`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/docstruct/ligatures.py` & `docstruct-1.0.9/docstruct/ligatures.py`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/docstruct/paragraph_detection/paragraph_extractor.py` & `docstruct-1.0.9/docstruct/paragraph_detection/paragraph_extractor.py`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/docstruct/paragraph_detection/paragraph_sorter.py` & `docstruct-1.0.9/docstruct/paragraph_detection/paragraph_sorter.py`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/docstruct/paragraph_detection/two_columns.py` & `docstruct-1.0.9/docstruct/paragraph_detection/two_columns.py`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/docstruct/point.py` & `docstruct-1.0.9/docstruct/point.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,69 @@
-import attr
-
-
-@attr.s(auto_attribs=True, frozen=True)
 class Point:
     """
     A point in 2D space."""
 
-    x: float
-    y: float
+    def __init__(self, x: float, y: float) -> None:
+        self.x = x
+        self.y = y
 
     def get_x(self) -> float:
         """Get the x coordinate of the point."""
         return self.x
 
     def get_y(self) -> float:
         """Get the y coordinate of the point."""
         return self.y
 
-    def __add__(self, other: "Point") -> "Point":
+    def __str__(self):
+        return f"Point(x={self.x:.3f}, y={self.y:.3f})"
 
+    def __repr__(self):
+        return self.__str__()
+
+    def __add__(self, other: "Point") -> "Point":
+        """Create a new point by adding two points."""
         if not isinstance(other, Point):
             raise TypeError(
                 "unsupported operand type(s) for +: "
                 + f"'{type(self).__name__}' and '{type(other).__name__}'"
             )
 
         return Point(self.x + other.x, self.y + other.y)
 
     def __sub__(self, other: "Point") -> "Point":
+        """Create a new point by subtracting two points."""
         if not isinstance(other, Point):
             raise TypeError(
                 "unsupported operand type(s) for -: "
                 + f"'{type(self).__name__}' and '{type(other).__name__}'"
             )
 
         return Point(self.x - other.x, self.y - other.y)
 
     def __mul__(self, other: float) -> "Point":
+        """Create a new point by multiplying a point by a scalar."""
         if not isinstance(other, (int, float)):
             raise TypeError(
                 "unsupported operand type(s) for *: "
                 + f"'{type(self).__name__}' and '{type(other).__name__}'"
             )
         return Point(self.x * other, self.y * other)
 
     def __rmul__(self, scalar: float) -> "Point":
         return self.__mul__(scalar)
 
     def __truediv__(self, other: float) -> "Point":
+        """Create a new point by dividing a point by a scalar."""
         if not isinstance(other, (int, float)):
             raise TypeError(
                 "unsupported operand type(s) for /: "
                 + f"'{type(self).__name__}' and '{type(other).__name__}'"
             )
         if other == 0:
             raise ZeroDivisionError("Division by zero is not allowed")
 
         return Point(self.x / other, self.y / other)
 
     def __abs__(self) -> float:
+        """Get the distance of the point from the origin."""
         return (self.x**2 + self.y**2) ** 0.5
```

### Comparing `docstruct-1.0.8/docstruct/searchable_pdf.py` & `docstruct-1.0.9/docstruct/searchable_pdf.py`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/docstruct/segment.py` & `docstruct-1.0.9/docstruct/segment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 class Segment:
     def __init__(self, left: float, right: float):
         self.left = left
         self.right = right
         self.validate_args()
 
     def validate_args(self):
+        """Check if the arguments are valid."""
         if self.left > self.right:
             raise ValueError(f"left={self.left} is greater than right={self.right}")
 
     def get_left(self) -> float:
         """Get the left value of the segment."""
         return self.left
```

### Comparing `docstruct-1.0.8/docstruct/space_partitioning.py` & `docstruct-1.0.9/docstruct/space_partitioning.py`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/docstruct/text_block.py` & `docstruct-1.0.9/docstruct/text_block.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 
         self.length: Optional[int] = None
         self.bounding_box: BoundingBox = bounding_box
         # self.children: list["TextBlock"] = children
         self.delimiter: str = delimiter
         self.set_children(children)
         self.set_parent(parent)
-        self.order: int = None
+        self.relative_order: int = None
         self.start_index: int = None
         self.end_index: int = None
 
-    def set_order(self, index: int):
-        """The index is the order of the block in the list of children of its parent."""
-        self.order = index
-
-    def get_order(self) -> int:
-        if self.order is None:
-            raise ValueError("The order of the block is not set")
-        return self.order
+    def set_relative_order(self, index: int):
+        """The index is the relative order of the block in the list of children of its parent."""
+        self.relative_order = index
+
+    def get_relative_order(self) -> int:
+        if self.relative_order is None:
+            raise ValueError("The relative order of the block is not set")
+        return self.relative_order
 
     def set_bounding_box(self):
         """
         Setting the bounding box of a box based on the bounding boxes of its children.
         For more information see the documentation of the BoundingBox class.
         """
         if self.bounding_box is not None:
@@ -174,15 +174,15 @@
 
     def get_ancestor(self, _class: type) -> "TextBlock":
         """
         Returns the ancestor of the block based on the type of the ancestor.
         """
         self_depth = TextBlock.get_depth_by_type(type(self))
         parent_depth = TextBlock.get_depth_by_type(_class)
-        if self_depth <= parent_depth:
+        if self_depth < parent_depth:
             raise TypeError(f"{_class} is not an ancestor of {type(self)}!")
         relative_depth = self_depth - parent_depth
         current = self
         for _ in range(relative_depth):
             current = current.get_parent()
         return current
 
@@ -193,15 +193,15 @@
         """
         if not isinstance(child, self.child_type):
             raise TypeError(
                 f"Child of type {type(self)} must be of type {self.child_type}"
             )
         self.children.append(child)
         child.set_parent(self)
-        child.set_order(len(self.children) - 1)
+        child.set_relative_order(len(self.children) - 1)
 
     def get_text(self):
         """
         Every block has an implicit text representation that can be retrieved by calling this method.
         """
         return self.delimiter.join([child.get_text() for child in self.children])
 
@@ -248,15 +248,15 @@
             self.set_length()
         return self.length
 
     def __str__(self):
         return self.get_text()
 
     def __repr__(self):
-        return f"{self.__class__.__name__}: {self.get_text()}"
+        return f"{self.__class__.__name__}:\n{self.get_text()}"
 
     def __len__(self):
         """The length of a block is the number of children it has."""
         return self.length
 
     def __iter__(self) -> Iterator["TextBlock"]:
         """Iterating over the children of a block."""
@@ -278,26 +278,37 @@
     def _get_char(self, index: int) -> Optional["Character"]:
         for child in self.children:
             if 0 <= index < child.length:
                 return child._get_char(index)
             index -= child.length + len(self.delimiter)
         return None
 
+    def set_absolute_order(self, absolute_order: int):
+        """
+        Set the absolute order of the block in the document.
+        """
+        self.absolute_order = absolute_order
+
+    def get_absolute_order(self) -> int:
+        """
+        Returns the absolute order of the block in the document.
+        """
+        return self.absolute_order
+
     def set_start_index(self) -> int:
         """
         Returns the index of the first character of the block in the document.
         """
         if self.parent is None:
             self.start_index = 0
             return
         start_index = self.parent.get_start_index()
-        for child in self.parent.children[: self.order]:
+        for child in self.parent.children[: self.relative_order]:
             start_index += child.get_length() + len(self.parent.delimiter)
         self.start_index = start_index
-        # TODO add here code
 
     def get_start_index(self):
         if self.start_index is None:
             self.set_start_index()
         return self.start_index
 
     def set_end_index(self):
@@ -311,15 +322,15 @@
             self.set_end_index()
         return self.end_index
 
 
 class Character(TextBlock):
     """
     The Character class represents a single character (not including delimiters).
-    Notice this class play a special role in the hierarchy of TextBox because it is the leaf of the document tree,
+    Notice this class play a special role in the hierarchy of TextBlock because it is the leaf of the document tree,
     and as such, it overrides some of the methods of its parent class.
     """
 
     child_type = None
 
     def __init__(self, bounding_box: BoundingBox, char: str):
         super().__init__(bounding_box=bounding_box)
@@ -424,14 +435,74 @@
     """
 
     child_type = Page
 
     def __init__(self, children: list[Page] = None):
         super().__init__(delimiter=PAGE_DELIMITER, children=children)
         self.set_length()
+
         for text_block in pre_order_traversal(self):
             text_block.set_start_index()
             text_block.set_end_index()
+        block_types = [Page, Paragraph, Line, Word, Character]
+        for block_type in block_types:
+            text_blocks = self.get_all(block_type)
+            for i, text_block in enumerate(text_blocks):
+                text_block.set_absolute_order(i)
+
         self.text = self.get_text()
 
     def set_bounding_box(self):
         return
+
+    def get_text_block_number(
+        self, index: int, text_block_type: type, absolute: bool
+    ) -> Optional[int]:
+        """Get the absolute or relative order of the text block of type text_block_type that contains
+        the character at index `index`."""
+        character = self[index]
+        if character is not None:
+            text_block = character.get_ancestor(text_block_type)
+            if absolute:
+                return text_block.get_absolute_order()
+            return text_block.get_relative_order()
+        previous_char = self[index - 1]
+        next_char = self[index + 1]
+        if previous_char is None or next_char is None:
+            return None
+        previous_text_block = previous_char.get_ancestor(text_block_type)
+        next_text_block = next_char.get_ancestor(text_block_type)
+        if previous_text_block == next_text_block:
+            if absolute:
+                return previous_text_block.get_absolute_order()
+            return previous_text_block.get_relative_order()
+        return None
+
+    def get_relative_page_number(self, index: int) -> int:
+        return self.get_text_block_number(index, Page, absolute=False)
+
+    def get_relative_paragraph_number(self, index: int) -> int:
+        return self.get_text_block_number(index, Paragraph, absolute=False)
+
+    def get_relative_line_number(self, index: int) -> int:
+        return self.get_text_block_number(index, Line, absolute=False)
+
+    def get_relative_word_number(self, index: int) -> int:
+        return self.get_text_block_number(index, Word, absolute=False)
+
+    def get_relative_character_number(self, index: int) -> int:
+        return self.get_text_block_number(index, Character, absolute=False)
+
+    def get_absolute_page_number(self, index: int) -> int:
+        return self.get_text_block_number(index, Page, absolute=True)
+
+    def get_absolute_paragraph_number(self, index: int) -> int:
+        return self.get_text_block_number(index, Paragraph, absolute=True)
+
+    def get_absolute_line_number(self, index: int) -> int:
+        return self.get_text_block_number(index, Line, absolute=True)
+
+    def get_absolute_word_number(self, index: int) -> int:
+        return self.get_text_block_number(index, Word, absolute=True)
+
+    def get_absolute_character_number(self, index: int) -> int:
+        return self.get_text_block_number(index, Character, absolute=True)
```

### Comparing `docstruct-1.0.8/docstruct/text_block_drawer.py` & `docstruct-1.0.9/docstruct/text_block_drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 
 class TextBlockDrawer:
     """
     This class is used to draw bounding boxes of text blocks on an image.
     Example:
 
-    from docstruct import TextBoxDrawer
+    from docstruct import TextBlockDrawer
     image_path = 'foo.png'
     page = Page() ...
-    drawer = TextBoxDrawer(image_path)
+    drawer = TextBlockDrawer(image_path)
     drawer.draw(page)
     drawer.show()
     """
 
     def __init__(self, image_path: str):
         self.image_path = image_path
         self.image = Image.open(image_path)
```

### Comparing `docstruct-1.0.8/docstruct/text_block_splitter.py` & `docstruct-1.0.9/docstruct/text_block_splitter.py`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/docstruct/textract_parser.py` & `docstruct-1.0.9/docstruct/textract_parser.py`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/docstruct/tree_traversals.py` & `docstruct-1.0.9/docstruct/tree_traversals.py`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/docstruct.egg-info/SOURCES.txt` & `docstruct-1.0.9/docstruct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docstruct-1.0.8/setup.py` & `docstruct-1.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name="docstruct",
-    version="1.0.8",
+    version="1.0.9",
     description="A package for representing documents as a tree of document, pages, paragraphs, lines, words, and characters",
     long_description=open("docstruct/README.md").read(),
+    long_description_content_type="text/markdown",
     author="Moran Nechushtan",
     author_email="moran.n@trullion.com",
     url="https://github.com/smrt-co/docstruct",
     packages=setuptools.find_packages(),
     install_requires=[
         "pillow>=8.1.1",
         "beautifulsoup4>=4.11.1",
```

