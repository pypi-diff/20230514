# Comparing `tmp/edc-subject-model-wrappers-0.3.8.tar.gz` & `tmp/edc-subject-model-wrappers-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-subject-model-wrappers-0.3.8.tar", last modified: Tue May 31 16:49:50 2022, max compression
+gzip compressed data, was "edc-subject-model-wrappers-0.3.9.tar", last modified: Fri Aug 12 12:18:29 2022, max compression
```

## Comparing `edc-subject-model-wrappers-0.3.8.tar` & `edc-subject-model-wrappers-0.3.9.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-31 16:49:50.478523 edc-subject-model-wrappers-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      138 2021-02-05 20:38:05.000000 edc-subject-model-wrappers-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-05 20:38:05.000000 edc-subject-model-wrappers-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-31 16:49:50.470618 edc-subject-model-wrappers-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-31 16:49:50.473197 edc-subject-model-wrappers-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1745 2022-05-19 02:12:43.000000 edc-subject-model-wrappers-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1235 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       88 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1699 2022-05-31 16:49:50.478626 edc-subject-model-wrappers-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      781 2021-02-05 20:38:05.000000 edc-subject-model-wrappers-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-05-31 16:49:41.000000 edc-subject-model-wrappers-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-02-05 20:38:05.000000 edc-subject-model-wrappers-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-31 16:49:50.475273 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/
--rw-r--r--   0 erikvw     (501) staff       (20)      573 2020-07-02 21:55:12.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4197 2022-05-31 16:49:41.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/appointment_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      129 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      775 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/crf_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      828 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/requisition_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      402 2020-05-15 03:17:56.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/subject_consent_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      232 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/subject_locator_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      444 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/subject_refusal_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1019 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/subject_refusal_model_wrapper_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2432 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/subject_visit_model_wrapper.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-31 16:49:50.476678 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      532 2021-02-05 20:38:05.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-31 16:49:50.477908 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      509 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)     1047 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-31 16:49:50.478349 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5263 2022-05-25 15:41:13.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/tests/test_appointment_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2072 2022-05-25 15:41:13.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/tests/test_subject_visit_model_wrapper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      380 2021-02-05 20:38:05.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3474 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/visit_schedule.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-31 16:49:50.475883 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1699 2022-05-31 16:49:50.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1959 2022-05-31 16:49:50.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-31 16:49:50.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       27 2022-05-31 16:49:50.000000 edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1613 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2269 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1227 2022-05-31 16:49:50.479189 edc-subject-model-wrappers-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:18:29.080690 edc-subject-model-wrappers-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      138 2021-02-05 20:38:05.000000 edc-subject-model-wrappers-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-05 20:38:05.000000 edc-subject-model-wrappers-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:18:29.067886 edc-subject-model-wrappers-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:18:29.072641 edc-subject-model-wrappers-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-12 12:18:20.000000 edc-subject-model-wrappers-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1235 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-12 12:18:20.000000 edc-subject-model-wrappers-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-12 12:18:20.000000 edc-subject-model-wrappers-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       88 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1828 2022-08-12 12:18:29.080824 edc-subject-model-wrappers-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      781 2021-02-05 20:38:05.000000 edc-subject-model-wrappers-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-12 12:18:20.000000 edc-subject-model-wrappers-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-12 12:18:20.000000 edc-subject-model-wrappers-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:18:29.076979 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/
+-rw-r--r--   0 erikvw     (501) staff       (20)      573 2020-07-02 21:55:12.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4115 2022-08-12 12:18:20.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/appointment_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      129 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      775 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/crf_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      828 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/requisition_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      402 2020-05-15 03:17:56.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/subject_consent_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      232 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/subject_locator_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      444 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/subject_refusal_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1019 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/subject_refusal_model_wrapper_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2432 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/subject_visit_model_wrapper.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:18:29.078790 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      532 2021-02-05 20:38:05.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:18:29.080057 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      509 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     1047 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:18:29.080457 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5258 2022-08-12 12:18:20.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/tests/test_appointment_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2072 2022-05-25 15:41:13.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/tests/test_subject_visit_model_wrapper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      380 2021-02-05 20:38:05.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3496 2022-08-12 12:18:20.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/visit_schedule.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:18:29.077898 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1828 2022-08-12 12:18:29.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1993 2022-08-12 12:18:29.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-12 12:18:29.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:21:43.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       27 2022-08-12 12:18:29.000000 edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1754 2022-08-12 12:18:20.000000 edc-subject-model-wrappers-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2269 2022-05-03 01:01:12.000000 edc-subject-model-wrappers-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1325 2022-08-12 12:18:29.081199 edc-subject-model-wrappers-0.3.9/setup.cfg
```

### Comparing `edc-subject-model-wrappers-0.3.8/.github/workflows/build.yml` & `edc-subject-model-wrappers-0.3.9/.github/workflows/build.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,70 @@
+---
 name: build
 
 on: [push, pull_request]
 
 jobs:
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.9']
-        django-version: ['3.2']
+        python-version: ['3.9', '3.10']
+        django-version: ['3.2', '4.0', '4.1', 'dev']
 
     services:
-
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
           MYSQL_ROOT_PASSWORD: mysql
         ports:
           - 3306:3306
         options: --health-cmd="mysqladmin ping" --health-interval=10s --health-timeout=5s --health-retries=3
 
     steps:
-    - name: Install pycups and words dependency
-      run: |
-        sudo apt-get install libcups2-dev wamerican
-
-    - uses: actions/checkout@v2
-
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python-version }}
-
-    - name: Get pip cache dir
-      id: pip-cache
-      run: |
-        echo "::set-output name=dir::$(pip cache dir)"
-
-    - name: Cache
-      uses: actions/cache@v2
-      with:
-        path: ${{ steps.pip-cache.outputs.dir }}
-        key:
-          ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
-        restore-keys: |
-          ${{ matrix.python-version }}-v1-
-
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        python -m pip install -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
-
-
-    - name: Tox tests
-      run: |
-        tox -v
-      env:
-        DJANGO: ${{ matrix.django-version }}
-
-    - name: Upload coverage
-      uses: codecov/codecov-action@v1
-      with:
-        name: Python ${{ matrix.python-version }}
+      - name: Install pycups and words dependency
+        run: |
+          sudo sed -i 's/azure\.//' /etc/apt/sources.list
+          sudo apt-get -y update
+          sudo apt-get install libcups2-dev wamerican
+
+      - uses: actions/checkout@v2
+
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Get pip cache dir
+        id: pip-cache
+        run: |
+          echo "::set-output name=dir::$(pip cache dir)"
+
+      - name: Cache
+        uses: actions/cache@v2
+        with:
+          path: ${{ steps.pip-cache.outputs.dir }}
+          key:
+            ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
+          restore-keys: |
+            ${{ matrix.python-version }}-v1-
+
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          python -m pip install -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
+
+
+      - name: Tox tests
+        run: |
+          tox -v
+        env:
+          DJANGO: ${{ matrix.django-version }}
+
+      - name: Upload coverage
+        uses: codecov/codecov-action@v1
+        with:
+          name: Python ${{ matrix.python-version }}
```

### Comparing `edc-subject-model-wrappers-0.3.8/.gitignore` & `edc-subject-model-wrappers-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/LICENSE` & `edc-subject-model-wrappers-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/PKG-INFO` & `edc-subject-model-wrappers-0.3.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: edc-subject-model-wrappers
-Version: 0.3.8
+Version: 0.3.9
 Summary: Subject Model wrappers for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-subject-model-wrappers
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc model wrapper dashboard classes and templates,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `edc-subject-model-wrappers-0.3.8/README.rst` & `edc-subject-model-wrappers-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/__init__.py` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/appointment_model_wrapper.py` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/appointment_model_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from decimal import Decimal
 from typing import Any
 
 from django.apps import apps as django_apps
-from django.core.exceptions import ObjectDoesNotExist
 from django.urls.base import reverse
 from edc_dashboard.url_names import url_names
 from edc_model_wrapper import ModelWrapper
 
 
 class AppointmentModelWrapperError(Exception):
     pass
```

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/crf_model_wrapper.py` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/crf_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/requisition_model_wrapper.py` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/requisition_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/subject_refusal_model_wrapper_mixin.py` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/subject_refusal_model_wrapper_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/subject_visit_model_wrapper.py` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/subject_visit_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/admin.py` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/admin.py`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/etc/user-rsa-local-private.pem` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/etc/user-rsa-restricted-private.pem` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/models.py` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/tests/test_appointment_model_wrapper.py` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/tests/test_appointment_model_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dateutil.relativedelta import relativedelta
-from django.test import TestCase, tag
+from django.test import TestCase
 from edc_dashboard.url_names import AlreadyRegistered, url_names
 from edc_facility import import_holidays
 from edc_model_wrapper import ModelWrapper, ModelWrapperModelError
 from edc_registration.models import RegisteredSubject
 from edc_utils import get_utcnow
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
```

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/tests/test_subject_visit_model_wrapper.py` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/tests/test_subject_visit_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers/tests/visit_schedule.py` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers/tests/visit_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
 schedule2 = Schedule(
     name="schedule2",
     onschedule_model="edc_subject_model_wrappers.onscheduletwo",
     offschedule_model="edc_subject_model_wrappers.offscheduletwo",
     consent_model="edc_visit_tracking.subjectconsent",
     appointment_model="edc_appointment.appointment",
+    base_timepoint=4,
 )
 
 
 visits = []
 for index in range(0, 4):
     visits.append(
         Visit(
```

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers.egg-info/PKG-INFO` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: edc-subject-model-wrappers
-Version: 0.3.8
+Version: 0.3.9
 Summary: Subject Model wrappers for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-subject-model-wrappers
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc model wrapper dashboard classes and templates,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
```

### Comparing `edc-subject-model-wrappers-0.3.8/edc_subject_model_wrappers.egg-info/SOURCES.txt` & `edc-subject-model-wrappers-0.3.9/edc_subject_model_wrappers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 .coveragerc
 .editorconfig
 .gitignore
+.pre-commit-config.yaml
+.yamllint
 AUTHORS
 CHANGES
 LICENSE
 MANIFEST.in
 README.rst
 VERSION
 codecov.yml
```

### Comparing `edc-subject-model-wrappers-0.3.8/pyproject.toml` & `edc-subject-model-wrappers-0.3.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -28,39 +28,47 @@
 skip_covered = true
 omit = ["requirements.txt"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{39}-dj{32,dev},
+    py{38,39,310}-dj{32,40,41,dev},
     lint
+
 isolated_build = true
 
 [gh-actions]
 python =
+    3.8: py38
     3.9: py39, lint
+    3.10: py310
 
 [gh-actions:env]
 DJANGO =
     3.2: dj32, lint
+    4.0: dj40
+    4.1: dj41
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
     dj32: Django>=3.2,<3.3
+    dj40: Django>=4.0,<4.1
+    dj41: Django>=4.1,<4.2
     djdev: https://github.com/django/django/tarball/main
 
 commands =
     pip install -U pip
     pip --version
+    pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
 commands =
     isort --profile=black --check --diff .
```

### Comparing `edc-subject-model-wrappers-0.3.8/runtests.py` & `edc-subject-model-wrappers-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-subject-model-wrappers-0.3.8/setup.cfg` & `edc-subject-model-wrappers-0.3.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django Edc model wrapper dashboard classes and templates, clinicedc, clinical trials
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
+	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
 python_requires = >=3.9
 zip_safe = False
 include_package_data = True
 packages = find:
@@ -34,14 +37,14 @@
 	bin*
 	edc_subject_model_wrappers.tests*
 
 [flake8]
 ignore = E226,W503,E203
 max-line-length = 95
 max-complexity = 10
-exclude = */migrations,.tox,.git,__pycache__,build,dist,.eggs
+exclude = */migrations/*,.tox,.git,__pycache__,build,dist,.eggs
 per-file-ignores = __init__.py: F401
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

