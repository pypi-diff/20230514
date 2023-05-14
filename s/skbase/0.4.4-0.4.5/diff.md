# Comparing `tmp/skbase-0.4.4.tar.gz` & `tmp/skbase-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skbase-0.4.4.tar", last modified: Sun May 14 00:31:11 2023, max compression
+gzip compressed data, was "skbase-0.4.5.tar", last modified: Sun May 14 14:07:44 2023, max compression
```

## Comparing `skbase-0.4.4.tar` & `skbase-0.4.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.260449 skbase-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-05-14 00:31:02.000000 skbase-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-14 00:31:11.260449 skbase-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-05-14 00:31:02.000000 skbase-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.252449 skbase-0.4.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.252449 skbase-0.4.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     9845 2023-05-14 00:31:02.000000 skbase-0.4.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-14 00:31:02.000000 skbase-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-05-14 00:31:11.260449 skbase-0.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.252449 skbase-0.4.4/skbase/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/_nopytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/base/
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43618 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    35626 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/base/_pretty_printing/
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/_pretty_printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11539 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/_pretty_printing/_object_html_repr.py
--rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/_pretty_printing/_pprint.py
--rw-r--r--   0 runner    (1001) docker     (122)     7290 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/base/_tagmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/lookup/
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    38936 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/lookup/_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/lookup/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/lookup/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36924 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/lookup/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36442 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/test_all_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/testing/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9890 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/_conditional_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/testing/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/tests/test_check_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/testing/utils/tests/test_deep_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8398 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase/tests/mock_package/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/mock_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/mock_package/test_mock_package.py
--rw-r--r--   0 runner    (1001) docker     (122)    41827 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/test_baseestimator.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/tests/test_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.260449 skbase-0.4.4/skbase/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     8037 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    11299 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/deep_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.260449 skbase-0.4.4/skbase/utils/dependencies/
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/dependencies/_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.260449 skbase-0.4.4/skbase/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/tests/test_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/utils/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.260449 skbase-0.4.4/skbase/validate/
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14777 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/validate/_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    12121 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/validate/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.260449 skbase-0.4.4/skbase/validate/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/validate/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/validate/tests/test_iterable_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-05-14 00:31:02.000000 skbase-0.4.4/skbase/validate/tests/test_type_validations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 00:31:11.256449 skbase-0.4.4/skbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-14 00:31:11.000000 skbase-0.4.4/skbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-14 00:31:11.000000 skbase-0.4.4/skbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 00:31:11.000000 skbase-0.4.4/skbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-05-14 00:31:11.000000 skbase-0.4.4/skbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-14 00:31:11.000000 skbase-0.4.4/skbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 00:31:10.000000 skbase-0.4.4/skbase.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.401671 skbase-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-05-14 14:07:33.000000 skbase-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-14 14:07:44.401671 skbase-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-05-14 14:07:33.000000 skbase-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.385670 skbase-0.4.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.389670 skbase-0.4.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     9845 2023-05-14 14:07:33.000000 skbase-0.4.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-14 14:07:33.000000 skbase-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-05-14 14:07:44.401671 skbase-0.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/_nopytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase/base/
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43618 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35626 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase/base/_pretty_printing/
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/_pretty_printing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11539 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/_pretty_printing/_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7290 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/_tagmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase/lookup/
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/lookup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38936 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/lookup/_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase/lookup/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/lookup/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36924 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/lookup/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36442 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/test_all_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.397671 skbase-0.4.5/skbase/testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9890 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/_conditional_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.397671 skbase-0.4.5/skbase/testing/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/tests/test_check_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/tests/test_deep_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.397671 skbase-0.4.5/skbase/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8398 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.397671 skbase-0.4.5/skbase/tests/mock_package/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/mock_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/mock_package/test_mock_package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41827 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/test_baseestimator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.397671 skbase-0.4.5/skbase/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8037 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11299 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/deep_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.397671 skbase-0.4.5/skbase/utils/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/dependencies/_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.401671 skbase-0.4.5/skbase/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/tests/test_nested_iter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.401671 skbase-0.4.5/skbase/validate/
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14777 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/validate/_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12121 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/validate/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.401671 skbase-0.4.5/skbase/validate/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/validate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/validate/tests/test_iterable_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/validate/tests/test_type_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-14 14:07:44.000000 skbase-0.4.5/skbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-14 14:07:44.000000 skbase-0.4.5/skbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 14:07:44.000000 skbase-0.4.5/skbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-05-14 14:07:44.000000 skbase-0.4.5/skbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-14 14:07:44.000000 skbase-0.4.5/skbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 14:07:44.000000 skbase-0.4.5/skbase.egg-info/zip-safe
```

### Comparing `skbase-0.4.4/LICENSE` & `skbase-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/PKG-INFO` & `skbase-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skbase
-Version: 0.4.4
+Version: 0.4.5
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
 
-:rocket: Version 0.4.4 is now available. Checkout our
+:rocket: Version 0.4.5 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `skbase-0.4.4/README.md` & `skbase-0.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.4 is now available. Checkout our
+:rocket: Version 0.4.5 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `skbase-0.4.4/docs/source/conf.py` & `skbase-0.4.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/pyproject.toml` & `skbase-0.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "skbase"
-version = "0.4.4"
+version = "0.4.5"
 description = "Base classes for sklearn-like parametric objects"
 authors = [
     {name = "Franz Király"},
     {name = "Markus Löning"},
     {name = "Ryan Kuhns"},
 ]
 maintainers = [
```

### Comparing `skbase-0.4.4/skbase/_exceptions.py` & `skbase-0.4.5/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/_nopytest_tests.py` & `skbase-0.4.5/skbase/_nopytest_tests.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/base/__init__.py` & `skbase-0.4.5/skbase/base/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/base/_base.py` & `skbase-0.4.5/skbase/base/_base.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/base/_meta.py` & `skbase-0.4.5/skbase/base/_meta.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/base/_pretty_printing/_object_html_repr.py` & `skbase-0.4.5/skbase/base/_pretty_printing/_object_html_repr.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/base/_pretty_printing/_pprint.py` & `skbase-0.4.5/skbase/base/_pretty_printing/_pprint.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/base/_tagmanager.py` & `skbase-0.4.5/skbase/base/_tagmanager.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/lookup/__init__.py` & `skbase-0.4.5/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/lookup/_lookup.py` & `skbase-0.4.5/skbase/lookup/_lookup.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/lookup/tests/test_lookup.py` & `skbase-0.4.5/skbase/lookup/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/testing/test_all_objects.py` & `skbase-0.4.5/skbase/testing/test_all_objects.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/testing/utils/_conditional_fixtures.py` & `skbase-0.4.5/skbase/testing/utils/_conditional_fixtures.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/testing/utils/inspect.py` & `skbase-0.4.5/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/testing/utils/tests/test_check_dependencies.py` & `skbase-0.4.5/skbase/testing/utils/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/testing/utils/tests/test_deep_equals.py` & `skbase-0.4.5/skbase/testing/utils/tests/test_deep_equals.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/tests/conftest.py` & `skbase-0.4.5/skbase/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/tests/mock_package/test_mock_package.py` & `skbase-0.4.5/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/tests/test_base.py` & `skbase-0.4.5/skbase/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/tests/test_baseestimator.py` & `skbase-0.4.5/skbase/tests/test_baseestimator.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/tests/test_exceptions.py` & `skbase-0.4.5/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/tests/test_meta.py` & `skbase-0.4.5/skbase/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/utils/__init__.py` & `skbase-0.4.5/skbase/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/utils/_check.py` & `skbase-0.4.5/skbase/utils/_check.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/utils/_iter.py` & `skbase-0.4.5/skbase/utils/_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/utils/_nested_iter.py` & `skbase-0.4.5/skbase/utils/_nested_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/utils/_utils.py` & `skbase-0.4.5/skbase/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/utils/deep_equals.py` & `skbase-0.4.5/skbase/utils/deep_equals.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/utils/dependencies/_dependencies.py` & `skbase-0.4.5/skbase/utils/dependencies/_dependencies.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/utils/tests/test_check.py` & `skbase-0.4.5/skbase/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/utils/tests/test_iter.py` & `skbase-0.4.5/skbase/utils/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/utils/tests/test_nested_iter.py` & `skbase-0.4.5/skbase/utils/tests/test_nested_iter.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/utils/tests/test_utils.py` & `skbase-0.4.5/skbase/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/validate/__init__.py` & `skbase-0.4.5/skbase/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/validate/_named_objects.py` & `skbase-0.4.5/skbase/validate/_named_objects.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/validate/_types.py` & `skbase-0.4.5/skbase/validate/_types.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/validate/tests/test_iterable_named_objects.py` & `skbase-0.4.5/skbase/validate/tests/test_iterable_named_objects.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase/validate/tests/test_type_validations.py` & `skbase-0.4.5/skbase/validate/tests/test_type_validations.py`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase.egg-info/PKG-INFO` & `skbase-0.4.5/skbase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skbase
-Version: 0.4.4
+Version: 0.4.5
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
 
-:rocket: Version 0.4.4 is now available. Checkout our
+:rocket: Version 0.4.5 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `skbase-0.4.4/skbase.egg-info/SOURCES.txt` & `skbase-0.4.5/skbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skbase-0.4.4/skbase.egg-info/requires.txt` & `skbase-0.4.5/skbase.egg-info/requires.txt`

 * *Files identical despite different names*

