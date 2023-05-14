# Comparing `tmp/var_print-0.0.2.tar.gz` & `tmp/var_print-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "var_print-0.0.2.tar", last modified: Sat Jan  7 19:02:54 2023, max compression
+gzip compressed data, was "var_print-0.0.4.tar", last modified: Sun May 14 20:12:49 2023, max compression
```

## Comparing `var_print-0.0.2.tar` & `var_print-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-01-07 19:02:54.376004 var_print-0.0.2/
--rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 var_print-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      159 2023-01-07 18:55:43.000000 var_print-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5750 2023-01-07 19:02:54.375003 var_print-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4986 2023-01-07 18:59:14.000000 var_print-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-01-07 19:02:54.376004 var_print-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1790 2023-01-07 18:55:43.000000 var_print-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-07 19:02:54.365001 var_print-0.0.2/var_print/
--rw-rw-rw-   0        0        0       63 2023-01-07 18:55:43.000000 var_print-0.0.2/var_print/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-07 19:02:54.374004 var_print-0.0.2/var_print/data/
--rw-rw-rw-   0        0        0     6221 2023-01-07 18:45:09.000000 var_print-0.0.2/var_print/data/color_schemes.pickle
--rw-rw-rw-   0        0        0    35727 2023-01-07 18:51:00.000000 var_print-0.0.2/var_print/varPrint.py
-drwxrwxrwx   0        0        0        0 2023-01-07 19:02:54.373003 var_print-0.0.2/var_print.egg-info/
--rw-rw-rw-   0        0        0     5750 2023-01-07 19:02:54.000000 var_print-0.0.2/var_print.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-01-07 19:02:54.000000 var_print-0.0.2/var_print.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-07 19:02:54.000000 var_print-0.0.2/var_print.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-01-07 19:02:54.000000 var_print-0.0.2/var_print.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-07 19:02:54.000000 var_print-0.0.2/var_print.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 20:12:49.165924 var_print-0.0.4/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 var_print-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      159 2023-01-07 18:55:43.000000 var_print-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5750 2023-05-14 20:12:49.165924 var_print-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4986 2023-01-07 18:59:14.000000 var_print-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-14 20:12:49.165924 var_print-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1803 2023-05-14 20:10:20.000000 var_print-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:12:49.155036 var_print-0.0.4/var_print/
+-rw-rw-rw-   0        0        0       63 2023-05-14 20:10:36.000000 var_print-0.0.4/var_print/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:12:49.163893 var_print-0.0.4/var_print/data/
+-rw-rw-rw-   0        0        0     6221 2023-01-07 18:45:09.000000 var_print-0.0.4/var_print/data/color_schemes.pickle
+-rw-rw-rw-   0        0        0    36197 2023-02-14 16:19:16.000000 var_print-0.0.4/var_print/varPrint.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:12:49.162333 var_print-0.0.4/var_print.egg-info/
+-rw-rw-rw-   0        0        0     5750 2023-05-14 20:12:48.000000 var_print-0.0.4/var_print.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-14 20:12:49.000000 var_print-0.0.4/var_print.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 20:12:48.000000 var_print-0.0.4/var_print.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-14 20:12:49.000000 var_print-0.0.4/var_print.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-14 20:12:49.000000 var_print-0.0.4/var_print.egg-info/top_level.txt
```

### Comparing `var_print-0.0.2/LICENSE` & `var_print-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `var_print-0.0.2/PKG-INFO` & `var_print-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: var_print
-Version: 0.0.2
+Version: 0.0.4
 Summary: Nicer printing with var_print: Colours and structure allow quick reading of the output, at the same time the name of the variable is displayed. 
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `var_print-0.0.2/README.md` & `var_print-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `var_print-0.0.2/setup.py` & `var_print-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.2"
+VERSION = "0.0.4"
 DESCRIPTION = "Nicer printing with var_print: Colours and structure allow quick reading of the output, at the same time the name of the variable is displayed. "
 
 # Setting up
 setup(
     name="var_print",
     version=VERSION,
     author="André Herber",
     author_email="andre.herber.programming@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     package_data={"": ["var_printer/data/color_schemes.pickle"]},
     include_package_data=True,
-    install_requires=["executing", "colorful_terminal"],
+    install_requires=["executing", "colorful_terminal", "asttokens"],
     keywords=["python"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `var_print-0.0.2/var_print/data/color_schemes.pickle` & `var_print-0.0.4/var_print/data/color_schemes.pickle`

 * *Files identical despite different names*

### Comparing `var_print-0.0.2/var_print/varPrint.py` & `var_print-0.0.4/var_print/varPrint.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         self,
         colored: bool = True,
         deactivated: bool = False,
         color_preset: VarPrintColors = varpFore.get_preset_by_name("Blue_Green_Yellow"),
         name_value_sep: str = " = ",
         comma: str = ", ",
         prefix: str = "",
-        iter_items_per_line: int = 10,
+        iter_items_per_line: int = 1,
         dict_items_per_line: int = 1,
         dict_alignment: str = "left",
         list_alignment: str = "left",
     ) -> None:
         # Controls
         self._colored = colored
         self.deactivated = deactivated
@@ -291,15 +291,18 @@
 
     def deactivate(self):
         self.deactivated = True
 
     def __call__(self, *vars) -> None:
         if not self.deactivated:
 
-            var_names = self.get_var_names()
+            try:
+                var_names = self.get_var_names()
+            except:
+                var_names = [f"{type(v)}" for v in vars]
 
             kwargs = {k: vars[i] for (i, k) in enumerate(var_names)}
 
             if len(kwargs) > 0:
                 out = self.format_vars_and_args(kwargs)
             else:
                 out = f"Testing varp: {Fore.CYAN} date and time: {Fore.get_rainbow_string(aktuelle_Zeit())}"
@@ -386,30 +389,35 @@
                     s += sep
                 # elif recursion_level == 0: print(n,"\n\n")
                 string += s
             return string
 
         def format_nested_dicts(dicte: dict, indent, recursion_level):
             iipl = self.dict_items_per_line
-            max_kl = max([len(pformat(k)) for k in dicte.keys()])
+            # max_kl = max([len(pformat(k)) for k in dicte.keys()])
+            max_kl = max([len(self.format_value(k, 0)) for k in dicte.keys()])
 
             ide = indent * " "
             kide = indent + max_kl + len("{") + len(": ")
             k_auf = "{"
             if len(self.dict_alignment) == 2:
                 key_alignment, value_alignment = self.dict_alignment
             else:
                 key_alignment = value_alignment = self.dict_alignment
 
             if key_alignment == "left":
-                jks = [pformat(k).ljust(max_kl) for k in dicte.keys()]
+                # jks = [pformat(k).ljust(max_kl) for k in dicte.keys()]
+                jks = [self.format_value(k, 0).ljust(max_kl) for k in dicte.keys()]
             elif key_alignment == "right":
-                jks = [pformat(k).rjust(max_kl) for k in dicte.keys()]
+                # jks = [pformat(k).rjust(max_kl) for k in dicte.keys()]
+                jks = [self.format_value(k, 0).rjust(max_kl) for k in dicte.keys()]
             else:
-                jks = [pformat(k) for k in dicte.keys()]
+                # jks = [pformat(k) for k in dicte.keys()]
+                jks = [self.format_value(k, 0) for k in dicte.keys()]
+
             max_vl = max(
                 [
                     len(self.format_value(v, kide, recursion_level))
                     for v in dicte.values()
                 ]
             )
 
@@ -1005,8 +1013,11 @@
             )
         self._list_alignment = value
 
 
 varp = VariableNameAndValuePrinter()
 
 if __name__ == "__main__":
-    varp.show_formating_of_different_types()
+    # varp.show_formating_of_different_types()
+
+    test = "test"
+    varp(test)
```

### Comparing `var_print-0.0.2/var_print.egg-info/PKG-INFO` & `var_print-0.0.4/var_print.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: var-print
-Version: 0.0.2
+Version: 0.0.4
 Summary: Nicer printing with var_print: Colours and structure allow quick reading of the output, at the same time the name of the variable is displayed. 
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

