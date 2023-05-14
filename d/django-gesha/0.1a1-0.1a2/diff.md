# Comparing `tmp/django-gesha-0.1a1.tar.gz` & `tmp/django-gesha-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-gesha-0.1a1.tar", last modified: Mon May  8 22:20:13 2023, max compression
+gzip compressed data, was "django-gesha-0.1a2.tar", last modified: Sun May 14 01:41:01 2023, max compression
```

## Comparing `django-gesha-0.1a1.tar` & `django-gesha-0.1a2.tar`

### file list

```diff
@@ -1,85 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.469610 django-gesha-0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-08 22:20:01.000000 django-gesha-0.1a1/.eslintrc.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.449609 django-gesha-0.1a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.457610 django-gesha-0.1a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-08 22:20:01.000000 django-gesha-0.1a1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-08 22:20:01.000000 django-gesha-0.1a1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-08 22:20:01.000000 django-gesha-0.1a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-08 22:20:01.000000 django-gesha-0.1a1/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-08 22:20:01.000000 django-gesha-0.1a1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-08 22:20:01.000000 django-gesha-0.1a1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 22:20:01.000000 django-gesha-0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-08 22:20:13.469610 django-gesha-0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-08 22:20:01.000000 django-gesha-0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.457610 django-gesha-0.1a1/django_gesha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-08 22:20:13.000000 django-gesha-0.1a1/django_gesha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-08 22:20:13.000000 django-gesha-0.1a1/django_gesha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:20:13.000000 django-gesha-0.1a1/django_gesha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-08 22:20:13.000000 django-gesha-0.1a1/django_gesha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 22:20:13.000000 django-gesha-0.1a1/django_gesha.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.461609 django-gesha-0.1a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:01.000000 django-gesha-0.1a1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-08 22:20:01.000000 django-gesha-0.1a1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-08 22:20:01.000000 django-gesha-0.1a1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-08 22:20:01.000000 django-gesha-0.1a1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.461609 django-gesha-0.1a1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-08 22:20:01.000000 django-gesha-0.1a1/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-08 22:20:01.000000 django-gesha-0.1a1/docs/user_guide.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.461609 django-gesha-0.1a1/gesha/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.449609 django-gesha-0.1a1/gesha/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.449609 django-gesha-0.1a1/gesha/static/gesha/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.449609 django-gesha-0.1a1/gesha/static/gesha/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.461609 django-gesha-0.1a1/gesha/static/gesha/dist/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/static/gesha/dist/js/django-gesha.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.465610 django-gesha-0.1a1/gesha/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/templatetags/gesha.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gesha/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-08 22:20:01.000000 django-gesha-0.1a1/gulpfile.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.465610 django-gesha-0.1a1/js_src/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_src/context.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_src/converters.ts
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_src/main.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_src/urls.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.465610 django-gesha-0.1a1/js_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_tests/context.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_tests/converters.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_tests/helpers.ts
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_tests/main.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_tests/test.html
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-08 22:20:01.000000 django-gesha-0.1a1/js_tests/urls.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-08 22:20:01.000000 django-gesha-0.1a1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)   342194 2023-05-08 22:20:01.000000 django-gesha-0.1a1/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-08 22:20:01.000000 django-gesha-0.1a1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-08 22:20:01.000000 django-gesha-0.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 22:20:13.469610 django-gesha-0.1a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.465610 django-gesha-0.1a1/test_project/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.469610 django-gesha-0.1a1/test_project/fake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.469610 django-gesha-0.1a1/test_project/fake/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.469610 django-gesha-0.1a1/test_project/fake/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/management/commands/printtestpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.469610 django-gesha-0.1a1/test_project/fake/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/templates/test.html
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/fake/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-05-08 22:20:01.000000 django-gesha-0.1a1/test_project/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:13.469610 django-gesha-0.1a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tests/test_jscontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tests/test_package_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 22:20:01.000000 django-gesha-0.1a1/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-14 01:40:47.000000 django-gesha-0.1a2/.eslintrc.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.672786 django-gesha-0.1a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.676786 django-gesha-0.1a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-14 01:40:47.000000 django-gesha-0.1a2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-14 01:40:47.000000 django-gesha-0.1a2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-14 01:40:47.000000 django-gesha-0.1a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-14 01:40:47.000000 django-gesha-0.1a2/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-14 01:40:47.000000 django-gesha-0.1a2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-14 01:40:47.000000 django-gesha-0.1a2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-14 01:40:47.000000 django-gesha-0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-14 01:41:01.680786 django-gesha-0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-14 01:40:47.000000 django-gesha-0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.676786 django-gesha-0.1a2/django_gesha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-14 01:41:01.000000 django-gesha-0.1a2/django_gesha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-14 01:41:01.000000 django-gesha-0.1a2/django_gesha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:41:01.000000 django-gesha-0.1a2/django_gesha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-14 01:41:01.000000 django-gesha-0.1a2/django_gesha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 01:41:01.000000 django-gesha-0.1a2/django_gesha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.676786 django-gesha-0.1a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/settings.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.676786 django-gesha-0.1a2/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-14 01:40:47.000000 django-gesha-0.1a2/docs/user_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.676786 django-gesha-0.1a2/gesha/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.672786 django-gesha-0.1a2/gesha/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.672786 django-gesha-0.1a2/gesha/static/gesha/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.672786 django-gesha-0.1a2/gesha/static/gesha/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/gesha/static/gesha/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/static/gesha/dist/js/django-gesha.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/gesha/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/templatetags/gesha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gesha/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-14 01:40:47.000000 django-gesha-0.1a2/gulpfile.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/js_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_src/context.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_src/converters.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_src/main.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_src/urls.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/js_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_tests/context.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_tests/converters.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_tests/helpers.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_tests/main.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_tests/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-14 01:40:47.000000 django-gesha-0.1a2/js_tests/urls.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-14 01:40:47.000000 django-gesha-0.1a2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   342194 2023-05-14 01:40:47.000000 django-gesha-0.1a2/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-14 01:40:47.000000 django-gesha-0.1a2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-14 01:40:47.000000 django-gesha-0.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:41:01.680786 django-gesha-0.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/test_project/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/test_project/fake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/test_project/fake/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/test_project/fake/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/management/commands/printtestpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/test_project/fake/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/templates/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/fake/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-05-14 01:40:47.000000 django-gesha-0.1a2/test_project/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:41:01.680786 django-gesha-0.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tests/test_jscontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tests/test_package_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-14 01:40:47.000000 django-gesha-0.1a2/tsconfig.json
```

### Comparing `django-gesha-0.1a1/.github/workflows/python-publish.yml` & `django-gesha-0.1a2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/.github/workflows/test.yml` & `django-gesha-0.1a2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/.gitignore` & `django-gesha-0.1a2/.gitignore`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/LICENSE` & `django-gesha-0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/PKG-INFO` & `django-gesha-0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gesha
-Version: 0.1a1
+Version: 0.1a2
 Summary: JavaScript utilities for Django projects.
 Author-email: elyas <elyas@ely.as>
 License: MIT
 Project-URL: homepage, https://django-gesha.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ely-as/django-gesha
 Project-URL: changelog, https://github.com/ely-as/django-gesha/blob/main/CHANGELOG.md
 Keywords: django,javascript
```

### Comparing `django-gesha-0.1a1/README.md` & `django-gesha-0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/django_gesha.egg-info/PKG-INFO` & `django-gesha-0.1a2/django_gesha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gesha
-Version: 0.1a1
+Version: 0.1a2
 Summary: JavaScript utilities for Django projects.
 Author-email: elyas <elyas@ely.as>
 License: MIT
 Project-URL: homepage, https://django-gesha.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ely-as/django-gesha
 Project-URL: changelog, https://github.com/ely-as/django-gesha/blob/main/CHANGELOG.md
 Keywords: django,javascript
```

### Comparing `django-gesha-0.1a1/django_gesha.egg-info/SOURCES.txt` & `django-gesha-0.1a2/django_gesha.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,23 @@
 django_gesha.egg-info/dependency_links.txt
 django_gesha.egg-info/requires.txt
 django_gesha.egg-info/top_level.txt
 docs/changelog.md
 docs/contributing.md
 docs/index.md
 docs/installation.md
+docs/settings.md
 docs/user_guide.md
 docs/stylesheets/extra.css
 gesha/__init__.py
 gesha/conf.py
 gesha/mixins.py
 gesha/types.py
 gesha/urls.py
+gesha/views.py
 gesha/static/gesha/dist/js/django-gesha.bundle.min.js
 gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map
 gesha/templatetags/__init__.py
 gesha/templatetags/gesha.py
 js_src/context.ts
 js_src/converters.ts
 js_src/main.ts
@@ -53,11 +55,12 @@
 test_project/fake/views.py
 test_project/fake/wsgi.py
 test_project/fake/management/__init__.py
 test_project/fake/management/commands/__init__.py
 test_project/fake/management/commands/printtestpage.py
 test_project/fake/templates/test.html
 tests/__init__.py
+tests/test_conf.py
 tests/test_init.py
 tests/test_jscontext.py
 tests/test_package_json.py
 tests/test_urls.py
```

### Comparing `django-gesha-0.1a1/docs/contributing.md` & `django-gesha-0.1a2/docs/contributing.md`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,22 @@
 $ tox -m py3.8 # (1)!
 ```
 
 1.  See the `labels` section in
     [`tox.ini`](https://github.com/ely-as/django-gesha/blob/main/tox.ini) for available
     Python labels.
 
+#### Run test project
+
+``` console
+$ cd test_project
+$ uvicorn fake.asgi:application --reload
+INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
+```
+
 ### TypeScript
 
 #### Lint
 
 ``` console
 $ npm run lint
 ```
```

### Comparing `django-gesha-0.1a1/docs/index.md` & `django-gesha-0.1a2/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 ---
 
 **Features:**
 
   - [Add context](user_guide/#add-context) in Django views to be used in JavaScript
     functions.
   - [Reverse URLs](user_guide/#reverse-urls) natively in JavaScript (equivalent to
-    `#!py reverse()` in Python and `#!django {% url %}` in templates).
+    `#!py reverse()` in Python and
+    <span style="white-space:nowrap;">`#!django {% url %}`</span> in templates).
   - Written in TypeScript and fully-typed Python.
 
 ---
 
 [**Documentation**](https://django-gesha.readthedocs.io/en/latest/)
 **&nbsp;•&nbsp;**
 [**Issue Tracker**](https://github.com/ely-as/django-gesha/issues)
```

### Comparing `django-gesha-0.1a1/docs/installation.md` & `django-gesha-0.1a2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/gesha/static/gesha/dist/js/django-gesha.bundle.min.js` & `django-gesha-0.1a2/gesha/static/gesha/dist/js/django-gesha.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map` & `django-gesha-0.1a2/gesha/static/gesha/dist/js/django-gesha.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/gesha/templatetags/gesha.py` & `django-gesha-0.1a2/gesha/templatetags/gesha.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/gesha/types.py` & `django-gesha-0.1a2/gesha/types.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/gulpfile.js` & `django-gesha-0.1a2/gulpfile.js`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/js_src/context.ts` & `django-gesha-0.1a2/js_src/context.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/js_src/converters.ts` & `django-gesha-0.1a2/js_src/converters.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/js_src/main.ts` & `django-gesha-0.1a2/js_src/main.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/js_src/urls.ts` & `django-gesha-0.1a2/js_src/urls.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/js_tests/converters.spec.ts` & `django-gesha-0.1a2/js_tests/converters.spec.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/js_tests/helpers.ts` & `django-gesha-0.1a2/js_tests/helpers.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/js_tests/test.html` & `django-gesha-0.1a2/js_tests/test.html`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/js_tests/urls.spec.ts` & `django-gesha-0.1a2/js_tests/urls.spec.ts`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/mkdocs.yml` & `django-gesha-0.1a2/mkdocs.yml`

 * *Files 13% similar despite different names*

```diff
@@ -25,11 +25,12 @@
   - pymdownx.tabbed:
       alternate_style: true
   - tables
 nav:
   - Home: index.md
   - Installation: installation.md
   - User Guide: user_guide.md
+  - Settings: settings.md
   - Contributing: contributing.md
   - Changelog: changelog.md
 extra_css:
   - stylesheets/extra.css
```

### Comparing `django-gesha-0.1a1/package-lock.json` & `django-gesha-0.1a2/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8999922744128555%*

 * *Differences: {"'packages'": "{'': {'version': '0.1.0-alpha2'}}", "'version'": "'0.1.0-alpha2'"}*

```diff
@@ -23,15 +23,15 @@
                 "typescript": "^5.0.4",
                 "vinyl-buffer": "^1.0.1",
                 "vinyl-source-stream": "^2.0.0",
                 "watchify": "^4.0.0"
             },
             "license": "MIT",
             "name": "django-gesha",
-            "version": "0.1.0-alpha1"
+            "version": "0.1.0-alpha2"
         },
         "node_modules/@cspotcode/source-map-support": {
             "dependencies": {
                 "@jridgewell/trace-mapping": "0.3.9"
             },
             "dev": true,
             "engines": {
@@ -9298,9 +9298,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "0.1.0-alpha1"
+    "version": "0.1.0-alpha2"
 }
```

### Comparing `django-gesha-0.1a1/package.json` & `django-gesha-0.1a2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.1.0-alpha2'"}*

```diff
@@ -37,9 +37,9 @@
         "type": "git",
         "url": "git+https://github.com/ely-as/django-gesha.git"
     },
     "scripts": {
         "lint": "eslint ./js_*/**/*.ts",
         "test": "mocha"
     },
-    "version": "0.1.0-alpha1"
+    "version": "0.1.0-alpha2"
 }
```

### Comparing `django-gesha-0.1a1/pyproject.toml` & `django-gesha-0.1a2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -60,27 +60,32 @@
     "beautifulsoup4",
     "lxml",
     "mypy",
     "pytest>=7",      # >=7 required for pythonpath option
     "pytest-cov",
     "pytest-django",
     "ruff",
+    "types-beautifulsoup4",
+    "uvicorn",
 ]
 
 [tool.coverage.run]
 omit = ["test_project/*"]
 
 [tool.mypy]
 warn_unused_configs = true
-ignore_missing_imports = true
 files = [
     "gesha/**/*.py",
     "tests/**/*.py",
 ]
 
+[[tool.mypy.overrides]]
+module = "django.*"
+ignore_missing_imports = true
+
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "fake.settings"
 pythonpath = [
   ".",
   "test_project",
 ]
```

### Comparing `django-gesha-0.1a1/test_project/fake/management/commands/printtestpage.py` & `django-gesha-0.1a2/test_project/fake/management/commands/printtestpage.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/test_project/fake/settings.py` & `django-gesha-0.1a2/test_project/fake/settings.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/test_project/manage.py` & `django-gesha-0.1a2/test_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/tests/test_package_json.py` & `django-gesha-0.1a2/tests/test_package_json.py`

 * *Files identical despite different names*

### Comparing `django-gesha-0.1a1/tox.ini` & `django-gesha-0.1a2/tox.ini`

 * *Files identical despite different names*

