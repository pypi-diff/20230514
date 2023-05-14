# Comparing `tmp/wiremock-2.3.1.tar.gz` & `tmp/wiremock-2.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiremock-2.3.1.tar", last modified: Tue May 18 16:21:09 2021, max compression
+gzip compressed data, was "wiremock-2.4.0a0.tar", max compression
```

## Comparing `wiremock-2.3.1.tar` & `wiremock-2.4.0a0.tar`

### file list

```diff
@@ -1,93 +1,42 @@
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.781913 wiremock-2.3.1/
--rw-r--r--   0 cody.lee   (501) staff       (20)       34 2020-06-30 16:53:57.000000 wiremock-2.3.1/AUTHORS
--rw-r--r--   0 cody.lee   (501) staff       (20)      549 2020-06-30 16:53:57.000000 wiremock-2.3.1/LICENSE
--rw-r--r--   0 cody.lee   (501) staff       (20)      150 2020-06-30 16:53:57.000000 wiremock-2.3.1/MANIFEST.in
--rw-r--r--   0 cody.lee   (501) staff       (20)     1313 2021-05-18 16:21:09.781617 wiremock-2.3.1/PKG-INFO
--rw-r--r--   0 cody.lee   (501) staff       (20)      940 2020-06-30 16:53:57.000000 wiremock-2.3.1/README.md
--rw-r--r--   0 cody.lee   (501) staff       (20)       38 2021-05-18 16:21:09.782069 wiremock-2.3.1/setup.cfg
--rw-r--r--   0 cody.lee   (501) staff       (20)     2300 2020-06-30 16:53:57.000000 wiremock-2.3.1/setup.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.707424 wiremock-2.3.1/wiremock/
--rw-r--r--   0 cody.lee   (501) staff       (20)        6 2021-05-18 16:17:27.000000 wiremock-2.3.1/wiremock/VERSION
--rw-r--r--   0 cody.lee   (501) staff       (20)      169 2021-02-18 16:28:07.000000 wiremock-2.3.1/wiremock/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     1649 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/_compat.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.710157 wiremock-2.3.1/wiremock/base/
--rw-r--r--   0 cody.lee   (501) staff       (20)       79 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/base/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)    12441 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/base/base_entity.py
--rw-r--r--   0 cody.lee   (501) staff       (20)    13525 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/base/base_resource.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     1106 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/client.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     1434 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/constants.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.714746 wiremock-2.3.1/wiremock/exceptions/
--rw-r--r--   0 cody.lee   (501) staff       (20)      537 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/exceptions/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)      287 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/exceptions/api_exception.py
--rw-r--r--   0 cody.lee   (501) staff       (20)       96 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/exceptions/api_unavailable_exception.py
--rw-r--r--   0 cody.lee   (501) staff       (20)       88 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/exceptions/client_exception.py
--rw-r--r--   0 cody.lee   (501) staff       (20)       91 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/exceptions/forbidden_exception.py
--rw-r--r--   0 cody.lee   (501) staff       (20)       94 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/exceptions/invalid_input_exception.py
--rw-r--r--   0 cody.lee   (501) staff       (20)       90 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/exceptions/not_found_exception.py
--rw-r--r--   0 cody.lee   (501) staff       (20)       95 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/exceptions/requires_login_exception.py
--rw-r--r--   0 cody.lee   (501) staff       (20)       88 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/exceptions/server_exception.py
--rw-r--r--   0 cody.lee   (501) staff       (20)       89 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/exceptions/timeout_exception.py
--rw-r--r--   0 cody.lee   (501) staff       (20)      100 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/exceptions/unexpected_response_exception.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.715098 wiremock-2.3.1/wiremock/resources/
--rw-r--r--   0 cody.lee   (501) staff       (20)        0 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/__init__.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.716398 wiremock-2.3.1/wiremock/resources/mappings/
--rw-r--r--   0 cody.lee   (501) staff       (20)      231 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/mappings/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     6099 2021-02-18 16:28:07.000000 wiremock-2.3.1/wiremock/resources/mappings/models.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     3614 2021-02-25 15:03:11.000000 wiremock-2.3.1/wiremock/resources/mappings/resource.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.717839 wiremock-2.3.1/wiremock/resources/near_misses/
--rw-r--r--   0 cody.lee   (501) staff       (20)      165 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/near_misses/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     3316 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/near_misses/models.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     1519 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/near_misses/resource.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.720820 wiremock-2.3.1/wiremock/resources/requests/
--rw-r--r--   0 cody.lee   (501) staff       (20)      188 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/requests/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     2501 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/requests/models.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     3622 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/requests/resource.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.721653 wiremock-2.3.1/wiremock/resources/scenarios/
--rw-r--r--   0 cody.lee   (501) staff       (20)        0 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/scenarios/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)      612 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/scenarios/resource.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.723405 wiremock-2.3.1/wiremock/resources/settings/
--rw-r--r--   0 cody.lee   (501) staff       (20)       34 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/settings/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)      275 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/settings/models.py
--rw-r--r--   0 cody.lee   (501) staff       (20)      532 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/resources/settings/resource.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.725605 wiremock-2.3.1/wiremock/server/
--rw-r--r--   0 cody.lee   (501) staff       (20)       93 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/server/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)      260 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/server/exceptions.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     3141 2021-05-18 16:17:27.000000 wiremock-2.3.1/wiremock/server/server.py
--rw-r--r--   0 cody.lee   (501) staff       (20) 10997073 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/server/wiremock-standalone-2.6.0.jar
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.754843 wiremock-2.3.1/wiremock/tests/
--rw-r--r--   0 cody.lee   (501) staff       (20)       37 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     2476 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/base.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.756909 wiremock-2.3.1/wiremock/tests/base_tests/
--rw-r--r--   0 cody.lee   (501) staff       (20)       58 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/base_tests/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     1039 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/base_tests/base_resource_tests.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.757545 wiremock-2.3.1/wiremock/tests/resource_tests/
--rw-r--r--   0 cody.lee   (501) staff       (20)        0 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/__init__.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.758587 wiremock-2.3.1/wiremock/tests/resource_tests/mappings_tests/
--rw-r--r--   0 cody.lee   (501) staff       (20)        0 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/mappings_tests/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     3959 2021-02-25 15:03:11.000000 wiremock-2.3.1/wiremock/tests/resource_tests/mappings_tests/resource_tests.py
--rw-r--r--   0 cody.lee   (501) staff       (20)    12982 2021-02-18 16:28:07.000000 wiremock-2.3.1/wiremock/tests/resource_tests/mappings_tests/serialization_tests.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.760199 wiremock-2.3.1/wiremock/tests/resource_tests/near_misses_tests/
--rw-r--r--   0 cody.lee   (501) staff       (20)        0 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/near_misses_tests/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     2544 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/near_misses_tests/resource_tests.py
--rw-r--r--   0 cody.lee   (501) staff       (20)    17985 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/near_misses_tests/serialization_tests.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.775857 wiremock-2.3.1/wiremock/tests/resource_tests/requests_tests/
--rw-r--r--   0 cody.lee   (501) staff       (20)        0 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/requests_tests/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     4750 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/requests_tests/resource_tests.py
--rw-r--r--   0 cody.lee   (501) staff       (20)    10047 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/requests_tests/serialization_tests.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.777766 wiremock-2.3.1/wiremock/tests/resource_tests/scenarios_tests/
--rw-r--r--   0 cody.lee   (501) staff       (20)        0 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/scenarios_tests/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)      462 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/scenarios_tests/resource_tests.py
--rw-r--r--   0 cody.lee   (501) staff       (20)       59 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/scenarios_tests/serialization_tests.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.779531 wiremock-2.3.1/wiremock/tests/resource_tests/settings_tests/
--rw-r--r--   0 cody.lee   (501) staff       (20)        0 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/settings_tests/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)      608 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/settings_tests/resource_tests.py
--rw-r--r--   0 cody.lee   (501) staff       (20)      709 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/resource_tests/settings_tests/serialization_tests.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.780825 wiremock-2.3.1/wiremock/tests/server_tests/
--rw-r--r--   0 cody.lee   (501) staff       (20)       57 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/server_tests/__init__.py
--rw-r--r--   0 cody.lee   (501) staff       (20)     4224 2020-06-30 16:53:57.000000 wiremock-2.3.1/wiremock/tests/server_tests/server_tests.py
-drwxr-xr-x   0 cody.lee   (501) staff       (20)        0 2021-05-18 16:21:09.708972 wiremock-2.3.1/wiremock.egg-info/
--rw-r--r--   0 cody.lee   (501) staff       (20)     1313 2021-05-18 16:21:09.000000 wiremock-2.3.1/wiremock.egg-info/PKG-INFO
--rw-r--r--   0 cody.lee   (501) staff       (20)     2802 2021-05-18 16:21:09.000000 wiremock-2.3.1/wiremock.egg-info/SOURCES.txt
--rw-r--r--   0 cody.lee   (501) staff       (20)       90 2021-05-18 16:21:09.000000 wiremock-2.3.1/wiremock.egg-info/dependency_links.txt
--rw-r--r--   0 cody.lee   (501) staff       (20)      317 2021-05-18 16:21:09.000000 wiremock-2.3.1/wiremock.egg-info/requires.txt
--rw-r--r--   0 cody.lee   (501) staff       (20)        9 2021-05-18 16:21:09.000000 wiremock-2.3.1/wiremock.egg-info/top_level.txt
+-rw-r--r--   0        0        0      549 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/LICENSE
+-rw-r--r--   0        0        0      904 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/README.md
+-rw-r--r--   0        0        0     1968 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/wiremock/VERSION
+-rw-r--r--   0        0        0      169 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/wiremock/__init__.py
+-rw-r--r--   0        0        0     1649 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/wiremock/_compat.py
+-rw-r--r--   0        0        0       79 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/wiremock/base/__init__.py
+-rw-r--r--   0        0        0    12441 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/wiremock/base/base_entity.py
+-rw-r--r--   0        0        0    14484 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/wiremock/base/base_resource.py
+-rw-r--r--   0        0        0     1106 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/wiremock/client.py
+-rw-r--r--   0        0        0     1434 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/wiremock/constants.py
+-rw-r--r--   0        0        0      537 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/wiremock/exceptions/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/wiremock/exceptions/api_exception.py
+-rw-r--r--   0        0        0       96 2023-05-14 20:38:27.248558 wiremock-2.4.0a0/wiremock/exceptions/api_unavailable_exception.py
+-rw-r--r--   0        0        0       88 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/exceptions/client_exception.py
+-rw-r--r--   0        0        0       91 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/exceptions/forbidden_exception.py
+-rw-r--r--   0        0        0       94 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/exceptions/invalid_input_exception.py
+-rw-r--r--   0        0        0       90 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/exceptions/not_found_exception.py
+-rw-r--r--   0        0        0       95 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/exceptions/requires_login_exception.py
+-rw-r--r--   0        0        0       88 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/exceptions/server_exception.py
+-rw-r--r--   0        0        0       89 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/exceptions/timeout_exception.py
+-rw-r--r--   0        0        0      100 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/exceptions/unexpected_response_exception.py
+-rw-r--r--   0        0        0        0 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/__init__.py
+-rw-r--r--   0        0        0      231 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/mappings/__init__.py
+-rw-r--r--   0        0        0     6148 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/mappings/models.py
+-rw-r--r--   0        0        0     4001 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/mappings/resource.py
+-rw-r--r--   0        0        0      165 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/near_misses/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/near_misses/models.py
+-rw-r--r--   0        0        0     1519 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/near_misses/resource.py
+-rw-r--r--   0        0        0      188 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/requests/__init__.py
+-rw-r--r--   0        0        0     2501 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/requests/models.py
+-rw-r--r--   0        0        0     3622 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/requests/resource.py
+-rw-r--r--   0        0        0        0 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/scenarios/__init__.py
+-rw-r--r--   0        0        0      612 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/scenarios/resource.py
+-rw-r--r--   0        0        0       34 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/settings/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/settings/models.py
+-rw-r--r--   0        0        0      532 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/resources/settings/resource.py
+-rw-r--r--   0        0        0       93 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/server/__init__.py
+-rw-r--r--   0        0        0      260 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/server/exceptions.py
+-rw-r--r--   0        0        0     3509 2023-05-14 20:38:27.252559 wiremock-2.4.0a0/wiremock/server/server.py
+-rw-r--r--   0        0        0 10997073 2023-05-14 20:38:27.312563 wiremock-2.4.0a0/wiremock/server/wiremock-standalone-2.6.0.jar
+-rw-r--r--   0        0        0     2652 1970-01-01 00:00:00.000000 wiremock-2.4.0a0/PKG-INFO
```

### Comparing `wiremock-2.3.1/LICENSE` & `wiremock-2.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `wiremock-2.3.1/README.md` & `wiremock-2.4.0a0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Python WireMock Admin API Client
-================================
+# Python WireMock Admin API Client
 
 This is a python admin API client to a standalone WireMock server.
 
-[![Build Status](https://travis-ci.org/platinummonkey/python-wiremock.svg?branch=master)](https://travis-ci.org/platinummonkey/python-wiremock)
-[![Coverage Status](https://coveralls.io/repos/github/platinummonkey/python-wiremock/badge.svg?branch=master)](https://coveralls.io/github/platinummonkey/python-wiremock?branch=master)
+[![Build Status](https://travis-ci.org/wiremock/python-wiremock.svg?branch=master)](https://travis-ci.org/wiremock/python-wiremock)
+[![Coverage Status](https://coveralls.io/repos/github/wiremock/python-wiremock/badge.svg?branch=master)](https://coveralls.io/github/wiremock/python-wiremock?branch=master)
 [![Docs](https://img.shields.io/badge/docs-latest-brightgreen.svg)](http://wiremock.readthedocs.org/)
 
-
-Install as Dependency
---------------------
+## Install as Dependency
 
 To install:
 
     pip install wiremock
 
-
-Documentation
--------------
+## Documentation
 
 wiremock documentation can be found at http://wiremock.readthedocs.org/
 
-
-Pull Requests
--------------
+## Pull Requests
 
 General Rules:
-  - All Tests must pass
-  - Coverage shouldn't decrease
-  - All Pull Requests should be rebased against master **before** submitting the PR.
+
+- All Tests must pass
+- Coverage shouldn't decrease
+- All Pull Requests should be rebased against master **before** submitting the PR.
+
+## Development
+
+Setup the project using poetry.
+
+`poetry install`
```

### Comparing `wiremock-2.3.1/wiremock/_compat.py` & `wiremock-2.4.0a0/wiremock/_compat.py`

 * *Files identical despite different names*

### Comparing `wiremock-2.3.1/wiremock/base/base_entity.py` & `wiremock-2.4.0a0/wiremock/base/base_entity.py`

 * *Files identical despite different names*

### Comparing `wiremock-2.3.1/wiremock/base/base_resource.py` & `wiremock-2.4.0a0/wiremock/base/base_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import json
+
 import requests
 from requests import exceptions as rexc
 
 from wiremock.base.base_entity import BaseAbstractEntity
-from wiremock.constants import make_headers, Config, logger
+from wiremock.constants import Config, logger, make_headers
 from wiremock.exceptions import *
 
 
 class RestClient(object):
-    def __init__(self, timeout=None, base_url=None, requests_verify=None, requests_cert=None):
+    def __init__(
+        self, timeout=None, base_url=None, requests_verify=None, requests_cert=None
+    ):
         self.timeout = timeout
         self.base_url = base_url
         self.requests_verify = requests_verify
         self.requests_cert = requests_cert
 
     def _base_url(self):
         return self.base_url or Config.base_url
@@ -24,15 +27,21 @@
         return self.requests_verify or Config.requests_verify
 
     def _requests_cert(self):
         return self.requests_cert or Config.requests_cert
 
     def _log(self, action, url, **kwargs):
         ctx = {"timeout": kwargs.get("timeout")}
-        logger.debug("%s [%s] - %s", action, url, kwargs.get("json", json.dumps(kwargs.get("data", None))), extra=ctx)
+        logger.debug(
+            "%s [%s] - %s",
+            action,
+            url,
+            kwargs.get("json", json.dumps(kwargs.get("data", None))),
+            extra=ctx,
+        )
 
     def post(self, uri, **kwargs):
         if "timeout" not in kwargs:
             kwargs["timeout"] = self._timeout()
         if "requests_verify" not in kwargs:
             kwargs["verify"] = self._requests_verify()
         if "requests_cert" not in kwargs:
@@ -185,15 +194,17 @@
     def get_base_uri(cls, endpoint, **id_dict):
         if id_dict:
             return endpoint.format(**id_dict)
         return endpoint
 
     @staticmethod
     def get_entity_id(entity_id, entityClass):
-        if not (isinstance(entity_id, (int, str)) or isinstance(entity_id, entityClass)):
+        if not (
+            isinstance(entity_id, (int, str)) or isinstance(entity_id, entityClass)
+        ):
             raise InvalidInputException(422, entity_id)
         if isinstance(entity_id, entityClass):
             entity_id = entity_id.id
 
         return entity_id
 
     @staticmethod
@@ -201,76 +212,106 @@
         if not isinstance(entity, entityClass):
             raise InvalidInputException(422, entity)
 
     @classmethod
     def _create(cls, entity, parameters=None, ids={}):  # pragma: no cover
         if isinstance(entity, BaseAbstractEntity):
             response = cls.REST_CLIENT.post(
-                cls.get_base_uri(cls.endpoint(), **ids), json=entity.get_json_data(), headers=make_headers(), params=parameters
+                cls.get_base_uri(cls.endpoint(), **ids),
+                json=entity.get_json_data(),
+                headers=make_headers(),
+                params=parameters,
             )
         else:
             response = cls.REST_CLIENT.post(
-                cls.get_base_uri(cls.endpoint(), **ids), data=json.dumps(entity), headers=make_headers(), params=parameters
+                cls.get_base_uri(cls.endpoint(), **ids),
+                data=json.dumps(entity),
+                headers=make_headers(),
+                params=parameters,
             )
 
         response = cls.REST_CLIENT.handle_response(response)
 
-        if cls.entity_class() is None or not issubclass(cls.entity_class(), BaseAbstractEntity):
+        if cls.entity_class() is None or not issubclass(
+            cls.entity_class(), BaseAbstractEntity
+        ):
             return response  # pragma: no cover
         else:
             return cls.entity_class().from_dict(response.json())
 
     @classmethod
     def _update(cls, entity, parameters=None, ids={}):  # pragma: no cover
         entity_id = getattr(entity, "id", None)
         if entity_id is not None:
             ids["id"] = entity_id
         if isinstance(entity, BaseAbstractEntity):
             response = cls.REST_CLIENT.put(
-                cls.get_base_uri(cls.endpoint_single(), **ids), json=entity.get_json_data(), headers=make_headers(), params=parameters
+                cls.get_base_uri(cls.endpoint_single(), **ids),
+                json=entity.get_json_data(),
+                headers=make_headers(),
+                params=parameters,
             )
         else:
             response = cls.REST_CLIENT.put(
-                cls.get_base_uri(cls.endpoint_single(), **ids), data=json.dumps(entity), headers=make_headers(), params=parameters
+                cls.get_base_uri(cls.endpoint_single(), **ids),
+                data=json.dumps(entity),
+                headers=make_headers(),
+                params=parameters,
             )
 
         response = cls.REST_CLIENT.handle_response(response)
 
-        if cls.entity_class() is None or not issubclass(cls.entity_class(), BaseAbstractEntity):
+        if cls.entity_class() is None or not issubclass(
+            cls.entity_class(), BaseAbstractEntity
+        ):
             return response  # pragma: no cover
         else:
             return cls.entity_class().from_dict(response.json())
 
     @classmethod
     def _partial_update(cls, entity, parameters=None, ids={}):  # pragma: no cover
         entity_id = getattr(entity, "id", None)
         if entity_id is not None:
             ids["id"] = entity_id
         if isinstance(entity, BaseAbstractEntity):
             response = cls.REST_CLIENT.patch(
-                cls.get_base_uri(cls.endpoint_single(), **ids), json=entity.get_json_data(), headers=make_headers(), params=parameters
+                cls.get_base_uri(cls.endpoint_single(), **ids),
+                json=entity.get_json_data(),
+                headers=make_headers(),
+                params=parameters,
             )
         else:
             response = cls.REST_CLIENT.patch(
-                cls.get_base_uri(cls.endpoint_single(), **ids), data=json.dumps(entity), headers=make_headers(), params=parameters
+                cls.get_base_uri(cls.endpoint_single(), **ids),
+                data=json.dumps(entity),
+                headers=make_headers(),
+                params=parameters,
             )
 
         response = cls.REST_CLIENT.handle_response(response)
 
-        if cls.entity_class() is None or not issubclass(cls.entity_class(), BaseAbstractEntity):
+        if cls.entity_class() is None or not issubclass(
+            cls.entity_class(), BaseAbstractEntity
+        ):
             return response  # pragma: no cover
         else:
             return cls.entity_class().from_dict(response.json())
 
     @classmethod
     def _retreive_all(cls, parameters=None, ids={}):  # pragma: no cover
-        response = cls.REST_CLIENT.get(cls.get_base_uri(cls.endpoint(), **ids), headers=make_headers(), params=parameters)
+        response = cls.REST_CLIENT.get(
+            cls.get_base_uri(cls.endpoint(), **ids),
+            headers=make_headers(),
+            params=parameters,
+        )
         response = cls.REST_CLIENT.handle_response(response)
 
-        if cls.entity_class() is None or not issubclass(cls.entity_class(), BaseAbstractEntity):
+        if cls.entity_class() is None or not issubclass(
+            cls.entity_class(), BaseAbstractEntity
+        ):
             return response  # pragma: no cover
         else:
             response_json = response.json()
             if isinstance(response_json, (tuple, list)):
                 results = []
                 for r in response_json:
                     if isinstance(r, dict):
@@ -279,46 +320,74 @@
             else:
                 return cls.entity_class().from_dict(response.json())
 
     @classmethod
     def _retreive_one(cls, entity, parameters=None, ids={}):  # pragma: no cover
         if isinstance(entity, (int, float)):
             ids["id"] = entity
-            response = cls.REST_CLIENT.get(cls.get_base_uri(cls.endpoint_single(), **ids), headers=make_headers(), params=parameters)
+            response = cls.REST_CLIENT.get(
+                cls.get_base_uri(cls.endpoint_single(), **ids),
+                headers=make_headers(),
+                params=parameters,
+            )
         elif entity is not None and issubclass(entity, BaseAbstractEntity):
             entity_id = getattr(entity, "id", None)
             ids["id"] = entity_id
-            response = cls.REST_CLIENT.get(cls.get_base_uri(cls.endpoint_single(), **ids), headers=make_headers(), params=parameters)
+            response = cls.REST_CLIENT.get(
+                cls.get_base_uri(cls.endpoint_single(), **ids),
+                headers=make_headers(),
+                params=parameters,
+            )
         else:
-            response = cls.REST_CLIENT.get(cls.get_base_uri(cls.endpoint_single(), **ids), headers=make_headers(), params=parameters)
+            response = cls.REST_CLIENT.get(
+                cls.get_base_uri(cls.endpoint_single(), **ids),
+                headers=make_headers(),
+                params=parameters,
+            )
 
         response = cls.REST_CLIENT.handle_response(response)
 
-        if cls.entity_class() is None or not issubclass(cls.entity_class(), BaseAbstractEntity):
+        if cls.entity_class() is None or not issubclass(
+            cls.entity_class(), BaseAbstractEntity
+        ):
             return response  # pragma: no cover
         else:
             return cls.entity_class().from_dict(response.json())
 
     @classmethod
     def _delete(cls, entity, parameters=None, ids={}):  # pragma: no cover
         if isinstance(entity, (int, float)):
             ids["id"] = entity
-            response = cls.REST_CLIENT.delete(cls.get_base_uri(cls.endpoint_single(), **ids), headers=make_headers(), params=parameters)
+            response = cls.REST_CLIENT.delete(
+                cls.get_base_uri(cls.endpoint_single(), **ids),
+                headers=make_headers(),
+                params=parameters,
+            )
         elif isinstance(entity, BaseAbstractEntity):
             entity_id = getattr(entity, "id", None)
             ids["id"] = entity_id
-            response = cls.REST_CLIENT.delete(cls.get_base_uri(cls.endpoint_single(), **ids), headers=make_headers(), params=parameters)
+            response = cls.REST_CLIENT.delete(
+                cls.get_base_uri(cls.endpoint_single(), **ids),
+                headers=make_headers(),
+                params=parameters,
+            )
         else:
-            response = cls.REST_CLIENT.delete(cls.get_base_uri(cls.endpoint_single(), **ids), headers=make_headers(), params=parameters)
+            response = cls.REST_CLIENT.delete(
+                cls.get_base_uri(cls.endpoint_single(), **ids),
+                headers=make_headers(),
+                params=parameters,
+            )
 
         response = cls.REST_CLIENT.handle_response(response)
         if response is None:
             return entity
 
-        if cls.entity_class() is None or not issubclass(cls.entity_class(), BaseAbstractEntity):
+        if cls.entity_class() is None or not issubclass(
+            cls.entity_class(), BaseAbstractEntity
+        ):
             return response  # pragma: no cover
         else:
             try:
                 return cls.entity_class().from_dict(response.json())
             except ValueError:
                 return response  # pragma: no cover
```

### Comparing `wiremock-2.3.1/wiremock/client.py` & `wiremock-2.4.0a0/wiremock/client.py`

 * *Files identical despite different names*

### Comparing `wiremock-2.3.1/wiremock/constants.py` & `wiremock-2.4.0a0/wiremock/constants.py`

 * *Files identical despite different names*

### Comparing `wiremock-2.3.1/wiremock/exceptions/__init__.py` & `wiremock-2.4.0a0/wiremock/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `wiremock-2.3.1/wiremock/resources/mappings/models.py` & `wiremock-2.4.0a0/wiremock/resources/mappings/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 from wiremock._compat import add_metaclass
-from wiremock.base import BaseEntity, JsonProperty, BaseAbstractEntity, BaseEntityMetaType
+from wiremock.base import (
+    BaseAbstractEntity,
+    BaseEntity,
+    BaseEntityMetaType,
+    JsonProperty,
+)
 
 
 class HttpMethods(object):
     ANY = "ANY"
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
@@ -120,25 +125,29 @@
 @add_metaclass(BaseEntityMetaType)
 class MappingRequest(BaseAbstractEntity):
     method = JsonProperty("method")
     url = JsonProperty("url")
     url_path = JsonProperty("urlPath")
     url_path_pattern = JsonProperty("urlPathPattern")
     url_pattern = JsonProperty("urlPattern")
-    basic_auth_credentials = JsonProperty("basicAuthCredentials", klass=BasicAuthCredentials)
+    basic_auth_credentials = JsonProperty(
+        "basicAuthCredentials", klass=BasicAuthCredentials
+    )
     cookies = JsonProperty("cookies", klass=dict)
     headers = JsonProperty("headers", klass=dict)
     query_parameters = JsonProperty("queryParameters", klass=dict)
     body_patterns = JsonProperty("bodyPatterns", klass=list, list_klass=dict)
     metadata = JsonProperty("metadata", klass=dict)
 
 
 @add_metaclass(BaseEntityMetaType)
 class MappingResponse(BaseAbstractEntity):
-    additional_proxy_request_headers = JsonProperty("additionalProxyRequestHeaders", klass=dict)
+    additional_proxy_request_headers = JsonProperty(
+        "additionalProxyRequestHeaders", klass=dict
+    )
     base64_body = JsonProperty("base64Body")
     body = JsonProperty("body")
     body_file_name = JsonProperty("bodyFileName")
     json_body = JsonProperty("jsonBody")
     delay_distribution = JsonProperty("delayDistribution", klass=DelayDistribution)
     fault = JsonProperty("fault")
     fixed_delay_milliseconds = JsonProperty("fixedDelayMilliseconds")
@@ -157,15 +166,15 @@
     request = JsonProperty("request", klass=MappingRequest)
     response = JsonProperty("response", klass=MappingResponse)
     persistent = JsonProperty("persistent")
     post_serve_actions = JsonProperty("postServeActions", klass=dict)
     new_scenario_state = JsonProperty("newScenarioState")
     required_scenario_state = JsonProperty("requiredScenarioState")
     scenario_name = JsonProperty("scenarioName")
-    metadata = JsonProperty('metadata', klass=dict)
+    metadata = JsonProperty("metadata", klass=dict)
 
 
 @add_metaclass(BaseEntityMetaType)
 class MappingMeta(BaseAbstractEntity):
     total = JsonProperty("total")
```

### Comparing `wiremock-2.3.1/wiremock/resources/mappings/resource.py` & `wiremock-2.4.0a0/wiremock/resources/mappings/resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from wiremock.constants import make_headers
 from wiremock.base.base_resource import BaseResource
-from wiremock.resources.mappings import Mapping, AllMappings, MappingResponse
+from wiremock.constants import make_headers
+from wiremock.resources.mappings import AllMappings, Mapping, MappingResponse
 
 
 class Mappings(BaseResource):
     @classmethod
     def endpoint(cls):
         return "/mappings"
 
@@ -19,68 +19,101 @@
     @classmethod
     def entity_class(cls):
         return MappingResponse
 
     @classmethod
     def create_mapping(cls, mapping, parameters={}):
         cls.validate_is_entity(mapping, Mapping)
-        response = cls.REST_CLIENT.post(cls.get_base_uri(cls.endpoint()), json=mapping.get_json_data(), headers=make_headers(), params=parameters)
+        response = cls.REST_CLIENT.post(
+            cls.get_base_uri(cls.endpoint()),
+            json=mapping.get_json_data(),
+            headers=make_headers(),
+            params=parameters,
+        )
         response = cls.REST_CLIENT.handle_response(response)
         return MappingResponse.from_dict(response.json())
 
     @classmethod
     def retrieve_all_mappings(cls, parameters={}):
-        response = cls.REST_CLIENT.get(cls.get_base_uri(cls.endpoint()), headers=make_headers(), params=parameters)
+        response = cls.REST_CLIENT.get(
+            cls.get_base_uri(cls.endpoint()), headers=make_headers(), params=parameters
+        )
         response = cls.REST_CLIENT.handle_response(response)
         return AllMappings.from_dict(response.json())
 
     @classmethod
     def retrieve_mapping(cls, mapping_id, parameters={}):
         mapping_id = cls.get_entity_id(mapping_id, Mapping)
         ids = {"id": mapping_id}
-        response = cls.REST_CLIENT.get(cls.get_base_uri(cls.endpoint_single(), **ids), headers=make_headers(), params=parameters)
+        response = cls.REST_CLIENT.get(
+            cls.get_base_uri(cls.endpoint_single(), **ids),
+            headers=make_headers(),
+            params=parameters,
+        )
         response = cls.REST_CLIENT.handle_response(response)
         return Mapping.from_dict(response.json())
 
     @classmethod
     def update_mapping(cls, mapping, parameters={}):
         cls.validate_is_entity(mapping, Mapping)
         mapping_id = cls.get_entity_id(mapping, Mapping)
         ids = {"id": mapping_id}
         response = cls.REST_CLIENT.put(
-            cls.get_base_uri(cls.endpoint_single(), **ids), json=mapping.get_json_data(), headers=make_headers(), params=parameters
+            cls.get_base_uri(cls.endpoint_single(), **ids),
+            json=mapping.get_json_data(),
+            headers=make_headers(),
+            params=parameters,
         )
         response = cls.REST_CLIENT.handle_response(response)
         return Mapping.from_dict(response.json())
 
     @classmethod
     def persist_mappings(cls, parameters={}):
         ids = {"id": "save"}
-        response = cls.REST_CLIENT.post(cls.get_base_uri(cls.endpoint_single(), **ids), headers=make_headers(), params=parameters)
+        response = cls.REST_CLIENT.post(
+            cls.get_base_uri(cls.endpoint_single(), **ids),
+            headers=make_headers(),
+            params=parameters,
+        )
         return cls.REST_CLIENT.handle_response(response)
 
     @classmethod
     def reset_mappings(cls, parameters={}):
         ids = {"id": "reset"}
-        response = cls.REST_CLIENT.post(cls.get_base_uri(cls.endpoint_single(), **ids), headers=make_headers(), params=parameters)
+        response = cls.REST_CLIENT.post(
+            cls.get_base_uri(cls.endpoint_single(), **ids),
+            headers=make_headers(),
+            params=parameters,
+        )
         return cls.REST_CLIENT.handle_response(response)
 
     @classmethod
     def delete_all_mappings(cls, parameters={}):
-        response = cls.REST_CLIENT.delete(cls.get_base_uri(cls.endpoint()), headers=make_headers(), params=parameters)
+        response = cls.REST_CLIENT.delete(
+            cls.get_base_uri(cls.endpoint()), headers=make_headers(), params=parameters
+        )
         return cls.REST_CLIENT.handle_response(response)
 
     @classmethod
     def delete_mapping(cls, mapping_id, parameters={}):
         mapping_id = cls.get_entity_id(mapping_id, Mapping)
         ids = {"id": mapping_id}
-        response = cls.REST_CLIENT.delete(cls.get_base_uri(cls.endpoint_single(), **ids), headers=make_headers(), params=parameters)
+        response = cls.REST_CLIENT.delete(
+            cls.get_base_uri(cls.endpoint_single(), **ids),
+            headers=make_headers(),
+            params=parameters,
+        )
         return cls.REST_CLIENT.handle_response(response)
 
     @classmethod
     def delete_mapping_by_metadata(cls, metadata, parameters={}):
-        response = cls.REST_CLIENT.post(cls.get_base_uri(cls.endpoint_delete_by_metadata()), headers=make_headers(), params=parameters, json=metadata)
+        response = cls.REST_CLIENT.post(
+            cls.get_base_uri(cls.endpoint_delete_by_metadata()),
+            headers=make_headers(),
+            params=parameters,
+            json=metadata,
+        )
 
         return cls.REST_CLIENT.handle_response(response)
 
 
 __all__ = ["Mappings"]
```

### Comparing `wiremock-2.3.1/wiremock/resources/near_misses/models.py` & `wiremock-2.4.0a0/wiremock/resources/near_misses/models.py`

 * *Files identical despite different names*

### Comparing `wiremock-2.3.1/wiremock/resources/near_misses/resource.py` & `wiremock-2.4.0a0/wiremock/resources/near_misses/resource.py`

 * *Files identical despite different names*

### Comparing `wiremock-2.3.1/wiremock/resources/requests/models.py` & `wiremock-2.4.0a0/wiremock/resources/requests/models.py`

 * *Files identical despite different names*

### Comparing `wiremock-2.3.1/wiremock/resources/requests/resource.py` & `wiremock-2.4.0a0/wiremock/resources/requests/resource.py`

 * *Files identical despite different names*

### Comparing `wiremock-2.3.1/wiremock/resources/scenarios/resource.py` & `wiremock-2.4.0a0/wiremock/resources/scenarios/resource.py`

 * *Files identical despite different names*

### Comparing `wiremock-2.3.1/wiremock/resources/settings/resource.py` & `wiremock-2.4.0a0/wiremock/resources/settings/resource.py`

 * *Files identical despite different names*

### Comparing `wiremock-2.3.1/wiremock/server/server.py` & `wiremock-2.4.0a0/wiremock/server/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 # -*- coding: utf-8 -*-
 """WireMock Server Management."""
 import atexit
 import socket
-
 import time
+from subprocess import PIPE, STDOUT, Popen
 
 import requests
-from pkg_resources import resource_filename
-from subprocess import Popen, PIPE, STDOUT
+from importlib_resources import files
 
-from wiremock.server.exceptions import WireMockServerAlreadyStartedError, WireMockServerNotStartedError
+from wiremock.server.exceptions import (
+    WireMockServerAlreadyStartedError,
+    WireMockServerNotStartedError,
+)
 
 
 class WireMockServer(object):
 
     DEFAULT_JAVA = "java"  # Assume java in PATH
-    DEFAULT_JAR = resource_filename("wiremock", "server/wiremock-standalone-2.6.0.jar")
+    DEFAULT_JAR = files("wiremock") / "server" / "wiremock-standalone-2.6.0.jar"
 
-    def __init__(self, java_path=DEFAULT_JAVA, jar_path=DEFAULT_JAR, port=None, max_attempts=10, root_dir=None):
+    def __init__(
+        self,
+        java_path=DEFAULT_JAVA,
+        jar_path=DEFAULT_JAR,
+        port=None,
+        max_attempts=10,
+        root_dir=None,
+    ):
         self.java_path = java_path
         self.jar_path = jar_path
         self.port = port or self._get_free_port()
         self.__subprocess = None
         self.__running = False
         self.max_attempts = max_attempts
         self.root_dir = root_dir
@@ -35,30 +44,45 @@
 
     @property
     def is_running(self):
         return self.__running
 
     def start(self):
         if self.is_running:
-            raise WireMockServerAlreadyStartedError("WireMockServer already started on port {}".format(self.port))
+            raise WireMockServerAlreadyStartedError(
+                "WireMockServer already started on port {}".format(self.port)
+            )
 
-        cmd = [self.java_path, "-jar", self.jar_path, "--port", str(self.port), "--local-response-templating"]
+        cmd = [
+            self.java_path,
+            "-jar",
+            self.jar_path,
+            "--port",
+            str(self.port),
+            "--local-response-templating",
+        ]
         if self.root_dir is not None:
             cmd.append("--root-dir=")
             cmd.append(str(self.root_dir))
         try:
             self.__subprocess = Popen(cmd, stdin=PIPE, stdout=PIPE, stderr=STDOUT)
         except OSError as e:
             raise WireMockServerNotStartedError(str(e))  # Problem with Java
 
         time.sleep(0.1)
         if self.__subprocess.poll() is not None:
             # Process complete - server not started
             raise WireMockServerNotStartedError(
-                "\n".join(["returncode: {}".format(self.__subprocess.returncode), "stdout:", str(self.__subprocess.stdout.read())])
+                "\n".join(
+                    [
+                        "returncode: {}".format(self.__subprocess.returncode),
+                        "stdout:",
+                        str(self.__subprocess.stdout.read()),
+                    ]
+                )
             )
 
         # Call the /__admin endpoint as a check for running state
         attempts = 0
         success = False
         while attempts < self.max_attempts:
             try:
@@ -69,15 +93,19 @@
                     break
             except requests.exceptions.ConnectionError:
                 pass
 
             time.sleep(0.25)
 
         if not success:
-            raise WireMockServerNotStartedError("unable to get a successful GET http://localhost:{}/__admin response".format(self.port))
+            raise WireMockServerNotStartedError(
+                "unable to get a successful GET http://localhost:{}/__admin response".format(
+                    self.port
+                )
+            )
 
         atexit.register(self.stop, raise_on_error=False)
         self.__running = True
 
     def stop(self, raise_on_error=True):
         try:
             self.__subprocess.kill()
```

### Comparing `wiremock-2.3.1/wiremock/server/wiremock-standalone-2.6.0.jar` & `wiremock-2.4.0a0/wiremock/server/wiremock-standalone-2.6.0.jar`

 * *Files identical despite different names*

