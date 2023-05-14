# Comparing `tmp/beancount-black-0.2.0.tar.gz` & `tmp/beancount_black-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount-black-0.2.0.tar", max compression
+gzip compressed data, was "beancount_black-0.2.1.tar", max compression
```

## Comparing `beancount-black-0.2.0.tar` & `beancount_black-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-03-10 23:02:04.285562 beancount-black-0.2.0/LICENSE
--rw-r--r--   0        0        0     4256 2023-03-10 23:02:04.285562 beancount-black-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-03-10 23:02:04.285562 beancount-black-0.2.0/beancount_black/__init__.py
--rw-r--r--   0        0        0    25185 2023-03-10 23:02:04.285562 beancount-black-0.2.0/beancount_black/formatter.py
--rw-r--r--   0        0        0     3218 2023-03-10 23:02:04.285562 beancount-black-0.2.0/beancount_black/main.py
--rw-r--r--   0        0        0      630 2023-03-10 23:02:04.285562 beancount-black-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5252 2023-03-10 23:02:07.645343 beancount-black-0.2.0/setup.py
--rw-r--r--   0        0        0     4977 2023-03-10 23:02:07.645787 beancount-black-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-14 19:19:59.944196 beancount_black-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4256 2023-05-14 19:19:59.944196 beancount_black-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-14 19:19:59.944196 beancount_black-0.2.1/beancount_black/__init__.py
+-rw-r--r--   0        0        0    25185 2023-05-14 19:19:59.944196 beancount_black-0.2.1/beancount_black/formatter.py
+-rw-r--r--   0        0        0     3218 2023-05-14 19:19:59.944196 beancount_black-0.2.1/beancount_black/main.py
+-rw-r--r--   0        0        0      629 2023-05-14 19:19:59.948196 beancount_black-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5027 1970-01-01 00:00:00.000000 beancount_black-0.2.1/PKG-INFO
```

### Comparing `beancount-black-0.2.0/LICENSE` & `beancount_black-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount-black-0.2.0/README.md` & `beancount_black-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `beancount-black-0.2.0/beancount_black/formatter.py` & `beancount_black-0.2.1/beancount_black/formatter.py`

 * *Files identical despite different names*

### Comparing `beancount-black-0.2.0/beancount_black/main.py` & `beancount_black-0.2.1/beancount_black/main.py`

 * *Files identical despite different names*

### Comparing `beancount-black-0.2.0/pyproject.toml` & `beancount_black-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "beancount-black"
-version = "0.2.0"
+version = "0.2.1"
 description = "Opinioned code formatter, just like Python's black code formatter but for Beancount"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 repository = "https://github.com/LaunchPlatform/beancount-black"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-beancount-parser = ">= 0.1.23, <0.2.0"
+beancount-parser = ">= 0.2.0, <0.3.0"
 click = ">=7.0.0, <9.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 
 [tool.poetry.scripts]
 bean-black = 'beancount_black.main:main'
```

### Comparing `beancount-black-0.2.0/setup.py` & `beancount_black-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,127 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: beancount-black
+Version: 0.2.1
+Summary: Opinioned code formatter, just like Python's black code formatter but for Beancount
+Home-page: https://github.com/LaunchPlatform/beancount-black
+License: MIT
+Author: Fang-Pen Lin
+Author-email: fangpen@launchplatform.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beancount-parser (>=0.2.0,<0.3.0)
+Requires-Dist: click (>=7.0.0,<9.0.0)
+Project-URL: Repository, https://github.com/LaunchPlatform/beancount-black
+Description-Content-Type: text/markdown
 
-packages = \
-['beancount_black']
+# beancount-black [![CircleCI](https://circleci.com/gh/LaunchPlatform/beancount-black/tree/master.svg?style=svg)](https://circleci.com/gh/LaunchPlatform/beancount-black/tree/master)
+Opinionated code formatter, just like Python's [black](https://pypi.org/project/black/) code formatter but for Beancount
 
-package_data = \
-{'': ['*']}
+Try it out online [here](https://app.beanhub.io/tools/beancount-formatter)
 
-install_requires = \
-['beancount-parser>=0.1.23,<0.2.0', 'click>=7.0.0,<9.0.0']
-
-entry_points = \
-{'console_scripts': ['bean-black = beancount_black.main:main']}
-
-setup_kwargs = {
-    'name': 'beancount-black',
-    'version': '0.2.0',
-    'description': "Opinioned code formatter, just like Python's black code formatter but for Beancount",
-    'long_description': '# beancount-black [![CircleCI](https://circleci.com/gh/LaunchPlatform/beancount-black/tree/master.svg?style=svg)](https://circleci.com/gh/LaunchPlatform/beancount-black/tree/master)\nOpinionated code formatter, just like Python\'s [black](https://pypi.org/project/black/) code formatter but for Beancount\n\nTry it out online [here](https://app.beanhub.io/tools/beancount-formatter)\n\n## Features\n\n- **MIT licensed** - based on [beancount-parser](https://github.com/LaunchPlatform/beancount-parser), a [Lark](https://github.com/lark-parser/lark) based LALR(1) Beancount syntax parser\n- **Extremely fast** - 5K+ lines file generated by `bean-example` can be formatted in around 1 second\n- **Section awareness** - entries separated by Emac org symbol mark `*` will be formatted in groups without changing the overall structure\n- **Comment preserving** - comments are preserved and will be formatted as well\n- **Auto column width** - calculate maximum column width and adjust accordingly\n- **Valid beancount file assumed** - please notice that the formatter assumes the given beacnount file is valid, it doesn\'t not perform any kind of validation\n\n# Sponsor\n\nThe original project beancount-black was meant to be an internal tool built by [Launch Platform LLC](https://launchplatform.com) for \n\n<p align="center">\n  <a href="https://beanhub.io"><img src="https://github.com/LaunchPlatform/beancount-black/raw/master/assets/beanhub.svg?raw=true" alt="BeanHub logo" /></a>\n</p>\n\nA modern accounting book service based on the most popular open source version control system [Git](https://git-scm.com/) and text-based double entry accounting book software [Beancount](https://beancount.github.io/docs/index.html).\nWe realized adding new entries with BeanHub automatically over time makes beancount file a mess.\nSo obviously, a strong code formatter is needed.\nWhile SaaS businesses won\'t be required to open source an internal tool like this, we still love that the service is only possible because of the open-source tool we are using.\nWe think it would be greatly beneficial for the community to access a tool like this, so we\'ve decided to open source it under MIT license, hope you find this tool useful 😄\n\n## Install\n\nTo install the formatter, simply run\n\n```bash\npip install beancount-black\n```\n\n## Usage\n\nRun\n\n```bash\nbean-black /path/to/file.bean\n```\n\nThen the file will be formatted.\nSince this tool is still in its early stage, a backup file at `<filepath>.backup` will be created automatically by default just in case.\nThe creation of backup files can be disabled by passing `-n` or `--no-backup` like this\n\n```bash\nbean-black -n /path/to/file.bean\n```\n\nIt\'s highly recommended to use [BeanHub](https://beanhub.io), Git or other version control system to track your Beancount book files before running the formatter against them without a backup.\n\nIf you want to run the formatter programmatically, you can do this\n\n```python\nimport io\n\nfrom beancount_parser.parser import make_parser\nfrom beancount_black.formatter import Formatter\n\nparser = make_parser()\nformatter = Formatter()\n\ntree = parser.parse(beancount_content)\noutput_file = io.StringIO()\nformatter.format(tree, output_file)\n```\n\n## Stdin mode\n\nYou can run the formatter in STDIN mode by passing `-s` or `--stdin-mode` argument like this:\n\n```bash\nbean-black -s\n```\n\n## Debug\n\nSometimes you might encounter problems when formatting some beancount files.\nTo debug and better understand which line is causing the problem, you can change the log level by passing `-l` argument with `debug` or `verbose`.\nFor example:\n\n```bash\nbean-black -n /path/to/file.bean -l verbose\n```\n\nWith `verbose`, details of the parsed object will be printed.\nWith `debug`, only the line number and type of entry will be printed.\nYou can also use `LOG_LEVEL` environment variable as well.\nThe available log level options are:\n\n- verbose\n- debug\n- info (default)\n- error\n- warning\n- fatal\n\n## Future features\n\n- Add argument for renaming account and commodity\n- Add argument for following other files from `include` statements and also format those files\n \nFeedbacks, bugs reporting or feature requests are welcome 🙌, just please open an issue.\nNo guarantee we have time to deal with them, but will see what we can do.\n',
-    'author': 'Fang-Pen Lin',
-    'author_email': 'fangpen@launchplatform.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/LaunchPlatform/beancount-black',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+## Features
 
+- **MIT licensed** - based on [beancount-parser](https://github.com/LaunchPlatform/beancount-parser), a [Lark](https://github.com/lark-parser/lark) based LALR(1) Beancount syntax parser
+- **Extremely fast** - 5K+ lines file generated by `bean-example` can be formatted in around 1 second
+- **Section awareness** - entries separated by Emac org symbol mark `*` will be formatted in groups without changing the overall structure
+- **Comment preserving** - comments are preserved and will be formatted as well
+- **Auto column width** - calculate maximum column width and adjust accordingly
+- **Valid beancount file assumed** - please notice that the formatter assumes the given beacnount file is valid, it doesn't not perform any kind of validation
+
+# Sponsor
+
+The original project beancount-black was meant to be an internal tool built by [Launch Platform LLC](https://launchplatform.com) for 
+
+<p align="center">
+  <a href="https://beanhub.io"><img src="https://github.com/LaunchPlatform/beancount-black/raw/master/assets/beanhub.svg?raw=true" alt="BeanHub logo" /></a>
+</p>
+
+A modern accounting book service based on the most popular open source version control system [Git](https://git-scm.com/) and text-based double entry accounting book software [Beancount](https://beancount.github.io/docs/index.html).
+We realized adding new entries with BeanHub automatically over time makes beancount file a mess.
+So obviously, a strong code formatter is needed.
+While SaaS businesses won't be required to open source an internal tool like this, we still love that the service is only possible because of the open-source tool we are using.
+We think it would be greatly beneficial for the community to access a tool like this, so we've decided to open source it under MIT license, hope you find this tool useful 😄
+
+## Install
+
+To install the formatter, simply run
+
+```bash
+pip install beancount-black
+```
+
+## Usage
+
+Run
+
+```bash
+bean-black /path/to/file.bean
+```
+
+Then the file will be formatted.
+Since this tool is still in its early stage, a backup file at `<filepath>.backup` will be created automatically by default just in case.
+The creation of backup files can be disabled by passing `-n` or `--no-backup` like this
+
+```bash
+bean-black -n /path/to/file.bean
+```
+
+It's highly recommended to use [BeanHub](https://beanhub.io), Git or other version control system to track your Beancount book files before running the formatter against them without a backup.
+
+If you want to run the formatter programmatically, you can do this
+
+```python
+import io
+
+from beancount_parser.parser import make_parser
+from beancount_black.formatter import Formatter
+
+parser = make_parser()
+formatter = Formatter()
+
+tree = parser.parse(beancount_content)
+output_file = io.StringIO()
+formatter.format(tree, output_file)
+```
+
+## Stdin mode
+
+You can run the formatter in STDIN mode by passing `-s` or `--stdin-mode` argument like this:
+
+```bash
+bean-black -s
+```
+
+## Debug
+
+Sometimes you might encounter problems when formatting some beancount files.
+To debug and better understand which line is causing the problem, you can change the log level by passing `-l` argument with `debug` or `verbose`.
+For example:
+
+```bash
+bean-black -n /path/to/file.bean -l verbose
+```
+
+With `verbose`, details of the parsed object will be printed.
+With `debug`, only the line number and type of entry will be printed.
+You can also use `LOG_LEVEL` environment variable as well.
+The available log level options are:
+
+- verbose
+- debug
+- info (default)
+- error
+- warning
+- fatal
+
+## Future features
+
+- Add argument for renaming account and commodity
+- Add argument for following other files from `include` statements and also format those files
+ 
+Feedbacks, bugs reporting or feature requests are welcome 🙌, just please open an issue.
+No guarantee we have time to deal with them, but will see what we can do.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,68 +1,65 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['beancount_black'] package_data = \ {'': ['*']} install_requires = \
-['beancount-parser>=0.1.23,<0.2.0', 'click>=7.0.0,<9.0.0'] entry_points = \
-{'console_scripts': ['bean-black = beancount_black.main:main']} setup_kwargs =
-{ 'name': 'beancount-black', 'version': '0.2.0', 'description': "Opinioned code
-formatter, just like Python's black code formatter but for Beancount",
-'long_description': '# beancount-black [![CircleCI](https://circleci.com/gh/
+Metadata-Version: 2.1 Name: beancount-black Version: 0.2.1 Summary: Opinioned
+code formatter, just like Python's black code formatter but for Beancount Home-
+page: https://github.com/LaunchPlatform/beancount-black License: MIT Author:
+Fang-Pen Lin Author-email: fangpen@launchplatform.com Requires-Python:
+>=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: beancount-parser
+(>=0.2.0,<0.3.0) Requires-Dist: click (>=7.0.0,<9.0.0) Project-URL: Repository,
+https://github.com/LaunchPlatform/beancount-black Description-Content-Type:
+text/markdown # beancount-black [![CircleCI](https://circleci.com/gh/
 LaunchPlatform/beancount-black/tree/master.svg?style=svg)](https://
-circleci.com/gh/LaunchPlatform/beancount-black/tree/master)\nOpinionated code
-formatter, just like Python\'s [black](https://pypi.org/project/black/) code
-formatter but for Beancount\n\nTry it out online [here](https://app.beanhub.io/
-tools/beancount-formatter)\n\n## Features\n\n- **MIT licensed** - based on
+circleci.com/gh/LaunchPlatform/beancount-black/tree/master) Opinionated code
+formatter, just like Python's [black](https://pypi.org/project/black/) code
+formatter but for Beancount Try it out online [here](https://app.beanhub.io/
+tools/beancount-formatter) ## Features - **MIT licensed** - based on
 [beancount-parser](https://github.com/LaunchPlatform/beancount-parser), a
 [Lark](https://github.com/lark-parser/lark) based LALR(1) Beancount syntax
-parser\n- **Extremely fast** - 5K+ lines file generated by `bean-example` can
-be formatted in around 1 second\n- **Section awareness** - entries separated by
+parser - **Extremely fast** - 5K+ lines file generated by `bean-example` can be
+formatted in around 1 second - **Section awareness** - entries separated by
 Emac org symbol mark `*` will be formatted in groups without changing the
-overall structure\n- **Comment preserving** - comments are preserved and will
-be formatted as well\n- **Auto column width** - calculate maximum column width
-and adjust accordingly\n- **Valid beancount file assumed** - please notice that
-the formatter assumes the given beacnount file is valid, it doesn\'t not
-perform any kind of validation\n\n# Sponsor\n\nThe original project beancount-
-black was meant to be an internal tool built by [Launch Platform LLC](https://
-launchplatform.com) for \n\n
-                              \n [BeanHub_logo]\n
-\n\nA modern accounting book service based on the most popular open source
-version control system [Git](https://git-scm.com/) and text-based double entry
+overall structure - **Comment preserving** - comments are preserved and will be
+formatted as well - **Auto column width** - calculate maximum column width and
+adjust accordingly - **Valid beancount file assumed** - please notice that the
+formatter assumes the given beacnount file is valid, it doesn't not perform any
+kind of validation # Sponsor The original project beancount-black was meant to
+be an internal tool built by [Launch Platform LLC](https://launchplatform.com)
+for
+                                [BeanHub_logo]
+A modern accounting book service based on the most popular open source version
+control system [Git](https://git-scm.com/) and text-based double entry
 accounting book software [Beancount](https://beancount.github.io/docs/
-index.html).\nWe realized adding new entries with BeanHub automatically over
-time makes beancount file a mess.\nSo obviously, a strong code formatter is
-needed.\nWhile SaaS businesses won\'t be required to open source an internal
-tool like this, we still love that the service is only possible because of the
-open-source tool we are using.\nWe think it would be greatly beneficial for the
-community to access a tool like this, so we\'ve decided to open source it under
-MIT license, hope you find this tool useful ð\n\n## Install\n\nTo install
-the formatter, simply run\n\n```bash\npip install beancount-black\n```\n\n##
-Usage\n\nRun\n\n```bash\nbean-black /path/to/file.bean\n```\n\nThen the file
-will be formatted.\nSince this tool is still in its early stage, a backup file
-at `.backup` will be created automatically by default just in case.\nThe
-creation of backup files can be disabled by passing `-n` or `--no-backup` like
-this\n\n```bash\nbean-black -n /path/to/file.bean\n```\n\nIt\'s highly
-recommended to use [BeanHub](https://beanhub.io), Git or other version control
-system to track your Beancount book files before running the formatter against
-them without a backup.\n\nIf you want to run the formatter programmatically,
-you can do this\n\n```python\nimport io\n\nfrom beancount_parser.parser import
-make_parser\nfrom beancount_black.formatter import Formatter\n\nparser =
-make_parser()\nformatter = Formatter()\n\ntree = parser.parse
-(beancount_content)\noutput_file = io.StringIO()\nformatter.format(tree,
-output_file)\n```\n\n## Stdin mode\n\nYou can run the formatter in STDIN mode
-by passing `-s` or `--stdin-mode` argument like this:\n\n```bash\nbean-black -
-s\n```\n\n## Debug\n\nSometimes you might encounter problems when formatting
-some beancount files.\nTo debug and better understand which line is causing the
-problem, you can change the log level by passing `-l` argument with `debug` or
-`verbose`.\nFor example:\n\n```bash\nbean-black -n /path/to/file.bean -
-l verbose\n```\n\nWith `verbose`, details of the parsed object will be
-printed.\nWith `debug`, only the line number and type of entry will be
-printed.\nYou can also use `LOG_LEVEL` environment variable as well.\nThe
-available log level options are:\n\n- verbose\n- debug\n- info (default)\n-
-error\n- warning\n- fatal\n\n## Future features\n\n- Add argument for renaming
-account and commodity\n- Add argument for following other files from `include`
-statements and also format those files\n \nFeedbacks, bugs reporting or feature
-requests are welcome ð, just please open an issue.\nNo guarantee we have
-time to deal with them, but will see what we can do.\n', 'author': 'Fang-Pen
-Lin', 'author_email': 'fangpen@launchplatform.com', 'maintainer': None,
-'maintainer_email': None, 'url': 'https://github.com/LaunchPlatform/beancount-
-black', 'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'entry_points': entry_points, 'python_requires':
-'>=3.9,<4.0', } setup(**setup_kwargs)
+index.html). We realized adding new entries with BeanHub automatically over
+time makes beancount file a mess. So obviously, a strong code formatter is
+needed. While SaaS businesses won't be required to open source an internal tool
+like this, we still love that the service is only possible because of the open-
+source tool we are using. We think it would be greatly beneficial for the
+community to access a tool like this, so we've decided to open source it under
+MIT license, hope you find this tool useful ð ## Install To install the
+formatter, simply run ```bash pip install beancount-black ``` ## Usage Run
+```bash bean-black /path/to/file.bean ``` Then the file will be formatted.
+Since this tool is still in its early stage, a backup file at `.backup` will be
+created automatically by default just in case. The creation of backup files can
+be disabled by passing `-n` or `--no-backup` like this ```bash bean-black -n /
+path/to/file.bean ``` It's highly recommended to use [BeanHub](https://
+beanhub.io), Git or other version control system to track your Beancount book
+files before running the formatter against them without a backup. If you want
+to run the formatter programmatically, you can do this ```python import io from
+beancount_parser.parser import make_parser from beancount_black.formatter
+import Formatter parser = make_parser() formatter = Formatter() tree =
+parser.parse(beancount_content) output_file = io.StringIO() formatter.format
+(tree, output_file) ``` ## Stdin mode You can run the formatter in STDIN mode
+by passing `-s` or `--stdin-mode` argument like this: ```bash bean-black -s ```
+## Debug Sometimes you might encounter problems when formatting some beancount
+files. To debug and better understand which line is causing the problem, you
+can change the log level by passing `-l` argument with `debug` or `verbose`.
+For example: ```bash bean-black -n /path/to/file.bean -l verbose ``` With
+`verbose`, details of the parsed object will be printed. With `debug`, only the
+line number and type of entry will be printed. You can also use `LOG_LEVEL`
+environment variable as well. The available log level options are: - verbose -
+debug - info (default) - error - warning - fatal ## Future features - Add
+argument for renaming account and commodity - Add argument for following other
+files from `include` statements and also format those files Feedbacks, bugs
+reporting or feature requests are welcome ð, just please open an issue. No
+guarantee we have time to deal with them, but will see what we can do.
```

