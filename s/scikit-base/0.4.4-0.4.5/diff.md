# Comparing `tmp/scikit-base-0.4.4.tar.gz` & `tmp/scikit-base-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-base-0.4.4.tar", last modified: Sat May 13 23:45:11 2023, max compression
+gzip compressed data, was "scikit-base-0.4.5.tar", last modified: Sun May 14 14:08:20 2023, max compression
```

## Comparing `scikit-base-0.4.4.tar` & `scikit-base-0.4.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.182057 scikit-base-0.4.4/
--rw-rw-rw-   0        0        0     1554 2022-09-08 21:53:10.000000 scikit-base-0.4.4/LICENSE
--rw-rw-rw-   0        0        0     6614 2023-05-13 23:45:11.182057 scikit-base-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     3322 2023-05-13 23:44:30.000000 scikit-base-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.749352 scikit-base-0.4.4/docs/
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.873777 scikit-base-0.4.4/docs/source/
--rw-rw-rw-   0        0        0    10144 2023-04-18 19:57:18.000000 scikit-base-0.4.4/docs/source/conf.py
--rw-rw-rw-   0        0        0     3468 2023-05-13 23:44:53.000000 scikit-base-0.4.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.909080 scikit-base-0.4.4/scikit_base.egg-info/
--rw-rw-rw-   0        0        0     6614 2023-05-13 23:45:10.000000 scikit-base-0.4.4/scikit_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1937 2023-05-13 23:45:10.000000 scikit-base-0.4.4/scikit_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 23:45:10.000000 scikit-base-0.4.4/scikit_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      517 2023-05-13 23:45:10.000000 scikit-base-0.4.4/scikit_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       51 2023-05-13 23:45:10.000000 scikit-base-0.4.4/scikit_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 19:54:18.000000 scikit-base-0.4.4/scikit_base.egg-info/zip-safe
--rw-rw-rw-   0        0        0      368 2023-05-13 23:45:11.199691 scikit-base-0.4.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.930804 scikit-base-0.4.4/skbase/
--rw-rw-rw-   0        0        0      468 2023-04-25 09:18:44.000000 scikit-base-0.4.4/skbase/__init__.py
--rw-rw-rw-   0        0        0     1144 2022-12-28 00:03:43.000000 scikit-base-0.4.4/skbase/_exceptions.py
--rw-rw-rw-   0        0        0     1112 2023-05-13 18:22:14.000000 scikit-base-0.4.4/skbase/_nopytest_tests.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.939323 scikit-base-0.4.4/skbase/base/
--rw-rw-rw-   0        0        0      649 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/base/__init__.py
--rw-rw-rw-   0        0        0    44796 2023-05-13 18:22:14.000000 scikit-base-0.4.4/skbase/base/_base.py
--rw-rw-rw-   0        0        0    36497 2023-04-26 13:58:57.000000 scikit-base-0.4.4/skbase/base/_meta.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.962327 scikit-base-0.4.4/skbase/base/_pretty_printing/
--rw-rw-rw-   0        0        0      503 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/base/_pretty_printing/__init__.py
--rw-rw-rw-   0        0        0    11931 2023-04-26 13:58:57.000000 scikit-base-0.4.4/skbase/base/_pretty_printing/_object_html_repr.py
--rw-rw-rw-   0        0        0    16046 2023-04-23 21:36:04.000000 scikit-base-0.4.4/skbase/base/_pretty_printing/_pprint.py
--rw-rw-rw-   0        0        0     7507 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/base/_tagmanager.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.969398 scikit-base-0.4.4/skbase/lookup/
--rw-rw-rw-   0        0        0     1120 2022-12-28 00:03:43.000000 scikit-base-0.4.4/skbase/lookup/__init__.py
--rw-rw-rw-   0        0        0    39934 2023-05-11 20:27:18.000000 scikit-base-0.4.4/skbase/lookup/_lookup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.969398 scikit-base-0.4.4/skbase/lookup/tests/
--rw-rw-rw-   0        0        0       70 2022-12-31 19:03:49.000000 scikit-base-0.4.4/skbase/lookup/tests/__init__.py
--rw-rw-rw-   0        0        0    37915 2023-04-26 14:48:09.000000 scikit-base-0.4.4/skbase/lookup/tests/test_lookup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.973905 scikit-base-0.4.4/skbase/testing/
--rw-rw-rw-   0        0        0      363 2022-12-28 00:00:00.000000 scikit-base-0.4.4/skbase/testing/__init__.py
--rw-rw-rw-   0        0        0    37298 2023-05-13 18:22:13.000000 scikit-base-0.4.4/skbase/testing/test_all_objects.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.989033 scikit-base-0.4.4/skbase/testing/utils/
--rw-rw-rw-   0        0        0      118 2022-12-31 19:03:49.000000 scikit-base-0.4.4/skbase/testing/utils/__init__.py
--rw-rw-rw-   0        0        0    10099 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/testing/utils/_conditional_fixtures.py
--rw-rw-rw-   0        0        0      484 2023-05-13 18:22:13.000000 scikit-base-0.4.4/skbase/testing/utils/_dependencies.py
--rw-rw-rw-   0        0        0      350 2023-05-13 23:40:38.000000 scikit-base-0.4.4/skbase/testing/utils/deep_equals.py
--rw-rw-rw-   0        0        0      771 2022-09-08 20:20:18.000000 scikit-base-0.4.4/skbase/testing/utils/inspect.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.999082 scikit-base-0.4.4/skbase/testing/utils/tests/
--rw-rw-rw-   0        0        0       73 2022-09-08 20:20:18.000000 scikit-base-0.4.4/skbase/testing/utils/tests/__init__.py
--rw-rw-rw-   0        0        0     2282 2022-12-30 11:07:07.000000 scikit-base-0.4.4/skbase/testing/utils/tests/test_check_dependencies.py
--rw-rw-rw-   0        0        0     1771 2023-05-13 18:22:13.000000 scikit-base-0.4.4/skbase/testing/utils/tests/test_deep_equals.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.025579 scikit-base-0.4.4/skbase/tests/
--rw-rw-rw-   0        0        0       39 2022-04-29 16:15:46.000000 scikit-base-0.4.4/skbase/tests/__init__.py
--rw-rw-rw-   0        0        0     8671 2023-05-13 23:40:38.000000 scikit-base-0.4.4/skbase/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.029092 scikit-base-0.4.4/skbase/tests/mock_package/
--rw-rw-rw-   0        0        0      140 2022-12-31 19:03:49.000000 scikit-base-0.4.4/skbase/tests/mock_package/__init__.py
--rw-rw-rw-   0        0        0     2095 2022-12-31 19:03:49.000000 scikit-base-0.4.4/skbase/tests/mock_package/test_mock_package.py
--rw-rw-rw-   0        0        0    43013 2023-05-13 18:22:14.000000 scikit-base-0.4.4/skbase/tests/test_base.py
--rw-rw-rw-   0        0        0     4860 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/tests/test_baseestimator.py
--rw-rw-rw-   0        0        0      652 2022-12-31 19:03:49.000000 scikit-base-0.4.4/skbase/tests/test_exceptions.py
--rw-rw-rw-   0        0        0     4567 2023-05-11 20:27:18.000000 scikit-base-0.4.4/skbase/tests/test_meta.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.059126 scikit-base-0.4.4/skbase/utils/
--rw-rw-rw-   0        0        0      654 2023-05-13 23:40:38.000000 scikit-base-0.4.4/skbase/utils/__init__.py
--rw-rw-rw-   0        0        0     1448 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/utils/_check.py
--rw-rw-rw-   0        0        0     8275 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/utils/_iter.py
--rw-rw-rw-   0        0        0     4746 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/utils/_nested_iter.py
--rw-rw-rw-   0        0        0     3225 2023-05-04 17:40:43.000000 scikit-base-0.4.4/skbase/utils/_utils.py
--rw-rw-rw-   0        0        0    11657 2023-05-13 18:22:13.000000 scikit-base-0.4.4/skbase/utils/deep_equals.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.097921 scikit-base-0.4.4/skbase/utils/dependencies/
--rw-rw-rw-   0        0        0      363 2023-05-13 18:22:13.000000 scikit-base-0.4.4/skbase/utils/dependencies/__init__.py
--rw-rw-rw-   0        0        0    10612 2023-05-13 18:22:13.000000 scikit-base-0.4.4/skbase/utils/dependencies/_dependencies.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.110165 scikit-base-0.4.4/skbase/utils/tests/
--rw-rw-rw-   0        0        0      169 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/utils/tests/__init__.py
--rw-rw-rw-   0        0        0      774 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/utils/tests/test_check.py
--rw-rw-rw-   0        0        0     5045 2023-05-04 17:40:43.000000 scikit-base-0.4.4/skbase/utils/tests/test_iter.py
--rw-rw-rw-   0        0        0     2314 2023-05-04 17:40:43.000000 scikit-base-0.4.4/skbase/utils/tests/test_nested_iter.py
--rw-rw-rw-   0        0        0     1219 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/utils/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.124468 scikit-base-0.4.4/skbase/validate/
--rw-rw-rw-   0        0        0      698 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/validate/__init__.py
--rw-rw-rw-   0        0        0    15180 2023-05-11 20:27:18.000000 scikit-base-0.4.4/skbase/validate/_named_objects.py
--rw-rw-rw-   0        0        0    12466 2023-05-11 20:51:59.000000 scikit-base-0.4.4/skbase/validate/_types.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.182057 scikit-base-0.4.4/skbase/validate/tests/
--rw-rw-rw-   0        0        0       72 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/validate/tests/__init__.py
--rw-rw-rw-   0        0        0     7638 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/validate/tests/test_iterable_named_objects.py
--rw-rw-rw-   0        0        0    14501 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/validate/tests/test_type_validations.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.770985 scikit-base-0.4.5/
+-rw-rw-rw-   0        0        0     1554 2022-09-08 21:53:10.000000 scikit-base-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0     6614 2023-05-14 14:08:20.770985 scikit-base-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3322 2023-05-14 13:54:44.000000 scikit-base-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:19.927915 scikit-base-0.4.5/docs/
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.162083 scikit-base-0.4.5/docs/source/
+-rw-rw-rw-   0        0        0    10144 2023-04-18 19:57:18.000000 scikit-base-0.4.5/docs/source/conf.py
+-rw-rw-rw-   0        0        0     3468 2023-05-14 14:07:55.000000 scikit-base-0.4.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.189737 scikit-base-0.4.5/scikit_base.egg-info/
+-rw-rw-rw-   0        0        0     6614 2023-05-14 14:08:19.000000 scikit-base-0.4.5/scikit_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1937 2023-05-14 14:08:19.000000 scikit-base-0.4.5/scikit_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:08:19.000000 scikit-base-0.4.5/scikit_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      517 2023-05-14 14:08:19.000000 scikit-base-0.4.5/scikit_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       51 2023-05-14 14:08:19.000000 scikit-base-0.4.5/scikit_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 19:54:18.000000 scikit-base-0.4.5/scikit_base.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      368 2023-05-14 14:08:20.775527 scikit-base-0.4.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.215207 scikit-base-0.4.5/skbase/
+-rw-rw-rw-   0        0        0      468 2023-04-25 09:18:44.000000 scikit-base-0.4.5/skbase/__init__.py
+-rw-rw-rw-   0        0        0     1144 2022-12-28 00:03:43.000000 scikit-base-0.4.5/skbase/_exceptions.py
+-rw-rw-rw-   0        0        0     1112 2023-05-13 18:22:14.000000 scikit-base-0.4.5/skbase/_nopytest_tests.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.230969 scikit-base-0.4.5/skbase/base/
+-rw-rw-rw-   0        0        0      649 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/base/__init__.py
+-rw-rw-rw-   0        0        0    44796 2023-05-13 18:22:14.000000 scikit-base-0.4.5/skbase/base/_base.py
+-rw-rw-rw-   0        0        0    36497 2023-04-26 13:58:57.000000 scikit-base-0.4.5/skbase/base/_meta.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.283991 scikit-base-0.4.5/skbase/base/_pretty_printing/
+-rw-rw-rw-   0        0        0      503 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/base/_pretty_printing/__init__.py
+-rw-rw-rw-   0        0        0    11931 2023-04-26 13:58:57.000000 scikit-base-0.4.5/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-rw-rw-   0        0        0    16046 2023-04-23 21:36:04.000000 scikit-base-0.4.5/skbase/base/_pretty_printing/_pprint.py
+-rw-rw-rw-   0        0        0     7507 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/base/_tagmanager.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.308561 scikit-base-0.4.5/skbase/lookup/
+-rw-rw-rw-   0        0        0     1120 2022-12-28 00:03:43.000000 scikit-base-0.4.5/skbase/lookup/__init__.py
+-rw-rw-rw-   0        0        0    39934 2023-05-11 20:27:18.000000 scikit-base-0.4.5/skbase/lookup/_lookup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.365675 scikit-base-0.4.5/skbase/lookup/tests/
+-rw-rw-rw-   0        0        0       70 2022-12-31 19:03:49.000000 scikit-base-0.4.5/skbase/lookup/tests/__init__.py
+-rw-rw-rw-   0        0        0    37915 2023-04-26 14:48:09.000000 scikit-base-0.4.5/skbase/lookup/tests/test_lookup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.386607 scikit-base-0.4.5/skbase/testing/
+-rw-rw-rw-   0        0        0      363 2022-12-28 00:00:00.000000 scikit-base-0.4.5/skbase/testing/__init__.py
+-rw-rw-rw-   0        0        0    37298 2023-05-13 18:22:13.000000 scikit-base-0.4.5/skbase/testing/test_all_objects.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.441619 scikit-base-0.4.5/skbase/testing/utils/
+-rw-rw-rw-   0        0        0      118 2022-12-31 19:03:49.000000 scikit-base-0.4.5/skbase/testing/utils/__init__.py
+-rw-rw-rw-   0        0        0    10099 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/testing/utils/_conditional_fixtures.py
+-rw-rw-rw-   0        0        0      484 2023-05-13 18:22:13.000000 scikit-base-0.4.5/skbase/testing/utils/_dependencies.py
+-rw-rw-rw-   0        0        0      350 2023-05-13 23:40:38.000000 scikit-base-0.4.5/skbase/testing/utils/deep_equals.py
+-rw-rw-rw-   0        0        0      771 2022-09-08 20:20:18.000000 scikit-base-0.4.5/skbase/testing/utils/inspect.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.462284 scikit-base-0.4.5/skbase/testing/utils/tests/
+-rw-rw-rw-   0        0        0       73 2022-09-08 20:20:18.000000 scikit-base-0.4.5/skbase/testing/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0     2282 2022-12-30 11:07:07.000000 scikit-base-0.4.5/skbase/testing/utils/tests/test_check_dependencies.py
+-rw-rw-rw-   0        0        0     1771 2023-05-13 18:22:13.000000 scikit-base-0.4.5/skbase/testing/utils/tests/test_deep_equals.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.521731 scikit-base-0.4.5/skbase/tests/
+-rw-rw-rw-   0        0        0       39 2022-04-29 16:15:46.000000 scikit-base-0.4.5/skbase/tests/__init__.py
+-rw-rw-rw-   0        0        0     8671 2023-05-13 23:40:38.000000 scikit-base-0.4.5/skbase/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.549208 scikit-base-0.4.5/skbase/tests/mock_package/
+-rw-rw-rw-   0        0        0      140 2022-12-31 19:03:49.000000 scikit-base-0.4.5/skbase/tests/mock_package/__init__.py
+-rw-rw-rw-   0        0        0     2095 2022-12-31 19:03:49.000000 scikit-base-0.4.5/skbase/tests/mock_package/test_mock_package.py
+-rw-rw-rw-   0        0        0    43013 2023-05-13 18:22:14.000000 scikit-base-0.4.5/skbase/tests/test_base.py
+-rw-rw-rw-   0        0        0     4860 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/tests/test_baseestimator.py
+-rw-rw-rw-   0        0        0      652 2022-12-31 19:03:49.000000 scikit-base-0.4.5/skbase/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0     4567 2023-05-11 20:27:18.000000 scikit-base-0.4.5/skbase/tests/test_meta.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.597140 scikit-base-0.4.5/skbase/utils/
+-rw-rw-rw-   0        0        0      654 2023-05-13 23:40:38.000000 scikit-base-0.4.5/skbase/utils/__init__.py
+-rw-rw-rw-   0        0        0     1448 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/utils/_check.py
+-rw-rw-rw-   0        0        0     8275 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/utils/_iter.py
+-rw-rw-rw-   0        0        0     4746 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/utils/_nested_iter.py
+-rw-rw-rw-   0        0        0     3225 2023-05-04 17:40:43.000000 scikit-base-0.4.5/skbase/utils/_utils.py
+-rw-rw-rw-   0        0        0    11657 2023-05-13 18:22:13.000000 scikit-base-0.4.5/skbase/utils/deep_equals.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.628352 scikit-base-0.4.5/skbase/utils/dependencies/
+-rw-rw-rw-   0        0        0      363 2023-05-13 18:22:13.000000 scikit-base-0.4.5/skbase/utils/dependencies/__init__.py
+-rw-rw-rw-   0        0        0    10612 2023-05-13 18:22:13.000000 scikit-base-0.4.5/skbase/utils/dependencies/_dependencies.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.707152 scikit-base-0.4.5/skbase/utils/tests/
+-rw-rw-rw-   0        0        0      169 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0      774 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/utils/tests/test_check.py
+-rw-rw-rw-   0        0        0     5045 2023-05-04 17:40:43.000000 scikit-base-0.4.5/skbase/utils/tests/test_iter.py
+-rw-rw-rw-   0        0        0     2314 2023-05-04 17:40:43.000000 scikit-base-0.4.5/skbase/utils/tests/test_nested_iter.py
+-rw-rw-rw-   0        0        0     1219 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/utils/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.743759 scikit-base-0.4.5/skbase/validate/
+-rw-rw-rw-   0        0        0      698 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/validate/__init__.py
+-rw-rw-rw-   0        0        0    15180 2023-05-11 20:27:18.000000 scikit-base-0.4.5/skbase/validate/_named_objects.py
+-rw-rw-rw-   0        0        0    12466 2023-05-11 20:51:59.000000 scikit-base-0.4.5/skbase/validate/_types.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:08:20.769985 scikit-base-0.4.5/skbase/validate/tests/
+-rw-rw-rw-   0        0        0       72 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/validate/tests/__init__.py
+-rw-rw-rw-   0        0        0     7638 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/validate/tests/test_iterable_named_objects.py
+-rw-rw-rw-   0        0        0    14501 2023-04-18 19:57:18.000000 scikit-base-0.4.5/skbase/validate/tests/test_type_validations.py
```

### Comparing `scikit-base-0.4.4/LICENSE` & `scikit-base-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/PKG-INFO` & `scikit-base-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
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
 
-:rocket: Version 0.4.3 is now available. Checkout our
+:rocket: Version 0.4.5 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `scikit-base-0.4.4/README.md` & `scikit-base-0.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 > A base class for scikit-learn-like and sktime-like parametric objects
 
 `skbase` provides base classes for creating scikit-learn-like parametric objects,
 along with tools to make it easier to build your own packages that follow these
 design patterns.
 
-:rocket: Version 0.4.3 is now available. Checkout our
+:rocket: Version 0.4.5 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `scikit-base-0.4.4/docs/source/conf.py` & `scikit-base-0.4.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/pyproject.toml` & `scikit-base-0.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scikit-base"
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

### Comparing `scikit-base-0.4.4/scikit_base.egg-info/PKG-INFO` & `scikit-base-0.4.5/scikit_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
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
 
-:rocket: Version 0.4.3 is now available. Checkout our
+:rocket: Version 0.4.5 is now available. Checkout our
 [release notes](https://skbase.readthedocs.io/en/latest/changelog.html).
 
 | Overview | |
 |---|---|
 | **CI/CD** | [![Tests](https://github.com/sktime/skbase/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/sktime/skbase/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/sktime/skbase/branch/main/graph/badge.svg?token=2J424NLO82)](https://codecov.io/gh/sktime/skbase) [![Documentation Status](https://readthedocs.org/projects/skbase/badge/?version=latest)](https://skbase.readthedocs.io/en/latest/?badge=latest) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sktime/skbase/main.svg)](https://results.pre-commit.ci/latest/github/sktime/skbase/main) |
 | **Code** |  [![!pypi](https://img.shields.io/pypi/v/scikit-base?color=orange)](https://pypi.org/project/skbase/)  [![!python-versions](https://img.shields.io/pypi/pyversions/scikit-base)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit) |
 | **Downloads**| [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=week&units=international_system&left_color=grey&right_color=blue&left_text=weekly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20(pypi))](https://pepy.tech/project/scikit-base) [![Downloads](https://static.pepy.tech/personalized-badge/scikit-base?period=total&units=international_system&left_color=grey&right_color=blue&left_text=cumulative%20(pypi))](https://pepy.tech/project/scikit-base) |
```

### Comparing `scikit-base-0.4.4/scikit_base.egg-info/SOURCES.txt` & `scikit-base-0.4.5/scikit_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/scikit_base.egg-info/requires.txt` & `scikit-base-0.4.5/scikit_base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/_exceptions.py` & `scikit-base-0.4.5/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/_nopytest_tests.py` & `scikit-base-0.4.5/skbase/_nopytest_tests.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/base/__init__.py` & `scikit-base-0.4.5/skbase/base/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/base/_base.py` & `scikit-base-0.4.5/skbase/base/_base.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/base/_meta.py` & `scikit-base-0.4.5/skbase/base/_meta.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/base/_pretty_printing/_object_html_repr.py` & `scikit-base-0.4.5/skbase/base/_pretty_printing/_object_html_repr.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/base/_pretty_printing/_pprint.py` & `scikit-base-0.4.5/skbase/base/_pretty_printing/_pprint.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/base/_tagmanager.py` & `scikit-base-0.4.5/skbase/base/_tagmanager.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/lookup/__init__.py` & `scikit-base-0.4.5/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/lookup/_lookup.py` & `scikit-base-0.4.5/skbase/lookup/_lookup.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/lookup/tests/test_lookup.py` & `scikit-base-0.4.5/skbase/lookup/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/testing/test_all_objects.py` & `scikit-base-0.4.5/skbase/testing/test_all_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/testing/utils/_conditional_fixtures.py` & `scikit-base-0.4.5/skbase/testing/utils/_conditional_fixtures.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/testing/utils/inspect.py` & `scikit-base-0.4.5/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/testing/utils/tests/test_check_dependencies.py` & `scikit-base-0.4.5/skbase/testing/utils/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/testing/utils/tests/test_deep_equals.py` & `scikit-base-0.4.5/skbase/testing/utils/tests/test_deep_equals.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/tests/conftest.py` & `scikit-base-0.4.5/skbase/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/tests/mock_package/test_mock_package.py` & `scikit-base-0.4.5/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/tests/test_base.py` & `scikit-base-0.4.5/skbase/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/tests/test_baseestimator.py` & `scikit-base-0.4.5/skbase/tests/test_baseestimator.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/tests/test_exceptions.py` & `scikit-base-0.4.5/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/tests/test_meta.py` & `scikit-base-0.4.5/skbase/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/utils/__init__.py` & `scikit-base-0.4.5/skbase/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/utils/_check.py` & `scikit-base-0.4.5/skbase/utils/_check.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/utils/_iter.py` & `scikit-base-0.4.5/skbase/utils/_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/utils/_nested_iter.py` & `scikit-base-0.4.5/skbase/utils/_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/utils/_utils.py` & `scikit-base-0.4.5/skbase/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/utils/deep_equals.py` & `scikit-base-0.4.5/skbase/utils/deep_equals.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/utils/dependencies/_dependencies.py` & `scikit-base-0.4.5/skbase/utils/dependencies/_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/utils/tests/test_check.py` & `scikit-base-0.4.5/skbase/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/utils/tests/test_iter.py` & `scikit-base-0.4.5/skbase/utils/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/utils/tests/test_nested_iter.py` & `scikit-base-0.4.5/skbase/utils/tests/test_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/utils/tests/test_utils.py` & `scikit-base-0.4.5/skbase/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/validate/__init__.py` & `scikit-base-0.4.5/skbase/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/validate/_named_objects.py` & `scikit-base-0.4.5/skbase/validate/_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/validate/_types.py` & `scikit-base-0.4.5/skbase/validate/_types.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/validate/tests/test_iterable_named_objects.py` & `scikit-base-0.4.5/skbase/validate/tests/test_iterable_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.4/skbase/validate/tests/test_type_validations.py` & `scikit-base-0.4.5/skbase/validate/tests/test_type_validations.py`

 * *Files identical despite different names*

