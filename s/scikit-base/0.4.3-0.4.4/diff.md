# Comparing `tmp/scikit-base-0.4.3.tar.gz` & `tmp/scikit-base-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-base-0.4.3.tar", last modified: Fri May  5 00:38:57 2023, max compression
+gzip compressed data, was "scikit-base-0.4.4.tar", last modified: Sat May 13 23:45:11 2023, max compression
```

## Comparing `scikit-base-0.4.3.tar` & `scikit-base-0.4.4.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.679311 scikit-base-0.4.3/
--rw-rw-rw-   0        0        0     1554 2022-09-08 21:53:10.000000 scikit-base-0.4.3/LICENSE
--rw-rw-rw-   0        0        0     6614 2023-05-05 00:38:57.680364 scikit-base-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     3322 2023-05-05 00:37:15.000000 scikit-base-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:56.371288 scikit-base-0.4.3/docs/
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:56.753497 scikit-base-0.4.3/docs/source/
--rw-rw-rw-   0        0        0    10144 2023-04-18 19:57:18.000000 scikit-base-0.4.3/docs/source/conf.py
--rw-rw-rw-   0        0        0     3468 2023-05-05 00:38:42.000000 scikit-base-0.4.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:56.851061 scikit-base-0.4.3/scikit_base.egg-info/
--rw-rw-rw-   0        0        0     6614 2023-05-05 00:38:56.000000 scikit-base-0.4.3/scikit_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1828 2023-05-05 00:38:56.000000 scikit-base-0.4.3/scikit_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 00:38:56.000000 scikit-base-0.4.3/scikit_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      517 2023-05-05 00:38:56.000000 scikit-base-0.4.3/scikit_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       51 2023-05-05 00:38:56.000000 scikit-base-0.4.3/scikit_base.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 19:54:18.000000 scikit-base-0.4.3/scikit_base.egg-info/zip-safe
--rw-rw-rw-   0        0        0      368 2023-05-05 00:38:57.707373 scikit-base-0.4.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:56.878875 scikit-base-0.4.3/skbase/
--rw-rw-rw-   0        0        0      468 2023-04-25 09:18:44.000000 scikit-base-0.4.3/skbase/__init__.py
--rw-rw-rw-   0        0        0     1144 2022-12-28 00:03:43.000000 scikit-base-0.4.3/skbase/_exceptions.py
--rw-rw-rw-   0        0        0      989 2023-05-05 00:37:09.000000 scikit-base-0.4.3/skbase/_nopytest_tests.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:56.941985 scikit-base-0.4.3/skbase/base/
--rw-rw-rw-   0        0        0      649 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/base/__init__.py
--rw-rw-rw-   0        0        0    44812 2023-05-04 22:01:38.000000 scikit-base-0.4.3/skbase/base/_base.py
--rw-rw-rw-   0        0        0    36497 2023-04-26 13:58:57.000000 scikit-base-0.4.3/skbase/base/_meta.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:56.991531 scikit-base-0.4.3/skbase/base/_pretty_printing/
--rw-rw-rw-   0        0        0      503 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/base/_pretty_printing/__init__.py
--rw-rw-rw-   0        0        0    11931 2023-04-26 13:58:57.000000 scikit-base-0.4.3/skbase/base/_pretty_printing/_object_html_repr.py
--rw-rw-rw-   0        0        0    16046 2023-04-23 21:36:04.000000 scikit-base-0.4.3/skbase/base/_pretty_printing/_pprint.py
--rw-rw-rw-   0        0        0     7507 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/base/_tagmanager.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.021323 scikit-base-0.4.3/skbase/lookup/
--rw-rw-rw-   0        0        0     1120 2022-12-28 00:03:43.000000 scikit-base-0.4.3/skbase/lookup/__init__.py
--rw-rw-rw-   0        0        0    39934 2023-05-01 22:18:40.000000 scikit-base-0.4.3/skbase/lookup/_lookup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.058675 scikit-base-0.4.3/skbase/lookup/tests/
--rw-rw-rw-   0        0        0       70 2022-12-31 19:03:49.000000 scikit-base-0.4.3/skbase/lookup/tests/__init__.py
--rw-rw-rw-   0        0        0    37915 2023-04-26 14:48:09.000000 scikit-base-0.4.3/skbase/lookup/tests/test_lookup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.088424 scikit-base-0.4.3/skbase/testing/
--rw-rw-rw-   0        0        0      363 2022-12-28 00:00:00.000000 scikit-base-0.4.3/skbase/testing/__init__.py
--rw-rw-rw-   0        0        0    37306 2023-05-04 22:01:38.000000 scikit-base-0.4.3/skbase/testing/test_all_objects.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.201146 scikit-base-0.4.3/skbase/testing/utils/
--rw-rw-rw-   0        0        0      118 2022-12-31 19:03:49.000000 scikit-base-0.4.3/skbase/testing/utils/__init__.py
--rw-rw-rw-   0        0        0    10099 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/testing/utils/_conditional_fixtures.py
--rw-rw-rw-   0        0        0    10612 2023-05-04 22:01:38.000000 scikit-base-0.4.3/skbase/testing/utils/_dependencies.py
--rw-rw-rw-   0        0        0    11410 2023-05-04 22:01:38.000000 scikit-base-0.4.3/skbase/testing/utils/deep_equals.py
--rw-rw-rw-   0        0        0      771 2022-09-08 20:20:18.000000 scikit-base-0.4.3/skbase/testing/utils/inspect.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.261374 scikit-base-0.4.3/skbase/testing/utils/tests/
--rw-rw-rw-   0        0        0       73 2022-09-08 20:20:18.000000 scikit-base-0.4.3/skbase/testing/utils/tests/__init__.py
--rw-rw-rw-   0        0        0     2282 2022-12-30 11:07:07.000000 scikit-base-0.4.3/skbase/testing/utils/tests/test_check_dependencies.py
--rw-rw-rw-   0        0        0     1779 2023-05-04 22:01:38.000000 scikit-base-0.4.3/skbase/testing/utils/tests/test_deep_equals.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.373755 scikit-base-0.4.3/skbase/tests/
--rw-rw-rw-   0        0        0       39 2022-04-29 16:15:46.000000 scikit-base-0.4.3/skbase/tests/__init__.py
--rw-rw-rw-   0        0        0     8048 2023-05-05 00:37:09.000000 scikit-base-0.4.3/skbase/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.406154 scikit-base-0.4.3/skbase/tests/mock_package/
--rw-rw-rw-   0        0        0      140 2022-12-31 19:03:49.000000 scikit-base-0.4.3/skbase/tests/mock_package/__init__.py
--rw-rw-rw-   0        0        0     2095 2022-12-31 19:03:49.000000 scikit-base-0.4.3/skbase/tests/mock_package/test_mock_package.py
--rw-rw-rw-   0        0        0    43013 2023-05-04 22:01:38.000000 scikit-base-0.4.3/skbase/tests/test_base.py
--rw-rw-rw-   0        0        0     4860 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/tests/test_baseestimator.py
--rw-rw-rw-   0        0        0      652 2022-12-31 19:03:49.000000 scikit-base-0.4.3/skbase/tests/test_exceptions.py
--rw-rw-rw-   0        0        0     4567 2023-05-02 00:24:16.000000 scikit-base-0.4.3/skbase/tests/test_meta.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.487029 scikit-base-0.4.3/skbase/utils/
--rw-rw-rw-   0        0        0      584 2023-05-04 16:33:39.000000 scikit-base-0.4.3/skbase/utils/__init__.py
--rw-rw-rw-   0        0        0     1448 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/utils/_check.py
--rw-rw-rw-   0        0        0     8275 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/utils/_iter.py
--rw-rw-rw-   0        0        0     4746 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/utils/_nested_iter.py
--rw-rw-rw-   0        0        0     3225 2023-05-04 17:40:43.000000 scikit-base-0.4.3/skbase/utils/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.588296 scikit-base-0.4.3/skbase/utils/tests/
--rw-rw-rw-   0        0        0      169 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/utils/tests/__init__.py
--rw-rw-rw-   0        0        0      774 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/utils/tests/test_check.py
--rw-rw-rw-   0        0        0     5045 2023-05-04 17:40:43.000000 scikit-base-0.4.3/skbase/utils/tests/test_iter.py
--rw-rw-rw-   0        0        0     2314 2023-05-04 17:40:43.000000 scikit-base-0.4.3/skbase/utils/tests/test_nested_iter.py
--rw-rw-rw-   0        0        0     1219 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/utils/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.624895 scikit-base-0.4.3/skbase/validate/
--rw-rw-rw-   0        0        0      698 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/validate/__init__.py
--rw-rw-rw-   0        0        0    15180 2023-05-01 22:18:40.000000 scikit-base-0.4.3/skbase/validate/_named_objects.py
--rw-rw-rw-   0        0        0    12466 2023-05-02 20:58:49.000000 scikit-base-0.4.3/skbase/validate/_types.py
-drwxrwxrwx   0        0        0        0 2023-05-05 00:38:57.678275 scikit-base-0.4.3/skbase/validate/tests/
--rw-rw-rw-   0        0        0       72 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/validate/tests/__init__.py
--rw-rw-rw-   0        0        0     7638 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/validate/tests/test_iterable_named_objects.py
--rw-rw-rw-   0        0        0    14501 2023-04-18 19:57:18.000000 scikit-base-0.4.3/skbase/validate/tests/test_type_validations.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.182057 scikit-base-0.4.4/
+-rw-rw-rw-   0        0        0     1554 2022-09-08 21:53:10.000000 scikit-base-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0     6614 2023-05-13 23:45:11.182057 scikit-base-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3322 2023-05-13 23:44:30.000000 scikit-base-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.749352 scikit-base-0.4.4/docs/
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.873777 scikit-base-0.4.4/docs/source/
+-rw-rw-rw-   0        0        0    10144 2023-04-18 19:57:18.000000 scikit-base-0.4.4/docs/source/conf.py
+-rw-rw-rw-   0        0        0     3468 2023-05-13 23:44:53.000000 scikit-base-0.4.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.909080 scikit-base-0.4.4/scikit_base.egg-info/
+-rw-rw-rw-   0        0        0     6614 2023-05-13 23:45:10.000000 scikit-base-0.4.4/scikit_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1937 2023-05-13 23:45:10.000000 scikit-base-0.4.4/scikit_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-13 23:45:10.000000 scikit-base-0.4.4/scikit_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      517 2023-05-13 23:45:10.000000 scikit-base-0.4.4/scikit_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       51 2023-05-13 23:45:10.000000 scikit-base-0.4.4/scikit_base.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 19:54:18.000000 scikit-base-0.4.4/scikit_base.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      368 2023-05-13 23:45:11.199691 scikit-base-0.4.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.930804 scikit-base-0.4.4/skbase/
+-rw-rw-rw-   0        0        0      468 2023-04-25 09:18:44.000000 scikit-base-0.4.4/skbase/__init__.py
+-rw-rw-rw-   0        0        0     1144 2022-12-28 00:03:43.000000 scikit-base-0.4.4/skbase/_exceptions.py
+-rw-rw-rw-   0        0        0     1112 2023-05-13 18:22:14.000000 scikit-base-0.4.4/skbase/_nopytest_tests.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.939323 scikit-base-0.4.4/skbase/base/
+-rw-rw-rw-   0        0        0      649 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/base/__init__.py
+-rw-rw-rw-   0        0        0    44796 2023-05-13 18:22:14.000000 scikit-base-0.4.4/skbase/base/_base.py
+-rw-rw-rw-   0        0        0    36497 2023-04-26 13:58:57.000000 scikit-base-0.4.4/skbase/base/_meta.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.962327 scikit-base-0.4.4/skbase/base/_pretty_printing/
+-rw-rw-rw-   0        0        0      503 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/base/_pretty_printing/__init__.py
+-rw-rw-rw-   0        0        0    11931 2023-04-26 13:58:57.000000 scikit-base-0.4.4/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-rw-rw-   0        0        0    16046 2023-04-23 21:36:04.000000 scikit-base-0.4.4/skbase/base/_pretty_printing/_pprint.py
+-rw-rw-rw-   0        0        0     7507 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/base/_tagmanager.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.969398 scikit-base-0.4.4/skbase/lookup/
+-rw-rw-rw-   0        0        0     1120 2022-12-28 00:03:43.000000 scikit-base-0.4.4/skbase/lookup/__init__.py
+-rw-rw-rw-   0        0        0    39934 2023-05-11 20:27:18.000000 scikit-base-0.4.4/skbase/lookup/_lookup.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.969398 scikit-base-0.4.4/skbase/lookup/tests/
+-rw-rw-rw-   0        0        0       70 2022-12-31 19:03:49.000000 scikit-base-0.4.4/skbase/lookup/tests/__init__.py
+-rw-rw-rw-   0        0        0    37915 2023-04-26 14:48:09.000000 scikit-base-0.4.4/skbase/lookup/tests/test_lookup.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.973905 scikit-base-0.4.4/skbase/testing/
+-rw-rw-rw-   0        0        0      363 2022-12-28 00:00:00.000000 scikit-base-0.4.4/skbase/testing/__init__.py
+-rw-rw-rw-   0        0        0    37298 2023-05-13 18:22:13.000000 scikit-base-0.4.4/skbase/testing/test_all_objects.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.989033 scikit-base-0.4.4/skbase/testing/utils/
+-rw-rw-rw-   0        0        0      118 2022-12-31 19:03:49.000000 scikit-base-0.4.4/skbase/testing/utils/__init__.py
+-rw-rw-rw-   0        0        0    10099 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/testing/utils/_conditional_fixtures.py
+-rw-rw-rw-   0        0        0      484 2023-05-13 18:22:13.000000 scikit-base-0.4.4/skbase/testing/utils/_dependencies.py
+-rw-rw-rw-   0        0        0      350 2023-05-13 23:40:38.000000 scikit-base-0.4.4/skbase/testing/utils/deep_equals.py
+-rw-rw-rw-   0        0        0      771 2022-09-08 20:20:18.000000 scikit-base-0.4.4/skbase/testing/utils/inspect.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:10.999082 scikit-base-0.4.4/skbase/testing/utils/tests/
+-rw-rw-rw-   0        0        0       73 2022-09-08 20:20:18.000000 scikit-base-0.4.4/skbase/testing/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0     2282 2022-12-30 11:07:07.000000 scikit-base-0.4.4/skbase/testing/utils/tests/test_check_dependencies.py
+-rw-rw-rw-   0        0        0     1771 2023-05-13 18:22:13.000000 scikit-base-0.4.4/skbase/testing/utils/tests/test_deep_equals.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.025579 scikit-base-0.4.4/skbase/tests/
+-rw-rw-rw-   0        0        0       39 2022-04-29 16:15:46.000000 scikit-base-0.4.4/skbase/tests/__init__.py
+-rw-rw-rw-   0        0        0     8671 2023-05-13 23:40:38.000000 scikit-base-0.4.4/skbase/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.029092 scikit-base-0.4.4/skbase/tests/mock_package/
+-rw-rw-rw-   0        0        0      140 2022-12-31 19:03:49.000000 scikit-base-0.4.4/skbase/tests/mock_package/__init__.py
+-rw-rw-rw-   0        0        0     2095 2022-12-31 19:03:49.000000 scikit-base-0.4.4/skbase/tests/mock_package/test_mock_package.py
+-rw-rw-rw-   0        0        0    43013 2023-05-13 18:22:14.000000 scikit-base-0.4.4/skbase/tests/test_base.py
+-rw-rw-rw-   0        0        0     4860 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/tests/test_baseestimator.py
+-rw-rw-rw-   0        0        0      652 2022-12-31 19:03:49.000000 scikit-base-0.4.4/skbase/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0     4567 2023-05-11 20:27:18.000000 scikit-base-0.4.4/skbase/tests/test_meta.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.059126 scikit-base-0.4.4/skbase/utils/
+-rw-rw-rw-   0        0        0      654 2023-05-13 23:40:38.000000 scikit-base-0.4.4/skbase/utils/__init__.py
+-rw-rw-rw-   0        0        0     1448 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/utils/_check.py
+-rw-rw-rw-   0        0        0     8275 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/utils/_iter.py
+-rw-rw-rw-   0        0        0     4746 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/utils/_nested_iter.py
+-rw-rw-rw-   0        0        0     3225 2023-05-04 17:40:43.000000 scikit-base-0.4.4/skbase/utils/_utils.py
+-rw-rw-rw-   0        0        0    11657 2023-05-13 18:22:13.000000 scikit-base-0.4.4/skbase/utils/deep_equals.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.097921 scikit-base-0.4.4/skbase/utils/dependencies/
+-rw-rw-rw-   0        0        0      363 2023-05-13 18:22:13.000000 scikit-base-0.4.4/skbase/utils/dependencies/__init__.py
+-rw-rw-rw-   0        0        0    10612 2023-05-13 18:22:13.000000 scikit-base-0.4.4/skbase/utils/dependencies/_dependencies.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.110165 scikit-base-0.4.4/skbase/utils/tests/
+-rw-rw-rw-   0        0        0      169 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0      774 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/utils/tests/test_check.py
+-rw-rw-rw-   0        0        0     5045 2023-05-04 17:40:43.000000 scikit-base-0.4.4/skbase/utils/tests/test_iter.py
+-rw-rw-rw-   0        0        0     2314 2023-05-04 17:40:43.000000 scikit-base-0.4.4/skbase/utils/tests/test_nested_iter.py
+-rw-rw-rw-   0        0        0     1219 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/utils/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.124468 scikit-base-0.4.4/skbase/validate/
+-rw-rw-rw-   0        0        0      698 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/validate/__init__.py
+-rw-rw-rw-   0        0        0    15180 2023-05-11 20:27:18.000000 scikit-base-0.4.4/skbase/validate/_named_objects.py
+-rw-rw-rw-   0        0        0    12466 2023-05-11 20:51:59.000000 scikit-base-0.4.4/skbase/validate/_types.py
+drwxrwxrwx   0        0        0        0 2023-05-13 23:45:11.182057 scikit-base-0.4.4/skbase/validate/tests/
+-rw-rw-rw-   0        0        0       72 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/validate/tests/__init__.py
+-rw-rw-rw-   0        0        0     7638 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/validate/tests/test_iterable_named_objects.py
+-rw-rw-rw-   0        0        0    14501 2023-04-18 19:57:18.000000 scikit-base-0.4.4/skbase/validate/tests/test_type_validations.py
```

### Comparing `scikit-base-0.4.3/LICENSE` & `scikit-base-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/PKG-INFO` & `scikit-base-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
-Version: 0.4.3
+Version: 0.4.4
 Summary: Base classes for sklearn-like parametric objects
 Author: Franz Király, Markus Löning, Ryan Kuhns
 Maintainer-email: Franz Kiraly <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
         All rights reserved.
```

### Comparing `scikit-base-0.4.3/README.md` & `scikit-base-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/docs/source/conf.py` & `scikit-base-0.4.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/pyproject.toml` & `scikit-base-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scikit-base"
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

### Comparing `scikit-base-0.4.3/scikit_base.egg-info/PKG-INFO` & `scikit-base-0.4.4/scikit_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-base
-Version: 0.4.3
+Version: 0.4.4
 Summary: Base classes for sklearn-like parametric objects
 Author: Franz Király, Markus Löning, Ryan Kuhns
 Maintainer-email: Franz Kiraly <f.kiraly@ucl.ac.uk>, Ryan Kuhns <rk.skbase@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, skbase Developers
         All rights reserved.
```

### Comparing `scikit-base-0.4.3/scikit_base.egg-info/SOURCES.txt` & `scikit-base-0.4.4/scikit_base.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

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

### Comparing `scikit-base-0.4.3/scikit_base.egg-info/requires.txt` & `scikit-base-0.4.4/scikit_base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/_exceptions.py` & `scikit-base-0.4.4/skbase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/_nopytest_tests.py` & `scikit-base-0.4.4/skbase/_nopytest_tests.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 
 # all_objectscrawls all modules excepting pytest test files
 # if it encounters an unisolated import, it will throw an exception
 results = all_objects(modules_to_ignore=MODULES_TO_IGNORE)
 
 # try to run all methods of BaseObject without arguments
 # very basic test, but needs to run without pytest
-METHODS = [
-    "clone",
-    "get_params",
-    "reset",
-    "get_param_names",
-    "get_param_defaults",
-    "get_params",
-    "get_class_tags",
-    "get_tags",
-    "get_config",
-    "get_test_params",
-    "create_test_instance",
-    "create_test_instances_and_names",
-    "is_composite",
-]
+METHODS = {
+    "clone": {},
+    "get_params": {},
+    "reset": {},
+    "get_param_names": {},
+    "get_param_defaults": {},
+    "get_class_tags": {},
+    "get_tags": {},
+    "get_config": {},
+    "get_test_params": {},
+    "create_test_instance": {},
+    "create_test_instances_and_names": {},
+    "is_composite": {},
+    "set_tags": {"foo": "bar"},
+    "set_config": {"bar": "foo"},
+}
 
 mybo = BaseObject()
-for method in METHODS:
-    getattr(mybo, method)
+for method, params in METHODS.items():
+    getattr(mybo, method)(**params)
```

### Comparing `scikit-base-0.4.3/skbase/base/__init__.py` & `scikit-base-0.4.4/skbase/base/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/base/_base.py` & `scikit-base-0.4.4/skbase/base/_base.py`

 * *Files 1% similar despite different names*

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

### Comparing `scikit-base-0.4.3/skbase/base/_meta.py` & `scikit-base-0.4.4/skbase/base/_meta.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/base/_pretty_printing/_object_html_repr.py` & `scikit-base-0.4.4/skbase/base/_pretty_printing/_object_html_repr.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/base/_pretty_printing/_pprint.py` & `scikit-base-0.4.4/skbase/base/_pretty_printing/_pprint.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/base/_tagmanager.py` & `scikit-base-0.4.4/skbase/base/_tagmanager.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/lookup/__init__.py` & `scikit-base-0.4.4/skbase/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/lookup/_lookup.py` & `scikit-base-0.4.4/skbase/lookup/_lookup.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/lookup/tests/test_lookup.py` & `scikit-base-0.4.4/skbase/lookup/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/testing/test_all_objects.py` & `scikit-base-0.4.4/skbase/testing/test_all_objects.py`

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

### Comparing `scikit-base-0.4.3/skbase/testing/utils/_conditional_fixtures.py` & `scikit-base-0.4.4/skbase/testing/utils/_conditional_fixtures.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/testing/utils/_dependencies.py` & `scikit-base-0.4.4/skbase/utils/dependencies/_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/testing/utils/deep_equals.py` & `scikit-base-0.4.4/skbase/utils/deep_equals.py`

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

### Comparing `scikit-base-0.4.3/skbase/testing/utils/inspect.py` & `scikit-base-0.4.4/skbase/testing/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/testing/utils/tests/test_check_dependencies.py` & `scikit-base-0.4.4/skbase/testing/utils/tests/test_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/testing/utils/tests/test_deep_equals.py` & `scikit-base-0.4.4/skbase/testing/utils/tests/test_deep_equals.py`

 * *Files 1% similar despite different names*

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

### Comparing `scikit-base-0.4.3/skbase/tests/conftest.py` & `scikit-base-0.4.4/skbase/tests/conftest.py`

 * *Files 6% similar despite different names*

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

### Comparing `scikit-base-0.4.3/skbase/tests/mock_package/test_mock_package.py` & `scikit-base-0.4.4/skbase/tests/mock_package/test_mock_package.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/tests/test_base.py` & `scikit-base-0.4.4/skbase/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/tests/test_baseestimator.py` & `scikit-base-0.4.4/skbase/tests/test_baseestimator.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/tests/test_exceptions.py` & `scikit-base-0.4.4/skbase/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/tests/test_meta.py` & `scikit-base-0.4.4/skbase/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/utils/__init__.py` & `scikit-base-0.4.4/skbase/utils/__init__.py`

 * *Files 11% similar despite different names*

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

### Comparing `scikit-base-0.4.3/skbase/utils/_check.py` & `scikit-base-0.4.4/skbase/utils/_check.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/utils/_iter.py` & `scikit-base-0.4.4/skbase/utils/_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/utils/_nested_iter.py` & `scikit-base-0.4.4/skbase/utils/_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/utils/_utils.py` & `scikit-base-0.4.4/skbase/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/utils/tests/test_check.py` & `scikit-base-0.4.4/skbase/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/utils/tests/test_iter.py` & `scikit-base-0.4.4/skbase/utils/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/utils/tests/test_nested_iter.py` & `scikit-base-0.4.4/skbase/utils/tests/test_nested_iter.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/utils/tests/test_utils.py` & `scikit-base-0.4.4/skbase/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/validate/__init__.py` & `scikit-base-0.4.4/skbase/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/validate/_named_objects.py` & `scikit-base-0.4.4/skbase/validate/_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/validate/_types.py` & `scikit-base-0.4.4/skbase/validate/_types.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/validate/tests/test_iterable_named_objects.py` & `scikit-base-0.4.4/skbase/validate/tests/test_iterable_named_objects.py`

 * *Files identical despite different names*

### Comparing `scikit-base-0.4.3/skbase/validate/tests/test_type_validations.py` & `scikit-base-0.4.4/skbase/validate/tests/test_type_validations.py`

 * *Files identical despite different names*

