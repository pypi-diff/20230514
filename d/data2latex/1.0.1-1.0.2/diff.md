# Comparing `tmp/data2latex-1.0.1.tar.gz` & `tmp/data2latex-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2latex-1.0.1.tar", last modified: Sun May 14 12:47:27 2023, max compression
+gzip compressed data, was "data2latex-1.0.2.tar", last modified: Sun May 14 14:53:21 2023, max compression
```

## Comparing `data2latex-1.0.1.tar` & `data2latex-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 12:47:27.477002 data2latex-1.0.1/
--rw-rw-rw-   0        0        0     1094 2023-05-14 10:51:18.000000 data2latex-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     4905 2023-05-14 12:47:27.476001 data2latex-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2510 2023-05-14 12:42:09.000000 data2latex-1.0.1/README.md
--rw-rw-rw-   0        0        0     1824 2023-05-14 12:45:50.000000 data2latex-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 12:47:27.477002 data2latex-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 12:47:27.451002 data2latex-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 12:47:27.465072 data2latex-1.0.1/src/data2latex/
--rw-rw-rw-   0        0        0      266 2023-05-11 19:09:04.000000 data2latex-1.0.1/src/data2latex/__init__.py
--rw-rw-rw-   0        0        0     8211 2023-05-11 23:03:20.000000 data2latex-1.0.1/src/data2latex/dm.py
--rw-rw-rw-   0        0        0     7300 2023-05-07 19:42:55.000000 data2latex-1.0.1/src/data2latex/environments.py
--rw-rw-rw-   0        0        0    10015 2023-05-13 22:01:26.000000 data2latex-1.0.1/src/data2latex/features.py
--rw-rw-rw-   0        0        0     7369 2023-05-10 13:28:58.000000 data2latex-1.0.1/src/data2latex/iter_protocols.py
--rw-rw-rw-   0        0        0    30923 2023-05-13 22:38:12.000000 data2latex-1.0.1/src/data2latex/plot.py
--rw-rw-rw-   0        0        0    18502 2023-05-13 21:52:50.000000 data2latex-1.0.1/src/data2latex/table.py
-drwxrwxrwx   0        0        0        0 2023-05-14 12:47:27.475002 data2latex-1.0.1/src/data2latex.egg-info/
--rw-rw-rw-   0        0        0     4905 2023-05-14 12:47:27.000000 data2latex-1.0.1/src/data2latex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-05-14 12:47:27.000000 data2latex-1.0.1/src/data2latex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 12:47:27.000000 data2latex-1.0.1/src/data2latex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-05-14 12:47:27.000000 data2latex-1.0.1/src/data2latex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-14 12:47:27.000000 data2latex-1.0.1/src/data2latex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 14:53:21.630355 data2latex-1.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-05-14 10:51:18.000000 data2latex-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4905 2023-05-14 14:53:21.629356 data2latex-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2510 2023-05-14 12:42:09.000000 data2latex-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1824 2023-05-14 14:53:03.000000 data2latex-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 14:53:21.630355 data2latex-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 14:53:21.586357 data2latex-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 14:53:21.606361 data2latex-1.0.2/src/data2latex/
+-rw-rw-rw-   0        0        0      266 2023-05-11 19:09:04.000000 data2latex-1.0.2/src/data2latex/__init__.py
+-rw-rw-rw-   0        0        0     8211 2023-05-11 23:03:20.000000 data2latex-1.0.2/src/data2latex/dm.py
+-rw-rw-rw-   0        0        0     7300 2023-05-07 19:42:55.000000 data2latex-1.0.2/src/data2latex/environments.py
+-rw-rw-rw-   0        0        0    10015 2023-05-13 22:01:26.000000 data2latex-1.0.2/src/data2latex/features.py
+-rw-rw-rw-   0        0        0     7658 2023-05-14 14:44:36.000000 data2latex-1.0.2/src/data2latex/iter_protocols.py
+-rw-rw-rw-   0        0        0    30916 2023-05-14 14:44:36.000000 data2latex-1.0.2/src/data2latex/plot.py
+-rw-rw-rw-   0        0        0    18502 2023-05-13 21:52:50.000000 data2latex-1.0.2/src/data2latex/table.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:53:21.628356 data2latex-1.0.2/src/data2latex.egg-info/
+-rw-rw-rw-   0        0        0     4905 2023-05-14 14:53:21.000000 data2latex-1.0.2/src/data2latex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-05-14 14:53:21.000000 data2latex-1.0.2/src/data2latex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:53:21.000000 data2latex-1.0.2/src/data2latex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-05-14 14:53:21.000000 data2latex-1.0.2/src/data2latex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-14 14:53:21.000000 data2latex-1.0.2/src/data2latex.egg-info/top_level.txt
```

### Comparing `data2latex-1.0.1/LICENSE` & `data2latex-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.1/PKG-INFO` & `data2latex-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2latex
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package prototype for simple generation of LaTeX tables and plots from scientific data for use in any document.
 Author-email: Richard Kokštein <richard.Kokstein@fs.cvut.cz>
 License: MIT License
         
         Copyright (c) 2023 Richard Kokstein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `data2latex-1.0.1/README.md` & `data2latex-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.1/pyproject.toml` & `data2latex-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "data2latex"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Richard Kokštein", email="richard.Kokstein@fs.cvut.cz" },
 ]
 description = "Package prototype for simple generation of LaTeX tables and plots from scientific data for use in any document."
 keywords = ["generation", "latex", "table", "plot", "graph", "array", "datatable"]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
```

### Comparing `data2latex-1.0.1/src/data2latex/dm.py` & `data2latex-1.0.2/src/data2latex/dm.py`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.1/src/data2latex/environments.py` & `data2latex-1.0.2/src/data2latex/environments.py`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.1/src/data2latex/features.py` & `data2latex-1.0.2/src/data2latex/features.py`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.1/src/data2latex/iter_protocols.py` & `data2latex-1.0.2/src/data2latex/iter_protocols.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,23 @@
     Tuple,
     TypeAlias,
     Union,
     runtime_checkable,
 )
 
 
+def replace_multiple(
+    source: str, to_be_replaced: List[str], replace_with: str = ""
+) -> str:
+    result: str = source
+    for substring in to_be_replaced:
+        result = result.replace(substring, replace_with)
+    return result
+
+
 def dict2str(
     data: Any | Dict[Any, Any],
     enclose: bool = False,
     level: int = 1,
 ) -> str:
     result: str = ""
     if isinstance(data, dict):
@@ -27,15 +36,15 @@
             elif value == "":
                 if key[0] == "`":
                     parts.append(key[1:])
                 else:
                     parts.append(key)
             else:
                 new_value: str = dict2str(value, enclose=True, level=level + 1)
-                if new_value == "{}":
+                if replace_multiple(new_value, ["\t", "\n", " ", "%"]) == "{}":
                     continue
                 parts.append(f"{key}={new_value}")
         tabs = "\t" * level
         result = f"%\n{tabs}" + (",%\n" + tabs).join(parts) + "%\n"
         if enclose:
             result += "\t" * max(level - 1, 0)
     else:
```

### Comparing `data2latex-1.0.1/src/data2latex/plot.py` & `data2latex-1.0.2/src/data2latex/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
         "black",
     ],
     mark_stroke_color: Union[None, Color, List[Union[None, Color]]] = None,
     mark_fill_opacity: Union[float, List[float]] = 1.0,
     mark_stroke_opacity: Union[float, List[float]] = 0.0,
 ) -> None:
     """
-    Generate LaTeX scatter or line plot from input data. The plot is created with ``pgfplots`` package (``tikzpicture`` + ``axis`` environment). Data can be in the form of a list or an array of numbers for single single line. For plotting more data sets, input data should be in the form of list of lists as shown below:
+    Generate LaTeX scatter or line plot from input data. The plot is created with ``pgfplots`` package (``tikzpicture`` + ``axis`` environment). Data can be in the form of a list or an array of numbers for single line. For plotting more data sets, input data should be in the form of list of lists as shown below:
 
     .. highlight:: python
     .. code-block:: python
 
         X = [[dataset1_x], [dataset2_x]]
         Y = [[dataset1_y], [dataset2_y]]
         legend = ["dataset1", "dataset2"]
```

### Comparing `data2latex-1.0.1/src/data2latex/table.py` & `data2latex-1.0.2/src/data2latex/table.py`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.1/src/data2latex.egg-info/PKG-INFO` & `data2latex-1.0.2/src/data2latex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2latex
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package prototype for simple generation of LaTeX tables and plots from scientific data for use in any document.
 Author-email: Richard Kokštein <richard.Kokstein@fs.cvut.cz>
 License: MIT License
         
         Copyright (c) 2023 Richard Kokstein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

