# Comparing `tmp/cliconfig-0.5.6.tar.gz` & `tmp/cliconfig-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.5.6.tar", last modified: Sat May 13 17:09:52 2023, max compression
+gzip compressed data, was "cliconfig-0.6.0.tar", last modified: Sun May 14 17:38:18 2023, max compression
```

## Comparing `cliconfig-0.5.6.tar` & `cliconfig-0.6.0.tar`

### file list

```diff
@@ -1,107 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.914167 cliconfig-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-13 17:09:36.000000 cliconfig-0.5.6/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-13 17:09:36.000000 cliconfig-0.5.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.902167 cliconfig-0.5.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.906167 cliconfig-0.5.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-13 17:09:36.000000 cliconfig-0.5.6/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-13 17:09:36.000000 cliconfig-0.5.6/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-13 17:09:36.000000 cliconfig-0.5.6/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-13 17:09:36.000000 cliconfig-0.5.6/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-13 17:09:36.000000 cliconfig-0.5.6/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-13 17:09:36.000000 cliconfig-0.5.6/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-13 17:09:36.000000 cliconfig-0.5.6/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-13 17:09:36.000000 cliconfig-0.5.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-13 17:09:36.000000 cliconfig-0.5.6/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-13 17:09:36.000000 cliconfig-0.5.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-13 17:09:36.000000 cliconfig-0.5.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-13 17:09:36.000000 cliconfig-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-13 17:09:52.914167 cliconfig-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-05-13 17:09:36.000000 cliconfig-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-13 17:09:36.000000 cliconfig-0.5.6/README_pypi.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.906167 cliconfig-0.5.6/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-13 17:09:36.000000 cliconfig-0.5.6/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-13 17:09:52.000000 cliconfig-0.5.6/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-13 17:09:36.000000 cliconfig-0.5.6/cliconfig/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-13 17:09:36.000000 cliconfig-0.5.6/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-13 17:09:36.000000 cliconfig-0.5.6/cliconfig/config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-05-13 17:09:36.000000 cliconfig-0.5.6/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-13 17:09:36.000000 cliconfig-0.5.6/cliconfig/process_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.906167 cliconfig-0.5.6/cliconfig/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-13 17:09:36.000000 cliconfig-0.5.6/cliconfig/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-13 17:09:36.000000 cliconfig-0.5.6/cliconfig/processing/_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-13 17:09:36.000000 cliconfig-0.5.6/cliconfig/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22217 2023-05-13 17:09:36.000000 cliconfig-0.5.6/cliconfig/processing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-13 17:09:36.000000 cliconfig-0.5.6/cliconfig/processing/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-13 17:09:36.000000 cliconfig-0.5.6/cliconfig/tag_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.906167 cliconfig-0.5.6/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-13 17:09:52.000000 cliconfig-0.5.6/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-13 17:09:52.000000 cliconfig-0.5.6/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 17:09:52.000000 cliconfig-0.5.6/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-13 17:09:52.000000 cliconfig-0.5.6/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-13 17:09:52.000000 cliconfig-0.5.6/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.910167 cliconfig-0.5.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.910167 cliconfig-0.5.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/_static/logo_extend.png
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/cliconfig.processing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-13 17:09:36.000000 cliconfig-0.5.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.910167 cliconfig-0.5.6/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-13 17:09:36.000000 cliconfig-0.5.6/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-13 17:09:36.000000 cliconfig-0.5.6/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-13 17:09:36.000000 cliconfig-0.5.6/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-13 17:09:36.000000 cliconfig-0.5.6/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-13 17:09:36.000000 cliconfig-0.5.6/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.910167 cliconfig-0.5.6/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-13 17:09:36.000000 cliconfig-0.5.6/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-13 17:09:36.000000 cliconfig-0.5.6/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-13 17:09:36.000000 cliconfig-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-13 17:09:36.000000 cliconfig-0.5.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-13 17:09:36.000000 cliconfig-0.5.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 17:09:52.914167 cliconfig-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-13 17:09:36.000000 cliconfig-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.910167 cliconfig-0.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.910167 cliconfig-0.5.6/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.910167 cliconfig-0.5.6/tests/configs/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/integration/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/integration/sub1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/integration/sub2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.910167 cliconfig-0.5.6/tests/configs/merge/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/merge/additional1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/merge/additional2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/merge/additional3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/merge/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/merge/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/configs/merge/default3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.910167 cliconfig-0.5.6/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/integration/test_inte_multiple_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.910167 cliconfig-0.5.6/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:09:52.914167 cliconfig-0.5.6/tests/unit/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/unit/processing/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/unit/processing/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/unit/processing/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/unit/processing/test_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/unit/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/unit/test_config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/unit/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/unit/test_ex_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/unit/test_process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-13 17:09:36.000000 cliconfig-0.5.6/tests/unit/test_tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.783929 cliconfig-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.787929 cliconfig-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-14 17:38:03.000000 cliconfig-0.6.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-14 17:38:03.000000 cliconfig-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 17:38:03.000000 cliconfig-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-14 17:38:18.799929 cliconfig-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-05-14 17:38:03.000000 cliconfig-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-14 17:38:03.000000 cliconfig-0.6.0/README_pypi.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.791929 cliconfig-0.6.0/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-14 17:38:18.000000 cliconfig-0.6.0/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.791929 cliconfig-0.6.0/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22776 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-14 17:38:03.000000 cliconfig-0.6.0/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.791929 cliconfig-0.6.0/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-14 17:38:18.000000 cliconfig-0.6.0/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-14 17:38:18.000000 cliconfig-0.6.0/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:38:18.000000 cliconfig-0.6.0/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 17:38:18.000000 cliconfig-0.6.0/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 17:38:18.000000 cliconfig-0.6.0/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/_static/logo_extend.png
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/cliconfig.processing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-14 17:38:03.000000 cliconfig-0.6.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 17:38:03.000000 cliconfig-0.6.0/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-14 17:38:03.000000 cliconfig-0.6.0/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-14 17:38:03.000000 cliconfig-0.6.0/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-14 17:38:03.000000 cliconfig-0.6.0/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-14 17:38:03.000000 cliconfig-0.6.0/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-14 17:38:03.000000 cliconfig-0.6.0/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-14 17:38:03.000000 cliconfig-0.6.0/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-14 17:38:03.000000 cliconfig-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-14 17:38:03.000000 cliconfig-0.6.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 17:38:03.000000 cliconfig-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:38:18.799929 cliconfig-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 17:38:03.000000 cliconfig-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.787929 cliconfig-0.6.0/tests/configs/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.795930 cliconfig-0.6.0/tests/configs/integration/test1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test1/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test1/sub1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test1/sub2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/tests/configs/integration/test2/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/exp1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/exp2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/tests/configs/integration/test2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/models/resnet100.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/models/resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/integration/test2/models/vit_b16.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/integration/test_inte_multiple_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:38:18.799929 cliconfig-0.6.0/tests/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/processing/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/test_config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/test_ex_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-14 17:38:03.000000 cliconfig-0.6.0/tests/unit/test_tag_routines.py
```

### Comparing `cliconfig-0.5.6/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.6.0/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/.github/workflows/pydocstyle.yaml` & `cliconfig-0.6.0/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/.github/workflows/pylint.yaml` & `cliconfig-0.6.0/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/.github/workflows/tests.yaml` & `cliconfig-0.6.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/.pylintrc` & `cliconfig-0.6.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/CONTRIBUTING.md` & `cliconfig-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/LICENSE` & `cliconfig-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/PKG-INFO` & `cliconfig-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.5.6
+Version: 0.6.0
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -135,33 +135,14 @@
 pip install -e .
 pip install -r requirements-dev.txt
 ```
 
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
-## Todo
-
-Priority:
-
-* [x] allow passing new arguments by CLI (with warning and no actual merge)
-* [ ] add a routine to check if a tag is in a key and robust to all other
-  possible tags
-* [ ] add an integration test with all built-in processing (and more)
-
-Secondary:
-
-* [ ] add `make_processing_keep_property` to make a processing that keep the
-  property of a parameter across merged configs. The property is any python object
-  returned by a function that takes the parameter as input
-* [ ] add `ProcessSelect` (with tag "@select") to select a subconfig (or parameter)
-  and delete the others configs at the same level (to cure the resulting config)
-* [ ] allow nested types in `ProcessTyping`
-* [x] add DefaultProcessings that stores default processing as list of processing
-
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
 it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `cliconfig-0.5.6/README.md` & `cliconfig-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 
 ```python
 # main.py
 from cliconfig import make_config, show_config
 
 config = make_config('default1.yaml', 'default2.yaml')
 show_config(config)  # print the config to check it
+config.dict  # the configuration as a dict
 ```
 
 Then you can add one or multiple additional config files that will be passed on
 command line and that will override the default values.
 
 ```yaml
 ---  # first.yaml
@@ -244,28 +245,18 @@
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ## Todo
 
 Priority:
 
-* [x] allow passing new arguments by CLI (with warning and no actual merge)
-* [x] add a routine to check if a tag is in a key and robust to all other
-  possible tags
-* [ ] add an integration test with all built-in processing (and more)
-
 Secondary:
 
-* [x] add `make_processing_keep_property` to make a processing that keep the
-  property of a parameter across merged configs. The property is any python object
-  returned by a function that takes the parameter as input
-* [x] add `ProcessSelect` (with tag "@select") to select a subconfig (or parameter)
-  and delete the others configs at the same level (to cure the resulting config)
-* [x] allow nested types in `ProcessTyping`
-* [x] add DefaultProcessings that stores default processing as list of processing
+* [ ] Add a `@delete` tag to delete a key from the config after pre-merge. Useful to make
+  processing action without introducing new keys in the config.
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
```

### Comparing `cliconfig-0.5.6/README_pypi.md` & `cliconfig-0.6.0/cliconfig.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: cliconfig
+Version: 0.6.0
+Summary: Merge your config files and set parameters from the command line in a simple way.
+Author-email: Valentin Goldite <valentin.goldite@gmail.com>
+Project-URL: Source, https://github.com/valentingol/cliconfig
+Keywords: logging,machine,learning
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CLI Config
 
 </p>
 <p align="center">
   <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
 </p>
 
@@ -123,33 +135,14 @@
 pip install -e .
 pip install -r requirements-dev.txt
 ```
 
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
-## Todo
-
-Priority:
-
-* [x] allow passing new arguments by CLI (with warning and no actual merge)
-* [ ] add a routine to check if a tag is in a key and robust to all other
-  possible tags
-* [ ] add an integration test with all built-in processing (and more)
-
-Secondary:
-
-* [ ] add `make_processing_keep_property` to make a processing that keep the
-  property of a parameter across merged configs. The property is any python object
-  returned by a function that takes the parameter as input
-* [ ] add `ProcessSelect` (with tag "@select") to select a subconfig (or parameter)
-  and delete the others configs at the same level (to cure the resulting config)
-* [ ] allow nested types in `ProcessTyping`
-* [x] add DefaultProcessings that stores default processing as list of processing
-
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
 it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `cliconfig-0.5.6/cliconfig/__init__.py` & `cliconfig-0.6.0/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/cliconfig/cli_parser.py` & `cliconfig-0.6.0/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/cliconfig/config_routines.py` & `cliconfig-0.6.0/cliconfig/config_routines.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,16 +63,15 @@
     .. code-block:: text
 
         python main.py -- config bestmodel.yaml,mydata.yaml \
             --architecture.layers.hidden_dim=64
 
     """
     # Create the processing list
-    if process_list is None:
-        process_list_: List[Processing] = []
+    process_list_: List[Processing] = [] if process_list is None else process_list
     if add_default_processing:
         process_list_ += DefaultProcessings().list
 
     config = Config({}, process_list_)
 
     # Merge default configs and additional configs
     additional_config_paths, cli_params_dict = parse_cli(sys.argv)
@@ -152,16 +151,15 @@
     -------
     config: Dict[str, Any]
         The loaded config. Contains the config dict (config.dict) and the processing
         list (config.process_list), which can be used to apply further processing
         routines.
     """
     # Crate process_list
-    if process_list is None:
-        process_list_ = []
+    process_list_: List[Processing] = [] if process_list is None else process_list
     if add_default_processing:
         process_list_ += DefaultProcessings().list
 
     config = Config({}, process_list_)
     if default_config_paths:
         for config_path in default_config_paths:
             config = merge_flat_paths_processing(
@@ -197,20 +195,19 @@
         The config to save.
     path : str
         The path to the yaml file to save the dict.
     """
     save_processing(config, path)
 
 
-def show_config(config: Config, start_indent: int = 1) -> None:
+def show_config(config: Config) -> None:
     """Show the config dict in a pretty way.
 
     The config dict is unflattened before.
 
     Parameters
     ----------
     config : Config
         The config to show.
-    start_indent : int, optional
-        The number of starting tab indent (4 spaces), by default 1.
     """
-    show_dict(config.dict, start_indent)
+    print("Config:")
+    show_dict(config.dict, start_indent=1)
```

### Comparing `cliconfig-0.5.6/cliconfig/dict_routines.py` & `cliconfig-0.6.0/cliconfig/dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/cliconfig/process_routines.py` & `cliconfig-0.6.0/cliconfig/process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/cliconfig/processing/_type_parser.py` & `cliconfig-0.6.0/cliconfig/processing/_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/cliconfig/processing/base.py` & `cliconfig-0.6.0/cliconfig/processing/base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/cliconfig/processing/builtin.py` & `cliconfig-0.6.0/cliconfig/processing/builtin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Built-in processing classes.
 
 Classes to apply pre-merge, post-merge, pre-save and post-load modifications
 to dict with processing routines (found in cliconfig.process_routines).
 """
-# pylint: disable=unused-argument
 from typing import Any, Dict, List, Set
 
 from cliconfig.base import Config
 from cliconfig.process_routines import (
     merge_flat_paths_processing,
     merge_flat_processing,
 )
@@ -161,16 +160,17 @@
 
 class ProcessCopy(Processing):
     """Copy a value with '@copy' tag. The copy is protected from updates.
 
     Tag your key with '@copy' and with value the name of the flat key to copy.
     Then, the value will be a copy of the corresponding value forever.
     The pre-merge processing will remove the tag. The post-merge processing
-    will set the value and occurs after most processing. The pre-save processing
-    restore the tag and the key to copy to keep the information on future loads.
+    will set the value (if the copied key exists) and occurs after most processing.
+    The pre-save processing restore the tag and the key to copy to keep the
+    information on future loads.
 
     The copy key is protected against any modification and will raise an error
     if you try to modify it.
 
     Pre-merge order: 0.0
     Post-merge order: 10.0
     Pre-save order: 10.0
@@ -185,14 +185,20 @@
           c@copy: a.b
 
     Before merging, the config is interpreted as the dict
 
     .. code-block:: python
 
         {'a': {'b': 1, 'c': 1}}
+
+    Note
+    ----
+        If the key to copy does not exist in the config on post-merge, the
+        processing will NOT raise an error to let the user the possibility
+        to add the key later via merge. However, the key still be protected.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.premerge_order = 0.0
         self.postmerge_order = 10.0
         self.presave_order = 10.0
@@ -225,27 +231,24 @@
                 flat_config.dict[clean_tag(flat_key, "copy")] = val
                 del flat_config.dict[flat_key]
         return flat_config
 
     def postmerge(self, flat_config: Config) -> Config:
         """Post-merge processing."""
         for key, val in self.keys_to_copy.items():
-            if key in flat_config.dict:
-                if val not in flat_config.dict:
-                    raise ValueError(
-                        f"Key to copy not found in config: {val}. "
-                        f"The problem occurs with key: {key}"
-                    )
+            # NOTE: Do not raise an error if the key to copy does not exist
+            # yet because it can be added later in a future merge
+            if key in flat_config.dict and val in flat_config.dict:
                 if flat_config.dict[key] != self.current_value[key]:
                     # The key has been modified
                     raise ValueError(
-                        "Found attempt to modify a key with '@copy' tag. The key is "
-                        "then protected against updates (except the copied value or "
-                        f"the original key to copy). Found key: {key} of value "
-                        f"{flat_config.dict[key]} that copy {val} of value "
+                        "Found attempt to modify a key with '@copy' tag. The key "
+                        "is then protected against updates (except the copied "
+                        f"value or the original key to copy). Found key: {key} of "
+                        f"value {flat_config.dict[key]} that copy {val} of value "
                         f"{flat_config.dict[val]}")
                 # Copy the value
                 flat_config.dict[key] = flat_config.dict[val]
                 # Update the current value
                 self.current_value[key] = flat_config.dict[val]
         return flat_config
 
@@ -356,21 +359,23 @@
                 del flat_config.dict[key]
         return flat_config
 
 
 class ProcessSelect(Processing):
     """Select a sub-config with and delete the rest of its parent config.
 
-    First look for a parameter tagged with '@select' containing a flat key
-    corresponding to a sub-configurations to keep. The parent configuration
-    is then deleted on pre-merge, except the selected sub-configuration
+    First look in pre-merge for a parameter tagged with '@select' containing a
+    flat key corresponding to a sub-configurations to keep. The parent configuration
+    is then deleted on post-merge, except the selected sub-configuration
     and eventually the tagged parameter (if it is in the same sub-configuration).
     It is also possible to select multiple keys of a same sub-configuration
     (meaning that the part before the last dot must be equal) by passing a
     list of flat keys.
+    Pre-merge order: 0.0
+    Post-merge order: 0.0
 
     Examples
     --------
     .. code-block:: yaml
 
         models:
             model_names@select: [models.model1, models.model3]
@@ -396,24 +401,23 @@
         (which is the case when the selected key doesn't contain a dot),
         and raises an error in this case.
 
     """
 
     def __init__(self) -> None:
         super().__init__()
-        # Slighly negative to prevent the use of tags involving keys to delete
-        self.premerge_order = -5.0
         self.keys_that_select: Set[str] = set()
+        self.subconfigs_to_delete: Set[str] = set()
+        self.keys_to_keep: Set[str] = set()
 
     def premerge(self, flat_config: Config) -> Config:
         """Pre-merge processing."""
         items = list(flat_config.dict.items())
         for flat_key, val in items:
-            # NOTE: Check if flat_key is in dict in case of deletion
-            if flat_key in flat_config.dict and is_tag_in(flat_key, "select"):
+            if is_tag_in(flat_key, "select"):
                 # Remove the tag
                 clean_key = clean_all_tags(flat_key)
                 del flat_config.dict[flat_key]
                 flat_config.dict[clean_tag(flat_key, "select")] = val
                 self.keys_that_select.add(clean_key)
                 if isinstance(val, str):
                     subconfig = ".".join(flat_key.split(".")[:-1])
@@ -438,23 +442,32 @@
                 subconfig = clean_all_tags(subconfig)
                 if subconfig == "":
                     raise ValueError(
                         "Find attempt to delete the configuration at the root. You "
                         "must pass a flat key with a least one dot on parameter "
                         f"tagged with @select. Find key: {flat_key} with value: {val}"
                     )
-                # Delete all keys on the subconfig except the ones to keep
-                for key in list(flat_config.dict.keys()):
-                    clean_key = clean_all_tags(key)
-                    if (clean_key.startswith(subconfig)
-                            and not any(clean_key.startswith(key_to_keep)
-                                        for key_to_keep in keys_to_keep)):
-                        del flat_config.dict[key]
+                self.subconfigs_to_delete.add(subconfig)
+                self.keys_to_keep.update(keys_to_keep)
         return flat_config
 
+    def postmerge(self, flat_config: Config) -> Config:
+        """Post-merge processing."""
+        def _is_in_subconfig(key: str, subconfig: str) -> bool:
+            """Check if a key is in a subconfig with the exact name."""
+            return key == subconfig or key.startswith(subconfig + ".")
+        # Delete all keys on the subconfigs except the ones to keep
+        for subconfig in self.subconfigs_to_delete:
+            for key in list(flat_config.dict.keys()):
+                if (_is_in_subconfig(key, subconfig)
+                        and not any(_is_in_subconfig(key, key_to_keep)
+                                    for key_to_keep in self.keys_to_keep)):
+                    del flat_config.dict[key]
+        return super().postmerge(flat_config)
+
     def presave(self, flat_config: Config) -> Config:
         """Pre-save processing."""
         # Restore the tag with the type to keep the information
         # on further loading
         for key in self.keys_that_select:
             if key in flat_config.dict:
                 new_key = key + "@select"
```

### Comparing `cliconfig-0.5.6/cliconfig/processing/create.py` & `cliconfig-0.6.0/cliconfig/processing/create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/cliconfig/tag_routines.py` & `cliconfig-0.6.0/cliconfig/tag_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.6.0/README_pypi.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: cliconfig
-Version: 0.5.6
-Summary: Merge your config files and set parameters from the command line in a simple way.
-Author-email: Valentin Goldite <valentin.goldite@gmail.com>
-Project-URL: Source, https://github.com/valentingol/cliconfig
-Keywords: logging,machine,learning
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CLI Config
 
 </p>
 <p align="center">
   <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
 </p>
 
@@ -135,33 +123,14 @@
 pip install -e .
 pip install -r requirements-dev.txt
 ```
 
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
-## Todo
-
-Priority:
-
-* [x] allow passing new arguments by CLI (with warning and no actual merge)
-* [ ] add a routine to check if a tag is in a key and robust to all other
-  possible tags
-* [ ] add an integration test with all built-in processing (and more)
-
-Secondary:
-
-* [ ] add `make_processing_keep_property` to make a processing that keep the
-  property of a parameter across merged configs. The property is any python object
-  returned by a function that takes the parameter as input
-* [ ] add `ProcessSelect` (with tag "@select") to select a subconfig (or parameter)
-  and delete the others configs at the same level (to cure the resulting config)
-* [ ] allow nested types in `ProcessTyping`
-* [x] add DefaultProcessings that stores default processing as list of processing
-
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
 it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `cliconfig-0.5.6/docs/Makefile` & `cliconfig-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/docs/_static/logo.png` & `cliconfig-0.6.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/docs/_static/logo_extend.png` & `cliconfig-0.6.0/docs/_static/logo_extend.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/docs/cliconfig_api.rst` & `cliconfig-0.6.0/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/docs/conf.py` & `cliconfig-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/docs/edge_cases.md` & `cliconfig-0.6.0/docs/edge_cases.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/docs/index.rst` & `cliconfig-0.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/docs/license.md` & `cliconfig-0.6.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/docs/make.bat` & `cliconfig-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/docs/processing.md` & `cliconfig-0.6.0/docs/processing.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/docs/quickstart.md` & `cliconfig-0.6.0/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.6.0/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/github_actions_utils/pylint_manager.py` & `cliconfig-0.6.0/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/github_actions_utils/pytest_manager.py` & `cliconfig-0.6.0/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.6.0/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/pyproject.toml` & `cliconfig-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/tests/conftest.py` & `cliconfig-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/tests/unit/processing/test_base.py` & `cliconfig-0.6.0/tests/unit/processing/test_base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/tests/unit/processing/test_builtin.py` & `cliconfig-0.6.0/tests/unit/processing/test_builtin.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,24 +140,17 @@
         ValueError,
         match=(
             "Key with '@copy' has change its value to copy. Found key: a@copy@tag "
             "with value: c, previous value to copy: b"
         )
     ):
         processing.premerge(Config({"a@copy@tag": "c"}, [processing]))
-    # Case of non-existing key (on post-merge)
+    # Case of non-existing key (on post-merge): do not raise error
     processing.keys_to_copy = {"a": "b"}
-    with pytest.raises(
-        ValueError,
-        match=(
-            "Key to copy not found in config: b. "
-            "The problem occurs with key: a"
-        )
-    ):
-        processing.postmerge(Config({"a": "b"}, [processing]))
+    processing.postmerge(Config({"a": "b"}, [processing]))
     # Case overwriting a key
     processing.current_value = {"a": 2}
     with pytest.raises(
         ValueError,
         match=re.escape(
             "Found attempt to modify a key with '@copy' tag. The key is "
             "then protected against updates (except the copied value or "
@@ -249,14 +242,15 @@
         "models.model_names": ["models.model1", "models.model3"],
         "models.model1.param1": 1,
         "models.model1.param2": 2,
         "models.model3.submodel.param": 5,
     }
     config = Config(flat_dict, [])
     config = processing.premerge(config)
+    config = processing.postmerge(config)
     check.equal(config.dict, expected_dict)
     config = processing.presave(config)
     check.is_in("models.model_names@select", config.dict)
     check.equal(
         config.dict["models.model_names@select"],
         ["models.model1", "models.model3"]
     )
```

### Comparing `cliconfig-0.5.6/tests/unit/processing/test_create.py` & `cliconfig-0.6.0/tests/unit/processing/test_create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/tests/unit/processing/test_type_parser.py` & `cliconfig-0.6.0/tests/unit/processing/test_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/tests/unit/test_cli_parser.py` & `cliconfig-0.6.0/tests/unit/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/tests/unit/test_config_routines.py` & `cliconfig-0.6.0/tests/unit/test_config_routines.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 import sys
 
 import pytest
 import pytest_check as check
 
 from cliconfig.base import Config
 from cliconfig.config_routines import load_config, make_config, save_config, show_config
+from cliconfig.processing.base import Processing
 
 
-def test_make_config(capsys: pytest.CaptureFixture) -> None:
+def test_make_config(capsys: pytest.CaptureFixture, process_add1: Processing) -> None:
     """Test make_config."""
     sys_argv = sys.argv.copy()
     sys.argv = [
         "tests/test_make_config.py.py",
         "--config",
         "tests/configs/config1.yaml,tests/configs/config2.yaml",
         "--unknown",
-        "--param2=6",
+        "--param2@add1=6",
         "--unknown2=8",  # check that not error but a warning in console
     ]
     capsys.readouterr()  # Clear stdout and stderr
     config = make_config(
         "tests/configs/default1.yaml",
-        "tests/configs/default2.yaml"
+        "tests/configs/default2.yaml",
+        process_list=[process_add1],
     )
     captured = capsys.readouterr()
     out = captured.out
     expected_config = {
         "param1": 4,
-        "param2": 6,
+        "param2": 7,
         "param3": 3,
         "letters": {
             "letter1": "f",
             "letter2": "e",
             "letter3": "c",
             "letter4": "d",
         },
@@ -64,27 +66,31 @@
             "letter1": "a",
             "letter2": "b",
             "letter3": "c",
             "letter4": "d",
         },
     }
     check.equal(config.dict, expected_config)
+    config = make_config(add_default_processing=False)
+    check.equal(config.dict, {})
+    check.equal(config.process_list, [])
 
     sys.argv = sys_argv.copy()
 
 
-def test_load_config() -> None:
+def test_load_config(process_add1: Processing) -> None:
     """Test and load_config."""
     # With default configs
     config = load_config(
         "tests/configs/config2.yaml",
         default_config_paths=[
             "tests/configs/default1.yaml",
             "tests/configs/default2.yaml",
-        ]
+        ],
+        process_list=[process_add1],
     )
     expected_config = {
         "param1": 4,
         "param2": 2,
         "param3": 3,
         "letters": {
             "letter1": "a",
```

### Comparing `cliconfig-0.5.6/tests/unit/test_dict_routines.py` & `cliconfig-0.6.0/tests/unit/test_dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/tests/unit/test_ex_docs.py` & `cliconfig-0.6.0/tests/unit/test_ex_docs.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/tests/unit/test_process_routines.py` & `cliconfig-0.6.0/tests/unit/test_process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.5.6/tests/unit/test_tag_routines.py` & `cliconfig-0.6.0/tests/unit/test_tag_routines.py`

 * *Files identical despite different names*

