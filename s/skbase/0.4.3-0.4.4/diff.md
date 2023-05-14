# Comparing `tmp/skbase-0.4.3.tar.gz` & `tmp/skbase-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skbase-0.4.3.tar", last modified: Fri May  5 00:37:28 2023, max compression
+gzip compressed data, was "skbase-0.4.4.tar", last modified: Sun May 14 00:31:11 2023, max compression
```

## Comparing `skbase-0.4.3.tar` & `skbase-0.4.4.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.397496 skbase-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-05-05 00:37:14.000000 skbase-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-05 00:37:28.397496 skbase-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-05-05 00:37:14.000000 skbase-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.377496 skbase-0.4.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.381496 skbase-0.4.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     9845 2023-05-05 00:37:14.000000 skbase-0.4.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-05 00:37:14.000000 skbase-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-05-05 00:37:28.397496 skbase-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.381496 skbase-0.4.3/skbase/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/_nopytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.385496 skbase-0.4.3/skbase/base/
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43634 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    35626 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.385496 skbase-0.4.3/skbase/base/_pretty_printing/
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/_pretty_printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11539 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/_pretty_printing/_object_html_repr.py
--rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/_pretty_printing/_pprint.py
--rw-r--r--   0 runner    (1001) docker     (122)     7290 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/base/_tagmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.385496 skbase-0.4.3/skbase/lookup/
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    38936 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/lookup/_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.385496 skbase-0.4.3/skbase/lookup/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/lookup/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36924 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/lookup/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.389496 skbase-0.4.3/skbase/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36450 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/test_all_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.389496 skbase-0.4.3/skbase/testing/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9890 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/_conditional_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    11063 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.389496 skbase-0.4.3/skbase/testing/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/tests/test_check_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/testing/utils/tests/test_deep_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.393496 skbase-0.4.3/skbase/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7792 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.393496 skbase-0.4.3/skbase/tests/mock_package/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/mock_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/mock_package/test_mock_package.py
--rw-r--r--   0 runner    (1001) docker     (122)    41827 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/test_baseestimator.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/tests/test_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.393496 skbase-0.4.3/skbase/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     8037 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.393496 skbase-0.4.3/skbase/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/tests/test_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/utils/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.397496 skbase-0.4.3/skbase/validate/
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14777 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/validate/_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    12121 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/validate/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.397496 skbase-0.4.3/skbase/validate/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/validate/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/validate/tests/test_iterable_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-05-05 00:37:14.000000 skbase-0.4.3/skbase/validate/tests/test_type_validations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 00:37:28.385496 skbase-0.4.3/skbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-05 00:37:28.000000 skbase-0.4.3/skbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-05-05 00:37:28.000000 skbase-0.4.3/skbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 00:37:28.000000 skbase-0.4.3/skbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-05-05 00:37:28.000000 skbase-0.4.3/skbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-05 00:37:28.000000 skbase-0.4.3/skbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 00:37:28.000000 skbase-0.4.3/skbase.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.260449 skbase-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-05-14 00:31:02.000000 skbase-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-14 00:31:11.260449 skbase-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-05-14 00:31:02.000000 skbase-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.252449 skbase-0.4.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.252449 skbase-0.4.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     9845 2023-05-14 00:31:02.000000 skbase-0.4.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-14 00:31:02.000000 skbase-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-05-14 00:31:11.260449 skbase-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.252449 skbase-0.4.4/skbase/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/_nopytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43618 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35626 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/base/_pretty_printing/
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/_pretty_printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11539 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/_pretty_printing/_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7290 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/_tagmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/lookup/
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/lookup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38936 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/lookup/_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/lookup/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/lookup/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36924 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/lookup/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36442 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/test_all_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9890 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/_conditional_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/testing/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/tests/test_check_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/tests/test_deep_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8398 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/tests/mock_package/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/mock_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/mock_package/test_mock_package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41827 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/test_baseestimator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.260449 skbase-0.4.4/skbase/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8037 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11299 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/deep_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.260449 skbase-0.4.4/skbase/utils/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/dependencies/_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.260449 skbase-0.4.4/skbase/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/tests/test_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.260449 skbase-0.4.4/skbase/validate/
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14777 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/validate/_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12121 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/validate/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.260449 skbase-0.4.4/skbase/validate/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/validate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/validate/tests/test_iterable_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/validate/tests/test_type_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-14 00:31:11.000000 skbase-0.4.4/skbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-14 00:31:11.000000 skbase-0.4.4/skbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 00:31:11.000000 skbase-0.4.4/skbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-05-14 00:31:11.000000 skbase-0.4.4/skbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-14 00:31:11.000000 skbase-0.4.4/skbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 00:31:10.000000 skbase-0.4.4/skbase.egg-info/zip-safe
```

### Comparing `skbase-0.4.3/LICENSE` & `skbase-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/PKG-INFO` & `skbase-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skbase
-Version: 0.4.3
+Version: 0.4.4
 Summary: Base classes for sklearn-like parametric objects
 Author: Franz Király, Markus Löning, Ryan Kuhns
 Maintainer-email: Franz Kiraly <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
         All rights reserved.
@@ -69,15 +69,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.3 is now available. Checkout our
+:rocket: Version 0.4.4 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `skbase-0.4.3/README.md` & `skbase-0.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.3 is now available. Checkout our
+:rocket: Version 0.4.4 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `skbase-0.4.3/docs/source/conf.py` & `skbase-0.4.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/pyproject.toml` & `skbase-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "skbase"
-version = "0.4.3"
+version = "0.4.4"
 description = "Base classes for sklearn-like parametric objects"
 authors = [
     {name = "Franz Király"},
     {name = "Markus Löning"},
     {name = "Ryan Kuhns"},
 ]
 maintainers = [
```

### Comparing `skbase-0.4.3/skbase/_exceptions.py` & `skbase-0.4.4/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/base/__init__.py` & `skbase-0.4.4/skbase/base/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/base/_base.py` & `skbase-0.4.4/skbase/base/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         """Equality dunder. Checks equal class and parameters.
 
         Returns True iff result of get_params(deep=False)
         results in equal parameter sets.
 
         Nested BaseObject descendants from get_params are compared via __eq__ as well.
         """
-        from skbase.testing.utils.deep_equals import deep_equals
+        from skbase.utils.deep_equals import deep_equals
 
         if not isinstance(other, BaseObject):
             return False
 
         self_params = self.get_params(deep=False)
         other_params = other.get_params(deep=False)
 
@@ -157,15 +157,15 @@
         self_params = self.get_params(deep=False)
         self_clone = type(self)(**self_params)
 
         # if checking the clone is turned off, return now
         if not self.get_config()["check_clone"]:
             return self_clone
 
-        from skbase.testing.utils.deep_equals import deep_equals
+        from skbase.utils.deep_equals import deep_equals
 
         # check that all attributes are written to the clone
         for attrname in self_params.keys():
             if not hasattr(self_clone, attrname):
                 raise RuntimeError(
                     f"error in {self}.clone, __init__ must write all arguments "
                     f"to self and not mutate them, but {attrname} was not found. "
```

### Comparing `skbase-0.4.3/skbase/base/_meta.py` & `skbase-0.4.4/skbase/base/_meta.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/base/_pretty_printing/_object_html_repr.py` & `skbase-0.4.4/skbase/base/_pretty_printing/_object_html_repr.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/base/_pretty_printing/_pprint.py` & `skbase-0.4.4/skbase/base/_pretty_printing/_pprint.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/base/_tagmanager.py` & `skbase-0.4.4/skbase/base/_tagmanager.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/lookup/__init__.py` & `skbase-0.4.4/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/lookup/_lookup.py` & `skbase-0.4.4/skbase/lookup/_lookup.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/lookup/tests/test_lookup.py` & `skbase-0.4.4/skbase/lookup/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/testing/test_all_objects.py` & `skbase-0.4.4/skbase/testing/test_all_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 from skbase.base import BaseObject
 from skbase.lookup import all_objects
 from skbase.testing.utils._conditional_fixtures import (
     create_conditional_fixtures_and_names,
 )
 from skbase.testing.utils._dependencies import _check_soft_dependencies
-from skbase.testing.utils.deep_equals import deep_equals
 from skbase.testing.utils.inspect import _get_args
+from skbase.utils.deep_equals import deep_equals
 
 __author__: List[str] = ["fkiraly"]
 
 
 class BaseFixtureGenerator:
     """Fixture generator for skbase testing functionality.
```

### Comparing `skbase-0.4.3/skbase/testing/utils/_conditional_fixtures.py` & `skbase-0.4.4/skbase/testing/utils/_conditional_fixtures.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/testing/utils/_dependencies.py` & `skbase-0.4.4/skbase/utils/dependencies/_dependencies.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/testing/utils/deep_equals.py` & `skbase-0.4.4/skbase/utils/deep_equals.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,34 @@
     types compatible with != comparison
     pd.Series, pd.DataFrame, np.ndarray
     lists, tuples, or dicts of a valid type (recursive)
 """
 from inspect import isclass
 from typing import List
 
-from skbase.testing.utils._dependencies import _check_soft_dependencies
-
 __author__: List[str] = ["fkiraly"]
 __all__: List[str] = ["deep_equals"]
 
 
 # flag variables for available soft dependencies
-pandas_available = _check_soft_dependencies("pandas", severity="none")
-numpy_available = _check_soft_dependencies("numpy", severity="none")
+# we are not using _check_soft_dependencies in order to keep
+# this utility uncoupled from the dependency on "packaging", of _check_soft_dependencies
+def _softdep_available(importname):
+    from importlib import import_module
+
+    try:
+        import_module(importname)
+    except ModuleNotFoundError:
+        return False
+    else:
+        return True
+
+
+numpy_available = _softdep_available("numpy")
+pandas_available = _softdep_available("pandas")
 
 
 def deep_equals(x, y, return_msg=False):
     """Test two objects for equality in value.
 
     Correct if x/y are one of the following valid types:
         types compatible with != comparison
```

### Comparing `skbase-0.4.3/skbase/testing/utils/inspect.py` & `skbase-0.4.4/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/testing/utils/tests/test_check_dependencies.py` & `skbase-0.4.4/skbase/testing/utils/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/testing/utils/tests/test_deep_equals.py` & `skbase-0.4.4/skbase/testing/utils/tests/test_deep_equals.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Tests for deep_equals utility."""
 from copy import deepcopy
 
 import numpy as np
 import pytest
 
 from skbase.testing.utils._dependencies import _check_soft_dependencies
-from skbase.testing.utils.deep_equals import deep_equals
+from skbase.utils.deep_equals import deep_equals
 
 # examples used for comparison below
 EXAMPLES = [
     42,
     [],
     ((((())))),
     [([([([()])])])],
```

### Comparing `skbase-0.4.3/skbase/tests/conftest.py` & `skbase-0.4.4/skbase/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,14 +46,17 @@
     "skbase.tests.test_baseestimator",
     "skbase.tests.mock_package.test_mock_package",
     "skbase.utils",
     "skbase.utils._check",
     "skbase.utils._iter",
     "skbase.utils._nested_iter",
     "skbase.utils._utils",
+    "skbase.utils.deep_equals",
+    "skbase.utils.dependencies",
+    "skbase.utils.dependencies._dependencies",
     "skbase.validate",
     "skbase.validate._named_objects",
     "skbase.validate._types",
 )
 SKBASE_PUBLIC_MODULES = (
     "skbase",
     "skbase.base",
@@ -69,14 +72,16 @@
     "skbase.testing.utils.tests.test_deep_equals",
     "skbase.tests",
     "skbase.tests.conftest",
     "skbase.tests.test_base",
     "skbase.tests.test_baseestimator",
     "skbase.tests.mock_package.test_mock_package",
     "skbase.utils",
+    "skbase.utils.deep_equals",
+    "skbase.utils.dependencies",
     "skbase.validate",
 )
 SKBASE_PUBLIC_CLASSES_BY_MODULE = {
     "skbase._exceptions": ("FixtureGenerationError", "NotFittedError"),
     "skbase.base": (
         "BaseEstimator",
         "BaseMetaEstimator",
@@ -129,14 +134,15 @@
     ),
     "skbase.validate._named_objects": (
         "check_sequence_named_objects",
         "is_named_object_tuple",
         "is_sequence_named_objects",
     ),
     "skbase.utils": (
+        "deep_equals",
         "flatten",
         "is_flat",
         "make_strings_unique",
         "subset_dict_keys",
         "unflat_len",
         "unflatten",
     ),
@@ -144,14 +150,15 @@
     "skbase.utils._nested_iter": (
         "flatten",
         "is_flat",
         "unflat_len",
         "unflatten",
     ),
     "skbase.utils._utils": ("subset_dict_keys",),
+    "skbase.utils.deep_equals": ("deep_equals",),
     "skbase.validate._types": ("check_sequence", "check_type", "is_sequence"),
 }
 SKBASE_FUNCTIONS_BY_MODULE = SKBASE_PUBLIC_FUNCTIONS_BY_MODULE.copy()
 SKBASE_FUNCTIONS_BY_MODULE.update(
     {
         "skbase.base._pretty_printing._object_html_repr": (
             "_get_visual_block",
@@ -175,41 +182,51 @@
             "_check_object_types",
             "_get_module_info",
         ),
         "skbase.testing.utils._dependencies": (
             "_check_soft_dependencies",
             "_check_python_version",
         ),
-        "skbase.testing.utils.deep_equals": (
-            "_pandas_equals",
-            "_dict_equals",
-            "_is_pandas",
-            "_is_npnan",
-            "_tuple_equals",
-            "_fh_equals",
-            "deep_equals",
-            "_is_npndarray",
-            "_coerce_list",
-        ),
+        "skbase.testing.utils.deep_equals": ("deep_equals",),
         "skbase.testing.utils.inspect": ("_get_args",),
         "skbase.utils._check": ("_is_scalar_nan",),
+        "skbase.utils.dependencies": (
+            "_check_soft_dependencies",
+            "_check_python_version",
+        ),
         "skbase.utils._iter": (
             "_format_seq_to_str",
             "_remove_type_text",
             "_scalar_to_seq",
             "make_strings_unique",
         ),
         "skbase.utils._nested_iter": (
             "flatten",
             "is_flat",
             "_remove_single",
             "unflat_len",
             "unflatten",
         ),
         "skbase.utils._utils": ("subset_dict_keys",),
+        "skbase.utils.deep_equals": (
+            "_coerce_list",
+            "_dict_equals",
+            "_fh_equals",
+            "_is_npnan",
+            "_is_npndarray",
+            "_is_pandas",
+            "_pandas_equals",
+            "_softdep_available",
+            "_tuple_equals",
+            "deep_equals",
+        ),
+        "skbase.utils.dependencies._dependencies": (
+            "_check_soft_dependencies",
+            "_check_python_version",
+        ),
         "skbase.validate._named_objects": (
             "check_sequence_named_objects",
             "is_named_object_tuple",
             "is_sequence_named_objects",
             "_named_baseobject_error_msg",
         ),
         "skbase.validate._types": (
```

### Comparing `skbase-0.4.3/skbase/tests/mock_package/test_mock_package.py` & `skbase-0.4.4/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/tests/test_base.py` & `skbase-0.4.4/skbase/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/tests/test_baseestimator.py` & `skbase-0.4.4/skbase/tests/test_baseestimator.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/tests/test_exceptions.py` & `skbase-0.4.4/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/tests/test_meta.py` & `skbase-0.4.4/skbase/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/utils/__init__.py` & `skbase-0.4.4/skbase/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 # copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
 """Utility functionality used through `skbase`."""
 from typing import List
 
 from skbase.utils._iter import make_strings_unique
 from skbase.utils._nested_iter import flatten, is_flat, unflat_len, unflatten
 from skbase.utils._utils import subset_dict_keys
+from skbase.utils.deep_equals import deep_equals
 
 __author__: List[str] = ["RNKuhns", "fkiraly"]
 __all__: List[str] = [
+    "deep_equals",
     "flatten",
     "is_flat",
     "make_strings_unique",
     "subset_dict_keys",
     "unflat_len",
     "unflatten",
 ]
```

### Comparing `skbase-0.4.3/skbase/utils/_check.py` & `skbase-0.4.4/skbase/utils/_check.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/utils/_iter.py` & `skbase-0.4.4/skbase/utils/_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/utils/_nested_iter.py` & `skbase-0.4.4/skbase/utils/_nested_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/utils/_utils.py` & `skbase-0.4.4/skbase/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/utils/tests/test_check.py` & `skbase-0.4.4/skbase/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/utils/tests/test_iter.py` & `skbase-0.4.4/skbase/utils/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/utils/tests/test_nested_iter.py` & `skbase-0.4.4/skbase/utils/tests/test_nested_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/utils/tests/test_utils.py` & `skbase-0.4.4/skbase/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/validate/__init__.py` & `skbase-0.4.4/skbase/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/validate/_named_objects.py` & `skbase-0.4.4/skbase/validate/_named_objects.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/validate/_types.py` & `skbase-0.4.4/skbase/validate/_types.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/validate/tests/test_iterable_named_objects.py` & `skbase-0.4.4/skbase/validate/tests/test_iterable_named_objects.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase/validate/tests/test_type_validations.py` & `skbase-0.4.4/skbase/validate/tests/test_type_validations.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.3/skbase.egg-info/PKG-INFO` & `skbase-0.4.4/skbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skbase
-Version: 0.4.3
+Version: 0.4.4
 Summary: Base classes for sklearn-like parametric objects
 Author: Franz Király, Markus Löning, Ryan Kuhns
 Maintainer-email: Franz Kiraly <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
         All rights reserved.
@@ -69,15 +69,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.3 is now available. Checkout our
+:rocket: Version 0.4.4 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `skbase-0.4.3/skbase.egg-info/SOURCES.txt` & `skbase-0.4.4/skbase.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 skbase/tests/mock_package/__init__.py
 skbase/tests/mock_package/test_mock_package.py
 skbase/utils/__init__.py
 skbase/utils/_check.py
 skbase/utils/_iter.py
 skbase/utils/_nested_iter.py
 skbase/utils/_utils.py
+skbase/utils/deep_equals.py
+skbase/utils/dependencies/__init__.py
+skbase/utils/dependencies/_dependencies.py
 skbase/utils/tests/__init__.py
 skbase/utils/tests/test_check.py
 skbase/utils/tests/test_iter.py
 skbase/utils/tests/test_nested_iter.py
 skbase/utils/tests/test_utils.py
 skbase/validate/__init__.py
 skbase/validate/_named_objects.py
```

### Comparing `skbase-0.4.3/skbase.egg-info/requires.txt` & `skbase-0.4.4/skbase.egg-info/requires.txt`

 * *Files identical despite different names*

