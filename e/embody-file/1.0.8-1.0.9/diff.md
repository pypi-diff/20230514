# Comparing `tmp/embody_file-1.0.8.tar.gz` & `tmp/embody_file-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embody_file-1.0.8.tar", max compression
+gzip compressed data, was "embody_file-1.0.9.tar", max compression
```

## Comparing `embody_file-1.0.8.tar` & `embody_file-1.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2022-12-10 12:24:30.838044 embody_file-1.0.8/LICENSE
--rw-r--r--   0        0        0     4841 2022-12-10 12:24:30.838044 embody_file-1.0.8/README.md
--rw-r--r--   0        0        0     1980 2022-12-10 12:24:44.506008 embody_file-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      208 2022-12-10 12:24:30.838044 embody_file-1.0.8/src/embodyfile/__init__.py
--rw-r--r--   0        0        0      239 2022-12-10 12:24:30.838044 embody_file-1.0.8/src/embodyfile/__main__.py
--rw-r--r--   0        0        0     4632 2022-12-10 12:24:30.838044 embody_file-1.0.8/src/embodyfile/cli.py
--rw-r--r--   0        0        0    17298 2022-12-10 12:24:44.506008 embody_file-1.0.8/src/embodyfile/embodyfile.py
--rw-r--r--   0        0        0        0 2022-12-10 12:24:30.838044 embody_file-1.0.8/src/embodyfile/py.typed
--rw-r--r--   0        0        0     5870 1970-01-01 00:00:00.000000 embody_file-1.0.8/setup.py
--rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 embody_file-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-12-11 11:24:59.870911 embody_file-1.0.9/LICENSE
+-rw-r--r--   0        0        0     4841 2022-12-11 11:24:59.870911 embody_file-1.0.9/README.md
+-rw-r--r--   0        0        0     1982 2022-12-11 11:25:11.323478 embody_file-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      208 2022-12-11 11:24:59.874911 embody_file-1.0.9/src/embodyfile/__init__.py
+-rw-r--r--   0        0        0      239 2022-12-11 11:24:59.874911 embody_file-1.0.9/src/embodyfile/__main__.py
+-rw-r--r--   0        0        0     4632 2022-12-11 11:24:59.874911 embody_file-1.0.9/src/embodyfile/cli.py
+-rw-r--r--   0        0        0    17284 2022-12-11 11:25:11.323478 embody_file-1.0.9/src/embodyfile/embodyfile.py
+-rw-r--r--   0        0        0        0 2022-12-11 11:24:59.874911 embody_file-1.0.9/src/embodyfile/py.typed
+-rw-r--r--   0        0        0     5872 1970-01-01 00:00:00.000000 embody_file-1.0.9/setup.py
+-rw-r--r--   0        0        0     5695 1970-01-01 00:00:00.000000 embody_file-1.0.9/PKG-INFO
```

### Comparing `embody_file-1.0.8/LICENSE` & `embody_file-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `embody_file-1.0.8/README.md` & `embody_file-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `embody_file-1.0.8/pyproject.toml` & `embody_file-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "embody-file"
-version = "1.0.8"
+version = "1.0.9"
 description = "Embody file converter"
 authors = ["Aidee Health <hello@aidee.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/aidee-health/embody-file"
 repository = "https://github.com/aidee-health/embody-file"
 packages = [
@@ -15,15 +15,15 @@
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/aidee-health/embody-file/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-embody-codec = ">1.0.9"
+embody-codec = ">=1.0.15"
 pandas = ">=1.5.1"
 matplotlib = ">=3.6.2"
 tables = ">=3.7.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.2.0"
 Pygments = ">=2.10.0"
```

### Comparing `embody_file-1.0.8/src/embodyfile/cli.py` & `embody_file-1.0.9/src/embodyfile/cli.py`

 * *Files identical despite different names*

### Comparing `embody_file-1.0.8/src/embodyfile/embodyfile.py` & `embody_file-1.0.9/src/embodyfile/embodyfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,15 +426,15 @@
 
     logging.info(f"Converted data to HDF: {fname}")
 
 
 def __analyze_timestamps(data: list[tuple[int, ProtocolMessageOrChildren]]) -> None:
     ts: list[int] = [x[0] for x in data]
     num_duplicates = len(ts) - len(set(ts))
-    diff = [x - y for x, y in zip(ts[1:], ts, strict=False)]
+    diff = [x - y for x, y in zip(ts[1:], ts)]
     num_big_leaps = len([x for x in diff if x > 20])
     num_small_leaps = len([x for x in diff if 4 < x <= 20])
     logging.debug(f"Found {num_big_leaps} big time leaps (>20ms)")
     logging.debug(f"Found {num_small_leaps} small time leaps (5-20ms)")
     logging.debug(f"Found {num_duplicates} duplicates")
```

### Comparing `embody_file-1.0.8/setup.py` & `embody_file-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 packages = \
 ['embodyfile']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['embody-codec>1.0.9', 'matplotlib>=3.6.2', 'pandas>=1.5.1', 'tables>=3.7.0']
+['embody-codec>=1.0.15', 'matplotlib>=3.6.2', 'pandas>=1.5.1', 'tables>=3.7.0']
 
 entry_points = \
 {'console_scripts': ['embody-file = embodyfile.cli:main']}
 
 setup_kwargs = {
     'name': 'embody-file',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': 'Embody file converter',
     'long_description': "# Embody File\n\n[![PyPI](https://img.shields.io/pypi/v/embody-file.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/embody-file.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/embody-file)][python version]\n[![License](https://img.shields.io/pypi/l/embody-file)][license]\n\n[![Tests](https://github.com/aidee-health/embody-file/workflows/Tests/badge.svg)][tests]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/embody-file/\n[status]: https://pypi.org/project/embody-file/\n[python version]: https://pypi.org/project/embody-file\n[tests]: https://github.com/aidee-health/embody-file/actions?workflow=Tests\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nThis is a Python based implementation for parsing binary files from the Aidee EmBody device.\n\n## Features\n\n- Converts binary embody files to HDF, CSV, etc\n- Integrates with [the EmBody Protocol Codec](https://github.com/aidee-health/embody-protocol-codec) project\n- CLI (command line interface)\n- Can be used as package in other projects\n- Type safe code using [mypy](https://mypy.readthedocs.io/) for type checking\n\n## Requirements\n\n- Python 3.8-3.10\n\n## Installation\n\nYou can install _Embody File_ via [pip]:\n\n```console\n$ pip install embody-file\n```\n\n## Usage\n\nTo use the command line, first install this library either globally or using venv:\n\n```console\n$ pip install embody-file\n```\n\nWhen this library has been installed, a new command is available, `embody-file` which can be used according to the examples below:\n\n### Get help\n\nTo get an updated overview of all command line options:\n\n```bash\nembody-file --help\n```\n\n### Print version number\n\n```bash\nembody-file --version\n```\n\n### Convert binary embody file to HDF\n\nTo convert to a [HDF 5 (hierarcical data format)](https://en.wikipedia.org/wiki/Hierarchical_Data_Format) format, run the following:\n\n```bash\nembody-file testfiles/v5_0_0_test_file.log --output-format HDF\n```\n\nThe file will be named the same as the input file, with the `.hdf` extension at the end of the file name.\n\n### Convert binary embody file to CSV\n\nTo convert to CSV format, run the following:\n\n```bash\nembody-file testfiles/v5_0_0_test_file.log --output-format CSV\n```\n\nThe file will be named the same as the input file, with the `.csv` extension at the end of the file name.\n\n### Print statistics for binary embody file\n\nTo print stats without conversion:\n\n```bash\nembody-file testfiles/v5_0_0_test_file.log --print-stats\n```\n\n### Fail on parse errors\n\nThe parser is lenient by default, accepting errors in the input file. If you want to the parsing to fail on any errors, use the `--strict` flag:\n\n```bash\nembody-file testfiles/v5_0_0_test_file.log --strict\n```\n\n### Plot binary file in graph\n\nTo show an ECG/PPG plot graph:\n\n```bash\nembody-file testfiles/v5_0_0_test_file.log --plot\n```\n\n## Troubleshooting\n\n### I get an error in the middle of the file - how do I start finding the root cause?\n\nTo get the best overview, start by running the parser in strict mode and with debug logging, so it stops at the first error:\n\n```bash\nembody-file troublesomefile.log --strict --log-level DEBUG\n```\n\nThis provides positional information per message so it's easier to continue searching for errors.\n\nIf this doesn't give us enough information, look at the protocol documentation and start looking and the problematic areas in the input file.\n\nThere are several command line tools you can use. On MAC and Linux, one good example is to use the `hexdump` tool:\n\n```bash\nhexdump -C -n 70 -s 0 troublesomefile.log\n```\n\nHere, `-n 70` is the amount of bytes to print in hex format, and `-s 0` tells hexdump to start at position 0 in the file. Adjust these parameters according to your needs.\n\nMake a note from the parser's error output of what position the first error started from, and based on that:\n\n- Look at the preceding bytes to see whether there were any errors in the previous protocol message\n- Look at the bytes from the reported (error) position to see if there are just a few bytes before a new, plausible protocol message starts\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n[file an issue]: https://github.com/aidee-health/embody-file/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/aidee-health/embody-file/blob/main/LICENSE\n[contributor guide]: https://github.com/aidee-health/embody-file/blob/main/CONTRIBUTING.md\n[command-line reference]: https://embody-file.readthedocs.io/en/latest/usage.html\n",
     'author': 'Aidee Health',
     'author_email': 'hello@aidee.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/aidee-health/embody-file',
```

### Comparing `embody_file-1.0.8/PKG-INFO` & `embody_file-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: embody-file
-Version: 1.0.8
+Version: 1.0.9
 Summary: Embody file converter
 Home-page: https://github.com/aidee-health/embody-file
 License: MIT
 Author: Aidee Health
 Author-email: hello@aidee.io
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: embody-codec (>1.0.9)
+Requires-Dist: embody-codec (>=1.0.15)
 Requires-Dist: matplotlib (>=3.6.2)
 Requires-Dist: pandas (>=1.5.1)
 Requires-Dist: tables (>=3.7.0)
 Project-URL: Changelog, https://github.com/aidee-health/embody-file/releases
 Project-URL: Repository, https://github.com/aidee-health/embody-file
 Description-Content-Type: text/markdown
```

