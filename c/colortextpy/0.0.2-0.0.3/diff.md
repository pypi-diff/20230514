# Comparing `tmp/colortextpy-0.0.2.tar.gz` & `tmp/colortextpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colortextpy-0.0.2.tar", last modified: Thu May 11 17:50:40 2023, max compression
+gzip compressed data, was "colortextpy-0.0.3.tar", last modified: Sun May 14 11:28:18 2023, max compression
```

## Comparing `colortextpy-0.0.2.tar` & `colortextpy-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-11 17:50:40.218054 colortextpy-0.0.2/
--rwxrwxrwx   0 ping      (1000) ping      (1000)     1063 2023-05-05 08:00:54.000000 colortextpy-0.0.2/LICENSE
--rwxrwxrwx   0 ping      (1000) ping      (1000)      111 2023-04-27 10:12:58.000000 colortextpy-0.0.2/MANIFEST.in
--rwxrwxrwx   0 ping      (1000) ping      (1000)     1315 2023-05-11 17:50:40.212545 colortextpy-0.0.2/PKG-INFO
--rwxrwxrwx   0 ping      (1000) ping      (1000)      363 2023-05-07 08:43:23.000000 colortextpy-0.0.2/README.md
-drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-11 17:50:40.026671 colortextpy-0.0.2/colortextpy/
--rwxrwxrwx   0 ping      (1000) ping      (1000)      156 2023-05-11 17:45:15.000000 colortextpy-0.0.2/colortextpy/__init__.py
--rwxrwxrwx   0 ping      (1000) ping      (1000)    10817 2023-05-11 17:45:15.000000 colortextpy-0.0.2/colortextpy/_modidx.py
--rwxrwxrwx   0 ping      (1000) ping      (1000)     3310 2023-05-11 17:45:15.000000 colortextpy-0.0.2/colortextpy/ansicolor.py
--rwxrwxrwx   0 ping      (1000) ping      (1000)    12619 2023-05-11 17:45:15.000000 colortextpy-0.0.2/colortextpy/color.py
--rwxrwxrwx   0 ping      (1000) ping      (1000)     8029 2023-05-11 17:45:15.000000 colortextpy-0.0.2/colortextpy/colorize.py
--rwxrwxrwx   0 ping      (1000) ping      (1000)     2474 2023-05-11 17:45:15.000000 colortextpy-0.0.2/colortextpy/printer.py
-drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-11 17:50:40.167996 colortextpy-0.0.2/colortextpy.egg-info/
--rwxrwxrwx   0 ping      (1000) ping      (1000)     1315 2023-05-11 17:50:39.000000 colortextpy-0.0.2/colortextpy.egg-info/PKG-INFO
--rwxrwxrwx   0 ping      (1000) ping      (1000)      437 2023-05-11 17:50:39.000000 colortextpy-0.0.2/colortextpy.egg-info/SOURCES.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)        1 2023-05-11 17:50:39.000000 colortextpy-0.0.2/colortextpy.egg-info/dependency_links.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)       44 2023-05-11 17:50:39.000000 colortextpy-0.0.2/colortextpy.egg-info/entry_points.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)        1 2023-05-06 16:09:06.000000 colortextpy-0.0.2/colortextpy.egg-info/not-zip-safe
--rwxrwxrwx   0 ping      (1000) ping      (1000)       27 2023-05-11 17:50:39.000000 colortextpy-0.0.2/colortextpy.egg-info/requires.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)       12 2023-05-11 17:50:39.000000 colortextpy-0.0.2/colortextpy.egg-info/top_level.txt
--rwxrwxrwx   0 ping      (1000) ping      (1000)      833 2023-05-11 17:44:37.000000 colortextpy-0.0.2/settings.ini
--rwxrwxrwx   0 ping      (1000) ping      (1000)       38 2023-05-11 17:50:40.220555 colortextpy-0.0.2/setup.cfg
--rwxrwxrwx   0 ping      (1000) ping      (1000)     2596 2023-04-27 10:12:58.000000 colortextpy-0.0.2/setup.py
+drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-14 11:28:18.220440 colortextpy-0.0.3/
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     1063 2023-05-05 08:00:54.000000 colortextpy-0.0.3/LICENSE
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      111 2023-04-27 10:12:58.000000 colortextpy-0.0.3/MANIFEST.in
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     1310 2023-05-14 11:28:18.218436 colortextpy-0.0.3/PKG-INFO
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      333 2023-05-14 11:27:03.000000 colortextpy-0.0.3/README.md
+drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-14 11:28:18.094269 colortextpy-0.0.3/colortextpy/
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      152 2023-05-14 11:27:13.000000 colortextpy-0.0.3/colortextpy/__init__.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)    12526 2023-05-14 11:28:01.000000 colortextpy-0.0.3/colortextpy/_modidx.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     6519 2023-05-14 11:27:13.000000 colortextpy-0.0.3/colortextpy/ansicolor.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)    13062 2023-05-14 11:27:13.000000 colortextpy-0.0.3/colortextpy/color.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     7114 2023-05-14 11:27:13.000000 colortextpy-0.0.3/colortextpy/colorizer.py
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     2704 2023-05-14 11:27:13.000000 colortextpy-0.0.3/colortextpy/printer.py
+drwxrwxrwx   0 ping      (1000) ping      (1000)        0 2023-05-14 11:28:18.200328 colortextpy-0.0.3/colortextpy.egg-info/
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     1310 2023-05-14 11:28:17.000000 colortextpy-0.0.3/colortextpy.egg-info/PKG-INFO
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      438 2023-05-14 11:28:17.000000 colortextpy-0.0.3/colortextpy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)        1 2023-05-14 11:28:17.000000 colortextpy-0.0.3/colortextpy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)       44 2023-05-14 11:28:17.000000 colortextpy-0.0.3/colortextpy.egg-info/entry_points.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)        1 2023-05-06 16:09:06.000000 colortextpy-0.0.3/colortextpy.egg-info/not-zip-safe
+-rwxrwxrwx   0 ping      (1000) ping      (1000)       27 2023-05-14 11:28:17.000000 colortextpy-0.0.3/colortextpy.egg-info/requires.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)       12 2023-05-14 11:28:17.000000 colortextpy-0.0.3/colortextpy.egg-info/top_level.txt
+-rwxrwxrwx   0 ping      (1000) ping      (1000)      858 2023-05-14 11:27:53.000000 colortextpy-0.0.3/settings.ini
+-rwxrwxrwx   0 ping      (1000) ping      (1000)       38 2023-05-14 11:28:18.220944 colortextpy-0.0.3/setup.cfg
+-rwxrwxrwx   0 ping      (1000) ping      (1000)     2596 2023-04-27 10:12:58.000000 colortextpy-0.0.3/setup.py
```

### Comparing `colortextpy-0.0.2/LICENSE` & `colortextpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `colortextpy-0.0.2/PKG-INFO` & `colortextpy-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: colortextpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Colortextpy is a Python package for adding colors and styles to terminal output, allowing you to create more visually appealing and organized command-line applications.
 Home-page: https://github.com/susuky/colortextpy
 Author: ping
 Author-email: hpisj322@gmail.com
 License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
+Keywords: console color terminal text formatting notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,25 +21,24 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # colortextpy
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-This file will become your README and also the index of your
-documentation.
-
 ## Install
 
+Tested on python 3.6-3.11, win11, win11 WSL2, Ubuntu, Nvidia Jetson Nano
+
+It doesn’t support win10
+
 ``` sh
 pip install colortextpy
 ```
 
-## How to use
-
-Fill me in please! Don’t forget code examples:
+## Usage
 
 ``` python
 Color.red.name, Color.red.hex, Color.red.rgb
 ```
 
     ('red', '#ff0000', (255, 0, 0))
```

### Comparing `colortextpy-0.0.2/colortextpy/_modidx.py` & `colortextpy-0.0.3/colortextpy/_modidx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/colortextpy',
                 'doc_host': 'https://susuky.github.io',
                 'git_url': 'https://github.com/susuky/colortextpy',
                 'lib_path': 'colortextpy'},
-  'syms': { 'colortextpy.ansicolor': { 'colortextpy.ansicolor._AnsiColor': ('ansicolor.html#_ansicolor', 'colortextpy/ansicolor.py'),
+  'syms': { 'colortextpy.ansicolor': { 'colortextpy.ansicolor.AnsiColor': ('ansicolor.html#ansicolor', 'colortextpy/ansicolor.py'),
+                                       'colortextpy.ansicolor.AnsiColor.__init__': ( 'ansicolor.html#ansicolor.__init__',
+                                                                                     'colortextpy/ansicolor.py'),
+                                       'colortextpy.ansicolor.AnsiColor.set_color': ( 'ansicolor.html#ansicolor.set_color',
+                                                                                      'colortextpy/ansicolor.py'),
+                                       'colortextpy.ansicolor._AnsiColor': ('ansicolor.html#_ansicolor', 'colortextpy/ansicolor.py'),
+                                       'colortextpy.ansicolor._AnsiColor.__call__': ( 'ansicolor.html#_ansicolor.__call__',
+                                                                                      'colortextpy/ansicolor.py'),
                                        'colortextpy.ansicolor._AnsiColor.__contains__': ( 'ansicolor.html#_ansicolor.__contains__',
                                                                                           'colortextpy/ansicolor.py'),
                                        'colortextpy.ansicolor._AnsiColor.__getattr__': ( 'ansicolor.html#_ansicolor.__getattr__',
                                                                                          'colortextpy/ansicolor.py'),
                                        'colortextpy.ansicolor._AnsiColor.__getitem__': ( 'ansicolor.html#_ansicolor.__getitem__',
                                                                                          'colortextpy/ansicolor.py'),
                                        'colortextpy.ansicolor._AnsiColor.__init__': ( 'ansicolor.html#_ansicolor.__init__',
                                                                                       'colortextpy/ansicolor.py'),
                                        'colortextpy.ansicolor._AnsiColor.__repr__': ( 'ansicolor.html#_ansicolor.__repr__',
                                                                                       'colortextpy/ansicolor.py'),
+                                       'colortextpy.ansicolor._AnsiColor.get_8bit_ansi': ( 'ansicolor.html#_ansicolor.get_8bit_ansi',
+                                                                                           'colortextpy/ansicolor.py'),
+                                       'colortextpy.ansicolor._AnsiColor.get_ansi': ( 'ansicolor.html#_ansicolor.get_ansi',
+                                                                                      'colortextpy/ansicolor.py'),
                                        'colortextpy.ansicolor._AnsiColor.get_template': ( 'ansicolor.html#_ansicolor.get_template',
                                                                                           'colortextpy/ansicolor.py'),
+                                       'colortextpy.ansicolor._AnsiColor.hex2ansi': ( 'ansicolor.html#_ansicolor.hex2ansi',
+                                                                                      'colortextpy/ansicolor.py'),
+                                       'colortextpy.ansicolor._AnsiColor.rgb2ansi': ( 'ansicolor.html#_ansicolor.rgb2ansi',
+                                                                                      'colortextpy/ansicolor.py'),
                                        'colortextpy.ansicolor._Style': ('ansicolor.html#_style', 'colortextpy/ansicolor.py'),
                                        'colortextpy.ansicolor._Style.__init__': ( 'ansicolor.html#_style.__init__',
                                                                                   'colortextpy/ansicolor.py'),
                                        'colortextpy.ansicolor._Style.available': ( 'ansicolor.html#_style.available',
                                                                                    'colortextpy/ansicolor.py'),
                                        'colortextpy.ansicolor._Style.n': ('ansicolor.html#_style.n', 'colortextpy/ansicolor.py'),
                                        'colortextpy.ansicolor._Style.widely': ('ansicolor.html#_style.widely', 'colortextpy/ansicolor.py')},
@@ -38,55 +53,54 @@
                                    'colortextpy.color._ClassPropertyDescriptor.__init__': ( 'color.html#_classpropertydescriptor.__init__',
                                                                                             'colortextpy/color.py'),
                                    'colortextpy.color._EnumMeta': ('color.html#_enummeta', 'colortextpy/color.py'),
                                    'colortextpy.color._EnumMeta.__repr__': ('color.html#_enummeta.__repr__', 'colortextpy/color.py'),
                                    'colortextpy.color._EnumMeta.__str__': ('color.html#_enummeta.__str__', 'colortextpy/color.py'),
                                    'colortextpy.color._EnumMeta.available': ('color.html#_enummeta.available', 'colortextpy/color.py'),
                                    'colortextpy.color._EnumMeta.str': ('color.html#_enummeta.str', 'colortextpy/color.py'),
+                                   'colortextpy.color.hex2rgb': ('color.html#hex2rgb', 'colortextpy/color.py'),
                                    'colortextpy.color.rgb2hex': ('color.html#rgb2hex', 'colortextpy/color.py')},
-            'colortextpy.colorize': { 'colortextpy.colorize.AnsiColorizer': ('colorize.html#ansicolorizer', 'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.AnsiColorizer.__call__': ( 'colorize.html#ansicolorizer.__call__',
-                                                                                       'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.AnsiColorizer.__repr__': ( 'colorize.html#ansicolorizer.__repr__',
-                                                                                       'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.AnsiColorizer._set_color': ( 'colorize.html#ansicolorizer._set_color',
-                                                                                         'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.AnsiColorizer.colorize': ( 'colorize.html#ansicolorizer.colorize',
-                                                                                       'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.AnsiColorizer.get_ansi': ( 'colorize.html#ansicolorizer.get_ansi',
-                                                                                       'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.AnsiColorizer.strip': ( 'colorize.html#ansicolorizer.strip',
-                                                                                    'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.ColorizedStream': ('colorize.html#colorizedstream', 'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.ColorizedStream.__enter__': ( 'colorize.html#colorizedstream.__enter__',
-                                                                                          'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.ColorizedStream.__exit__': ( 'colorize.html#colorizedstream.__exit__',
-                                                                                         'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.ColorizedStream.__init__': ( 'colorize.html#colorizedstream.__init__',
-                                                                                         'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.ColorizedStream._set_color': ( 'colorize.html#colorizedstream._set_color',
-                                                                                           'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.ColorizedStream.affect_global_stream': ( 'colorize.html#colorizedstream.affect_global_stream',
-                                                                                                     'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.ColorizedStream.flush': ( 'colorize.html#colorizedstream.flush',
-                                                                                      'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.ColorizedStream.unAffect_global_stream': ( 'colorize.html#colorizedstream.unaffect_global_stream',
-                                                                                                       'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.ColorizedStream.write': ( 'colorize.html#colorizedstream.write',
-                                                                                      'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.SystemStream': ('colorize.html#systemstream', 'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.SystemStream.__init__': ( 'colorize.html#systemstream.__init__',
-                                                                                      'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.SystemStream.__new__': ( 'colorize.html#systemstream.__new__',
-                                                                                     'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.SystemStream.restore': ( 'colorize.html#systemstream.restore',
-                                                                                     'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.SystemStream.stderr': ( 'colorize.html#systemstream.stderr',
-                                                                                    'colortextpy/colorize.py'),
-                                      'colortextpy.colorize.SystemStream.stdout': ( 'colorize.html#systemstream.stdout',
-                                                                                    'colortextpy/colorize.py')},
+            'colortextpy.colorizer': { 'colortextpy.colorizer.AnsiColorizer': ('colorizer.html#ansicolorizer', 'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.AnsiColorizer.__call__': ( 'colorizer.html#ansicolorizer.__call__',
+                                                                                         'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.AnsiColorizer.__repr__': ( 'colorizer.html#ansicolorizer.__repr__',
+                                                                                         'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.AnsiColorizer.colorize': ( 'colorizer.html#ansicolorizer.colorize',
+                                                                                         'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.AnsiColorizer.get_ansi': ( 'colorizer.html#ansicolorizer.get_ansi',
+                                                                                         'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.AnsiColorizer.get_end_ansi': ( 'colorizer.html#ansicolorizer.get_end_ansi',
+                                                                                             'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.AnsiColorizer.strip': ( 'colorizer.html#ansicolorizer.strip',
+                                                                                      'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.ColorStream': ('colorizer.html#colorstream', 'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.ColorStream.__enter__': ( 'colorizer.html#colorstream.__enter__',
+                                                                                        'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.ColorStream.__exit__': ( 'colorizer.html#colorstream.__exit__',
+                                                                                       'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.ColorStream.__init__': ( 'colorizer.html#colorstream.__init__',
+                                                                                       'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.ColorStream.affect_global_stream': ( 'colorizer.html#colorstream.affect_global_stream',
+                                                                                                   'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.ColorStream.flush': ( 'colorizer.html#colorstream.flush',
+                                                                                    'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.ColorStream.unAffect_global_stream': ( 'colorizer.html#colorstream.unaffect_global_stream',
+                                                                                                     'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.ColorStream.write': ( 'colorizer.html#colorstream.write',
+                                                                                    'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.SystemStream': ('colorizer.html#systemstream', 'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.SystemStream.__init__': ( 'colorizer.html#systemstream.__init__',
+                                                                                        'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.SystemStream.__new__': ( 'colorizer.html#systemstream.__new__',
+                                                                                       'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.SystemStream.restore': ( 'colorizer.html#systemstream.restore',
+                                                                                       'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.SystemStream.stderr': ( 'colorizer.html#systemstream.stderr',
+                                                                                      'colortextpy/colorizer.py'),
+                                       'colortextpy.colorizer.SystemStream.stdout': ( 'colorizer.html#systemstream.stdout',
+                                                                                      'colortextpy/colorizer.py')},
             'colortextpy.printer': { 'colortextpy.printer._Printer': ('printer.html#_printer', 'colortextpy/printer.py'),
                                      'colortextpy.printer._Printer.__init__': ('printer.html#_printer.__init__', 'colortextpy/printer.py'),
                                      'colortextpy.printer._Printer.__repr__': ('printer.html#_printer.__repr__', 'colortextpy/printer.py'),
                                      'colortextpy.printer._Printer._create_printer': ( 'printer.html#_printer._create_printer',
                                                                                        'colortextpy/printer.py'),
                                      'colortextpy.printer.colorprint': ('printer.html#colorprint', 'colortextpy/printer.py')}}}
```

### Comparing `colortextpy-0.0.2/colortextpy/color.py` & `colortextpy-0.0.3/colortextpy/color.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_color.ipynb.
 
 # %% auto 0
-__all__ = ['Color', 'rgb2hex']
+__all__ = ['Color', 'rgb2hex', 'hex2rgb']
 
-# %% ../nbs/00_color.ipynb 4
+# %% ../nbs/00_color.ipynb 3
 import enum
 
 class _ClassPropertyDescriptor:
     def __init__(self, fget):
         self.fget = fget
 
     def __get__(self, obj, klass=None):
@@ -202,17 +202,38 @@
     def bgr(self):
         return self._bgr
     
     @property
     def __contains__(cls, other):
         return other in cls.available
 
-# %% ../nbs/00_color.ipynb 11
+# %% ../nbs/00_color.ipynb 10
 # def rgb2hex(*rgb) -> str:
 #     return '#{0:x}{1:x}{2:x}'.format(*rgb)
 
 
 def rgb2hex(r: int, g: int, b: int) -> str:
     '''
     convert rgb color to hex
+    
+    Examples
+    --------
+    >>> rgb = (255, 255, 255)
+    >>> rgb2hex(*rgb)
+    >>> '#ffffff'
+    >>> rgb2hex(43, 159, 225)
+    >>> '#2b9fe1'
     '''
     return f'#{r:x}{g:x}{b:x}'
+
+def hex2rgb(h: str) -> tuple:
+    '''
+    convert hex color to rgb tuple
+    
+    Examples
+    --------
+    >>> hex2rgb('#ffffff')
+    >>> (255, 255, 255)
+    >>> hex2rgb('#1af1eb')
+    >>> (26, 241, 235)
+    '''    
+    return tuple(int(h[2*i+1:2*i+3], base=16) for i in range(3))
```

### Comparing `colortextpy-0.0.2/colortextpy/colorize.py` & `colortextpy-0.0.3/colortextpy/colorizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_colorize.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_colorizer.ipynb.
 
 # %% auto 0
-__all__ = ['system_stream', 'colorizer', 'SystemStream', 'ColorizedStream', 'AnsiColorizer']
+__all__ = ['system_stream', 'colorize', 'SystemStream', 'ColorStream', 'AnsiColorizer']
 
-# %% ../nbs/02_colorize.ipynb 4
+# %% ../nbs/02_colorizer.ipynb 4
 import contextlib
 import io
 import re
 import sys
 
-from .ansicolor import Fore, Back, Style
+from .ansicolor import Fore, Back, Style, AnsiColor
 
 
 class SystemStream:
     _instance = None
 
     def __new__(cls):
         if cls._instance is None:
@@ -34,58 +34,63 @@
     def stdout(self): return self.orig_stdout
     
     @property
     def stderr(self): return self.orig_stderr
             
 system_stream = SystemStream()
 
-class ColorizedStream(contextlib.ContextDecorator):
+
+class ColorStream(contextlib.ContextDecorator):
+    '''
+    Enables context managers to work as decorators 
+    to colorize the `sys.stdout` or `sys.stderr`
+    
+    Some usage:
+    
+    ```python
+        with ColorStream(fore='red'):
+            print('text')        
+
+        @ColorStream(fore=Fore.dark_orange)
+        def foo():
+            print('FOO')
+    ```
+    '''
+    
     _regex_tag = re.compile('stdout|stderr')
     
-    def __init__(self, fore=None, back=None, styles=None, autoreset=True, streams=('stdout', )):
+    def __init__(self, fore=None, back=None, style=None, autoreset=True, streams=('stdout', )):
         '''
-        fore: str
-                See Fore.available
-        back: str
-                See Back.available
-        styles: str, tuple
-                See Style.available
+        Parameters
+        ----------
+        fore : `Fore`, str, int, optional
+            Foreground color. Could be hex, rgb string or tuple, `Fore`, 8-bits color
+
+        back : `Back`, str, rgb, int, optional
+            Background color, Could be hex, rgb string or tuple, `Back`, 8-bits color
+
+        style : `Style`, str, tuple, optional
+            Text style. Seee `Style.available`.
+            
         autoreset: bool
         
         streams: str, tuple
             One of {stdout, stderr}, Could be tuple
         '''
-        self.fore = self._set_color(fore, Fore)
-        self.back = self._set_color(back, Back)
-        self.style = (
-            ''.join(self._set_color(s, Style) for s in styles) 
-            if isinstance(styles, (tuple, list)) else 
-            self._set_color(styles, Style)
-        )
+        self.ansi = AnsiColor(fore, back, style)
+        
         self._global_flag = False
         self.autoreset = autoreset
         self._ori_reset = autoreset
         
-        
         self.streams = streams if isinstance(streams, (list, tuple)) else (streams, )
         
         self.files = [getattr(sys, stream) for stream in streams]
         self.ori_files = []
-        
-             
-    def _set_color(self, color, Color):
-        if color is None: return ''
-        elif '[' in color: return color
-        elif color in Color: return Color[color]
-        elif isinstance(color, tuple):
-            if Color.name == 'fore':
-                return colorstr.get_ansi('fg {0}, {1}, {2}'.format(*color))
-            elif Color.name == 'back':
-                return colorstr.get_ansi('bg {0}, {1}, {2}'.format(*color))
-        else: return colorstr.get_ansi(color)
+
             
     def affect_global_stream(self):
         if not self._global_flag:
             self.__enter__()
             self._ori_reset = self.autoreset
             
         self.autoreset = False
@@ -107,131 +112,135 @@
             for stream, ori_file in zip(self.streams, self.ori_files):
                 setattr(sys, stream, ori_file)
             self.ori_files = []
 
     def write(self, text):
         for file in self.ori_files:
             reset = Style.reset_all if self.autoreset else ''
-            file.write(f'{self.style}{self.fore}{self.back}{text}{reset}')
+            file.write(f'{self.ansi.ansi_fmt}{text}{reset}')
             file.flush()
             
     def flush(self):
         for file in self.ori_files:
             file.flush()           
-            
+      
+    
 class AnsiColorizer:
+    r'''
+    For `text` parameter, you can add color tag. Start with <tag> end with </tag>.
+    
+    Some usage:
+        text = 'something'
+        
+        1. blue text tag: 
+            f'<blue>{text}</fg>'
+            f'<blue>{text}</blue>'
+            
+        2. specify fg:
+            f'<fg red>{text}</fg>
+            
+        3. specify bg:
+            f'<bg purple>{text}</bg>
+            
+        4. style:
+            f'<bold>{text}</bold>'
+            
+        5. support rgb format:
+            f'<255, 255, 255>{text}</fg>'
+            f'<fg 255, 255, 255>{text}</fg>'
+            f'<bg 255, 255, 255>{text}</bg>'
+            
+        6. support hex format:
+            f'<#FFFFFF>{text}</fg>'
+            f'<fg #FFFFFF>{text}</fg>'
+            f'<bg #FFFFFF>{text}</bg>'
+        
+        7. support 8-bits color:
+            f'<50>{text}</fg>'
+            f'<fg 50>{text}</fg>'
+            f'<bg 50>{text}</bg>'
+            
+        8. mix of above is ok:
+            f'<fg red>{text}--<bg green>{text}--</fg>{text}--</bg>{text}'
+            
+    '''
+    
     _regex_tag = re.compile(r"<([/\w\s,#]*)>")
     
-    def __call__(self, text, fore=None, back=None, styles=None, raw=False, strip=False):
+    def __call__(self, text, fore=None, back=None, style=None, raw=False, strip=False):
         '''
+        Parameters
+        ----------
         text: str
-        Some usage:
-            text = 'something'
-            1. blue text tag: f'<blue>{text}</fg>'
-            2. blue text tag: f'<blue>{text}</blue>
-            3. red text tag: f'<fg red>{text}</fg>'
-            4. rgb text tag: f'<224, 224, 224>{text}</fg>'
-            5. rgb text tag: f'<fg 224, 224, 224>{text}</fg>'
-            6. blue background tag: f'<bg blue>{text}</bg>'
-            7. HEX code text tag: f'<fg #FFFFFF>{text}</fg>'
-            8. HEX code background tag: f'<bg #FFFFFF>{text}</bg>'
-            9. style text tag: f'<bold>{text}</bold>'
-            10. mix tags: f'<bold><yellow>{text}<bg #FA45BBB>test567</fg></bg></bold>'
-        
-        
-        fore: str
-                Foreground. See Fore.available
-                Both Fore.red and 'red' are acceptable.
-        back: str
-                Background. See Back.available
-                Both Back.red and 'red' are acceptable.
-        styles: str, tuple
-                See Style.available
-                Both Style.bold and 'bold' are acceptable.
-        '''        
-        if any((fore, back, styles)):
-            return (
-                f'{self._set_color(fore, Fore)}'
-                f'{self._set_color(back, Back)}'
-                f'{"".join(self._set_color(s, Style) for s in styles) if isinstance(styles, (list, tuple)) else self._set_color(styles, Style)}'
-                f'{text}'
-                f'{Style.reset_all}'
-            )
+        
+        fore : `Fore`, str, int, optional
+            Foreground color. Could be hex, rgb string or tuple, `Fore`, 8-bits color
+
+        back : `Back`, str, rgb, int, optional
+            Background color, Could be hex, rgb string or tuple, `Back`, 8-bits color
+
+        style : `Style`, str, tuple, optional
+            Text style. Seee `Style.available`.
+            
+        raw : bool
+            return raw text
+            
+        strip : bool
+            remove <tag>
+        '''  
         if raw:     return text
         elif strip: return self.strip(text)
-        else:       return self.colorize(text)
-    
-    def _set_color(self, color, Color):
-        if color is None:
-            return ''
-        else:
-            return color if '\033[' in color else Color[color]
-        
+        elif any((fore, back, style)):
+            ansi = AnsiColor(fore, back, style)
+            return f'{ansi.ansi_fmt}{text}{Style.end}'
+        else: return self.colorize(text)
+
     def get_ansi(self, tag):
         tag = tag.lower()
 
-        # Substitute on a direct match.
         if tag in Style:
             return Style[tag]
-        elif tag in Fore:
-            return Fore[tag]
 
-        # An alternative syntax for setting the color (e.g. <fg red>, <bg red>).
+        if tag.startswith('fg ') or tag.startswith('bg '):
+            st, color = tag[:2], tag[3:]
+            if st == 'fg': return Fore[color]
+            elif st == 'bg': return Back[color]
         else:
-            if tag.startswith('fg ') or tag.startswith('bg '):
-                st, color = tag[:2], tag[3:]
-            else:
-                st, color = '', tag
-
-            code = '48' if st == 'bg' else '38'
-
-            if st == 'fg' and color in Fore:
-                return Fore[color]
-
-            elif st == 'bg' and color in Back:
-                return Back[color]
-            
-            # 8-bits
-            elif color.isdigit() and int(color) <= 255:
-                return '\033[%s;5;%sm' % (code, color)
-            
-            # HEX 24-bits
-            elif re.match(r'#(?:[a-fA-F0-9]{3}){1,2}$', color):
-                hex_color = color[1:]
-                if len(hex_color) == 3: hex_color *= 2
-                rgb = tuple(int(hex_color[i: i + 2], 16) for i in (0, 2, 4))
-                return '\033[%s;2;%s;%s;%sm' % ((code,) + rgb)
-            
-            # 24-bits
-            elif color.count(',') == 2:
-                colors = tuple(color.split(', '))
-                if all(x.isdigit() and int(x) <= 255 for x in colors):
-                    return '\033[%s;2;%s;%s;%sm' % ((code,) + colors)
+            text = Fore[tag]
+            if text: return text
         return ''
 
+    def get_end_ansi(self, tag):
+        if tag.startswith('/fg'): return Fore.reset
+        if tag.startswith('/bg'): return Back.reset
+        
+        tag = tag[1:]
+        if tag in Style:
+            return Style[f'no_{tag}']
+        elif tag in Fore:
+            return Fore.reset
+        else:
+            Style.end    
+    
     def colorize(self, text):
         position = 0
         tokens = []
         for i, match in enumerate(self._regex_tag.finditer(text)):
             markup, tag = match.group(0), match.group(1)
             tokens.append(text[position: match.start()])
             if tag[0] == '/':
-                token = (
-                    Fore.reset if tag.startswith('/fg') else
-                    Back.reset if tag.startswith('/bg') else
-                    Style.reset_all
-                )
+                token = self.get_end_ansi(tag)
             else:
                 token = self.get_ansi(tag)
             tokens.append(token)
             position = match.end()
 
         tokens.append(text[position:])
         return ''.join(tokens)
-    
+        
     def strip(self, text):
         return self._regex_tag.sub('', text)
     
     def __repr__(self):
         return 'AnsiColorizer'
     
-colorizer = AnsiColorizer()
+colorize = AnsiColorizer()
```

### Comparing `colortextpy-0.0.2/colortextpy/printer.py` & `colortextpy-0.0.3/colortextpy/printer.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 # %% auto 0
 __all__ = ['Printer', 'colorprint']
 
 # %% ../nbs/03_printer.ipynb 4
 import sys
 
-from . import colorizer, Fore
+from . import colorize, Fore
 
 
-def colorprint(*value, color='black', bold=False, sep=' ', end='\n', file=sys.stdout, flush=False):
+def colorprint(*value, color=None, background=None, bold=False, sep=' ', end='\n', file=sys.stdout, flush=False):
     '''
     Prints the values to a stream, or to sys.stdout by default with `Fore.color` color.
 
     Parameters
     ----------
     color : str, Fore,
-        For example: 'red', Fore.red
+        Text color. Acceptable format: 'red', Fore.red, '#ff0000', (255, 0, 0)
+    
+    background : str, Fore,
+        background color. Acceptable format: 'red', Back.red, '#ff0000', (255, 0, 0)    
     
     bold : bool
         Whether to use bold font
 
     file : 
         A file-like object (stream); defaults to the current sys.stdout.
 
@@ -31,17 +34,21 @@
         String appended after the last value, default a newline.
 
     flush : bool 
         Whether to forcibly flush the stream.
     '''
     
     text = sep.join(f'{f}' for f in value)
-    print(colorizer(text, fore=color, styles='bold' if bold else ''), sep=sep, end=end, file=file, flush=flush)
-    
-    
+    print(
+        colorize(text, fore=color, back=background, style='bold' if bold else ''), 
+        sep=sep, 
+        end=end, 
+        file=file, 
+        flush=flush
+    )
 
 class _Printer:
     def __init__(self):
         available = []
         for color in Fore.available:
             available.append(f'{color}_print')
             self._create_printer(color)
@@ -71,15 +78,15 @@
 
             flush: bool 
                 whether to forcibly flush the stream.
 
         '''        
         func_body = (
         "    text = sep.join(f'{f}' for f in value)\n"
-        f"    print(colorizer(text, fore='{color}', styles='bold' if bold else ''), sep=sep, end=end, file=file, flush=flush)"
+        f"    print(colorize(text, fore='{color}', style='bold' if bold else ''), sep=sep, end=end, file=file, flush=flush)"
         )
         exec('def {0}({1}):\n    """{2}"""\n{3}'.format(name, args, document, func_body))
         setattr(self, name, locals()[name])
         
     def __repr__(self):
         return 'Printer'
```

### Comparing `colortextpy-0.0.2/colortextpy.egg-info/PKG-INFO` & `colortextpy-0.0.3/colortextpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: colortextpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Colortextpy is a Python package for adding colors and styles to terminal output, allowing you to create more visually appealing and organized command-line applications.
 Home-page: https://github.com/susuky/colortextpy
 Author: ping
 Author-email: hpisj322@gmail.com
 License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
+Keywords: console color terminal text formatting notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,25 +21,24 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # colortextpy
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-This file will become your README and also the index of your
-documentation.
-
 ## Install
 
+Tested on python 3.6-3.11, win11, win11 WSL2, Ubuntu, Nvidia Jetson Nano
+
+It doesn’t support win10
+
 ``` sh
 pip install colortextpy
 ```
 
-## How to use
-
-Fill me in please! Don’t forget code examples:
+## Usage
 
 ``` python
 Color.red.name, Color.red.hex, Color.red.rgb
 ```
 
     ('red', '#ff0000', (255, 0, 0))
```

### Comparing `colortextpy-0.0.2/settings.ini` & `colortextpy-0.0.3/settings.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = colortextpy
 lib_name = colortextpy
-version = 0.0.2
+version = 0.0.3
 min_python = 3.6
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = colortextpy
 nbs_path = nbs
 recursive = True
@@ -18,14 +18,14 @@
 git_url = https://github.com/susuky/colortextpy
 title = colortextpy
 audience = Developers
 author = ping
 author_email = hpisj322@gmail.com
 copyright = 2023 onwards, ping
 description = Colortextpy is a Python package for adding colors and styles to terminal output, allowing you to create more visually appealing and organized command-line applications.
-keywords = nbdev jupyter notebook python
+keywords = console color terminal text formatting notebook python
 language = English
 status = 3
 user = susuky
 requirements = fastcore matplotlib
 host = github
```

### Comparing `colortextpy-0.0.2/setup.py` & `colortextpy-0.0.3/setup.py`

 * *Files identical despite different names*

