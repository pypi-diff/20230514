# Comparing `tmp/pyhanko-certvalidator-0.22.0.tar.gz` & `tmp/pyhanko-certvalidator-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhanko-certvalidator-0.22.0.tar", last modified: Sun Apr 23 17:17:01 2023, max compression
+gzip compressed data, was "pyhanko-certvalidator-0.23.0.tar", last modified: Sun May 14 16:55:21 2023, max compression
```

## Comparing `pyhanko-certvalidator-0.22.0.tar` & `pyhanko-certvalidator-0.23.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.880287 pyhanko-certvalidator-0.22.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-23 17:17:01.880287 pyhanko-certvalidator-0.22.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.872284 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/_asyncio_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/asn1_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/authority.py
--rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.876286 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.876286 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/cert_fetch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/crl_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/ocsp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.876286 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/cert_fetch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/crl_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/ocsp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.876286 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/ades_past.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/poe.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/time_slide.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/name_trees.py
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    19124 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/policy_decl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/policy_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22057 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.880287 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/archival.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    47720 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/validate_crl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23041 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/validate_ocsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    55273 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.872284 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-23 17:17:01.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-23 17:17:01.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:17:01.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-23 17:17:01.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 17:17:01.000000 pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:17:01.880287 pyhanko-certvalidator-0.22.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:17:01.880287 pyhanko-certvalidator-0.22.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18398 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_ac_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_ades_time_slide.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_certificate_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_crl_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_freshness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_ocsp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_policy_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    22461 2023-04-23 17:16:47.000000 pyhanko-certvalidator-0.22.0/tests/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:55:21.521014 pyhanko-certvalidator-0.23.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-14 16:55:21.521014 pyhanko-certvalidator-0.23.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:55:21.513013 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/_asyncio_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/asn1_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/authority.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:55:21.513013 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:55:21.517014 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/cert_fetch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/crl_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/ocsp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:55:21.517014 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/requests_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/requests_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/requests_fetchers/cert_fetch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/requests_fetchers/crl_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/requests_fetchers/ocsp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/requests_fetchers/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:55:21.517014 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/ltv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/ltv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/ltv/ades_past.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/ltv/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/ltv/poe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/ltv/time_slide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/ltv/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/name_trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/policy_decl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/policy_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22057 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:55:21.517014 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/revinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/revinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/revinfo/archival.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/revinfo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/revinfo/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47720 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/revinfo/validate_crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23041 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/revinfo/validate_ocsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55273 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:55:21.513013 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-14 16:55:21.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-14 16:55:21.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:55:21.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-14 16:55:21.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-14 16:55:21.000000 pyhanko-certvalidator-0.23.0/pyhanko_certvalidator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:55:21.521014 pyhanko-certvalidator-0.23.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:55:21.521014 pyhanko-certvalidator-0.23.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18398 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/tests/test_ac_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/tests/test_ades_time_slide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/tests/test_certificate_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/tests/test_crl_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/tests/test_freshness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/tests/test_ocsp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/tests/test_policy_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22461 2023-05-14 16:55:10.000000 pyhanko-certvalidator-0.23.0/tests/test_validate.py
```

### Comparing `pyhanko-certvalidator-0.22.0/LICENSE` & `pyhanko-certvalidator-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/PKG-INFO` & `pyhanko-certvalidator-0.23.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhanko-certvalidator
-Version: 0.22.0
+Version: 0.23.0
 Summary: Validates X.509 certificates and paths; forked from wbond/certvalidator
 Author-email: Matthias Valvekens <dev@mvalvekens.be>
 License: MIT
 Project-URL: Homepage, https://github.com/MatthiasValvekens/certvalidator
 Keywords: crypto,pki,x509,certificate,crl,ocsp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security :: Cryptography
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: async-http
 Provides-Extra: testing
 Provides-Extra: mypy
 License-File: LICENSE
 
 # certvalidator
@@ -81,15 +82,15 @@
 ## Dependencies
 
  - *asn1crypto*
  - *cryptography*
  - *uritools*
  - *oscrypto*
  - *requests* or *aiohttp* (use the latter for more efficient asyncio, requires resource management)
- - Python 3.7, 3.8, 3.9 or 3.10
+ - Python 3.7 or higher
 
  ### Note on compatibility
 
  Starting with `pyhanko-certvalidator` version `0.17.0`, the library has been refactored to use asynchronous I/O as much as possible. Most high-level API entrypoints can still be used synchronously, but have been deprecated in favour of their asyncio equivalents. 
  As part of this move, the OCSP and CRL clients now have two separate implementations: a `requests`-based one, and an `aiohttp`-based one. The latter is probably more performant, but requires more resource management efforts on the caller's part, which was impossible to implement without making major breaking changes to the public API that would make the migration path more complicated. Therefore, the `requests`-based fetcher will remain the default for the time being.
 
 
@@ -100,23 +101,15 @@
 ```
 
 ## License
 
 *certvalidator* is licensed under the terms of the MIT license. See the
 [LICENSE](LICENSE) file for the exact license text.
 
-## Documentation
 
-[*certvalidator* documentation](docs/readme.md)
-
-## Continuous Integration
-
-Various combinations of platforms and versions of Python are tested via:
-
- - [GitHub Actions](https://github.com/MatthiasValvekens/certvalidator/actions)
 
 ## Testing
 
 ### Test framework
 
 Tests are written using `pytest` and require an asynchronous test case backend
 such as `pytest-asyncio`.
```

### Comparing `pyhanko-certvalidator-0.22.0/README.md` & `pyhanko-certvalidator-0.23.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ## Dependencies
 
  - *asn1crypto*
  - *cryptography*
  - *uritools*
  - *oscrypto*
  - *requests* or *aiohttp* (use the latter for more efficient asyncio, requires resource management)
- - Python 3.7, 3.8, 3.9 or 3.10
+ - Python 3.7 or higher
 
  ### Note on compatibility
 
  Starting with `pyhanko-certvalidator` version `0.17.0`, the library has been refactored to use asynchronous I/O as much as possible. Most high-level API entrypoints can still be used synchronously, but have been deprecated in favour of their asyncio equivalents. 
  As part of this move, the OCSP and CRL clients now have two separate implementations: a `requests`-based one, and an `aiohttp`-based one. The latter is probably more performant, but requires more resource management efforts on the caller's part, which was impossible to implement without making major breaking changes to the public API that would make the migration path more complicated. Therefore, the `requests`-based fetcher will remain the default for the time being.
 
 
@@ -76,23 +76,15 @@
 ```
 
 ## License
 
 *certvalidator* is licensed under the terms of the MIT license. See the
 [LICENSE](LICENSE) file for the exact license text.
 
-## Documentation
 
-[*certvalidator* documentation](docs/readme.md)
-
-## Continuous Integration
-
-Various combinations of platforms and versions of Python are tested via:
-
- - [GitHub Actions](https://github.com/MatthiasValvekens/certvalidator/actions)
 
 ## Testing
 
 ### Test framework
 
 Tests are written using `pytest` and require an asynchronous test case backend
 such as `pytest-asyncio`.
```

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/__init__.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/_asyncio_compat.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/_asyncio_compat.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/_state.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/_state.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/asn1_types.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/asn1_types.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/authority.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/authority.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/context.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/context.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/errors.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/errors.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/__init__.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/cert_fetch_client.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/cert_fetch_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/crl_client.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/crl_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/ocsp_client.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/ocsp_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/util.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/aiohttp_fetchers/util.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/api.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class CRLFetcher(abc.ABC):
     """Utility interface to fetch and cache CRLs."""
 
     async def fetch(
         self,
         cert: Union[x509.Certificate, cms.AttributeCertificateV2],
         *,
-        use_deltas=None
+        use_deltas=None,
     ) -> Iterable[crl.CertificateList]:
         """
         Fetches the CRLs for a certificate.
 
         :param cert:
             An asn1crypto.x509.Certificate object to get the CRL for
```

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/common_utils.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/common_utils.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/__init__.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/requests_fetchers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/cert_fetch_client.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/requests_fetchers/cert_fetch_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/crl_client.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/requests_fetchers/crl_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/ocsp_client.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/requests_fetchers/ocsp_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/fetchers/requests_fetchers/util.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/fetchers/requests_fetchers/util.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/ades_past.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/ltv/ades_past.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/poe.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/ltv/poe.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/time_slide.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/ltv/time_slide.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/ltv/types.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/ltv/types.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/name_trees.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/name_trees.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/path.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/path.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/policy_decl.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/policy_decl.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,21 @@
 
 
 DEFAULT_WEAK_HASH_ALGOS = frozenset(['md2', 'md5', 'sha1'])
 """
 Digest algorithms considered weak by default.
 """
 
+FRESHNESS_FALLBACK_VALIDITY_DEFAULT = timedelta(minutes=30)
+"""
+Default freshness used by the default/legacy freshness policy
+when the revocation information does not specify a next update
+time. In practice this only applies to OCSP responses.
+"""
+
 
 @enum.unique
 class RevocationCheckingRule(enum.Enum):
     """
     Rules determining in what circumstances revocation data has to be checked,
     and what kind.
     """
@@ -248,14 +255,16 @@
     """
 
     freshness: Optional[timedelta] = None
     """
     Freshness interval. If not specified, this defaults to the distance
     between ``thisUpdate`` and ``nextUpdate`` for the given piece of revocation
     information.
+    If the ``nextUpdate`` field is not present, then the effective default
+    is 30 minutes.
     """
 
     freshness_req_type: FreshnessReqType = FreshnessReqType.DEFAULT
     """
     Controls whether the freshness requirement applies relatively to the
     signing time or to the validation time.
     """
```

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/policy_tree.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/policy_tree.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/registry.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/registry.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/archival.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/revinfo/archival.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from pyhanko_certvalidator._types import type_name
 from pyhanko_certvalidator.ltv.types import (
     IssuedItemContainer,
     ValidationTimingParams,
 )
 from pyhanko_certvalidator.policy_decl import (
+    FRESHNESS_FALLBACK_VALIDITY_DEFAULT,
     CertRevTrustPolicy,
     FreshnessReqType,
 )
 
 __all__ = [
     'RevinfoUsabilityRating',
     'RevinfoUsability',
@@ -81,15 +82,15 @@
     rating: RevinfoUsabilityRating
     """
     The rating assigned.
     """
 
     last_usable_at: Optional[datetime] = None
     """
-    The last date at which the revocation infromation could have been
+    The last date at which the revocation information could have been
     considered usable, if applicable.
     """
 
 
 class RevinfoContainer(IssuedItemContainer, abc.ABC):
     """
     A container for a piece of revocation information.
@@ -215,15 +216,20 @@
                 RevinfoUsabilityRating.STALE,
                 last_usable_at=this_update + freshness_delta,
             )
     elif policy.freshness_req_type == FreshnessReqType.DEFAULT:
         # check whether the validation time falls within the
         # thisUpdate-nextUpdate window (non-AdES!!)
         if next_update is None:
-            return RevinfoUsability(RevinfoUsabilityRating.UNCLEAR)
+            # OCSP semantics of nextUpdate = VOID is "please request
+            # another update whenever you like".
+            # In our default/legacy validation model this is difficult to
+            # interpret.
+            # for historical point-in-time validation, this is disqualifying
+            next_update = this_update + FRESHNESS_FALLBACK_VALIDITY_DEFAULT
 
         retroactive = policy.retroactive_revinfo
 
         if not retroactive and validation_time < this_update - time_tolerance:
             return RevinfoUsability(RevinfoUsabilityRating.TOO_NEW)
         if validation_time > next_update + time_tolerance:
             return RevinfoUsability(
```

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/constants.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/revinfo/constants.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/manager.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/revinfo/manager.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/validate_crl.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/revinfo/validate_crl.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/revinfo/validate_ocsp.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/revinfo/validate_ocsp.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/util.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/util.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator/validate.py` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator/validate.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/PKG-INFO` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhanko-certvalidator
-Version: 0.22.0
+Version: 0.23.0
 Summary: Validates X.509 certificates and paths; forked from wbond/certvalidator
 Author-email: Matthias Valvekens <dev@mvalvekens.be>
 License: MIT
 Project-URL: Homepage, https://github.com/MatthiasValvekens/certvalidator
 Keywords: crypto,pki,x509,certificate,crl,ocsp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security :: Cryptography
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: async-http
 Provides-Extra: testing
 Provides-Extra: mypy
 License-File: LICENSE
 
 # certvalidator
@@ -81,15 +82,15 @@
 ## Dependencies
 
  - *asn1crypto*
  - *cryptography*
  - *uritools*
  - *oscrypto*
  - *requests* or *aiohttp* (use the latter for more efficient asyncio, requires resource management)
- - Python 3.7, 3.8, 3.9 or 3.10
+ - Python 3.7 or higher
 
  ### Note on compatibility
 
  Starting with `pyhanko-certvalidator` version `0.17.0`, the library has been refactored to use asynchronous I/O as much as possible. Most high-level API entrypoints can still be used synchronously, but have been deprecated in favour of their asyncio equivalents. 
  As part of this move, the OCSP and CRL clients now have two separate implementations: a `requests`-based one, and an `aiohttp`-based one. The latter is probably more performant, but requires more resource management efforts on the caller's part, which was impossible to implement without making major breaking changes to the public API that would make the migration path more complicated. Therefore, the `requests`-based fetcher will remain the default for the time being.
 
 
@@ -100,23 +101,15 @@
 ```
 
 ## License
 
 *certvalidator* is licensed under the terms of the MIT license. See the
 [LICENSE](LICENSE) file for the exact license text.
 
-## Documentation
 
-[*certvalidator* documentation](docs/readme.md)
-
-## Continuous Integration
-
-Various combinations of platforms and versions of Python are tested via:
-
- - [GitHub Actions](https://github.com/MatthiasValvekens/certvalidator/actions)
 
 ## Testing
 
 ### Test framework
 
 Tests are written using `pytest` and require an asynchronous test case backend
 such as `pytest-asyncio`.
```

### Comparing `pyhanko-certvalidator-0.22.0/pyhanko_certvalidator.egg-info/SOURCES.txt` & `pyhanko-certvalidator-0.23.0/pyhanko_certvalidator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/pyproject.toml` & `pyhanko-certvalidator-0.23.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Security :: Cryptography",
 ]
+requires-python = ">=3.7"
 dependencies = [
     "asn1crypto>=1.5.1",
     "oscrypto>=1.1.0",
     "cryptography>=3.3.1",
     "uritools>=3.0.1",
     "requests>=2.24.0",
 ]
```

### Comparing `pyhanko-certvalidator-0.22.0/tests/test_ac_validate.py` & `pyhanko-certvalidator-0.23.0/tests/test_ac_validate.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/tests/test_ades_time_slide.py` & `pyhanko-certvalidator-0.23.0/tests/test_ades_time_slide.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/tests/test_certificate_validator.py` & `pyhanko-certvalidator-0.23.0/tests/test_certificate_validator.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/tests/test_crl_client.py` & `pyhanko-certvalidator-0.23.0/tests/test_crl_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/tests/test_freshness.py` & `pyhanko-certvalidator-0.23.0/tests/test_freshness.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/tests/test_ocsp_client.py` & `pyhanko-certvalidator-0.23.0/tests/test_ocsp_client.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/tests/test_policy_proc.py` & `pyhanko-certvalidator-0.23.0/tests/test_policy_proc.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/tests/test_registry.py` & `pyhanko-certvalidator-0.23.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `pyhanko-certvalidator-0.22.0/tests/test_validate.py` & `pyhanko-certvalidator-0.23.0/tests/test_validate.py`

 * *Files identical despite different names*

