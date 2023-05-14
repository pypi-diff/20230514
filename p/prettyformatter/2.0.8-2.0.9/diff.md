# Comparing `tmp/prettyformatter-2.0.8.tar.gz` & `tmp/prettyformatter-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettyformatter-2.0.8.tar", last modified: Wed Jan 25 02:11:07 2023, max compression
+gzip compressed data, was "prettyformatter-2.0.9.tar", last modified: Wed Jan 25 04:03:26 2023, max compression
```

## Comparing `prettyformatter-2.0.8.tar` & `prettyformatter-2.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 02:11:07.485370 prettyformatter-2.0.8/
--rw-rw-rw-   0        0        0     1087 2022-09-26 04:08:23.000000 prettyformatter-2.0.8/LICENSE
--rw-rw-rw-   0        0        0     5049 2023-01-25 02:11:07.479377 prettyformatter-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4003 2022-09-26 04:08:23.000000 prettyformatter-2.0.8/README.md
--rw-rw-rw-   0        0        0     1032 2022-09-26 04:08:23.000000 prettyformatter-2.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-25 02:11:07.490273 prettyformatter-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0      240 2022-09-26 04:08:23.000000 prettyformatter-2.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-25 02:11:07.027468 prettyformatter-2.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-01-25 02:11:07.319350 prettyformatter-2.0.8/src/prettyformatter/
--rw-rw-rw-   0        0        0     7049 2023-01-25 02:08:08.000000 prettyformatter-2.0.8/src/prettyformatter/__init__.py
--rw-rw-rw-   0        0        0     5596 2022-10-26 14:49:09.000000 prettyformatter-2.0.8/src/prettyformatter/_pretty_class.py
--rw-rw-rw-   0        0        0     2249 2022-10-26 14:49:49.000000 prettyformatter-2.0.8/src/prettyformatter/_pretty_dataclass.py
--rw-rw-rw-   0        0        0    40864 2023-01-25 02:07:38.000000 prettyformatter-2.0.8/src/prettyformatter/_prettyformatter.py
-drwxrwxrwx   0        0        0        0 2023-01-25 02:11:07.466560 prettyformatter-2.0.8/src/prettyformatter.egg-info/
--rw-rw-rw-   0        0        0     5049 2023-01-25 02:11:06.000000 prettyformatter-2.0.8/src/prettyformatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-01-25 02:11:06.000000 prettyformatter-2.0.8/src/prettyformatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 02:11:06.000000 prettyformatter-2.0.8/src/prettyformatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-01-25 02:11:06.000000 prettyformatter-2.0.8/src/prettyformatter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-01-25 04:03:26.475518 prettyformatter-2.0.9/
+-rw-rw-rw-   0        0        0     1087 2022-09-26 04:08:23.000000 prettyformatter-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5049 2023-01-25 04:03:26.464517 prettyformatter-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4003 2022-09-26 04:08:23.000000 prettyformatter-2.0.9/README.md
+-rw-rw-rw-   0        0        0     1032 2022-09-26 04:08:23.000000 prettyformatter-2.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-01-25 04:03:26.476518 prettyformatter-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      240 2022-09-26 04:08:23.000000 prettyformatter-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-25 04:03:25.917518 prettyformatter-2.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-01-25 04:03:26.291514 prettyformatter-2.0.9/src/prettyformatter/
+-rw-rw-rw-   0        0        0     7049 2023-01-25 03:57:03.000000 prettyformatter-2.0.9/src/prettyformatter/__init__.py
+-rw-rw-rw-   0        0        0     5596 2022-10-26 14:49:09.000000 prettyformatter-2.0.9/src/prettyformatter/_pretty_class.py
+-rw-rw-rw-   0        0        0     2249 2022-10-26 14:49:49.000000 prettyformatter-2.0.9/src/prettyformatter/_pretty_dataclass.py
+-rw-rw-rw-   0        0        0    40887 2023-01-25 03:56:13.000000 prettyformatter-2.0.9/src/prettyformatter/_prettyformatter.py
+drwxrwxrwx   0        0        0        0 2023-01-25 04:03:26.450515 prettyformatter-2.0.9/src/prettyformatter.egg-info/
+-rw-rw-rw-   0        0        0     5049 2023-01-25 04:03:25.000000 prettyformatter-2.0.9/src/prettyformatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2023-01-25 04:03:25.000000 prettyformatter-2.0.9/src/prettyformatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-25 04:03:25.000000 prettyformatter-2.0.9/src/prettyformatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-01-25 04:03:25.000000 prettyformatter-2.0.9/src/prettyformatter.egg-info/top_level.txt
```

### Comparing `prettyformatter-2.0.8/LICENSE` & `prettyformatter-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prettyformatter-2.0.8/PKG-INFO` & `prettyformatter-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyformatter
-Version: 2.0.8
+Version: 2.0.9
 Summary: Pretty formatter enables pretty formatting using hanging indents, dataclasses, ellipses, and simple customizability by registering formatters.
 License: mit
 Project-URL: Bug Tracker, https://github.com/SimpleArt/prettyformatter/issues
 Project-URL: Documentation, https://simpleart.github.io/prettyformatter/
 Project-URL: Homepage, https://simpleart.github.io/prettyformatter/
 Project-URL: Repository, https://github.com/SimpleArt/prettyformatter
 Keywords: pretty,print,format,indent,dataclass
```

### Comparing `prettyformatter-2.0.8/README.md` & `prettyformatter-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `prettyformatter-2.0.8/pyproject.toml` & `prettyformatter-2.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prettyformatter-2.0.8/src/prettyformatter/__init__.py` & `prettyformatter-2.0.9/src/prettyformatter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         >>> pprint(dict.fromkeys("ABC", np.arange(9).reshape(3, 3)), json=True)
         {
             "A" : [[0, 1, 2], [3, 4, 5], [6, 7, 8]],
             "B" : [[0, 1, 2], [3, 4, 5], [6, 7, 8]],
             "C" : [[0, 1, 2], [3, 4, 5], [6, 7, 8]]
         }
 """
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 from ._pretty_class import PrettyClass
 from ._prettyformatter import Specifier, pformat, pprint, register
 
 try:
     from ._pretty_dataclass import PrettyDataclass
 except:
```

### Comparing `prettyformatter-2.0.8/src/prettyformatter/_pretty_class.py` & `prettyformatter-2.0.9/src/prettyformatter/_pretty_class.py`

 * *Files identical despite different names*

### Comparing `prettyformatter-2.0.8/src/prettyformatter/_pretty_dataclass.py` & `prettyformatter-2.0.9/src/prettyformatter/_pretty_dataclass.py`

 * *Files identical despite different names*

### Comparing `prettyformatter-2.0.8/src/prettyformatter/_prettyformatter.py` & `prettyformatter-2.0.9/src/prettyformatter/_prettyformatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1098,59 +1098,56 @@
                 pformat(x, **plus_indent)
                 for x in args
             ])
         if len(args) > 0 < len(kwargs):
             s += ",\n" + " " * depth_plus
         if isinstance(kwargs_specifier, dict):
             content = [
-                name
-                + "="
-                + pformat(value, **dict_specifier(key=name, **no_indent))
+                pformat(value, **dict_specifier(key=name, **no_indent))
                 for name, value in kwargs.items()
             ]
         else:
             content = [
-                name
-                + "="
-                + pformat(value, **no_indent)
-                for name, value in kwargs.items()
+                pformat(value, **no_indent)
+                for value in kwargs.values()
             ]
         newlines = {i for i, c in enumerate(content) if "\n" in c}
         alignment = align(Counter(
             len(name) // indent
             for i, (name, c) in enumerate(zip(kwargs, content))
             if len(name) + len(c) < 90
             if i not in newlines
         ))
         for i, (name, c) in enumerate(zip(kwargs, content)):
             if i in newlines:
                 content[i] = ""
                 continue
             elif len(name) + len(c) >= 90:
+                content[i] = name + "=\n" + " " * depth_plus + c
                 continue
             content[i] = (
                 name
                 + " " * (
                     1 + (~len(name) % indent) + indent * alignment[len(name) // indent]
                 )
                 + ("= " + c)
             )
         if isinstance(kwargs_specifier, dict):
             for i, (name, value) in enumerate(kwargs.items()):
-                if i not in newlines:
+                if i not in newlines or len(name) + len(c) >= 90:
                     continue
                 content[i] = (
                     name
                     + "=\n"
                     + " " * (depth_plus + indent)
                     + pformat(value, **dict_specifier(key=name, **plus_plus_indent))
                 )
         else:
             for i, (name, value) in enumerate(kwargs.items()):
-                if i not in newlines:
+                if i not in newlines or len(name) + len(c) >= 90:
                     continue
                 content[i] = (
                     name
                     + "=\n"
                     + " " * (depth_plus + indent)
                     + pformat(value, **plus_plus_indent)
                 )
```

### Comparing `prettyformatter-2.0.8/src/prettyformatter.egg-info/PKG-INFO` & `prettyformatter-2.0.9/src/prettyformatter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyformatter
-Version: 2.0.8
+Version: 2.0.9
 Summary: Pretty formatter enables pretty formatting using hanging indents, dataclasses, ellipses, and simple customizability by registering formatters.
 License: mit
 Project-URL: Bug Tracker, https://github.com/SimpleArt/prettyformatter/issues
 Project-URL: Documentation, https://simpleart.github.io/prettyformatter/
 Project-URL: Homepage, https://simpleart.github.io/prettyformatter/
 Project-URL: Repository, https://github.com/SimpleArt/prettyformatter
 Keywords: pretty,print,format,indent,dataclass
```

