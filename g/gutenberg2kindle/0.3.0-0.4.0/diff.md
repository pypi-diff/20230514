# Comparing `tmp/gutenberg2kindle-0.3.0.tar.gz` & `tmp/gutenberg2kindle-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gutenberg2kindle-0.3.0.tar", max compression
+gzip compressed data, was "gutenberg2kindle-0.4.0.tar", max compression
```

## Comparing `gutenberg2kindle-0.3.0.tar` & `gutenberg2kindle-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    34523 2021-12-12 03:13:59.631009 gutenberg2kindle-0.3.0/LICENSE
--rw-r--r--   0        0        0     2611 2022-05-23 19:40:50.824396 gutenberg2kindle-0.3.0/README.md
--rw-r--r--   0        0        0      137 2022-05-23 19:43:33.268056 gutenberg2kindle-0.3.0/gutenberg2kindle/__init__.py
--rw-r--r--   0        0        0     4924 2022-02-06 19:46:42.873275 gutenberg2kindle-0.3.0/gutenberg2kindle/cli.py
--rw-r--r--   0        0        0     3241 2022-05-23 19:40:40.560334 gutenberg2kindle-0.3.0/gutenberg2kindle/config.py
--rw-r--r--   0        0        0     2217 2022-05-23 19:40:46.452249 gutenberg2kindle-0.3.0/gutenberg2kindle/email.py
--rw-r--r--   0        0        0     1850 2022-05-23 19:41:43.531229 gutenberg2kindle-0.3.0/gutenberg2kindle/gutenberg.py
--rw-r--r--   0        0        0     1377 2022-05-23 19:44:54.474006 gutenberg2kindle-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3590 2022-05-23 19:49:04.920642 gutenberg2kindle-0.3.0/setup.py
--rw-r--r--   0        0        0     3987 2022-05-23 19:49:04.920899 gutenberg2kindle-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-01 05:47:57.287656 gutenberg2kindle-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2611 2023-05-01 05:47:57.287842 gutenberg2kindle-0.4.0/README.md
+-rw-r--r--   0        0        0      137 2023-05-14 19:15:45.358842 gutenberg2kindle-0.4.0/gutenberg2kindle/__init__.py
+-rw-r--r--   0        0        0     4924 2023-05-01 05:47:57.288274 gutenberg2kindle-0.4.0/gutenberg2kindle/cli.py
+-rw-r--r--   0        0        0     3241 2023-05-01 05:47:57.288366 gutenberg2kindle-0.4.0/gutenberg2kindle/config.py
+-rw-r--r--   0        0        0     2217 2023-05-01 05:47:57.288436 gutenberg2kindle-0.4.0/gutenberg2kindle/email.py
+-rw-r--r--   0        0        0     1911 2023-05-01 05:47:57.288508 gutenberg2kindle-0.4.0/gutenberg2kindle/gutenberg.py
+-rw-r--r--   0        0        0     1378 2023-05-14 19:15:37.642698 gutenberg2kindle-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4038 1970-01-01 00:00:00.000000 gutenberg2kindle-0.4.0/PKG-INFO
```

### Comparing `gutenberg2kindle-0.3.0/LICENSE` & `gutenberg2kindle-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gutenberg2kindle-0.3.0/README.md` & `gutenberg2kindle-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gutenberg2kindle-0.3.0/gutenberg2kindle/cli.py` & `gutenberg2kindle-0.4.0/gutenberg2kindle/cli.py`

 * *Files identical despite different names*

### Comparing `gutenberg2kindle-0.3.0/gutenberg2kindle/config.py` & `gutenberg2kindle-0.4.0/gutenberg2kindle/config.py`

 * *Files identical despite different names*

### Comparing `gutenberg2kindle-0.3.0/gutenberg2kindle/email.py` & `gutenberg2kindle-0.4.0/gutenberg2kindle/email.py`

 * *Files identical despite different names*

### Comparing `gutenberg2kindle-0.3.0/gutenberg2kindle/gutenberg.py` & `gutenberg2kindle-0.4.0/gutenberg2kindle/gutenberg.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 GUTENBERG_BOOK_WITH_IMAGES_BASE_URL: Final[str] = (
     "https://www.gutenberg.org/ebooks/{book_id}.epub.images"
 )
 GUTENBERG_BOOK_BASE_URL: Final[str] = (
     "https://www.gutenberg.org/ebooks/{book_id}.epub"
 )
 
+REQUESTS_TIMEOUT: Final[int] = 10
+
 
 def download_book(book_id: int) -> Optional[BytesIO]:
     """
     Given a Gutenberg book ID as an integer, and the expected format,
     fetches the content of the book into memory and returns it wrapped
     in a Bytes IO instance.
     """
@@ -55,15 +57,15 @@
 def fetch_book_from_url(book_url: str) -> Optional[BytesIO]:
     """
     Given a Gutenberg book URL, fetches the content
     of the book into memory and returns it wrapped in a BytesIO
     instance
     """
 
-    response = requests.get(book_url)
+    response = requests.get(book_url, timeout=REQUESTS_TIMEOUT)
     if response.status_code != 200:
         return None
     book_content = response.content
 
     memory_bytes = BytesIO()
     memory_bytes.write(book_content)
     memory_bytes.seek(0)
```

### Comparing `gutenberg2kindle-0.3.0/pyproject.toml` & `gutenberg2kindle-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gutenberg2kindle"
-version = "0.3.0"
+version = "0.4.0"
 description = "A small Python tool to download and send ebooks from Project Gutenberg to a Kindle email address via SMTP"
 authors = ["Andrés Ignacio Torres <dev@aitorres.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/aitorres/gutenberg2kindle"
 keywords = [
     "python",
@@ -29,23 +29,23 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/aitorres/gutenberg2kindle/issues"
 "Change Log" = "https://github.com/aitorres/gutenberg2kindle/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 usersettings = "^1.1.5"
-requests = "^2.27.1"
+requests = "^2.30.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
-flake8 = "^4.0.1"
-mypy = "^0.950"
-pylint = "^2.13.9"
-types-requests = "^2.27.27"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+flake8 = "^6.0.0"
+mypy = "^1.3.0"
+pylint = "^2.17.4"
+types-requests = "^2.30.0.0"
 
 [tool.poetry.scripts]
 gutenberg2kindle = "gutenberg2kindle.cli:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gutenberg2kindle-0.3.0/setup.py` & `gutenberg2kindle-0.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,103 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gutenberg2kindle
+Version: 0.4.0
+Summary: A small Python tool to download and send ebooks from Project Gutenberg to a Kindle email address via SMTP
+Home-page: https://github.com/aitorres/gutenberg2kindle
+License: AGPL-3.0-only
+Keywords: python,cli,ebooks,kindle,gutenberg,project gutenberg
+Author: Andrés Ignacio Torres
+Author-email: dev@aitorres.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Communications :: File Sharing
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: usersettings (>=1.1.5,<2.0.0)
+Project-URL: Bug Tracker, https://github.com/aitorres/gutenberg2kindle/issues
+Project-URL: Change Log, https://github.com/aitorres/gutenberg2kindle/blob/main/CHANGELOG.md
+Project-URL: Repository, https://github.com/aitorres/gutenberg2kindle
+Description-Content-Type: text/markdown
 
-packages = \
-['gutenberg2kindle']
+# Gutenberg2Kindle
 
-package_data = \
-{'': ['*']}
+A small Python tool to download and send ebooks from Project Gutenberg to a Kindle email address via SMTP
 
-install_requires = \
-['requests>=2.27.1,<3.0.0', 'usersettings>=1.1.5,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['gutenberg2kindle = gutenberg2kindle.cli:main']}
-
-setup_kwargs = {
-    'name': 'gutenberg2kindle',
-    'version': '0.3.0',
-    'description': 'A small Python tool to download and send ebooks from Project Gutenberg to a Kindle email address via SMTP',
-    'long_description': "# Gutenberg2Kindle\n\nA small Python tool to download and send ebooks from Project Gutenberg to a Kindle email address via SMTP\n\n## What's this?\n\n`gutenberg2kindle` is a small command-line interface tool that aims to automatically download an `.epub` book from [Project Gutenberg](https://www.gutenberg.org/)'s library of free books in the public domain, and then send the ebook's file to a Kindle email address (although, generally, it can be sent to any email address), with just one command.\n\nThe book is sent through a SMTP server with TLS, requiring the user to configure the server settings beforehand via tool commands.\n\n## Installation\n\nYou can use your Python package manager (e.g. [pip](https://pip.pypa.io/en/stable/)) to install `gutenberg2kindle`.\n\n```bash\npip install gutenberg2kindle\n```\n\n## Usage\n\n`gutenberg2kindle` comes with a command-line interface; its help text can be accessed via:\n\n```bash\ngutenberg2kindle --help\n```\n\nYou can check the tool's current configuration via:\n\n```bash\n# will print all config variables with their current values\ngutenberg2kindle get-config\n\n# will print only the value for the key you're specifying\ngutenberg2kindle get-config --name <key name>\n```\n\nYou can set a value for any of the settings via:\n\n```bash\ngutenberg2kindle set-config --name <key name> --value <key value>\n```\n\nOr you can do it all at once interactively, being able to check (and modify, if needed) the current config, just by running:\n\n```bash\ngutenberg2kindle interactive-config\n```\n\nFinally, once you're done configuring your project, you can send any ebook via its Project Gutenberg book ID (with flags `-b` or `--book-id`):\n\n```bash\ngutenberg2kindle send -b <book id as an integer, e.g. 1>\n```\n\nYou can send multiple books at the same time in the same run, the `-b` / `--book-id` flag accepts multiple arguments.\n\n```bash\ngutenberg2kindle send -b <first book id> [<second book id> <third book id>...]\n```\n\nNote that, if using Gmail as your SMTP server, you might need to set up an [App Password](https://support.google.com/accounts/answer/185833) to use instead of your regular password.\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Contributions for issues that are already open by maintainers are welcome and encouraged.\n\nPlease make sure to update tests as appropriate; a minimum coverage of 75% is expected (and enforced by Github Actions!).\n\n## License\n\nThis project is licensed under the [GNU Affero General Public License v3.0](https://github.com/aitorres/gutenberg2kindle/blob/main/LICENSE).\n",
-    'author': 'Andrés Ignacio Torres',
-    'author_email': 'dev@aitorres.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/aitorres/gutenberg2kindle',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+## What's this?
 
+`gutenberg2kindle` is a small command-line interface tool that aims to automatically download an `.epub` book from [Project Gutenberg](https://www.gutenberg.org/)'s library of free books in the public domain, and then send the ebook's file to a Kindle email address (although, generally, it can be sent to any email address), with just one command.
+
+The book is sent through a SMTP server with TLS, requiring the user to configure the server settings beforehand via tool commands.
+
+## Installation
+
+You can use your Python package manager (e.g. [pip](https://pip.pypa.io/en/stable/)) to install `gutenberg2kindle`.
+
+```bash
+pip install gutenberg2kindle
+```
+
+## Usage
+
+`gutenberg2kindle` comes with a command-line interface; its help text can be accessed via:
+
+```bash
+gutenberg2kindle --help
+```
+
+You can check the tool's current configuration via:
+
+```bash
+# will print all config variables with their current values
+gutenberg2kindle get-config
+
+# will print only the value for the key you're specifying
+gutenberg2kindle get-config --name <key name>
+```
+
+You can set a value for any of the settings via:
+
+```bash
+gutenberg2kindle set-config --name <key name> --value <key value>
+```
+
+Or you can do it all at once interactively, being able to check (and modify, if needed) the current config, just by running:
+
+```bash
+gutenberg2kindle interactive-config
+```
+
+Finally, once you're done configuring your project, you can send any ebook via its Project Gutenberg book ID (with flags `-b` or `--book-id`):
+
+```bash
+gutenberg2kindle send -b <book id as an integer, e.g. 1>
+```
+
+You can send multiple books at the same time in the same run, the `-b` / `--book-id` flag accepts multiple arguments.
+
+```bash
+gutenberg2kindle send -b <first book id> [<second book id> <third book id>...]
+```
+
+Note that, if using Gmail as your SMTP server, you might need to set up an [App Password](https://support.google.com/accounts/answer/185833) to use instead of your regular password.
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Contributions for issues that are already open by maintainers are welcome and encouraged.
+
+Please make sure to update tests as appropriate; a minimum coverage of 75% is expected (and enforced by Github Actions!).
+
+## License
+
+This project is licensed under the [GNU Affero General Public License v3.0](https://github.com/aitorres/gutenberg2kindle/blob/main/LICENSE).
 
-setup(**setup_kwargs)
```

