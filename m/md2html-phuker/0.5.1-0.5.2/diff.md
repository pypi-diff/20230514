# Comparing `tmp/md2html-phuker-0.5.1.tar.gz` & `tmp/md2html-phuker-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2html-phuker-0.5.1.tar", last modified: Wed Apr 26 12:19:31 2023, max compression
+gzip compressed data, was "md2html-phuker-0.5.2.tar", last modified: Sun May 14 09:22:39 2023, max compression
```

## Comparing `md2html-phuker-0.5.1.tar` & `md2html-phuker-0.5.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:19:31.884824 md2html-phuker-0.5.1/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-26 12:19:08.000000 md2html-phuker-0.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-26 12:19:08.000000 md2html-phuker-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      759 2023-04-26 12:19:31.884824 md2html-phuker-0.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-26 12:19:08.000000 md2html-phuker-0.5.1/Readme.PyPI.md
--rw-r--r--   0 root         (0) root         (0)     5895 2023-04-26 12:19:08.000000 md2html-phuker-0.5.1/Readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:19:31.876824 md2html-phuker-0.5.1/md2html/
--rwxr-xr-x   0 root         (0) root         (0)     9586 2023-04-26 12:19:09.000000 md2html-phuker-0.5.1/md2html/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16608 2023-04-26 12:19:09.000000 md2html-phuker-0.5.1/md2html/github-markdown.css
--rw-r--r--   0 root         (0) root         (0)     3144 2023-04-26 12:19:09.000000 md2html-phuker-0.5.1/md2html/main.css
--rw-r--r--   0 root         (0) root         (0)     4394 2023-04-26 12:19:09.000000 md2html-phuker-0.5.1/md2html/pygments.css
--rw-r--r--   0 root         (0) root         (0)     1063 2023-04-26 12:19:09.000000 md2html-phuker-0.5.1/md2html/style-dark.css
--rw-r--r--   0 root         (0) root         (0)      419 2023-04-26 12:19:09.000000 md2html-phuker-0.5.1/md2html/style-sidebar-toc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:19:31.884824 md2html-phuker-0.5.1/md2html_phuker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      759 2023-04-26 12:19:31.000000 md2html-phuker-0.5.1/md2html_phuker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-26 12:19:31.000000 md2html-phuker-0.5.1/md2html_phuker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 12:19:31.000000 md2html-phuker-0.5.1/md2html_phuker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-26 12:19:31.000000 md2html-phuker-0.5.1/md2html_phuker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-26 12:19:31.000000 md2html-phuker-0.5.1/md2html_phuker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 12:19:31.000000 md2html-phuker-0.5.1/md2html_phuker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-26 12:19:31.884824 md2html-phuker-0.5.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1193 2023-04-26 12:19:08.000000 md2html-phuker-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:22:39.517781 md2html-phuker-0.5.2/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      759 2023-05-14 09:22:39.517781 md2html-phuker-0.5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/Readme.PyPI.md
+-rw-r--r--   0 root         (0) root         (0)     5886 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/Readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:22:39.509781 md2html-phuker-0.5.2/md2html/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/md2html/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      112 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/md2html/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    16608 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/md2html/github-markdown.css
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/md2html/main.css
+-rwxr-xr-x   0 root         (0) root         (0)     9598 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/md2html/md2html.py
+-rw-r--r--   0 root         (0) root         (0)     4394 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/md2html/pygments.css
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/md2html/style-dark.css
+-rw-r--r--   0 root         (0) root         (0)      419 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/md2html/style-sidebar-toc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:22:39.517781 md2html-phuker-0.5.2/md2html_phuker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      759 2023-05-14 09:22:39.000000 md2html-phuker-0.5.2/md2html_phuker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      471 2023-05-14 09:22:39.000000 md2html-phuker-0.5.2/md2html_phuker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:22:39.000000 md2html-phuker-0.5.2/md2html_phuker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-14 09:22:39.000000 md2html-phuker-0.5.2/md2html_phuker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-14 09:22:39.000000 md2html-phuker-0.5.2/md2html_phuker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-14 09:22:39.000000 md2html-phuker-0.5.2/md2html_phuker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2023-05-14 09:22:39.521781 md2html-phuker-0.5.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1201 2023-05-14 09:22:20.000000 md2html-phuker-0.5.2/setup.py
```

### Comparing `md2html-phuker-0.5.1/LICENSE` & `md2html-phuker-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.5.1/PKG-INFO` & `md2html-phuker-0.5.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2html-phuker
-Version: 0.5.1
+Version: 0.5.2
 Summary: Yet another markdown to html converter, generate an offline all-in-one single HTML file.
 Home-page: https://github.com/Phuker/md2html
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: GNU General Public License v3.0
 Keywords: markdown html convert
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `md2html-phuker-0.5.1/Readme.md` & `md2html-phuker-0.5.2/Readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 - [CodeHilite](https://python-markdown.github.io/extensions/code_hilite/)
 - [Table of Contents](https://python-markdown.github.io/extensions/toc/)
 - [New Line to Break](https://python-markdown.github.io/extensions/nl2br/)
 - [Admonition](https://python-markdown.github.io/extensions/admonition/)
 - `<a target="_blank"`
 - Part of GitHub Flavored Markdown
 
-For details, see `convert()` function of `md2html/__init__.py`, and the demo below.
+For details, see `convert()` function of `md2html/md2html.py`, and the demo below.
 
 ## Demo
 
 - Default style: [docs/demo-default.html](https://phuker.github.io/md2html/demo-default.html)
 - With addon `--style sidebar-toc`: [docs/demo-sidebar-toc.html](https://phuker.github.io/md2html/demo-sidebar-toc.html)
 - With addon `--style dark`: [docs/demo-dark.html](https://phuker.github.io/md2html/demo-dark.html)
 - With addon `--style sidebar-toc --style dark`: [docs/demo-sidebar-toc-dark.html](https://phuker.github.io/md2html/demo-sidebar-toc-dark.html)
@@ -65,15 +65,15 @@
 
 ### Show help
 
 ```console
 $ md2html --help
 usage: md2html [-h] [-t TITLE] [-f] [-o FILE] [--style PRESET] [--append-css FILE] [--head-insert HTML] [--head-append HTML] [--body-insert HTML] [--body-append HTML] [-V] [-v] [input_file]
 
-md2html version 0.5.0
+md2html 0.5.1
 Yet another markdown to html converter, generate an offline all-in-one single HTML file.
 https://github.com/Phuker/md2html
 
 positional arguments:
   input_file            If omitted or "-", use stdin.
 
 options:
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_hcf3pwjs_/tmps8fbntwg_TarContainer/0/5.md", line 177, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_hcf3pwjs_/tmps8fbntwg_TarContainer/0/5.md", line 177, column 0: CDATA terminal not found*

```diff
@@ -16,34 +16,34 @@
 Flavored Markdown (GFM)](https://github.github.com/gfm/). Default enabled
 Markdown features: - [Extra](https://python-markdown.github.io/extensions/
 extra/) extensions - [CodeHilite](https://python-markdown.github.io/extensions/
 code_hilite/) - [Table of Contents](https://python-markdown.github.io/
 extensions/toc/) - [New Line to Break](https://python-markdown.github.io/
 extensions/nl2br/) - [Admonition](https://python-markdown.github.io/extensions/
 admonition/) - ` - Part of GitHub Flavored Markdown For details, see `convert
-()` function of `md2html/__init__.py`, and the demo below. ## Demo - Default
+()` function of `md2html/md2html.py`, and the demo below. ## Demo - Default
 style: [docs/demo-default.html](https://phuker.github.io/md2html/demo-
 default.html) - With addon `--style sidebar-toc`: [docs/demo-sidebar-toc.html]
 (https://phuker.github.io/md2html/demo-sidebar-toc.html) - With addon `--style
 dark`: [docs/demo-dark.html](https://phuker.github.io/md2html/demo-dark.html) -
 With addon `--style sidebar-toc --style dark`: [docs/demo-sidebar-toc-
 dark.html](https://phuker.github.io/md2html/demo-sidebar-toc-dark.html) All
 above files are generated from [docs/demo.md](./docs/demo.md). You can view its
 content to see supported syntax. ## Requirements - Python >= `3.6`, with `pip`
 installed ## Install ```bash python3 -m pip install -U md2html-phuker ``` There
 are too many similar projects with similar names in PyPI, `md2html`, `md-to-
 html`, `markdown2html`, `markdown-to-html`, `mrkdwn2html` ... I have to add a
 suffix to keep away from this war of naming. ## Usage ### Show help ```console
 $ md2html --help usage: md2html [-h] [-t TITLE] [-f] [-o FILE] [--style PRESET]
 [--append-css FILE] [--head-insert HTML] [--head-append HTML] [--body-insert
-HTML] [--body-append HTML] [-V] [-v] [input_file] md2html version 0.5.0 Yet
-another markdown to html converter, generate an offline all-in-one single HTML
-file. https://github.com/Phuker/md2html positional arguments: input_file If
-omitted or "-", use stdin. options: -h, --help show this help message and exit
--t TITLE, --title TITLE If omitted, generate from input filename -f, --force
+HTML] [--body-append HTML] [-V] [-v] [input_file] md2html 0.5.1 Yet another
+markdown to html converter, generate an offline all-in-one single HTML file.
+https://github.com/Phuker/md2html positional arguments: input_file If omitted
+or "-", use stdin. options: -h, --help show this help message and exit -
+t TITLE, --title TITLE If omitted, generate from input filename -f, --force
 Force overwrite if output file exists -o FILE, --output-file FILE If omitted,
 auto decide. If "-", stdout. --style PRESET Preset style addons, choices:
 sidebar-toc, dark --append-css FILE Append embedded CSS files, may specify
 multiple times. --head-insert HTML HTML to insert to the start of
 , may specify multiple times. --head-append HTML HTML to append to the end of
 , may specify multiple times. --body-insert HTML HTML to insert to the start of
 , may specify multiple times. --body-append HTML HTML to append to the end of
```

### Comparing `md2html-phuker-0.5.1/md2html/__init__.py` & `md2html-phuker-0.5.2/md2html/md2html.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 import markdown.extensions.toc
 import markdown.extensions.nl2br
 import markdown.extensions.admonition
 import markdown_link_attr_modifier
 import gfm
 
 
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 VERSION_STR_SHORT = f'md2html {__version__}'
 VERSION_STR_LONG = f'md2html {__version__}\n{__doc__.strip()}'
 
 logger = logging.getLogger(__name__)
 
 
 def _assert(expr, msg=''):
     if not expr:
         raise AssertionError(msg)
 
 
-def _init_logging():
+def init_logging():
     logging_stream = sys.stderr
     logging_format = '\x1b[1m%(asctime)s [%(levelname)s]:\x1b[0m%(message)s'
     logging_level = logging.INFO
 
     if logging_stream.isatty():
         logging_date_format = '%H:%M:%S'
     else:
@@ -56,21 +56,22 @@
     logging.addLevelName(logging.CRITICAL, '\x1b[31m{}\x1b[39m'.format(logging.getLevelName(logging.CRITICAL)))
     logging.addLevelName(logging.ERROR, '\x1b[31m{}\x1b[39m'.format(logging.getLevelName(logging.ERROR)))
     logging.addLevelName(logging.WARNING, '\x1b[33m{}\x1b[39m'.format(logging.getLevelName(logging.WARNING)))
     logging.addLevelName(logging.INFO, '\x1b[36m{}\x1b[39m'.format(logging.getLevelName(logging.INFO)))
     logging.addLevelName(logging.DEBUG, '\x1b[36m{}\x1b[39m'.format(logging.getLevelName(logging.DEBUG)))
 
 
-def _parse_args(args=sys.argv[1:]):
+def parse_args(args=None):
     choices_style = [
         'sidebar-toc',
         'dark',
     ]
 
     parser = argparse.ArgumentParser(
+        prog='md2html',
         description=VERSION_STR_LONG,
         formatter_class=argparse.RawDescriptionHelpFormatter,
         add_help=True
     )
 
     parser.add_argument('-t', '--title', help='If omitted, generate from input filename')
     parser.add_argument('-f', '--force', action='store_true', help='Force overwrite if output file exists')
@@ -244,16 +245,16 @@
         'body_insert': body_insert,
         'body_append': body_append,
     }
     return template.format(**template_args)
 
 
 def main():
-    _init_logging()
-    shell_args = _parse_args()
+    init_logging()
+    shell_args = parse_args()
 
     if sys.stderr.isatty():
         atexit.register(lambda: logger.info('Exiting'))
     else:
         atexit.register(lambda: logger.info('Exiting\n'))
 
     logger.info(VERSION_STR_SHORT)
```

### Comparing `md2html-phuker-0.5.1/md2html/github-markdown.css` & `md2html-phuker-0.5.2/md2html/github-markdown.css`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.5.1/md2html/main.css` & `md2html-phuker-0.5.2/md2html/main.css`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.5.1/md2html/pygments.css` & `md2html-phuker-0.5.2/md2html/pygments.css`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.5.1/md2html/style-dark.css` & `md2html-phuker-0.5.2/md2html/style-dark.css`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.5.1/md2html_phuker.egg-info/PKG-INFO` & `md2html-phuker-0.5.2/md2html_phuker.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2html-phuker
-Version: 0.5.1
+Version: 0.5.2
 Summary: Yet another markdown to html converter, generate an offline all-in-one single HTML file.
 Home-page: https://github.com/Phuker/md2html
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: GNU General Public License v3.0
 Keywords: markdown html convert
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `md2html-phuker-0.5.1/setup.py` & `md2html-phuker-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     packages=['md2html'],
     py_modules = [],
     package_data={
         'md2html': ['*.css'],
     },
     entry_points={
         'console_scripts': [
-            'md2html=md2html:main'
+            'md2html=md2html.md2html:main'
         ]
     },
     install_requires=[
         'markdown>=3',
         'pygments',
         'markdown-link-attr-modifier >= 0.2.0',
         'py-gfm',
```

