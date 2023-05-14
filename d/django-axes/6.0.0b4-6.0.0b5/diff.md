# Comparing `tmp/django-axes-6.0.0b4.tar.gz` & `tmp/django-axes-6.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-axes-6.0.0b4.tar", last modified: Sat May 13 11:11:13 2023, max compression
+gzip compressed data, was "django-axes-6.0.0b5.tar", last modified: Sun May 14 21:43:55 2023, max compression
```

## Comparing `django-axes-6.0.0b4.tar` & `django-axes-6.0.0b5.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.171756 django-axes-6.0.0b4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.163756 django-axes-6.0.0b4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.163756 django-axes-6.0.0b4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    32031 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36297 2023-05-13 11:11:13.171756 django-axes-6.0.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.163756 django-axes-6.0.0b4/axes/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.163756 django-axes-6.0.0b4/axes/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/handlers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/handlers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/handlers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/handlers/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/handlers/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.159756 django-axes-6.0.0b4/axes/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.159756 django-axes-6.0.0b4/axes/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.163756 django-axes-6.0.0b4/axes/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.159756 django-axes-6.0.0b4/axes/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.163756 django-axes-6.0.0b4/axes/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.159756 django-axes-6.0.0b4/axes/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.163756 django-axes-6.0.0b4/axes/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.159756 django-axes-6.0.0b4/axes/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.167756 django-axes-6.0.0b4/axes/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.159756 django-axes-6.0.0b4/axes/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.167756 django-axes-6.0.0b4/axes/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.167756 django-axes-6.0.0b4/axes/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.167756 django-axes-6.0.0b4/axes/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/management/commands/axes_list_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/management/commands/axes_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/management/commands/axes_reset_failure_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/management/commands/axes_reset_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/management/commands/axes_reset_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/management/commands/axes_reset_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.167756 django-axes-6.0.0b4/axes/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/migrations/0002_auto_20151217_2044.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/migrations/0003_auto_20160322_0929.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/migrations/0004_auto_20181024_1538.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/migrations/0005_remove_accessattempt_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/migrations/0006_remove_accesslog_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/migrations/0007_alter_accessattempt_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/migrations/0008_accessfailurelog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/axes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.167756 django-axes-6.0.0b4/django_axes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36297 2023-05-13 11:11:13.000000 django-axes-6.0.0b4/django_axes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-13 11:11:13.000000 django-axes-6.0.0b4/django_axes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 11:11:13.000000 django-axes-6.0.0b4/django_axes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 11:11:13.000000 django-axes-6.0.0b4/django_axes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-13 11:11:13.000000 django-axes-6.0.0b4/django_axes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-13 11:11:13.000000 django-axes-6.0.0b4/django_axes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.171756 django-axes-6.0.0b4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/10_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/1_requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/2_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/3_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/4_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/5_customization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/6_integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/7_architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/8_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/9_contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.171756 django-axes-6.0.0b4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/images/flow.png
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/requirements-qa.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 11:11:13.171756 django-axes-6.0.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:13.171756 django-axes-6.0.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_failures.py
--rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-13 11:11:00.000000 django-axes-6.0.0b4/tests/urls_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.749219 django-axes-6.0.0b5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.737218 django-axes-6.0.0b5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.737218 django-axes-6.0.0b5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    32155 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36421 2023-05-14 21:43:55.749219 django-axes-6.0.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.737218 django-axes-6.0.0b5/axes/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/handlers/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.733219 django-axes-6.0.0b5/axes/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.733219 django-axes-6.0.0b5/axes/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.733219 django-axes-6.0.0b5/axes/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.733219 django-axes-6.0.0b5/axes/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.733219 django-axes-6.0.0b5/axes/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.733219 django-axes-6.0.0b5/axes/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/axes_list_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/axes_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/axes_reset_failure_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/axes_reset_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/axes_reset_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/management/commands/axes_reset_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.741219 django-axes-6.0.0b5/axes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0002_auto_20151217_2044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0003_auto_20160322_0929.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0004_auto_20181024_1538.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0005_remove_accessattempt_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0006_remove_accesslog_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0007_alter_accessattempt_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/0008_accessfailurelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/axes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.745219 django-axes-6.0.0b5/django_axes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36421 2023-05-14 21:43:55.000000 django-axes-6.0.0b5/django_axes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-14 21:43:55.000000 django-axes-6.0.0b5/django_axes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 21:43:55.000000 django-axes-6.0.0b5/django_axes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 21:43:55.000000 django-axes-6.0.0b5/django_axes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-14 21:43:55.000000 django-axes-6.0.0b5/django_axes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-14 21:43:55.000000 django-axes-6.0.0b5/django_axes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.745219 django-axes-6.0.0b5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/10_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/1_requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/2_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/3_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/4_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/5_customization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/6_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/7_architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/8_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/9_contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.745219 django-axes-6.0.0b5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/images/flow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/requirements-qa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 21:43:55.749219 django-axes-6.0.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:55.749219 django-axes-6.0.0b5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 21:43:42.000000 django-axes-6.0.0b5/tests/urls_empty.py
```

### Comparing `django-axes-6.0.0b4/.github/workflows/codeql.yml` & `django-axes-6.0.0b5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/.github/workflows/release.yml` & `django-axes-6.0.0b5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/.github/workflows/test.yml` & `django-axes-6.0.0b5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/CHANGES.rst` & `django-axes-6.0.0b5/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 
 Changes
 =======
 
 
+6.0.0b5 (2023-05-15)
+--------------------
+
+- Deprecate ``is_admin_site`` API call with misleading naming.
+  [hirotasoshu]
+
+
 6.0.0b4 (2023-05-13)
 --------------------
 
 - Add ``AXES_LOCKOUT_PARAMETERS`` configuration flag that will supersede ``AXES_ONLY_USER_FAILURES``, ``AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP``, ``AXES_LOCK_OUT_BY_USER_OR_IP``, and ``AXES_USE_USER_AGENT`` configurations. Add deprecation warnings for old flags. See project documentation on RTD for update instructions.
   [hirotasoshu]
 - Improve translations.
   [hirotasoshu]
```

### Comparing `django-axes-6.0.0b4/CODE_OF_CONDUCT.md` & `django-axes-6.0.0b5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/CONTRIBUTING.rst` & `django-axes-6.0.0b5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/LICENSE` & `django-axes-6.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/PKG-INFO` & `django-axes-6.0.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.0b4
+Version: 6.0.0b5
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -124,14 +124,21 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
+6.0.0b5 (2023-05-15)
+--------------------
+
+- Deprecate ``is_admin_site`` API call with misleading naming.
+  [hirotasoshu]
+
+
 6.0.0b4 (2023-05-13)
 --------------------
 
 - Add ``AXES_LOCKOUT_PARAMETERS`` configuration flag that will supersede ``AXES_ONLY_USER_FAILURES``, ``AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP``, ``AXES_LOCK_OUT_BY_USER_OR_IP``, and ``AXES_USE_USER_AGENT`` configurations. Add deprecation warnings for old flags. See project documentation on RTD for update instructions.
   [hirotasoshu]
 - Improve translations.
   [hirotasoshu]
```

### Comparing `django-axes-6.0.0b4/README.rst` & `django-axes-6.0.0b5/README.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/admin.py` & `django-axes-6.0.0b5/axes/admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/apps.py` & `django-axes-6.0.0b5/axes/apps.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/attempts.py` & `django-axes-6.0.0b5/axes/attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/backends.py` & `django-axes-6.0.0b5/axes/backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/checks.py` & `django-axes-6.0.0b5/axes/checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/conf.py` & `django-axes-6.0.0b5/axes/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/decorators.py` & `django-axes-6.0.0b5/axes/decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/handlers/base.py` & `django-axes-6.0.0b5/axes/handlers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 from abc import ABC, abstractmethod
 from typing import Optional
+from warnings import warn
 
 from django.urls import reverse
 from django.urls.exceptions import NoReverseMatch
 
 from axes.conf import settings
 from axes.helpers import (
     get_failure_limit,
@@ -77,15 +78,15 @@
         This checker can implement arbitrary checks such as IP whitelisting or blacklisting,
         request frequency checking, failed attempt monitoring or similar functions.
 
         Please refer to the ``axes.handlers.database.AxesDatabaseHandler`` for the default implementation
         and inspiration on some common checks and access restrictions before writing your own implementation.
         """
 
-        if self.is_admin_site(request):
+        if settings.AXES_ONLY_ADMIN_SITE and not self.is_admin_request(request):
             return True
 
         if self.is_blacklisted(request, credentials):
             return False
 
         if self.is_whitelisted(request, credentials):
             return True
@@ -130,18 +131,49 @@
             # get_failures will have to be implemented by each specialized handler
             return self.get_failures(  # type: ignore
                 request, credentials
             ) >= get_failure_limit(request, credentials)
 
         return False
 
+    def get_admin_url(self) -> Optional[str]:
+        """
+        Returns admin url if exists, otherwise returns None
+        """
+        try:
+            return reverse("admin:index")
+        except NoReverseMatch:
+            return None
+
+    def is_admin_request(self, request) -> bool:
+        """
+        Checks that request located under admin site
+        """
+        if hasattr(request, "path"):
+            admin_url = self.get_admin_url()
+            return (
+                admin_url is not None
+                and re.match(f"^{admin_url}", request.path) is not None
+            )
+
+        return False
+
     def is_admin_site(self, request) -> bool:
         """
-        Checks if the request is for admin site.
+        Checks if the request is NOT for admin site
+        if `settings.AXES_ONLY_ADMIN_SITE` is True.
         """
+        warn(
+            (
+                "This method is deprecated and will be removed in future versions. "
+                "If you looking for method that checks if `request.path` located under "
+                "admin site, use `is_admin_request` instead."
+            ),
+            DeprecationWarning,
+        )
         if settings.AXES_ONLY_ADMIN_SITE and hasattr(request, "path"):
             try:
                 admin_url = reverse("admin:index")
             except NoReverseMatch:
                 return True
             return not re.match(f"^{admin_url}", request.path)
```

### Comparing `django-axes-6.0.0b4/axes/handlers/cache.py` & `django-axes-6.0.0b5/axes/handlers/cache.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/handlers/database.py` & `django-axes-6.0.0b5/axes/handlers/database.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/handlers/dummy.py` & `django-axes-6.0.0b5/axes/handlers/dummy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/handlers/proxy.py` & `django-axes-6.0.0b5/axes/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/handlers/test.py` & `django-axes-6.0.0b5/axes/handlers/test.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/helpers.py` & `django-axes-6.0.0b5/axes/helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/locale/ar/LC_MESSAGES/django.mo` & `django-axes-6.0.0b5/axes/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/locale/ar/LC_MESSAGES/django.po` & `django-axes-6.0.0b5/axes/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/locale/de/LC_MESSAGES/django.mo` & `django-axes-6.0.0b5/axes/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/locale/de/LC_MESSAGES/django.po` & `django-axes-6.0.0b5/axes/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/locale/pl/LC_MESSAGES/django.mo` & `django-axes-6.0.0b5/axes/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/locale/pl/LC_MESSAGES/django.po` & `django-axes-6.0.0b5/axes/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/locale/ru/LC_MESSAGES/django.mo` & `django-axes-6.0.0b5/axes/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/locale/ru/LC_MESSAGES/django.po` & `django-axes-6.0.0b5/axes/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/locale/tr/LC_MESSAGES/django.mo` & `django-axes-6.0.0b5/axes/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/locale/tr/LC_MESSAGES/django.po` & `django-axes-6.0.0b5/axes/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/management/commands/axes_reset_failure_logs.py` & `django-axes-6.0.0b5/axes/management/commands/axes_reset_failure_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/management/commands/axes_reset_ip.py` & `django-axes-6.0.0b5/axes/management/commands/axes_reset_ip.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/management/commands/axes_reset_logs.py` & `django-axes-6.0.0b5/axes/management/commands/axes_reset_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/management/commands/axes_reset_username.py` & `django-axes-6.0.0b5/axes/management/commands/axes_reset_username.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/middleware.py` & `django-axes-6.0.0b5/axes/middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/migrations/0001_initial.py` & `django-axes-6.0.0b5/axes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/migrations/0002_auto_20151217_2044.py` & `django-axes-6.0.0b5/axes/migrations/0002_auto_20151217_2044.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/migrations/0003_auto_20160322_0929.py` & `django-axes-6.0.0b5/axes/migrations/0003_auto_20160322_0929.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/migrations/0004_auto_20181024_1538.py` & `django-axes-6.0.0b5/axes/migrations/0004_auto_20181024_1538.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/migrations/0007_alter_accessattempt_unique_together.py` & `django-axes-6.0.0b5/axes/migrations/0007_alter_accessattempt_unique_together.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/migrations/0008_accessfailurelog.py` & `django-axes-6.0.0b5/axes/migrations/0008_accessfailurelog.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/models.py` & `django-axes-6.0.0b5/axes/models.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/signals.py` & `django-axes-6.0.0b5/axes/signals.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/axes/utils.py` & `django-axes-6.0.0b5/axes/utils.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/django_axes.egg-info/PKG-INFO` & `django-axes-6.0.0b5/django_axes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.0b4
+Version: 6.0.0b5
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -124,14 +124,21 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
+6.0.0b5 (2023-05-15)
+--------------------
+
+- Deprecate ``is_admin_site`` API call with misleading naming.
+  [hirotasoshu]
+
+
 6.0.0b4 (2023-05-13)
 --------------------
 
 - Add ``AXES_LOCKOUT_PARAMETERS`` configuration flag that will supersede ``AXES_ONLY_USER_FAILURES``, ``AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP``, ``AXES_LOCK_OUT_BY_USER_OR_IP``, and ``AXES_USE_USER_AGENT`` configurations. Add deprecation warnings for old flags. See project documentation on RTD for update instructions.
   [hirotasoshu]
 - Improve translations.
   [hirotasoshu]
```

### Comparing `django-axes-6.0.0b4/django_axes.egg-info/SOURCES.txt` & `django-axes-6.0.0b5/django_axes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/docs/1_requirements.rst` & `django-axes-6.0.0b5/docs/1_requirements.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/docs/2_installation.rst` & `django-axes-6.0.0b5/docs/2_installation.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/docs/3_usage.rst` & `django-axes-6.0.0b5/docs/3_usage.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/docs/4_configuration.rst` & `django-axes-6.0.0b5/docs/4_configuration.rst`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | AXES_LOCK_OUT_AT_FAILURE                             | True                                         | After the number of allowed login attempts are exceeded, should we lock out this IP (and optional user agent)?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | AXES_COOLOFF_TIME                                    | None                                         | If set, defines a period of inactivity after which  old failed login attempts will be cleared.  Can be set to a Python timedelta object, an integer, a float, a callable, or a string path to a callable which takes no arguments.  If an integer or float, will be interpreted as a number of hours:  ``AXES_COOLOFF_TIME = 2`` 2 hours,   ``AXES_COOLOFF_TIME = 2.0`` 2 hours, 120 minutes,  ``AXES_COOLOFF_TIME = 1.7`` 1.7 hours, 102 minutes, 6120 seconds                                                                                                                                                                                                                                                                           |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | AXES_ONLY_ADMIN_SITE                                 | False                                        | If ``True``, lock is only enabled for admin site. Admin site is determined by checking request path against the path of ``"admin:index"`` view. If admin urls are not registered in current urlconf, all requests will not be locked.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
-| AXES_ONLY_USER_FAILURES                              | False                                        | DEPRECATED: USE ``AXES_LOCKOUT_PARAMETERS ISNTEAD``. If ``True``, only lock based on username, and never lock based on IP if attempts exceed the limit. Otherwise utilize the existing IP and user locking logic.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| AXES_ONLY_USER_FAILURES                              | False                                        | DEPRECATED: USE ``AXES_LOCKOUT_PARAMETERS`` INSTEAD. If ``True``, only lock based on username, and never lock based on IP if attempts exceed the limit. Otherwise utilize the existing IP and user locking logic.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | AXES_ENABLE_ADMIN                                    | True                                         | If ``True``, admin views for access attempts and logins are shown in Django admin interface.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP             | False                                        | DEPRECATED: USE ``AXES_LOCKOUT_PARAMETERS`` INSTEAD. If ``True``, prevent login from IP under a particular username if the attempt limit has been exceeded, otherwise lock out based on IP.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | AXES_LOCK_OUT_BY_USER_OR_IP                          | False                                        | DEPRECATED: USE ``AXES_LOCKOUT_PARAMETERS`` INSTEAD. If ``True``, prevent login from if the attempt limit has been exceeded for IP or username.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
 +------------------------------------------------------+----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
```

### Comparing `django-axes-6.0.0b4/docs/5_customization.rst` & `django-axes-6.0.0b5/docs/5_customization.rst`

 * *Files 2% similar despite different names*

```diff
@@ -199,23 +199,23 @@
     def get_lockout_parameters(request_or_attempt, credentials):
 
         if isinstance(request_or_attempt, HttpRequest):
            is_localhost = request.META.get("REMOTE_ADDR") == "127.0.0.1"
 
         else:
            is_localhost = request_or_attempt.ip_address == "127.0.0.1"
-        
+
         if is_localhost:
-           return ["username"] 
-        
+           return ["username"]
+
         return ["ip_address", "username"]
 
 ``settings.py``::
 
-    AXES_LOCKOUT_CALLABLE = "example.utils.get_lockout_parameters"
+    AXES_LOCKOUT_PARAMETERS = "example.utils.get_lockout_parameters"
 
 This way, if client ip_address is localhost, axes will lockout client only by username. In other case, axes will lockout client by username and/or ip_address.
 
 Customizing client ip address lookups
 -------------------------------------
 
 Axes can be configured with ``AXES_CLIENT_IP_CALLABLE`` to use custom client ip address lookup logic.
@@ -223,8 +223,8 @@
 ``example/utils.py``::
 
     def get_client_ip(request):
         return request.META.get("REMOTE_ADDR")
 
 ``settings.py``::
 
-    AXES_LOCKOUT_CALLABLE = "example.utils.get_client_ip"
+    AXES_CLIENT_IP_CALLABLE = "example.utils.get_client_ip"
```

### Comparing `django-axes-6.0.0b4/docs/6_integration.rst` & `django-axes-6.0.0b5/docs/6_integration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/docs/7_architecture.rst` & `django-axes-6.0.0b5/docs/7_architecture.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/docs/Makefile` & `django-axes-6.0.0b5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/docs/conf.py` & `django-axes-6.0.0b5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/docs/images/flow.png` & `django-axes-6.0.0b5/docs/images/flow.png`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/pyproject.toml` & `django-axes-6.0.0b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/setup.py` & `django-axes-6.0.0b5/setup.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/base.py` & `django-axes-6.0.0b5/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/settings.py` & `django-axes-6.0.0b5/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/test_admin.py` & `django-axes-6.0.0b5/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/test_attempts.py` & `django-axes-6.0.0b5/tests/test_attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/test_backends.py` & `django-axes-6.0.0b5/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/test_checks.py` & `django-axes-6.0.0b5/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/test_decorators.py` & `django-axes-6.0.0b5/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/test_failures.py` & `django-axes-6.0.0b5/tests/test_failures.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/test_handlers.py` & `django-axes-6.0.0b5/tests/test_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,22 +51,44 @@
             (False, "/test/", False),
             (False, reverse("admin:index"), False),
         )
 
         for setting_value, url, expected in tests:
             with override_settings(AXES_ONLY_ADMIN_SITE=setting_value):
                 request.path = url
-                self.assertEqual(AxesProxyHandler().is_admin_site(request), expected)
+                with self.assertWarns(DeprecationWarning):
+                    self.assertEqual(AxesProxyHandler().is_admin_site(request), expected)
+
+    def test_is_admin_request(self):
+        request = MagicMock()
+        tests = (  # (URL, Expected)
+            ("/test/", False),
+            (reverse("admin:index"), True),
+        )
+
+        for url, expected in tests:
+            request.path = url
+            self.assertEqual(AxesProxyHandler().is_admin_request(request), expected)
 
     @override_settings(ROOT_URLCONF="tests.urls_empty")
     @override_settings(AXES_ONLY_ADMIN_SITE=True)
     def test_is_admin_site_no_admin_site(self):
         request = MagicMock()
         request.path = "/admin/"
-        self.assertTrue(AxesProxyHandler().is_admin_site(self.request))
+        with self.assertWarns(DeprecationWarning):
+            self.assertTrue(AxesProxyHandler().is_admin_site(self.request))
+
+    @override_settings(ROOT_URLCONF="tests.urls_empty")
+    def test_is_admin_request_no_admin_site(self):
+        request = MagicMock()
+        request.path = "/admin/"
+        self.assertFalse(AxesProxyHandler().is_admin_request(self.request))
+
+    def test_is_admin_request_no_path(self):
+        self.assertFalse(AxesProxyHandler().is_admin_request(self.request))
 
 
 class AxesProxyHandlerTestCase(AxesTestCase):
     def setUp(self):
         self.sender = MagicMock()
         self.credentials = MagicMock()
         self.request = MagicMock()
```

### Comparing `django-axes-6.0.0b4/tests/test_helpers.py` & `django-axes-6.0.0b5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/test_logging.py` & `django-axes-6.0.0b5/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/test_login.py` & `django-axes-6.0.0b5/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/test_management.py` & `django-axes-6.0.0b5/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/test_middleware.py` & `django-axes-6.0.0b5/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b4/tests/test_models.py` & `django-axes-6.0.0b5/tests/test_models.py`

 * *Files identical despite different names*

