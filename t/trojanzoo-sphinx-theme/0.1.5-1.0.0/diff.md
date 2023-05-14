# Comparing `tmp/trojanzoo_sphinx_theme-0.1.5.tar.gz` & `tmp/trojanzoo_sphinx_theme-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trojanzoo_sphinx_theme-0.1.5.tar", last modified: Wed Jan 11 12:19:11 2023, max compression
+gzip compressed data, was "trojanzoo_sphinx_theme-1.0.0.tar", last modified: Sun May 14 09:40:26 2023, max compression
```

## Comparing `trojanzoo_sphinx_theme-0.1.5.tar` & `trojanzoo_sphinx_theme-1.0.0.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.434750 trojanzoo_sphinx_theme-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-01-11 12:19:11.434750 trojanzoo_sphinx_theme-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.418749 trojanzoo_sphinx_theme-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.418749 trojanzoo_sphinx_theme-0.1.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/configuring.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.418749 trojanzoo_sphinx_theme-0.1.5/docs/source/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/demo/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/demo/demo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/demo/lists_tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/demo/long.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/demo/structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.422749 trojanzoo_sphinx_theme-0.1.5/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/images/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.422749 trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/trojanzoo-logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/trojanzoo-logo-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/trojanzoo-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/images/yi_jing_01_chien.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/installing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.422749 trojanzoo_sphinx_theme-0.1.5/docs/source/test_py_module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/test_py_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/test_py_module/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-01-11 12:19:11.434750 trojanzoo_sphinx_theme-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.422749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/fonts.html
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/linkcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.418749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.422749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   266305 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/css/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.418749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.426749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.426749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/
--rw-r--r--   0 runner    (1001) docker     (123)    39560 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    31812 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    32396 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    25672 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33944 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    26832 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff
--rw-r--r--   0 runner    (1001) docker     (123)    25120 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    29304 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26908 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff
--rw-r--r--   0 runner    (1001) docker     (123)    21012 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    19420 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    32072 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff
--rw-r--r--   0 runner    (1001) docker     (123)    25460 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.430750 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/
--rw-r--r--   0 runner    (1001) docker     (123)    50680 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff
--rw-r--r--   0 runner    (1001) docker     (123)    35916 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff
--rw-r--r--   0 runner    (1001) docker     (123)    36648 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    50664 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    35536 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    52936 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    37592 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.434750 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/arrow-down-orange.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/arrow-right-with-tail.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-grey.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-orange.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-right-orange.svg
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-right-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)    38907 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/home-footer-background.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/icon-close.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/search-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.434750 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    36099 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/js/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.434750 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.422749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.290729 trojanzoo_sphinx_theme-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-14 09:40:26.290729 trojanzoo_sphinx_theme-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.278729 trojanzoo_sphinx_theme-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.278729 trojanzoo_sphinx_theme-1.0.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/configuring.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.278729 trojanzoo_sphinx_theme-1.0.0/docs/source/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/demo/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/demo/demo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/demo/lists_tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/demo/long.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/demo/structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.278729 trojanzoo_sphinx_theme-1.0.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/images/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.278729 trojanzoo_sphinx_theme-1.0.0/docs/source/images/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/images/logo/trojanzoo-logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/images/logo/trojanzoo-logo-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/images/logo/trojanzoo-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/images/yi_jing_01_chien.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/installing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.282729 trojanzoo_sphinx_theme-1.0.0/docs/source/test_py_module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/test_py_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/docs/source/test_py_module/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-14 09:40:26.290729 trojanzoo_sphinx_theme-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.282729 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/fonts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/linkcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.278729 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.282729 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   266311 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/css/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.278729 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.286729 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FontAwesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.286729 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/
+-rw-r--r--   0 runner    (1001) docker     (123)    39560 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    31812 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    32396 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    25672 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33944 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    26832 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    25120 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    29304 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26908 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21012 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    19420 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    32072 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    25460 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.290729 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/
+-rw-r--r--   0 runner    (1001) docker     (123)    50680 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35916 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    36648 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    50664 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35536 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    52936 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    37592 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.290729 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/arrow-down-orange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/arrow-right-with-tail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/chevron-down-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/chevron-down-grey.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/chevron-down-orange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/chevron-down-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/chevron-right-orange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/chevron-right-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38907 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/home-footer-background.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/icon-close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/search-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.290729 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/js/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.290729 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58072 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/js/vendor/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/js/vendor/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-14 09:40:16.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:40:26.282729 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-14 09:40:26.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-14 09:40:26.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:40:26.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 09:40:26.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:40:26.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 09:40:26.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 09:40:26.000000 trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme.egg-info/top_level.txt
```

### Comparing `trojanzoo_sphinx_theme-0.1.5/LICENSE` & `trojanzoo_sphinx_theme-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/PKG-INFO` & `trojanzoo_sphinx_theme-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trojanzoo_sphinx_theme
-Version: 0.1.5
+Version: 1.0.0
 Summary: TrojanZoo Sphinx Theme
 Home-page: https://github.com/ain-soph/trojanzoo_sphinx_theme
 Author: Ren Pang
 Author-email: rbp5354@psu.edu
 License: GPL-3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Sphinx :: Theme
@@ -19,16 +19,19 @@
 Classifier: Topic :: Software Development :: Documentation
 Requires-Python: >3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TrojanZoo Sphinx Theme
 
+
+![sphinx>=7.0](https://img.shields.io/badge/sphinx->=7.0-informational.svg)
+
 [![demo](https://github.com/ain-soph/trojanzoo_sphinx_theme/workflows/demo/badge.svg)](https://ain-soph.github.io/trojanzoo_sphinx_theme/)
-[![release](https://img.shields.io/github/v/release/ain-soph/trojanzoo_sphinx_theme)](https://github.com/ain-soph/trojanzoo/releases)
+[![release](https://img.shields.io/github/v/release/ain-soph/trojanzoo_sphinx_theme)](https://github.com/ain-soph/trojanzoo_sphinx_theme/releases)
 [![pypi](https://img.shields.io/pypi/v/trojanzoo_sphinx_theme)](https://pypi.org/project/trojanzoo_sphinx_theme/)
 
 Sphinx theme for [TrojanZoo Docs](https://ain-soph.github.io/trojanzoo) based on the [Read the Docs Sphinx Theme](https://sphinx-rtd-theme.readthedocs.io/en/latest). Forked from [Pytorch Sphinx Theme](https://github.com/pytorch/pytorch_sphinx_theme) with commit `b4d0005` at 09/24/2021.
 
 ## Difference from pytorch_sphinx_theme
 This work removes all pytorch-related things and support many customizations. It also removes all other unnecessary items to make it a pure doc template.  
 See demos at:
```

### Comparing `trojanzoo_sphinx_theme-0.1.5/README.md` & `trojanzoo_sphinx_theme-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # TrojanZoo Sphinx Theme
 
+
+![sphinx>=7.0](https://img.shields.io/badge/sphinx->=7.0-informational.svg)
+
 [![demo](https://github.com/ain-soph/trojanzoo_sphinx_theme/workflows/demo/badge.svg)](https://ain-soph.github.io/trojanzoo_sphinx_theme/)
-[![release](https://img.shields.io/github/v/release/ain-soph/trojanzoo_sphinx_theme)](https://github.com/ain-soph/trojanzoo/releases)
+[![release](https://img.shields.io/github/v/release/ain-soph/trojanzoo_sphinx_theme)](https://github.com/ain-soph/trojanzoo_sphinx_theme/releases)
 [![pypi](https://img.shields.io/pypi/v/trojanzoo_sphinx_theme)](https://pypi.org/project/trojanzoo_sphinx_theme/)
 
 Sphinx theme for [TrojanZoo Docs](https://ain-soph.github.io/trojanzoo) based on the [Read the Docs Sphinx Theme](https://sphinx-rtd-theme.readthedocs.io/en/latest). Forked from [Pytorch Sphinx Theme](https://github.com/pytorch/pytorch_sphinx_theme) with commit `b4d0005` at 09/24/2021.
 
 ## Difference from pytorch_sphinx_theme
 This work removes all pytorch-related things and support many customizations. It also removes all other unnecessary items to make it a pure doc template.  
 See demos at:
```

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/make.bat` & `trojanzoo_sphinx_theme-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/conf.py` & `trojanzoo_sphinx_theme-1.0.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 # -- Extension configuration ----------------------------------------------
 
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.githubpages',
     'sphinx.ext.intersphinx',
     'sphinx.ext.linkcode',  # viewcode
+    'sphinxcontrib.jquery',
     'sphinx_copybutton',
 ]
 
 
 def linkcode_resolve(domain, info):
     return linkcode_helper(
         domain, info,
@@ -82,15 +83,15 @@
 templates_path = ['_templates']
 source_suffix = '.rst'  # ['.rst', '.md']
 root_doc = 'index'
 
 release = pkg_version
 version = release if release.find('a') == -1 else release[:release.find('a')]
 
-language = None
+language = 'en'
 exclude_patterns = []
 
 # -- General default extension configuration ------------------------------
 
 # autodoc options
 autodoc_docstring_signature = True
 autodoc_inherit_docstrings = False
```

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/configuring.rst` & `trojanzoo_sphinx_theme-1.0.0/docs/source/configuring.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/demo/api.rst` & `trojanzoo_sphinx_theme-1.0.0/docs/source/demo/api.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/demo/demo.rst` & `trojanzoo_sphinx_theme-1.0.0/docs/source/demo/demo.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/demo/lists_tables.rst` & `trojanzoo_sphinx_theme-1.0.0/docs/source/demo/lists_tables.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/demo/long.rst` & `trojanzoo_sphinx_theme-1.0.0/docs/source/demo/long.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/demo/structure.rst` & `trojanzoo_sphinx_theme-1.0.0/docs/source/demo/structure.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/images/favicon.ico` & `trojanzoo_sphinx_theme-1.0.0/docs/source/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/trojanzoo-logo-dark.svg` & `trojanzoo_sphinx_theme-1.0.0/docs/source/images/logo/trojanzoo-logo-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/trojanzoo-logo-icon.svg` & `trojanzoo_sphinx_theme-1.0.0/docs/source/images/logo/trojanzoo-logo-icon.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/trojanzoo-logo.svg` & `trojanzoo_sphinx_theme-1.0.0/docs/source/images/logo/trojanzoo-logo.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/images/yi_jing_01_chien.jpg` & `trojanzoo_sphinx_theme-1.0.0/docs/source/images/yi_jing_01_chien.jpg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/docs/source/test_py_module/test.py` & `trojanzoo_sphinx_theme-1.0.0/docs/source/test_py_module/test.py`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/setup.cfg` & `trojanzoo_sphinx_theme-1.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 universal = 1
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = trojanzoo_sphinx_theme
 install_requires = 
-	sphinx>=4.2.0,<5.2.0
-	docutils>=0.17.1
+	sphinx
+	docutils
 python_requires = >3
 
 [options.package_data]
 trojanzoo_sphinx_theme = 
 	theme.conf
 	*.html
 	static/css/*.css
```

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/__init__.py` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-from .version import __version__
+from .version import __version__  # noqa: F401
 
 from os import path
 from sphinx.util import isurl
 from sphinx.util.fileutil import copy_asset
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
```

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/breadcrumbs.html` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/fonts.html` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/fonts.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/footer.html` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/footer.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/layout.html` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/layout.html`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
   <link rel="search" type="application/opensearchdescription+xml"
     title="{% trans docstitle=docstitle|e %}Search within {{ docstitle }}{% endtrans %}"
     href="{{ pathto('_static/opensearch.xml', 1) }}" />
   {% endif %}
 
   {% endif %}
 
-  <link rel="stylesheet" href="{{ pathto('_static/' + style, 1) }}" type="text/css" />
+  <link rel="stylesheet" href="{{ pathto('_static/' + styles[-1], 1) }}" type="text/css" />
   <!-- <link rel="stylesheet" href="{{ pathto('_static/pygments.css', 1) }}" type="text/css" /> -->
   {%- for css in css_files %}
   {%- if css|attr("rel") %}
   <link rel="{{ css.rel }}" href="{{ pathto(css.filename, 1) }}" type="text/css" {% if css.title is not none %}
     title="{{ css.title }}" {% endif %} />
   {%- else %}
   <link rel="stylesheet" href="{{ pathto(css, 1) }}" type="text/css" />
```

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/linkcode.py` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/linkcode.py`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/search.html` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/css/theme.css` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/css/theme.css`

 * *Files 0% similar despite different names*

```diff
@@ -15978,668 +15978,668 @@
 0003e690: 7068 696e 782d 7465 6d70 6c61 7465 2d72  phinx-template-r
 0003e6a0: 6967 6874 2d6d 656e 7520 613a 6163 7469  ight-menu a:acti
 0003e6b0: 7665 207b 0a20 2063 7572 736f 723a 2070  ve {.  cursor: p
 0003e6c0: 6f69 6e74 6572 3b0a 7d0a 0a2e 7370 6869  ointer;.}...sphi
 0003e6d0: 6e78 2d74 656d 706c 6174 652d 6c65 6674  nx-template-left
 0003e6e0: 2d6d 656e 7520 756c 207b 0a20 2070 6164  -menu ul {.  pad
 0003e6f0: 6469 6e67 2d6c 6566 743a 2030 3b0a 7d0a  ding-left: 0;.}.
-0003e700: 0a2e 7370 6869 6e78 2d74 656d 706c 6174  ..sphinx-templat
-0003e710: 652d 7269 6768 742d 6d65 6e75 2061 3a6c  e-right-menu a:l
-0003e720: 696e 6b2c 0a2e 7370 6869 6e78 2d74 656d  ink,..sphinx-tem
-0003e730: 706c 6174 652d 7269 6768 742d 6d65 6e75  plate-right-menu
-0003e740: 2061 3a76 6973 6974 6564 2c0a 2e73 7068   a:visited,..sph
-0003e750: 696e 782d 7465 6d70 6c61 7465 2d72 6967  inx-template-rig
-0003e760: 6874 2d6d 656e 7520 613a 686f 7665 7220  ht-menu a:hover 
-0003e770: 7b0a 2020 636f 6c6f 723a 2023 3663 3663  {.  color: #6c6c
-0003e780: 3664 3b0a 7d0a 2e73 7068 696e 782d 7465  6d;.}..sphinx-te
-0003e790: 6d70 6c61 7465 2d72 6967 6874 2d6d 656e  mplate-right-men
-0003e7a0: 7520 613a 6c69 6e6b 2073 7061 6e2e 7072  u a:link span.pr
-0003e7b0: 652c 0a2e 7370 6869 6e78 2d74 656d 706c  e,..sphinx-templ
-0003e7c0: 6174 652d 7269 6768 742d 6d65 6e75 2061  ate-right-menu a
-0003e7d0: 3a76 6973 6974 6564 2073 7061 6e2e 7072  :visited span.pr
-0003e7e0: 652c 0a2e 7370 6869 6e78 2d74 656d 706c  e,..sphinx-templ
-0003e7f0: 6174 652d 7269 6768 742d 6d65 6e75 2061  ate-right-menu a
-0003e800: 3a68 6f76 6572 2073 7061 6e2e 7072 6520  :hover span.pre 
-0003e810: 7b0a 2020 636f 6c6f 723a 2023 3663 3663  {.  color: #6c6c
-0003e820: 3664 3b0a 7d0a 2e73 7068 696e 782d 7465  6d;.}..sphinx-te
-0003e830: 6d70 6c61 7465 2d72 6967 6874 2d6d 656e  mplate-right-men
-0003e840: 7520 612e 7265 6665 7265 6e63 652e 696e  u a.reference.in
-0003e850: 7465 726e 616c 2062 7574 746f 6e20 7b0a  ternal button {.
-0003e860: 2020 6469 7370 6c61 793a 2062 6c6f 636b    display: block
-0003e870: 3b0a 2020 7061 6464 696e 673a 2030 3b0a  ;.  padding: 0;.
-0003e880: 2020 626f 7264 6572 3a20 303b 0a20 206d    border: 0;.  m
-0003e890: 6172 6769 6e3a 2030 3b0a 2020 636f 6c6f  argin: 0;.  colo
-0003e8a0: 723a 2069 6e68 6572 6974 3b0a 7d0a 2e73  r: inherit;.}..s
-0003e8b0: 7068 696e 782d 7465 6d70 6c61 7465 2d72  phinx-template-r
-0003e8c0: 6967 6874 2d6d 656e 7520 612e 7265 6665  ight-menu a.refe
-0003e8d0: 7265 6e63 652e 696e 7465 726e 616c 5b61  rence.internal[a
-0003e8e0: 7269 612d 6578 7061 6e64 6564 3d22 7472  ria-expanded="tr
-0003e8f0: 7565 225d 2062 7574 746f 6e3a 6265 666f  ue"] button:befo
-0003e900: 7265 207b 0a20 2063 6f6e 7465 6e74 3a20  re {.  content: 
-0003e910: 222d 223b 0a20 2066 6f6e 742d 6661 6d69  "-";.  font-fami
-0003e920: 6c79 3a20 6d6f 6e6f 7370 6163 653b 0a20  ly: monospace;. 
-0003e930: 2070 6f73 6974 696f 6e3a 2061 6273 6f6c   position: absol
-0003e940: 7574 653b 0a20 206c 6566 743a 202d 3132  ute;.  left: -12
-0003e950: 7078 3b0a 7d0a 2e73 7068 696e 782d 7465  px;.}..sphinx-te
-0003e960: 6d70 6c61 7465 2d72 6967 6874 2d6d 656e  mplate-right-men
-0003e970: 7520 612e 7265 6665 7265 6e63 652e 696e  u a.reference.in
-0003e980: 7465 726e 616c 5b61 7269 612d 6578 7061  ternal[aria-expa
-0003e990: 6e64 6564 3d22 6661 6c73 6522 5d20 6275  nded="false"] bu
-0003e9a0: 7474 6f6e 3a62 6566 6f72 6520 7b0a 2020  tton:before {.  
-0003e9b0: 636f 6e74 656e 743a 2022 2b22 3b0a 2020  content: "+";.  
-0003e9c0: 666f 6e74 2d66 616d 696c 793a 206d 6f6e  font-family: mon
-0003e9d0: 6f73 7061 6365 3b0a 2020 706f 7369 7469  ospace;.  positi
-0003e9e0: 6f6e 3a20 6162 736f 6c75 7465 3b0a 2020  on: absolute;.  
-0003e9f0: 6c65 6674 3a20 2d31 3270 783b 0a7d 0a2e  left: -12px;.}..
-0003ea00: 7370 6869 6e78 2d74 656d 706c 6174 652d  sphinx-template-
-0003ea10: 7269 6768 742d 6d65 6e75 206c 692e 6163  right-menu li.ac
-0003ea20: 7469 7665 203e 2061 207b 0a20 2063 6f6c  tive > a {.  col
-0003ea30: 6f72 3a20 7661 7228 2d2d 7079 746f 7263  or: var(--pytorc
-0003ea40: 682d 7265 6429 3b0a 7d0a 2e73 7068 696e  h-red);.}..sphin
-0003ea50: 782d 7465 6d70 6c61 7465 2d72 6967 6874  x-template-right
-0003ea60: 2d6d 656e 7520 6c69 2e61 6374 6976 6520  -menu li.active 
-0003ea70: 3e20 6120 7370 616e 2e70 7265 2c20 2e73  > a span.pre, .s
-0003ea80: 7068 696e 782d 7465 6d70 6c61 7465 2d72  phinx-template-r
-0003ea90: 6967 6874 2d6d 656e 7520 6c69 2e61 6374  ight-menu li.act
-0003eaa0: 6976 6520 3e20 613a 6265 666f 7265 207b  ive > a:before {
-0003eab0: 0a20 2063 6f6c 6f72 3a20 7661 7228 2d2d  .  color: var(--
-0003eac0: 7079 746f 7263 682d 7265 6429 3b0a 7d0a  pytorch-red);.}.
-0003ead0: 2e73 7068 696e 782d 7465 6d70 6c61 7465  .sphinx-template
-0003eae0: 2d72 6967 6874 2d6d 656e 7520 6c69 2e61  -right-menu li.a
-0003eaf0: 6374 6976 6520 3e20 613a 6166 7465 7220  ctive > a:after 
-0003eb00: 7b0a 2020 636f 6e74 656e 743a 2022 5c32  {.  content: "\2
-0003eb10: 3032 3222 3b0a 2020 636f 6c6f 723a 2076  022";.  color: v
-0003eb20: 6172 282d 2d70 7974 6f72 6368 293b 0a20  ar(--pytorch);. 
-0003eb30: 2064 6973 706c 6179 3a20 696e 6c69 6e65   display: inline
-0003eb40: 2d62 6c6f 636b 3b0a 2020 666f 6e74 2d73  -block;.  font-s
-0003eb50: 697a 653a 2031 2e33 3735 7265 6d3b 0a20  ize: 1.375rem;. 
-0003eb60: 206c 6566 743a 202d 3137 7078 3b0a 2020   left: -17px;.  
-0003eb70: 706f 7369 7469 6f6e 3a20 6162 736f 6c75  position: absolu
-0003eb80: 7465 3b0a 2020 746f 703a 2031 7078 3b0a  te;.  top: 1px;.
-0003eb90: 7d0a 2e73 7068 696e 782d 7465 6d70 6c61  }..sphinx-templa
-0003eba0: 7465 2d72 6967 6874 2d6d 656e 7520 2e73  te-right-menu .s
-0003ebb0: 7068 696e 782d 7465 6d70 6c61 7465 2d73  phinx-template-s
-0003ebc0: 6964 652d 7363 726f 6c6c 203e 2075 6c20  ide-scroll > ul 
-0003ebd0: 3e20 6c69 203e 2075 6c20 3e20 6c69 207b  > li > ul > li {
-0003ebe0: 0a20 206d 6172 6769 6e2d 626f 7474 6f6d  .  margin-bottom
-0003ebf0: 3a20 303b 0a7d 0a2e 7370 6869 6e78 2d74  : 0;.}..sphinx-t
-0003ec00: 656d 706c 6174 652d 7269 6768 742d 6d65  emplate-right-me
-0003ec10: 6e75 2075 6c20 756c 207b 0a20 2070 6164  nu ul ul {.  pad
-0003ec20: 6469 6e67 2d6c 6566 743a 2030 3b0a 7d0a  ding-left: 0;.}.
-0003ec30: 2e73 7068 696e 782d 7465 6d70 6c61 7465  .sphinx-template
-0003ec40: 2d72 6967 6874 2d6d 656e 7520 756c 2075  -right-menu ul u
-0003ec50: 6c20 6c69 207b 0a20 2070 6164 6469 6e67  l li {.  padding
-0003ec60: 2d6c 6566 743a 2030 7078 3b0a 7d0a 2e73  -left: 0px;.}..s
-0003ec70: 7068 696e 782d 7465 6d70 6c61 7465 2d72  phinx-template-r
-0003ec80: 6967 6874 2d6d 656e 7520 756c 2075 6c20  ight-menu ul ul 
-0003ec90: 6c69 2061 2e72 6566 6572 656e 6365 2e69  li a.reference.i
-0003eca0: 6e74 6572 6e61 6c20 7b0a 2020 7061 6464  nternal {.  padd
-0003ecb0: 696e 672d 6c65 6674 3a20 303b 0a7d 0a2e  ing-left: 0;.}..
-0003ecc0: 7370 6869 6e78 2d74 656d 706c 6174 652d  sphinx-template-
-0003ecd0: 7269 6768 742d 6d65 6e75 2075 6c20 756c  right-menu ul ul
-0003ece0: 206c 6920 756c 207b 0a20 2064 6973 706c   li ul {.  displ
-0003ecf0: 6179 3a20 6e6f 6e65 3b0a 2020 7061 6464  ay: none;.  padd
-0003ed00: 696e 672d 6c65 6674 3a20 3130 7078 3b0a  ing-left: 10px;.
-0003ed10: 7d0a 2e73 7068 696e 782d 7465 6d70 6c61  }..sphinx-templa
-0003ed20: 7465 2d72 6967 6874 2d6d 656e 7520 756c  te-right-menu ul
-0003ed30: 2075 6c20 6c69 206c 6920 612e 7265 6665   ul li li a.refe
-0003ed40: 7265 6e63 652e 696e 7465 726e 616c 207b  rence.internal {
-0003ed50: 0a20 2070 6164 6469 6e67 2d6c 6566 743a  .  padding-left:
-0003ed60: 2030 3b0a 7d0a 2e73 7068 696e 782d 7465   0;.}..sphinx-te
-0003ed70: 6d70 6c61 7465 2d72 6967 6874 2d6d 656e  mplate-right-men
-0003ed80: 7520 6c69 2075 6c20 7b0a 2020 6469 7370  u li ul {.  disp
-0003ed90: 6c61 793a 2062 6c6f 636b 3b0a 7d0a 0a2e  lay: block;.}...
-0003eda0: 7370 6869 6e78 2d74 656d 706c 6174 652d  sphinx-template-
-0003edb0: 7269 6768 742d 6d65 6e75 202e 7370 6869  right-menu .sphi
-0003edc0: 6e78 2d74 656d 706c 6174 652d 7369 6465  nx-template-side
-0003edd0: 2d73 6372 6f6c 6c20 7b0a 2020 7061 6464  -scroll {.  padd
-0003ede0: 696e 672d 746f 703a 2032 3070 783b 0a7d  ing-top: 20px;.}
-0003edf0: 0a40 6d65 6469 6120 7363 7265 656e 2061  .@media screen a
-0003ee00: 6e64 2028 6d69 6e2d 7769 6474 683a 2031  nd (min-width: 1
-0003ee10: 3130 3170 7829 207b 0a20 202e 7370 6869  101px) {.  .sphi
-0003ee20: 6e78 2d74 656d 706c 6174 652d 7269 6768  nx-template-righ
-0003ee30: 742d 6d65 6e75 202e 7370 6869 6e78 2d74  t-menu .sphinx-t
-0003ee40: 656d 706c 6174 652d 7369 6465 2d73 6372  emplate-side-scr
-0003ee50: 6f6c 6c20 7b0a 2020 2020 7769 6474 683a  oll {.    width:
-0003ee60: 2031 3230 253b 0a20 207d 0a7d 0a40 6d65   120%;.  }.}.@me
-0003ee70: 6469 6120 7363 7265 656e 2061 6e64 2028  dia screen and (
-0003ee80: 6d69 6e2d 7769 6474 683a 2031 3630 3070  min-width: 1600p
-0003ee90: 7829 207b 0a20 202e 7370 6869 6e78 2d74  x) {.  .sphinx-t
-0003eea0: 656d 706c 6174 652d 7269 6768 742d 6d65  emplate-right-me
-0003eeb0: 6e75 202e 7370 6869 6e78 2d74 656d 706c  nu .sphinx-templ
-0003eec0: 6174 652d 7369 6465 2d73 6372 6f6c 6c20  ate-side-scroll 
-0003eed0: 7b0a 2020 2020 7769 6474 683a 2034 3030  {.    width: 400
-0003eee0: 7078 3b0a 2020 7d0a 7d0a 2e73 7068 696e  px;.  }.}..sphin
-0003eef0: 782d 7465 6d70 6c61 7465 2d72 6967 6874  x-template-right
-0003ef00: 2d6d 656e 7520 2e73 7068 696e 782d 7465  -menu .sphinx-te
-0003ef10: 6d70 6c61 7465 2d73 6964 652d 7363 726f  mplate-side-scro
-0003ef20: 6c6c 203e 2075 6c20 7b0a 2020 7061 6464  ll > ul {.  padd
-0003ef30: 696e 672d 6c65 6674 3a20 3130 253b 0a20  ing-left: 10%;. 
-0003ef40: 2070 6164 6469 6e67 2d72 6967 6874 3a20   padding-right: 
-0003ef50: 3130 253b 0a20 206d 6172 6769 6e2d 626f  10%;.  margin-bo
-0003ef60: 7474 6f6d 3a20 303b 0a7d 0a40 6d65 6469  ttom: 0;.}.@medi
-0003ef70: 6120 7363 7265 656e 2061 6e64 2028 6d69  a screen and (mi
-0003ef80: 6e2d 7769 6474 683a 2031 3630 3070 7829  n-width: 1600px)
-0003ef90: 207b 0a20 202e 7370 6869 6e78 2d74 656d   {.  .sphinx-tem
-0003efa0: 706c 6174 652d 7269 6768 742d 6d65 6e75  plate-right-menu
-0003efb0: 202e 7370 6869 6e78 2d74 656d 706c 6174   .sphinx-templat
-0003efc0: 652d 7369 6465 2d73 6372 6f6c 6c20 3e20  e-side-scroll > 
-0003efd0: 756c 207b 0a20 2020 2070 6164 6469 6e67  ul {.    padding
-0003efe0: 2d6c 6566 743a 2032 3570 783b 0a20 207d  -left: 25px;.  }
-0003eff0: 0a7d 0a2e 7370 6869 6e78 2d74 656d 706c  .}..sphinx-templ
-0003f000: 6174 652d 7269 6768 742d 6d65 6e75 202e  ate-right-menu .
-0003f010: 7370 6869 6e78 2d74 656d 706c 6174 652d  sphinx-template-
-0003f020: 7369 6465 2d73 6372 6f6c 6c20 3e20 756c  side-scroll > ul
-0003f030: 203e 206c 6920 3e20 612e 7265 6665 7265   > li > a.refere
-0003f040: 6e63 652e 696e 7465 726e 616c 207b 0a20  nce.internal {. 
-0003f050: 2063 6f6c 6f72 3a20 2332 3632 3632 363b   color: #262626;
-0003f060: 0a20 2066 6f6e 742d 7765 6967 6874 3a20  .  font-weight: 
-0003f070: 3530 303b 0a7d 0a2e 7370 6869 6e78 2d74  500;.}..sphinx-t
-0003f080: 656d 706c 6174 652d 7269 6768 742d 6d65  emplate-right-me
-0003f090: 6e75 202e 7370 6869 6e78 2d74 656d 706c  nu .sphinx-templ
-0003f0a0: 6174 652d 7369 6465 2d73 6372 6f6c 6c20  ate-side-scroll 
-0003f0b0: 756c 206c 6920 7b0a 2020 706f 7369 7469  ul li {.  positi
-0003f0c0: 6f6e 3a20 7265 6c61 7469 7665 3b0a 7d0a  on: relative;.}.
-0003f0d0: 0a23 7370 6869 6e78 2d74 656d 706c 6174  .#sphinx-templat
-0003f0e0: 652d 7269 6768 742d 6d65 6e75 2075 6c20  e-right-menu ul 
-0003f0f0: 6c69 2075 6c20 6c69 202e 7369 6465 2d73  li ul li .side-s
-0003f100: 6372 6f6c 6c2d 6869 6768 6c69 6768 7420  croll-highlight 
-0003f110: 7b0a 2020 636f 6c6f 723a 2076 6172 282d  {.  color: var(-
-0003f120: 2d70 7974 6f72 6368 2d72 6564 293b 0a7d  -pytorch-red);.}
-0003f130: 0a23 7370 6869 6e78 2d74 656d 706c 6174  .#sphinx-templat
-0003f140: 652d 7269 6768 742d 6d65 6e75 2075 6c20  e-right-menu ul 
-0003f150: 6c69 2075 6c20 6c69 2075 6c20 6c69 202e  li ul li ul li .
-0003f160: 7369 6465 2d73 6372 6f6c 6c2d 6869 6768  side-scroll-high
-0003f170: 6c69 6768 7420 7b0a 2020 636f 6c6f 723a  light {.  color:
-0003f180: 2076 6172 282d 2d6c 6967 6874 6e69 6e67   var(--lightning
-0003f190: 293b 0a7d 0a23 7370 6869 6e78 2d74 656d  );.}.#sphinx-tem
-0003f1a0: 706c 6174 652d 7269 6768 742d 6d65 6e75  plate-right-menu
-0003f1b0: 2075 6c20 6c69 2075 6c20 6c69 2075 6c20   ul li ul li ul 
-0003f1c0: 6c69 2075 6c20 6c69 202e 7369 6465 2d73  li ul li .side-s
-0003f1d0: 6372 6f6c 6c2d 6869 6768 6c69 6768 7420  croll-highlight 
-0003f1e0: 7b0a 2020 636f 6c6f 723a 2076 6172 282d  {.  color: var(-
-0003f1f0: 2d67 6f6f 676c 652d 6772 6565 6e29 3b0a  -google-green);.
-0003f200: 7d0a 2373 7068 696e 782d 7465 6d70 6c61  }.#sphinx-templa
-0003f210: 7465 2d72 6967 6874 2d6d 656e 7520 756c  te-right-menu ul
-0003f220: 206c 6920 756c 206c 6920 756c 206c 6920   li ul li ul li 
-0003f230: 756c 206c 6920 756c 206c 6920 2e73 6964  ul li ul li .sid
-0003f240: 652d 7363 726f 6c6c 2d68 6967 686c 6967  e-scroll-highlig
-0003f250: 6874 207b 0a20 2063 6f6c 6f72 3a20 7661  ht {.  color: va
-0003f260: 7228 2d2d 7265 6164 7468 6564 6f63 293b  r(--readthedoc);
-0003f270: 0a7d 0a0a 2e68 6561 6465 722d 636f 6e74  .}...header-cont
-0003f280: 6169 6e65 7220 7b0a 2020 6d61 782d 7769  ainer {.  max-wi
-0003f290: 6474 683a 206e 6f6e 653b 0a20 206d 6172  dth: none;.  mar
-0003f2a0: 6769 6e2d 746f 703a 2034 7078 3b0a 7d0a  gin-top: 4px;.}.
-0003f2b0: 406d 6564 6961 2073 6372 6565 6e20 616e  @media screen an
-0003f2c0: 6420 286d 696e 2d77 6964 7468 3a20 3131  d (min-width: 11
-0003f2d0: 3031 7078 2920 7b0a 2020 2e68 6561 6465  01px) {.  .heade
-0003f2e0: 722d 636f 6e74 6169 6e65 7220 7b0a 2020  r-container {.  
-0003f2f0: 2020 6d61 7267 696e 2d74 6f70 3a20 303b    margin-top: 0;
-0003f300: 0a20 207d 0a7d 0a40 6d65 6469 6120 7363  .  }.}.@media sc
-0003f310: 7265 656e 2061 6e64 2028 6d69 6e2d 7769  reen and (min-wi
-0003f320: 6474 683a 2031 3630 3070 7829 207b 0a20  dth: 1600px) {. 
-0003f330: 202e 6865 6164 6572 2d63 6f6e 7461 696e   .header-contain
-0003f340: 6572 207b 0a20 2020 206d 6172 6769 6e2d  er {.    margin-
-0003f350: 746f 703a 2030 3b0a 2020 7d0a 7d0a 0a2e  top: 0;.  }.}...
-0003f360: 636f 6e74 6169 6e65 722d 666c 7569 642e  container-fluid.
-0003f370: 6865 6164 6572 2d68 6f6c 6465 7220 7b0a  header-holder {.
-0003f380: 2020 7061 6464 696e 672d 7269 6768 743a    padding-right:
-0003f390: 2030 3b0a 2020 7061 6464 696e 672d 6c65   0;.  padding-le
-0003f3a0: 6674 3a20 303b 0a7d 0a0a 2e68 6561 6465  ft: 0;.}...heade
-0003f3b0: 722d 686f 6c64 6572 202e 636f 6e74 6169  r-holder .contai
-0003f3c0: 6e65 7220 7b0a 2020 6d61 782d 7769 6474  ner {.  max-widt
-0003f3d0: 683a 206e 6f6e 653b 0a20 2070 6164 6469  h: none;.  paddi
-0003f3e0: 6e67 2d72 6967 6874 3a20 312e 3837 3572  ng-right: 1.875r
-0003f3f0: 656d 3b0a 2020 7061 6464 696e 672d 6c65  em;.  padding-le
-0003f400: 6674 3a20 312e 3837 3572 656d 3b0a 7d0a  ft: 1.875rem;.}.
-0003f410: 406d 6564 6961 2073 6372 6565 6e20 616e  @media screen an
-0003f420: 6420 286d 696e 2d77 6964 7468 3a20 3131  d (min-width: 11
-0003f430: 3031 7078 2920 7b0a 2020 2e68 6561 6465  01px) {.  .heade
-0003f440: 722d 686f 6c64 6572 202e 636f 6e74 6169  r-holder .contai
-0003f450: 6e65 7220 7b0a 2020 2020 7061 6464 696e  ner {.    paddin
-0003f460: 672d 7269 6768 743a 2031 2e38 3735 7265  g-right: 1.875re
-0003f470: 6d3b 0a20 2020 2070 6164 6469 6e67 2d6c  m;.    padding-l
-0003f480: 6566 743a 2031 2e38 3735 7265 6d3b 0a20  eft: 1.875rem;. 
-0003f490: 207d 0a7d 0a0a 2e68 6561 6465 722d 686f   }.}...header-ho
-0003f4a0: 6c64 6572 202e 6d61 696e 2d6d 656e 7520  lder .main-menu 
-0003f4b0: 7b0a 2020 2d77 6562 6b69 742d 626f 782d  {.  -webkit-box-
-0003f4c0: 7061 636b 3a20 756e 7365 743b 0a20 2020  pack: unset;.   
-0003f4d0: 2020 202d 6d73 2d66 6c65 782d 7061 636b     -ms-flex-pack
-0003f4e0: 3a20 756e 7365 743b 0a20 2020 2020 2020  : unset;.       
-0003f4f0: 2020 206a 7573 7469 6679 2d63 6f6e 7465     justify-conte
-0003f500: 6e74 3a20 756e 7365 743b 0a20 2070 6f73  nt: unset;.  pos
-0003f510: 6974 696f 6e3a 2072 656c 6174 6976 653b  ition: relative;
-0003f520: 0a7d 0a40 6d65 6469 6120 7363 7265 656e  .}.@media screen
-0003f530: 2061 6e64 2028 6d69 6e2d 7769 6474 683a   and (min-width:
-0003f540: 2031 3130 3170 7829 207b 0a20 202e 6865   1101px) {.  .he
-0003f550: 6164 6572 2d68 6f6c 6465 7220 2e6d 6169  ader-holder .mai
-0003f560: 6e2d 6d65 6e75 2075 6c20 7b0a 2020 2020  n-menu ul {.    
-0003f570: 7061 6464 696e 672d 6c65 6674 3a20 303b  padding-left: 0;
-0003f580: 0a20 2020 206d 6172 6769 6e2d 6c65 6674  .    margin-left
-0003f590: 3a20 3236 253b 0a20 207d 0a7d 0a40 6d65  : 26%;.  }.}.@me
-0003f5a0: 6469 6120 7363 7265 656e 2061 6e64 2028  dia screen and (
-0003f5b0: 6d69 6e2d 7769 6474 683a 2031 3630 3070  min-width: 1600p
-0003f5c0: 7829 207b 0a20 202e 6865 6164 6572 2d68  x) {.  .header-h
-0003f5d0: 6f6c 6465 7220 2e6d 6169 6e2d 6d65 6e75  older .main-menu
-0003f5e0: 2075 6c20 7b0a 2020 2020 7061 6464 696e   ul {.    paddin
-0003f5f0: 672d 6c65 6674 3a20 3338 7078 3b0a 2020  g-left: 38px;.  
-0003f600: 2020 6d61 7267 696e 2d6c 6566 743a 2033    margin-left: 3
-0003f610: 3130 7078 3b0a 2020 7d0a 7d0a 0a2e 7370  10px;.  }.}...sp
-0003f620: 6869 6e78 2d74 656d 706c 6174 652d 7061  hinx-template-pa
-0003f630: 6765 2d6c 6576 656c 2d62 6172 207b 0a20  ge-level-bar {. 
-0003f640: 2064 6973 706c 6179 3a20 6e6f 6e65 3b0a   display: none;.
-0003f650: 2020 2d77 6562 6b69 742d 626f 782d 616c    -webkit-box-al
-0003f660: 6967 6e3a 2063 656e 7465 723b 0a20 2020  ign: center;.   
-0003f670: 2020 202d 6d73 2d66 6c65 782d 616c 6967     -ms-flex-alig
-0003f680: 6e3a 2063 656e 7465 723b 0a20 2020 2020  n: center;.     
-0003f690: 2020 2020 2061 6c69 676e 2d69 7465 6d73       align-items
-0003f6a0: 3a20 6365 6e74 6572 3b0a 2020 6261 636b  : center;.  back
-0003f6b0: 6772 6f75 6e64 2d63 6f6c 6f72 3a20 2366  ground-color: #f
-0003f6c0: 6666 6666 663b 0a20 2062 6f72 6465 722d  fffff;.  border-
-0003f6d0: 626f 7474 6f6d 3a20 3170 7820 736f 6c69  bottom: 1px soli
-0003f6e0: 6420 2365 3265 3265 323b 0a20 2077 6964  d #e2e2e2;.  wid
-0003f6f0: 7468 3a20 3130 3025 3b0a 2020 7a2d 696e  th: 100%;.  z-in
-0003f700: 6465 783a 2032 3031 3b0a 7d0a 406d 6564  dex: 201;.}.@med
-0003f710: 6961 2073 6372 6565 6e20 616e 6420 286d  ia screen and (m
-0003f720: 696e 2d77 6964 7468 3a20 3131 3031 7078  in-width: 1101px
-0003f730: 2920 7b0a 2020 2e73 7068 696e 782d 7465  ) {.  .sphinx-te
-0003f740: 6d70 6c61 7465 2d70 6167 652d 6c65 7665  mplate-page-leve
-0003f750: 6c2d 6261 7220 7b0a 2020 2020 6c65 6674  l-bar {.    left
-0003f760: 3a20 303b 0a20 2020 2064 6973 706c 6179  : 0;.    display
-0003f770: 3a20 2d77 6562 6b69 742d 626f 783b 0a20  : -webkit-box;. 
-0003f780: 2020 2064 6973 706c 6179 3a20 2d6d 732d     display: -ms-
-0003f790: 666c 6578 626f 783b 0a20 2020 2064 6973  flexbox;.    dis
-0003f7a0: 706c 6179 3a20 666c 6578 3b0a 2020 2020  play: flex;.    
-0003f7b0: 6865 6967 6874 3a20 3435 7078 3b0a 2020  height: 45px;.  
-0003f7c0: 2020 7061 6464 696e 672d 6c65 6674 3a20    padding-left: 
-0003f7d0: 303b 0a20 2020 2077 6964 7468 3a20 3130  0;.    width: 10
-0003f7e0: 3025 3b0a 2020 2020 706f 7369 7469 6f6e  0%;.    position
-0003f7f0: 3a20 6162 736f 6c75 7465 3b0a 2020 2020  : absolute;.    
-0003f800: 7a2d 696e 6465 783a 2031 3b0a 2020 7d0a  z-index: 1;.  }.
-0003f810: 2020 2e73 7068 696e 782d 7465 6d70 6c61    .sphinx-templa
-0003f820: 7465 2d70 6167 652d 6c65 7665 6c2d 6261  te-page-level-ba
-0003f830: 722e 6c65 6674 2d6d 656e 752d 6973 2d66  r.left-menu-is-f
-0003f840: 6978 6564 207b 0a20 2020 2070 6f73 6974  ixed {.    posit
-0003f850: 696f 6e3a 2066 6978 6564 3b0a 2020 2020  ion: fixed;.    
-0003f860: 746f 703a 2030 3b0a 2020 2020 6c65 6674  top: 0;.    left
-0003f870: 3a20 3235 253b 0a20 2020 2070 6164 6469  : 25%;.    paddi
-0003f880: 6e67 2d6c 6566 743a 2030 3b0a 2020 2020  ng-left: 0;.    
-0003f890: 7269 6768 743a 2030 3b0a 2020 2020 7769  right: 0;.    wi
-0003f8a0: 6474 683a 2037 3525 3b0a 2020 7d0a 7d0a  dth: 75%;.  }.}.
-0003f8b0: 406d 6564 6961 2073 6372 6565 6e20 616e  @media screen an
-0003f8c0: 6420 286d 696e 2d77 6964 7468 3a20 3136  d (min-width: 16
-0003f8d0: 3030 7078 2920 7b0a 2020 2e73 7068 696e  00px) {.  .sphin
-0003f8e0: 782d 7465 6d70 6c61 7465 2d70 6167 652d  x-template-page-
-0003f8f0: 6c65 7665 6c2d 6261 7220 7b0a 2020 2020  level-bar {.    
-0003f900: 6c65 6674 3a20 303b 0a20 2020 2072 6967  left: 0;.    rig
-0003f910: 6874 3a20 303b 0a20 2020 2077 6964 7468  ht: 0;.    width
-0003f920: 3a20 6175 746f 3b0a 2020 2020 7a2d 696e  : auto;.    z-in
-0003f930: 6465 783a 2031 3b0a 2020 7d0a 2020 2e73  dex: 1;.  }.  .s
-0003f940: 7068 696e 782d 7465 6d70 6c61 7465 2d70  phinx-template-p
-0003f950: 6167 652d 6c65 7665 6c2d 6261 722e 6c65  age-level-bar.le
-0003f960: 6674 2d6d 656e 752d 6973 2d66 6978 6564  ft-menu-is-fixed
-0003f970: 207b 0a20 2020 206c 6566 743a 2033 3530   {.    left: 350
-0003f980: 7078 3b0a 2020 2020 7269 6768 743a 2030  px;.    right: 0
-0003f990: 3b0a 2020 2020 7769 6474 683a 2061 7574  ;.    width: aut
-0003f9a0: 6f3b 0a20 207d 0a7d 0a2e 7370 6869 6e78  o;.  }.}..sphinx
-0003f9b0: 2d74 656d 706c 6174 652d 7061 6765 2d6c  -template-page-l
-0003f9c0: 6576 656c 2d62 6172 2075 6c2c 202e 7370  evel-bar ul, .sp
-0003f9d0: 6869 6e78 2d74 656d 706c 6174 652d 7061  hinx-template-pa
-0003f9e0: 6765 2d6c 6576 656c 2d62 6172 206c 6920  ge-level-bar li 
-0003f9f0: 7b0a 2020 6d61 7267 696e 3a20 303b 0a7d  {.  margin: 0;.}
-0003fa00: 0a0a 2e73 7068 696e 782d 7465 6d70 6c61  ...sphinx-templa
-0003fa10: 7465 2d73 686f 7274 6375 7473 2d77 7261  te-shortcuts-wra
-0003fa20: 7070 6572 207b 0a20 2064 6973 706c 6179  pper {.  display
-0003fa30: 3a20 6e6f 6e65 3b0a 7d0a 406d 6564 6961  : none;.}.@media
-0003fa40: 2073 6372 6565 6e20 616e 6420 286d 696e   screen and (min
-0003fa50: 2d77 6964 7468 3a20 3131 3031 7078 2920  -width: 1101px) 
-0003fa60: 7b0a 2020 2e73 7068 696e 782d 7465 6d70  {.  .sphinx-temp
-0003fa70: 6c61 7465 2d73 686f 7274 6375 7473 2d77  late-shortcuts-w
-0003fa80: 7261 7070 6572 207b 0a20 2020 2066 6f6e  rapper {.    fon
-0003fa90: 742d 7369 7a65 3a20 302e 3837 3572 656d  t-size: 0.875rem
-0003faa0: 3b0a 2020 2020 666c 6f61 743a 206c 6566  ;.    float: lef
-0003fab0: 743b 0a20 2020 206d 6172 6769 6e2d 6c65  t;.    margin-le
-0003fac0: 6674 3a20 3225 3b0a 2020 7d0a 7d0a 406d  ft: 2%;.  }.}.@m
-0003fad0: 6564 6961 2073 6372 6565 6e20 616e 6420  edia screen and 
-0003fae0: 286d 696e 2d77 6964 7468 3a20 3136 3030  (min-width: 1600
-0003faf0: 7078 2920 7b0a 2020 2e73 7068 696e 782d  px) {.  .sphinx-
-0003fb00: 7465 6d70 6c61 7465 2d73 686f 7274 6375  template-shortcu
-0003fb10: 7473 2d77 7261 7070 6572 207b 0a20 2020  ts-wrapper {.   
-0003fb20: 206d 6172 6769 6e2d 6c65 6674 3a20 312e   margin-left: 1.
-0003fb30: 3837 3572 656d 3b0a 2020 7d0a 7d0a 0a2e  875rem;.  }.}...
-0003fb40: 636f 6f6b 6965 2d62 616e 6e65 722d 7772  cookie-banner-wr
-0003fb50: 6170 7065 7220 7b0a 2020 6469 7370 6c61  apper {.  displa
-0003fb60: 793a 206e 6f6e 653b 0a7d 0a2e 636f 6f6b  y: none;.}..cook
-0003fb70: 6965 2d62 616e 6e65 722d 7772 6170 7065  ie-banner-wrappe
-0003fb80: 7220 2e63 6f6e 7461 696e 6572 207b 0a20  r .container {. 
-0003fb90: 2070 6164 6469 6e67 2d6c 6566 743a 2031   padding-left: 1
-0003fba0: 2e38 3735 7265 6d3b 0a20 2070 6164 6469  .875rem;.  paddi
-0003fbb0: 6e67 2d72 6967 6874 3a20 312e 3837 3572  ng-right: 1.875r
-0003fbc0: 656d 3b0a 2020 6d61 782d 7769 6474 683a  em;.  max-width:
-0003fbd0: 2031 3234 3070 783b 0a7d 0a2e 636f 6f6b   1240px;.}..cook
-0003fbe0: 6965 2d62 616e 6e65 722d 7772 6170 7065  ie-banner-wrappe
-0003fbf0: 722e 6973 2d76 6973 6962 6c65 207b 0a20  r.is-visible {. 
-0003fc00: 2064 6973 706c 6179 3a20 626c 6f63 6b3b   display: block;
-0003fc10: 0a20 2070 6f73 6974 696f 6e3a 2066 6978  .  position: fix
-0003fc20: 6564 3b0a 2020 626f 7474 6f6d 3a20 303b  ed;.  bottom: 0;
-0003fc30: 0a20 2062 6163 6b67 726f 756e 642d 636f  .  background-co
-0003fc40: 6c6f 723a 2023 6633 6634 6637 3b0a 2020  lor: #f3f4f7;.  
-0003fc50: 6d69 6e2d 6865 6967 6874 3a20 3130 3070  min-height: 100p
-0003fc60: 783b 0a20 2077 6964 7468 3a20 3130 3025  x;.  width: 100%
-0003fc70: 3b0a 2020 7a2d 696e 6465 783a 2034 3031  ;.  z-index: 401
-0003fc80: 3b0a 2020 626f 7264 6572 2d74 6f70 3a20  ;.  border-top: 
-0003fc90: 3370 7820 736f 6c69 6420 2365 6465 6465  3px solid #edede
-0003fca0: 653b 0a7d 0a2e 636f 6f6b 6965 2d62 616e  e;.}..cookie-ban
-0003fcb0: 6e65 722d 7772 6170 7065 7220 2e67 6470  ner-wrapper .gdp
-0003fcc0: 722d 6e6f 7469 6365 207b 0a20 2063 6f6c  r-notice {.  col
-0003fcd0: 6f72 3a20 2336 6336 6336 643b 0a20 206d  or: #6c6c6d;.  m
-0003fce0: 6172 6769 6e2d 746f 703a 2031 2e35 3632  argin-top: 1.562
-0003fcf0: 3572 656d 3b0a 2020 7465 7874 2d61 6c69  5rem;.  text-ali
-0003fd00: 676e 3a20 6c65 6674 3b0a 2020 6d61 782d  gn: left;.  max-
-0003fd10: 7769 6474 683a 2031 3434 3070 783b 0a7d  width: 1440px;.}
-0003fd20: 0a40 6d65 6469 6120 7363 7265 656e 2061  .@media screen a
-0003fd30: 6e64 2028 6d69 6e2d 7769 6474 683a 2037  nd (min-width: 7
-0003fd40: 3638 7078 2920 7b0a 2020 2e63 6f6f 6b69  68px) {.  .cooki
-0003fd50: 652d 6261 6e6e 6572 2d77 7261 7070 6572  e-banner-wrapper
-0003fd60: 202e 6764 7072 2d6e 6f74 6963 6520 7b0a   .gdpr-notice {.
-0003fd70: 2020 2020 7769 6474 683a 2037 3725 3b0a      width: 77%;.
-0003fd80: 2020 7d0a 7d0a 406d 6564 6961 2028 6d69    }.}.@media (mi
-0003fd90: 6e2d 7769 6474 683a 2037 3638 7078 2920  n-width: 768px) 
-0003fda0: 616e 6420 286d 6178 2d77 6964 7468 3a20  and (max-width: 
-0003fdb0: 3132 3339 7078 2920 7b0a 2020 2e63 6f6f  1239px) {.  .coo
-0003fdc0: 6b69 652d 6261 6e6e 6572 2d77 7261 7070  kie-banner-wrapp
-0003fdd0: 6572 202e 6764 7072 2d6e 6f74 6963 6520  er .gdpr-notice 
-0003fde0: 7b0a 2020 2020 7769 6474 683a 2069 6e68  {.    width: inh
-0003fdf0: 6572 6974 3b0a 2020 7d0a 7d0a 2e63 6f6f  erit;.  }.}..coo
-0003fe00: 6b69 652d 6261 6e6e 6572 2d77 7261 7070  kie-banner-wrapp
-0003fe10: 6572 202e 6764 7072 2d6e 6f74 6963 6520  er .gdpr-notice 
-0003fe20: 2e63 6f6f 6b69 652d 706f 6c69 6379 2d6c  .cookie-policy-l
-0003fe30: 696e 6b20 7b0a 2020 636f 6c6f 723a 2023  ink {.  color: #
-0003fe40: 3334 3334 3334 3b0a 7d0a 2e63 6f6f 6b69  343434;.}..cooki
-0003fe50: 652d 6261 6e6e 6572 2d77 7261 7070 6572  e-banner-wrapper
-0003fe60: 202e 636c 6f73 652d 6275 7474 6f6e 207b   .close-button {
-0003fe70: 0a20 202d 7765 626b 6974 2d61 7070 6561  .  -webkit-appea
-0003fe80: 7261 6e63 653a 206e 6f6e 653b 0a20 2020  rance: none;.   
-0003fe90: 2020 2d6d 6f7a 2d61 7070 6561 7261 6e63    -moz-appearanc
-0003fea0: 653a 206e 6f6e 653b 0a20 2020 2020 2020  e: none;.       
-0003feb0: 2020 2061 7070 6561 7261 6e63 653a 206e     appearance: n
-0003fec0: 6f6e 653b 0a20 2062 6163 6b67 726f 756e  one;.  backgroun
-0003fed0: 643a 2074 7261 6e73 7061 7265 6e74 3b0a  d: transparent;.
-0003fee0: 2020 626f 7264 6572 3a20 3170 7820 736f    border: 1px so
-0003fef0: 6c69 6420 2366 3366 3466 373b 0a20 2068  lid #f3f4f7;.  h
-0003ff00: 6569 6768 743a 2031 2e33 3132 3572 656d  eight: 1.3125rem
-0003ff10: 3b0a 2020 706f 7369 7469 6f6e 3a20 6162  ;.  position: ab
-0003ff20: 736f 6c75 7465 3b0a 2020 626f 7474 6f6d  solute;.  bottom
-0003ff30: 3a20 3432 7078 3b0a 2020 7269 6768 743a  : 42px;.  right:
-0003ff40: 2030 3b0a 2020 746f 703a 2030 3b0a 2020   0;.  top: 0;.  
-0003ff50: 6375 7273 6f72 3a20 706f 696e 7465 723b  cursor: pointer;
-0003ff60: 0a20 206f 7574 6c69 6e65 3a20 6e6f 6e65  .  outline: none
-0003ff70: 3b0a 7d0a 406d 6564 6961 2073 6372 6565  ;.}.@media scree
-0003ff80: 6e20 616e 6420 286d 696e 2d77 6964 7468  n and (min-width
-0003ff90: 3a20 3736 3870 7829 207b 0a20 202e 636f  : 768px) {.  .co
-0003ffa0: 6f6b 6965 2d62 616e 6e65 722d 7772 6170  okie-banner-wrap
-0003ffb0: 7065 7220 2e63 6c6f 7365 2d62 7574 746f  per .close-butto
-0003ffc0: 6e20 7b0a 2020 2020 7269 6768 743a 2032  n {.    right: 2
-0003ffd0: 3025 3b0a 2020 2020 746f 703a 2069 6e68  0%;.    top: inh
-0003ffe0: 6572 6974 3b0a 2020 7d0a 7d0a 406d 6564  erit;.  }.}.@med
-0003fff0: 6961 2028 6d69 6e2d 7769 6474 683a 2037  ia (min-width: 7
-00040000: 3638 7078 2920 616e 6420 286d 6178 2d77  68px) and (max-w
-00040010: 6964 7468 3a20 3132 3339 7078 2920 7b0a  idth: 1239px) {.
-00040020: 2020 2e63 6f6f 6b69 652d 6261 6e6e 6572    .cookie-banner
-00040030: 2d77 7261 7070 6572 202e 636c 6f73 652d  -wrapper .close-
-00040040: 6275 7474 6f6e 207b 0a20 2020 2072 6967  button {.    rig
-00040050: 6874 3a20 303b 0a20 2020 2074 6f70 3a20  ht: 0;.    top: 
-00040060: 303b 0a20 207d 0a7d 0a0a 2e6d 6169 6e2d  0;.  }.}...main-
-00040070: 6d65 6e75 2075 6c20 6c69 202e 7265 736f  menu ul li .reso
-00040080: 7572 6365 732d 6472 6f70 646f 776e 2061  urces-dropdown a
-00040090: 207b 0a20 2063 7572 736f 723a 2070 6f69   {.  cursor: poi
-000400a0: 6e74 6572 3b0a 7d0a 2e6d 6169 6e2d 6d65  nter;.}..main-me
-000400b0: 6e75 2075 6c20 6c69 202e 6472 6f70 646f  nu ul li .dropdo
-000400c0: 776e 2d6d 656e 7520 7b0a 2020 626f 7264  wn-menu {.  bord
-000400d0: 6572 2d72 6164 6975 733a 2030 3b0a 2020  er-radius: 0;.  
-000400e0: 7061 6464 696e 673a 2030 3b0a 7d0a 2e6d  padding: 0;.}..m
-000400f0: 6169 6e2d 6d65 6e75 2075 6c20 6c69 202e  ain-menu ul li .
-00040100: 6472 6f70 646f 776e 2d6d 656e 7520 2e64  dropdown-menu .d
-00040110: 726f 7064 6f77 6e2d 6974 656d 207b 0a20  ropdown-item {. 
-00040120: 2063 6f6c 6f72 3a20 2336 6336 6336 643b   color: #6c6c6d;
-00040130: 0a20 2062 6f72 6465 722d 626f 7474 6f6d  .  border-bottom
-00040140: 3a20 3170 7820 736f 6c69 6420 2365 3265  : 1px solid #e2e
-00040150: 3265 323b 0a7d 0a2e 6d61 696e 2d6d 656e  2e2;.}..main-men
-00040160: 7520 756c 206c 6920 2e64 726f 7064 6f77  u ul li .dropdow
-00040170: 6e2d 6d65 6e75 202e 6472 6f70 646f 776e  n-menu .dropdown
-00040180: 2d69 7465 6d3a 6c61 7374 2d6f 662d 7479  -item:last-of-ty
-00040190: 7065 207b 0a20 2062 6f72 6465 722d 626f  pe {.  border-bo
-000401a0: 7474 6f6d 2d63 6f6c 6f72 3a20 7472 616e  ttom-color: tran
-000401b0: 7370 6172 656e 743b 0a7d 0a2e 6d61 696e  sparent;.}..main
-000401c0: 2d6d 656e 7520 756c 206c 6920 2e64 726f  -menu ul li .dro
-000401d0: 7064 6f77 6e2d 6d65 6e75 202e 6472 6f70  pdown-menu .drop
-000401e0: 646f 776e 2d69 7465 6d3a 686f 7665 7220  down-item:hover 
-000401f0: 7b0a 2020 6261 636b 6772 6f75 6e64 2d63  {.  background-c
-00040200: 6f6c 6f72 3a20 7661 7228 2d2d 7079 746f  olor: var(--pyto
-00040210: 7263 6829 3b0a 7d0a 2e6d 6169 6e2d 6d65  rch);.}..main-me
-00040220: 6e75 2075 6c20 6c69 202e 6472 6f70 646f  nu ul li .dropdo
-00040230: 776e 2d6d 656e 7520 2e64 726f 7064 6f77  wn-menu .dropdow
-00040240: 6e2d 6974 656d 2070 207b 0a20 2066 6f6e  n-item p {.  fon
-00040250: 742d 7369 7a65 3a20 3172 656d 3b0a 2020  t-size: 1rem;.  
-00040260: 636f 6c6f 723a 2023 3937 3937 3937 3b0a  color: #979797;.
-00040270: 7d0a 2e6d 6169 6e2d 6d65 6e75 2075 6c20  }..main-menu ul 
-00040280: 6c69 202e 6472 6f70 646f 776e 2d6d 656e  li .dropdown-men
-00040290: 7520 612e 6472 6f70 646f 776e 2d69 7465  u a.dropdown-ite
-000402a0: 6d3a 686f 7665 7220 7b0a 2020 636f 6c6f  m:hover {.  colo
-000402b0: 723a 2023 6666 6666 6666 3b0a 7d0a 2e6d  r: #ffffff;.}..m
-000402c0: 6169 6e2d 6d65 6e75 2075 6c20 6c69 202e  ain-menu ul li .
-000402d0: 6472 6f70 646f 776e 2d6d 656e 7520 612e  dropdown-menu a.
-000402e0: 6472 6f70 646f 776e 2d69 7465 6d3a 686f  dropdown-item:ho
-000402f0: 7665 7220 7020 7b0a 2020 636f 6c6f 723a  ver p {.  color:
-00040300: 2023 6666 6666 6666 3b0a 7d0a 0a2e 7265   #ffffff;.}...re
-00040310: 736f 7572 6365 732d 6472 6f70 646f 776e  sources-dropdown
-00040320: 2d6d 656e 7520 7b0a 2020 6c65 6674 3a20  -menu {.  left: 
-00040330: 2d37 3570 783b 0a20 2077 6964 7468 3a20  -75px;.  width: 
-00040340: 3232 3670 783b 0a20 2064 6973 706c 6179  226px;.  display
-00040350: 3a20 6e6f 6e65 3b0a 2020 706f 7369 7469  : none;.  positi
-00040360: 6f6e 3a20 6162 736f 6c75 7465 3b0a 2020  on: absolute;.  
-00040370: 7a2d 696e 6465 783a 2031 3030 303b 0a20  z-index: 1000;. 
-00040380: 2064 6973 706c 6179 3a20 6e6f 6e65 3b0a   display: none;.
-00040390: 2020 666c 6f61 743a 206c 6566 743b 0a20    float: left;. 
-000403a0: 206d 696e 2d77 6964 7468 3a20 3130 7265   min-width: 10re
-000403b0: 6d3b 0a20 2070 6164 6469 6e67 3a20 302e  m;.  padding: 0.
-000403c0: 3572 656d 2030 3b0a 2020 666f 6e74 2d73  5rem 0;.  font-s
-000403d0: 697a 653a 2031 7265 6d3b 0a20 2063 6f6c  ize: 1rem;.  col
-000403e0: 6f72 3a20 2332 3132 3532 393b 0a20 2074  or: #212529;.  t
-000403f0: 6578 742d 616c 6967 6e3a 206c 6566 743b  ext-align: left;
-00040400: 0a20 206c 6973 742d 7374 796c 653a 206e  .  list-style: n
-00040410: 6f6e 653b 0a20 2062 6163 6b67 726f 756e  one;.  backgroun
-00040420: 642d 636f 6c6f 723a 2023 6666 6666 6666  d-color: #ffffff
-00040430: 3b0a 2020 6261 636b 6772 6f75 6e64 2d63  ;.  background-c
-00040440: 6c69 703a 2070 6164 6469 6e67 2d62 6f78  lip: padding-box
-00040450: 3b0a 2020 626f 7264 6572 3a20 3170 7820  ;.  border: 1px 
-00040460: 736f 6c69 6420 7267 6261 2830 2c20 302c  solid rgba(0, 0,
-00040470: 2030 2c20 302e 3135 293b 0a20 2062 6f72   0, 0.15);.  bor
-00040480: 6465 722d 7261 6469 7573 3a20 302e 3235  der-radius: 0.25
-00040490: 7265 6d3b 0a7d 0a0a 2e72 6573 6f75 7263  rem;.}...resourc
-000404a0: 6573 2d64 726f 7064 6f77 6e3a 686f 7665  es-dropdown:hove
-000404b0: 7220 2e72 6573 6f75 7263 6573 2d64 726f  r .resources-dro
-000404c0: 7064 6f77 6e2d 6d65 6e75 207b 0a20 2064  pdown-menu {.  d
-000404d0: 6973 706c 6179 3a20 626c 6f63 6b3b 0a7d  isplay: block;.}
-000404e0: 0a0a 2e6d 6169 6e2d 6d65 6e75 2075 6c20  ...main-menu ul 
-000404f0: 6c69 202e 7265 736f 7572 6365 732d 6472  li .resources-dr
-00040500: 6f70 646f 776e 2d6d 656e 7520 7b0a 2020  opdown-menu {.  
-00040510: 626f 7264 6572 2d72 6164 6975 733a 2030  border-radius: 0
-00040520: 3b0a 2020 7061 6464 696e 673a 2030 3b0a  ;.  padding: 0;.
-00040530: 7d0a 2e6d 6169 6e2d 6d65 6e75 2075 6c20  }..main-menu ul 
-00040540: 6c69 2e61 6374 6976 653a 686f 7665 7220  li.active:hover 
-00040550: 2e72 6573 6f75 7263 6573 2d64 726f 7064  .resources-dropd
-00040560: 6f77 6e2d 6d65 6e75 207b 0a20 2064 6973  own-menu {.  dis
-00040570: 706c 6179 3a20 626c 6f63 6b3b 0a7d 0a0a  play: block;.}..
-00040580: 2e6d 6169 6e2d 6d65 6e75 2075 6c20 6c69  .main-menu ul li
-00040590: 202e 7265 736f 7572 6365 732d 6472 6f70   .resources-drop
-000405a0: 646f 776e 2d6d 656e 7520 2e64 726f 7064  down-menu .dropd
-000405b0: 6f77 6e2d 6974 656d 207b 0a20 2063 6f6c  own-item {.  col
-000405c0: 6f72 3a20 2336 6336 6336 643b 0a20 2062  or: #6c6c6d;.  b
-000405d0: 6f72 6465 722d 626f 7474 6f6d 3a20 3170  order-bottom: 1p
-000405e0: 7820 736f 6c69 6420 2365 3265 3265 323b  x solid #e2e2e2;
-000405f0: 0a7d 0a0a 2e72 6573 6f75 7263 6573 2d64  .}...resources-d
-00040600: 726f 7064 6f77 6e20 2e77 6974 682d 646f  ropdown .with-do
-00040610: 776e 2d6f 7261 6e67 652d 6172 726f 7720  wn-orange-arrow 
-00040620: 7b0a 2020 7061 6464 696e 672d 7269 6768  {.  padding-righ
-00040630: 743a 2032 7265 6d3b 0a20 2070 6f73 6974  t: 2rem;.  posit
-00040640: 696f 6e3a 2072 656c 6174 6976 653b 0a20  ion: relative;. 
-00040650: 2062 6163 6b67 726f 756e 643a 2075 726c   background: url
-00040660: 2822 2e2e 2f69 6d61 6765 732f 6368 6576  ("../images/chev
-00040670: 726f 6e2d 646f 776e 2d6f 7261 6e67 652e  ron-down-orange.
-00040680: 7376 6722 293b 0a20 2062 6163 6b67 726f  svg");.  backgro
-00040690: 756e 642d 7369 7a65 3a20 3134 7078 2031  und-size: 14px 1
-000406a0: 3870 783b 0a20 2062 6163 6b67 726f 756e  8px;.  backgroun
-000406b0: 642d 706f 7369 7469 6f6e 3a20 746f 7020  d-position: top 
-000406c0: 3770 7820 7269 6768 7420 3130 7078 3b0a  7px right 10px;.
-000406d0: 2020 6261 636b 6772 6f75 6e64 2d72 6570    background-rep
-000406e0: 6561 743a 206e 6f2d 7265 7065 6174 3b0a  eat: no-repeat;.
-000406f0: 7d0a 0a2e 7769 7468 2d64 6f77 6e2d 6172  }...with-down-ar
-00040700: 726f 7720 7b0a 2020 7061 6464 696e 672d  row {.  padding-
-00040710: 7269 6768 743a 2032 7265 6d3b 0a20 2070  right: 2rem;.  p
-00040720: 6f73 6974 696f 6e3a 2072 656c 6174 6976  osition: relativ
-00040730: 653b 0a20 2062 6163 6b67 726f 756e 642d  e;.  background-
-00040740: 696d 6167 653a 2075 726c 2822 2e2e 2f69  image: url("../i
-00040750: 6d61 6765 732f 6368 6576 726f 6e2d 646f  mages/chevron-do
-00040760: 776e 2d62 6c61 636b 2e73 7667 2229 3b0a  wn-black.svg");.
-00040770: 2020 6261 636b 6772 6f75 6e64 2d73 697a    background-siz
-00040780: 653a 2031 3470 7820 3138 7078 3b0a 2020  e: 14px 18px;.  
-00040790: 6261 636b 6772 6f75 6e64 2d70 6f73 6974  background-posit
-000407a0: 696f 6e3a 2074 6f70 2037 7078 2072 6967  ion: top 7px rig
-000407b0: 6874 2031 3070 783b 0a20 2062 6163 6b67  ht 10px;.  backg
-000407c0: 726f 756e 642d 7265 7065 6174 3a20 6e6f  round-repeat: no
-000407d0: 2d72 6570 6561 743b 0a7d 0a2e 7769 7468  -repeat;.}..with
-000407e0: 2d64 6f77 6e2d 6172 726f 773a 686f 7665  -down-arrow:hove
-000407f0: 7220 7b0a 2020 6261 636b 6772 6f75 6e64  r {.  background
-00040800: 2d69 6d61 6765 3a20 7572 6c28 222e 2e2f  -image: url("../
-00040810: 696d 6167 6573 2f63 6865 7672 6f6e 2d64  images/chevron-d
-00040820: 6f77 6e2d 6f72 616e 6765 2e73 7667 2229  own-orange.svg")
-00040830: 3b0a 2020 6261 636b 6772 6f75 6e64 2d72  ;.  background-r
-00040840: 6570 6561 743a 206e 6f2d 7265 7065 6174  epeat: no-repeat
-00040850: 3b0a 7d0a 0a2e 6865 6164 6572 2d68 6f6c  ;.}...header-hol
-00040860: 6465 7220 2e6d 6169 6e2d 6d65 6e75 2075  der .main-menu u
-00040870: 6c20 6c69 202e 7265 736f 7572 6365 732d  l li .resources-
-00040880: 6472 6f70 646f 776e 202e 646f 632d 6472  dropdown .doc-dr
-00040890: 6f70 646f 776e 2d6f 7074 696f 6e20 7b0a  opdown-option {.
-000408a0: 2020 7061 6464 696e 672d 746f 703a 2031    padding-top: 1
-000408b0: 7265 6d3b 0a7d 0a0a 2e68 6561 6465 722d  rem;.}...header-
-000408c0: 686f 6c64 6572 202e 6d61 696e 2d6d 656e  holder .main-men
-000408d0: 7520 756c 206c 6920 612e 6e61 762d 6472  u ul li a.nav-dr
-000408e0: 6f70 646f 776e 2d69 7465 6d20 7b0a 2020  opdown-item {.  
-000408f0: 6469 7370 6c61 793a 2062 6c6f 636b 3b0a  display: block;.
-00040900: 2020 666f 6e74 2d73 697a 653a 2031 7265    font-size: 1re
-00040910: 6d3b 0a20 206c 696e 652d 6865 6967 6874  m;.  line-height
-00040920: 3a20 312e 3331 3235 7265 6d3b 0a20 2077  : 1.3125rem;.  w
-00040930: 6964 7468 3a20 3130 3025 3b0a 2020 7061  idth: 100%;.  pa
-00040940: 6464 696e 673a 2030 2e32 3572 656d 2031  dding: 0.25rem 1
-00040950: 2e35 7265 6d3b 0a20 2063 6c65 6172 3a20  .5rem;.  clear: 
-00040960: 626f 7468 3b0a 2020 666f 6e74 2d77 6569  both;.  font-wei
-00040970: 6768 743a 2034 3030 3b0a 2020 636f 6c6f  ght: 400;.  colo
-00040980: 723a 2023 3937 3937 3937 3b0a 2020 7465  r: #979797;.  te
-00040990: 7874 2d61 6c69 676e 3a20 6365 6e74 6572  xt-align: center
-000409a0: 3b0a 2020 6261 636b 6772 6f75 6e64 2d63  ;.  background-c
-000409b0: 6f6c 6f72 3a20 7472 616e 7370 6172 656e  olor: transparen
-000409c0: 743b 0a20 2062 6f72 6465 722d 626f 7474  t;.  border-bott
-000409d0: 6f6d 3a20 3170 7820 736f 6c69 6420 2365  om: 1px solid #e
-000409e0: 3265 3265 323b 0a7d 0a2e 6865 6164 6572  2e2e2;.}..header
-000409f0: 2d68 6f6c 6465 7220 2e6d 6169 6e2d 6d65  -holder .main-me
-00040a00: 6e75 2075 6c20 6c69 2061 2e6e 6176 2d64  nu ul li a.nav-d
-00040a10: 726f 7064 6f77 6e2d 6974 656d 2e61 6374  ropdown-item.act
-00040a20: 6976 653a 6265 666f 7265 207b 0a20 2063  ive:before {.  c
-00040a30: 6f6e 7465 6e74 3a20 225c 4630 4133 223b  ontent: "\F0A3";
-00040a40: 0a20 2066 6f6e 742d 6661 6d69 6c79 3a20  .  font-family: 
-00040a50: 466f 6e74 4177 6573 6f6d 653b 0a20 2063  FontAwesome;.  c
-00040a60: 6f6c 6f72 3a20 7661 7228 2d2d 6c69 6768  olor: var(--ligh
-00040a70: 746e 696e 6729 3b0a 2020 7061 6464 696e  tning);.  paddin
-00040a80: 673a 2030 2e35 7265 6d20 3072 656d 3b0a  g: 0.5rem 0rem;.
-00040a90: 2020 666f 6e74 2d73 697a 653a 2031 2e33    font-size: 1.3
-00040aa0: 7265 6d3b 0a20 206c 6566 743a 2033 7078  rem;.  left: 3px
-00040ab0: 3b0a 2020 706f 7369 7469 6f6e 3a20 6162  ;.  position: ab
-00040ac0: 736f 6c75 7465 3b0a 2020 7465 7874 2d61  solute;.  text-a
-00040ad0: 6c69 676e 3a20 6c65 6674 3b0a 7d0a 2e68  lign: left;.}..h
-00040ae0: 6561 6465 722d 686f 6c64 6572 202e 6d61  eader-holder .ma
-00040af0: 696e 2d6d 656e 7520 756c 206c 6920 612e  in-menu ul li a.
-00040b00: 6e61 762d 6472 6f70 646f 776e 2d69 7465  nav-dropdown-ite
-00040b10: 6d2e 6163 7469 7665 3a68 6f76 6572 3a62  m.active:hover:b
-00040b20: 6566 6f72 6520 7b0a 2020 636f 6c6f 723a  efore {.  color:
-00040b30: 2076 6172 282d 2d67 6f6f 676c 652d 6772   var(--google-gr
-00040b40: 6565 6e29 3b0a 7d0a 2e68 6561 6465 722d  een);.}..header-
-00040b50: 686f 6c64 6572 202e 6d61 696e 2d6d 656e  holder .main-men
-00040b60: 7520 756c 206c 6920 612e 6e61 762d 6472  u ul li a.nav-dr
-00040b70: 6f70 646f 776e 2d69 7465 6d3a 6c61 7374  opdown-item:last
-00040b80: 2d6f 662d 7479 7065 207b 0a20 2062 6f72  -of-type {.  bor
-00040b90: 6465 722d 626f 7474 6f6d 2d63 6f6c 6f72  der-bottom-color
-00040ba0: 3a20 7472 616e 7370 6172 656e 743b 0a7d  : transparent;.}
-00040bb0: 0a2e 6865 6164 6572 2d68 6f6c 6465 7220  ..header-holder 
-00040bc0: 2e6d 6169 6e2d 6d65 6e75 2075 6c20 6c69  .main-menu ul li
-00040bd0: 2061 2e6e 6176 2d64 726f 7064 6f77 6e2d   a.nav-dropdown-
-00040be0: 6974 656d 3a68 6f76 6572 207b 0a20 2062  item:hover {.  b
-00040bf0: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-00040c00: 2076 6172 282d 2d70 7974 6f72 6368 293b   var(--pytorch);
-00040c10: 0a20 2063 6f6c 6f72 3a20 7768 6974 653b  .  color: white;
-00040c20: 0a7d 0a2e 6865 6164 6572 2d68 6f6c 6465  .}..header-holde
-00040c30: 7220 2e6d 6169 6e2d 6d65 6e75 2075 6c20  r .main-menu ul 
-00040c40: 6c69 2061 2e6e 6176 2d64 726f 7064 6f77  li a.nav-dropdow
-00040c50: 6e2d 6974 656d 202e 6472 6f70 646f 776e  n-item .dropdown
-00040c60: 2d74 6974 6c65 207b 0a20 2066 6f6e 742d  -title {.  font-
-00040c70: 7369 7a65 3a20 312e 3132 3572 656d 3b0a  size: 1.125rem;.
-00040c80: 2020 636f 6c6f 723a 2023 3663 3663 3664    color: #6c6c6d
-00040c90: 3b0a 2020 6c65 7474 6572 2d73 7061 6369  ;.  letter-spaci
-00040ca0: 6e67 3a20 303b 0a20 206c 696e 652d 6865  ng: 0;.  line-he
-00040cb0: 6967 6874 3a20 3334 7078 3b0a 7d0a 0a2e  ight: 34px;.}...
-00040cc0: 6865 6164 6572 2d68 6f6c 6465 7220 2e6d  header-holder .m
-00040cd0: 6169 6e2d 6d65 6e75 2075 6c20 6c69 2061  ain-menu ul li a
-00040ce0: 2e6e 6176 2d64 726f 7064 6f77 6e2d 6974  .nav-dropdown-it
-00040cf0: 656d 3a68 6f76 6572 202e 6472 6f70 646f  em:hover .dropdo
-00040d00: 776e 2d74 6974 6c65 207b 0a20 2062 6163  wn-title {.  bac
-00040d10: 6b67 726f 756e 642d 636f 6c6f 723a 2076  kground-color: v
-00040d20: 6172 282d 2d70 7974 6f72 6368 293b 0a20  ar(--pytorch);. 
-00040d30: 2063 6f6c 6f72 3a20 7768 6974 653b 0a7d   color: white;.}
-00040d40: 0a0a 2e66 613a 6265 666f 7265 207b 0a20  ...fa:before {. 
-00040d50: 2066 6f6e 742d 6661 6d69 6c79 3a20 466f   font-family: Fo
-00040d60: 6e74 4177 6573 6f6d 653b 0a20 2064 6973  ntAwesome;.  dis
-00040d70: 706c 6179 3a20 696e 6c69 6e65 2d62 6c6f  play: inline-blo
-00040d80: 636b 3b0a 2020 666f 6e74 2d73 7479 6c65  ck;.  font-style
-00040d90: 3a20 6e6f 726d 616c 3b0a 2020 666f 6e74  : normal;.  font
-00040da0: 2d77 6569 6768 743a 2034 3030 3b0a 2020  -weight: 400;.  
-00040db0: 666f 6e74 2d73 697a 653a 2069 6e68 6572  font-size: inher
-00040dc0: 6974 3b0a 2020 6c69 6e65 2d68 6569 6768  it;.  line-heigh
-00040dd0: 743a 2031 3b0a 2020 7061 6464 696e 672d  t: 1;.  padding-
-00040de0: 7269 6768 743a 2032 7078 3b0a 7d0a 2e66  right: 2px;.}..f
-00040df0: 612d 626c 6163 6b3a 6265 666f 7265 207b  a-black:before {
-00040e00: 0a20 2063 6f6c 6f72 3a20 2762 6c61 636b  .  color: 'black
-00040e10: 273b 0a7d 0a2e 6661 2d62 6c75 653a 6265  ';.}..fa-blue:be
-00040e20: 666f 7265 207b 0a20 2063 6f6c 6f72 3a20  fore {.  color: 
-00040e30: 7661 7228 2d2d 7265 6164 7468 6564 6f63  var(--readthedoc
-00040e40: 293b 0a7d 0a2e 6661 2d6c 6172 6765 3a62  );.}..fa-large:b
-00040e50: 6566 6f72 6520 7b0a 2020 666f 6e74 2d73  efore {.  font-s
-00040e60: 697a 653a 206c 6172 6765 3b0a 7d0a 2e66  ize: large;.}..f
-00040e70: 612e 6661 2d68 6f6d 653a 6265 666f 7265  a.fa-home:before
-00040e80: 207b 0a20 2063 6f6e 7465 6e74 3a20 225c   {.  content: "\
-00040e90: 4630 3135 223b 0a7d 0a2e 6661 2e66 612d  F015";.}..fa.fa-
-00040ea0: 6769 7468 7562 3a62 6566 6f72 6520 7b0a  github:before {.
-00040eb0: 2020 636f 6e74 656e 743a 2022 5c46 3039    content: "\F09
-00040ec0: 4222 3b0a 7d0a 2e66 612e 6661 2d61 7272  B";.}..fa.fa-arr
-00040ed0: 6f77 2d63 6972 636c 652d 6c65 6674 3a62  ow-circle-left:b
-00040ee0: 6566 6f72 6520 7b0a 2020 636f 6e74 656e  efore {.  conten
-00040ef0: 743a 2022 5c46 3041 3822 3b0a 7d0a 2e66  t: "\F0A8";.}..f
-00040f00: 612e 6661 2d61 7272 6f77 2d63 6972 636c  a.fa-arrow-circl
-00040f10: 652d 7269 6768 743a 6265 666f 7265 207b  e-right:before {
-00040f20: 0a20 2063 6f6e 7465 6e74 3a20 225c 4630  .  content: "\F0
-00040f30: 4139 223b 0a7d 0a0a 2e74 6f63 7472 6565  A9";.}...toctree
-00040f40: 2d77 7261 7070 6572 202e 746f 6374 7265  -wrapper .toctre
-00040f50: 652d 6c32 2061 207b 0a20 2063 6f6c 6f72  e-l2 a {.  color
-00040f60: 3a20 7661 7228 2d2d 6c69 6768 746e 696e  : var(--lightnin
-00040f70: 6729 3b0a 7d0a 2e74 6f63 7472 6565 2d77  g);.}..toctree-w
-00040f80: 7261 7070 6572 202e 746f 6374 7265 652d  rapper .toctree-
-00040f90: 6c32 202e 746f 6374 7265 652d 6c33 2061  l2 .toctree-l3 a
-00040fa0: 207b 0a20 2063 6f6c 6f72 3a20 7661 7228   {.  color: var(
-00040fb0: 2d2d 676f 6f67 6c65 2d67 7265 656e 293b  --google-green);
-00040fc0: 0a7d 0a2e 746f 6374 7265 652d 7772 6170  .}..toctree-wrap
-00040fd0: 7065 7220 2e74 6f63 7472 6565 2d6c 3220  per .toctree-l2 
-00040fe0: 2e74 6f63 7472 6565 2d6c 3320 2e74 6f63  .toctree-l3 .toc
-00040ff0: 7472 6565 2d6c 3420 6120 7b0a 2020 636f  tree-l4 a {.  co
-00041000: 6c6f 723a 2076 6172 282d 2d72 6561 6474  lor: var(--readt
-00041010: 6865 646f 6329 3b0a 7d0a 0a2f 2a23 2073  hedoc);.}../*# s
-00041020: 6f75 7263 654d 6170 7069 6e67 5552 4c3d  ourceMappingURL=
-00041030: 7468 656d 652e 6373 732e 6d61 7020 2a2f  theme.css.map */
-00041040: 0a                                       .
+0003e700: 0a2f 2a20 2e73 7068 696e 782d 7465 6d70  ./* .sphinx-temp
+0003e710: 6c61 7465 2d72 6967 6874 2d6d 656e 7520  late-right-menu 
+0003e720: 613a 6c69 6e6b 2c0a 2e73 7068 696e 782d  a:link,..sphinx-
+0003e730: 7465 6d70 6c61 7465 2d72 6967 6874 2d6d  template-right-m
+0003e740: 656e 7520 613a 7669 7369 7465 642c 0a2e  enu a:visited,..
+0003e750: 7370 6869 6e78 2d74 656d 706c 6174 652d  sphinx-template-
+0003e760: 7269 6768 742d 6d65 6e75 2061 3a68 6f76  right-menu a:hov
+0003e770: 6572 207b 0a20 2063 6f6c 6f72 3a20 2336  er {.  color: #6
+0003e780: 6336 6336 643b 0a7d 0a2e 7370 6869 6e78  c6c6d;.}..sphinx
+0003e790: 2d74 656d 706c 6174 652d 7269 6768 742d  -template-right-
+0003e7a0: 6d65 6e75 2061 3a6c 696e 6b20 7370 616e  menu a:link span
+0003e7b0: 2e70 7265 2c0a 2e73 7068 696e 782d 7465  .pre,..sphinx-te
+0003e7c0: 6d70 6c61 7465 2d72 6967 6874 2d6d 656e  mplate-right-men
+0003e7d0: 7520 613a 7669 7369 7465 6420 7370 616e  u a:visited span
+0003e7e0: 2e70 7265 2c0a 2e73 7068 696e 782d 7465  .pre,..sphinx-te
+0003e7f0: 6d70 6c61 7465 2d72 6967 6874 2d6d 656e  mplate-right-men
+0003e800: 7520 613a 686f 7665 7220 7370 616e 2e70  u a:hover span.p
+0003e810: 7265 207b 0a20 2063 6f6c 6f72 3a20 2336  re {.  color: #6
+0003e820: 6336 6336 643b 0a7d 202a 2f0a 2e73 7068  c6c6d;.} */..sph
+0003e830: 696e 782d 7465 6d70 6c61 7465 2d72 6967  inx-template-rig
+0003e840: 6874 2d6d 656e 7520 612e 7265 6665 7265  ht-menu a.refere
+0003e850: 6e63 652e 696e 7465 726e 616c 2062 7574  nce.internal but
+0003e860: 746f 6e20 7b0a 2020 6469 7370 6c61 793a  ton {.  display:
+0003e870: 2062 6c6f 636b 3b0a 2020 7061 6464 696e   block;.  paddin
+0003e880: 673a 2030 3b0a 2020 626f 7264 6572 3a20  g: 0;.  border: 
+0003e890: 303b 0a20 206d 6172 6769 6e3a 2030 3b0a  0;.  margin: 0;.
+0003e8a0: 2020 636f 6c6f 723a 2069 6e68 6572 6974    color: inherit
+0003e8b0: 3b0a 7d0a 2e73 7068 696e 782d 7465 6d70  ;.}..sphinx-temp
+0003e8c0: 6c61 7465 2d72 6967 6874 2d6d 656e 7520  late-right-menu 
+0003e8d0: 612e 7265 6665 7265 6e63 652e 696e 7465  a.reference.inte
+0003e8e0: 726e 616c 5b61 7269 612d 6578 7061 6e64  rnal[aria-expand
+0003e8f0: 6564 3d22 7472 7565 225d 2062 7574 746f  ed="true"] butto
+0003e900: 6e3a 6265 666f 7265 207b 0a20 2063 6f6e  n:before {.  con
+0003e910: 7465 6e74 3a20 222d 223b 0a20 2066 6f6e  tent: "-";.  fon
+0003e920: 742d 6661 6d69 6c79 3a20 6d6f 6e6f 7370  t-family: monosp
+0003e930: 6163 653b 0a20 2070 6f73 6974 696f 6e3a  ace;.  position:
+0003e940: 2061 6273 6f6c 7574 653b 0a20 206c 6566   absolute;.  lef
+0003e950: 743a 202d 3132 7078 3b0a 7d0a 2e73 7068  t: -12px;.}..sph
+0003e960: 696e 782d 7465 6d70 6c61 7465 2d72 6967  inx-template-rig
+0003e970: 6874 2d6d 656e 7520 612e 7265 6665 7265  ht-menu a.refere
+0003e980: 6e63 652e 696e 7465 726e 616c 5b61 7269  nce.internal[ari
+0003e990: 612d 6578 7061 6e64 6564 3d22 6661 6c73  a-expanded="fals
+0003e9a0: 6522 5d20 6275 7474 6f6e 3a62 6566 6f72  e"] button:befor
+0003e9b0: 6520 7b0a 2020 636f 6e74 656e 743a 2022  e {.  content: "
+0003e9c0: 2b22 3b0a 2020 666f 6e74 2d66 616d 696c  +";.  font-famil
+0003e9d0: 793a 206d 6f6e 6f73 7061 6365 3b0a 2020  y: monospace;.  
+0003e9e0: 706f 7369 7469 6f6e 3a20 6162 736f 6c75  position: absolu
+0003e9f0: 7465 3b0a 2020 6c65 6674 3a20 2d31 3270  te;.  left: -12p
+0003ea00: 783b 0a7d 0a2e 7370 6869 6e78 2d74 656d  x;.}..sphinx-tem
+0003ea10: 706c 6174 652d 7269 6768 742d 6d65 6e75  plate-right-menu
+0003ea20: 206c 692e 6163 7469 7665 203e 2061 207b   li.active > a {
+0003ea30: 0a20 2063 6f6c 6f72 3a20 7661 7228 2d2d  .  color: var(--
+0003ea40: 7079 746f 7263 682d 7265 6429 3b0a 7d0a  pytorch-red);.}.
+0003ea50: 2e73 7068 696e 782d 7465 6d70 6c61 7465  .sphinx-template
+0003ea60: 2d72 6967 6874 2d6d 656e 7520 6c69 2e61  -right-menu li.a
+0003ea70: 6374 6976 6520 3e20 6120 7370 616e 2e70  ctive > a span.p
+0003ea80: 7265 2c20 2e73 7068 696e 782d 7465 6d70  re, .sphinx-temp
+0003ea90: 6c61 7465 2d72 6967 6874 2d6d 656e 7520  late-right-menu 
+0003eaa0: 6c69 2e61 6374 6976 6520 3e20 613a 6265  li.active > a:be
+0003eab0: 666f 7265 207b 0a20 2063 6f6c 6f72 3a20  fore {.  color: 
+0003eac0: 7661 7228 2d2d 7079 746f 7263 682d 7265  var(--pytorch-re
+0003ead0: 6429 3b0a 7d0a 2e73 7068 696e 782d 7465  d);.}..sphinx-te
+0003eae0: 6d70 6c61 7465 2d72 6967 6874 2d6d 656e  mplate-right-men
+0003eaf0: 7520 6c69 2e61 6374 6976 6520 3e20 613a  u li.active > a:
+0003eb00: 6166 7465 7220 7b0a 2020 636f 6e74 656e  after {.  conten
+0003eb10: 743a 2022 5c32 3032 3222 3b0a 2020 636f  t: "\2022";.  co
+0003eb20: 6c6f 723a 2076 6172 282d 2d70 7974 6f72  lor: var(--pytor
+0003eb30: 6368 293b 0a20 2064 6973 706c 6179 3a20  ch);.  display: 
+0003eb40: 696e 6c69 6e65 2d62 6c6f 636b 3b0a 2020  inline-block;.  
+0003eb50: 666f 6e74 2d73 697a 653a 2031 2e33 3735  font-size: 1.375
+0003eb60: 7265 6d3b 0a20 206c 6566 743a 202d 3137  rem;.  left: -17
+0003eb70: 7078 3b0a 2020 706f 7369 7469 6f6e 3a20  px;.  position: 
+0003eb80: 6162 736f 6c75 7465 3b0a 2020 746f 703a  absolute;.  top:
+0003eb90: 2031 7078 3b0a 7d0a 2e73 7068 696e 782d   1px;.}..sphinx-
+0003eba0: 7465 6d70 6c61 7465 2d72 6967 6874 2d6d  template-right-m
+0003ebb0: 656e 7520 2e73 7068 696e 782d 7465 6d70  enu .sphinx-temp
+0003ebc0: 6c61 7465 2d73 6964 652d 7363 726f 6c6c  late-side-scroll
+0003ebd0: 203e 2075 6c20 3e20 6c69 203e 2075 6c20   > ul > li > ul 
+0003ebe0: 3e20 6c69 207b 0a20 206d 6172 6769 6e2d  > li {.  margin-
+0003ebf0: 626f 7474 6f6d 3a20 303b 0a7d 0a2e 7370  bottom: 0;.}..sp
+0003ec00: 6869 6e78 2d74 656d 706c 6174 652d 7269  hinx-template-ri
+0003ec10: 6768 742d 6d65 6e75 2075 6c20 756c 207b  ght-menu ul ul {
+0003ec20: 0a20 2070 6164 6469 6e67 2d6c 6566 743a  .  padding-left:
+0003ec30: 2030 3b0a 7d0a 2e73 7068 696e 782d 7465   0;.}..sphinx-te
+0003ec40: 6d70 6c61 7465 2d72 6967 6874 2d6d 656e  mplate-right-men
+0003ec50: 7520 756c 2075 6c20 6c69 207b 0a20 2070  u ul ul li {.  p
+0003ec60: 6164 6469 6e67 2d6c 6566 743a 2030 7078  adding-left: 0px
+0003ec70: 3b0a 7d0a 2e73 7068 696e 782d 7465 6d70  ;.}..sphinx-temp
+0003ec80: 6c61 7465 2d72 6967 6874 2d6d 656e 7520  late-right-menu 
+0003ec90: 756c 2075 6c20 6c69 2061 2e72 6566 6572  ul ul li a.refer
+0003eca0: 656e 6365 2e69 6e74 6572 6e61 6c20 7b0a  ence.internal {.
+0003ecb0: 2020 7061 6464 696e 672d 6c65 6674 3a20    padding-left: 
+0003ecc0: 303b 0a7d 0a2e 7370 6869 6e78 2d74 656d  0;.}..sphinx-tem
+0003ecd0: 706c 6174 652d 7269 6768 742d 6d65 6e75  plate-right-menu
+0003ece0: 2075 6c20 756c 206c 6920 756c 207b 0a20   ul ul li ul {. 
+0003ecf0: 2064 6973 706c 6179 3a20 6e6f 6e65 3b0a   display: none;.
+0003ed00: 2020 7061 6464 696e 672d 6c65 6674 3a20    padding-left: 
+0003ed10: 3130 7078 3b0a 7d0a 2e73 7068 696e 782d  10px;.}..sphinx-
+0003ed20: 7465 6d70 6c61 7465 2d72 6967 6874 2d6d  template-right-m
+0003ed30: 656e 7520 756c 2075 6c20 6c69 206c 6920  enu ul ul li li 
+0003ed40: 612e 7265 6665 7265 6e63 652e 696e 7465  a.reference.inte
+0003ed50: 726e 616c 207b 0a20 2070 6164 6469 6e67  rnal {.  padding
+0003ed60: 2d6c 6566 743a 2030 3b0a 7d0a 2e73 7068  -left: 0;.}..sph
+0003ed70: 696e 782d 7465 6d70 6c61 7465 2d72 6967  inx-template-rig
+0003ed80: 6874 2d6d 656e 7520 6c69 2075 6c20 7b0a  ht-menu li ul {.
+0003ed90: 2020 6469 7370 6c61 793a 2062 6c6f 636b    display: block
+0003eda0: 3b0a 7d0a 0a2e 7370 6869 6e78 2d74 656d  ;.}...sphinx-tem
+0003edb0: 706c 6174 652d 7269 6768 742d 6d65 6e75  plate-right-menu
+0003edc0: 202e 7370 6869 6e78 2d74 656d 706c 6174   .sphinx-templat
+0003edd0: 652d 7369 6465 2d73 6372 6f6c 6c20 7b0a  e-side-scroll {.
+0003ede0: 2020 7061 6464 696e 672d 746f 703a 2032    padding-top: 2
+0003edf0: 3070 783b 0a7d 0a40 6d65 6469 6120 7363  0px;.}.@media sc
+0003ee00: 7265 656e 2061 6e64 2028 6d69 6e2d 7769  reen and (min-wi
+0003ee10: 6474 683a 2031 3130 3170 7829 207b 0a20  dth: 1101px) {. 
+0003ee20: 202e 7370 6869 6e78 2d74 656d 706c 6174   .sphinx-templat
+0003ee30: 652d 7269 6768 742d 6d65 6e75 202e 7370  e-right-menu .sp
+0003ee40: 6869 6e78 2d74 656d 706c 6174 652d 7369  hinx-template-si
+0003ee50: 6465 2d73 6372 6f6c 6c20 7b0a 2020 2020  de-scroll {.    
+0003ee60: 7769 6474 683a 2031 3230 253b 0a20 207d  width: 120%;.  }
+0003ee70: 0a7d 0a40 6d65 6469 6120 7363 7265 656e  .}.@media screen
+0003ee80: 2061 6e64 2028 6d69 6e2d 7769 6474 683a   and (min-width:
+0003ee90: 2031 3630 3070 7829 207b 0a20 202e 7370   1600px) {.  .sp
+0003eea0: 6869 6e78 2d74 656d 706c 6174 652d 7269  hinx-template-ri
+0003eeb0: 6768 742d 6d65 6e75 202e 7370 6869 6e78  ght-menu .sphinx
+0003eec0: 2d74 656d 706c 6174 652d 7369 6465 2d73  -template-side-s
+0003eed0: 6372 6f6c 6c20 7b0a 2020 2020 7769 6474  croll {.    widt
+0003eee0: 683a 2034 3030 7078 3b0a 2020 7d0a 7d0a  h: 400px;.  }.}.
+0003eef0: 2e73 7068 696e 782d 7465 6d70 6c61 7465  .sphinx-template
+0003ef00: 2d72 6967 6874 2d6d 656e 7520 2e73 7068  -right-menu .sph
+0003ef10: 696e 782d 7465 6d70 6c61 7465 2d73 6964  inx-template-sid
+0003ef20: 652d 7363 726f 6c6c 203e 2075 6c20 7b0a  e-scroll > ul {.
+0003ef30: 2020 7061 6464 696e 672d 6c65 6674 3a20    padding-left: 
+0003ef40: 3130 253b 0a20 2070 6164 6469 6e67 2d72  10%;.  padding-r
+0003ef50: 6967 6874 3a20 3130 253b 0a20 206d 6172  ight: 10%;.  mar
+0003ef60: 6769 6e2d 626f 7474 6f6d 3a20 303b 0a7d  gin-bottom: 0;.}
+0003ef70: 0a40 6d65 6469 6120 7363 7265 656e 2061  .@media screen a
+0003ef80: 6e64 2028 6d69 6e2d 7769 6474 683a 2031  nd (min-width: 1
+0003ef90: 3630 3070 7829 207b 0a20 202e 7370 6869  600px) {.  .sphi
+0003efa0: 6e78 2d74 656d 706c 6174 652d 7269 6768  nx-template-righ
+0003efb0: 742d 6d65 6e75 202e 7370 6869 6e78 2d74  t-menu .sphinx-t
+0003efc0: 656d 706c 6174 652d 7369 6465 2d73 6372  emplate-side-scr
+0003efd0: 6f6c 6c20 3e20 756c 207b 0a20 2020 2070  oll > ul {.    p
+0003efe0: 6164 6469 6e67 2d6c 6566 743a 2032 3570  adding-left: 25p
+0003eff0: 783b 0a20 207d 0a7d 0a2e 7370 6869 6e78  x;.  }.}..sphinx
+0003f000: 2d74 656d 706c 6174 652d 7269 6768 742d  -template-right-
+0003f010: 6d65 6e75 202e 7370 6869 6e78 2d74 656d  menu .sphinx-tem
+0003f020: 706c 6174 652d 7369 6465 2d73 6372 6f6c  plate-side-scrol
+0003f030: 6c20 3e20 756c 203e 206c 6920 3e20 612e  l > ul > li > a.
+0003f040: 7265 6665 7265 6e63 652e 696e 7465 726e  reference.intern
+0003f050: 616c 207b 0a20 2063 6f6c 6f72 3a20 2332  al {.  color: #2
+0003f060: 3632 3632 363b 0a20 2066 6f6e 742d 7765  62626;.  font-we
+0003f070: 6967 6874 3a20 3530 303b 0a7d 0a2e 7370  ight: 500;.}..sp
+0003f080: 6869 6e78 2d74 656d 706c 6174 652d 7269  hinx-template-ri
+0003f090: 6768 742d 6d65 6e75 202e 7370 6869 6e78  ght-menu .sphinx
+0003f0a0: 2d74 656d 706c 6174 652d 7369 6465 2d73  -template-side-s
+0003f0b0: 6372 6f6c 6c20 756c 206c 6920 7b0a 2020  croll ul li {.  
+0003f0c0: 706f 7369 7469 6f6e 3a20 7265 6c61 7469  position: relati
+0003f0d0: 7665 3b0a 7d0a 0a23 7370 6869 6e78 2d74  ve;.}..#sphinx-t
+0003f0e0: 656d 706c 6174 652d 7269 6768 742d 6d65  emplate-right-me
+0003f0f0: 6e75 2075 6c20 6c69 2075 6c20 6c69 202e  nu ul li ul li .
+0003f100: 7369 6465 2d73 6372 6f6c 6c2d 6869 6768  side-scroll-high
+0003f110: 6c69 6768 7420 7b0a 2020 636f 6c6f 723a  light {.  color:
+0003f120: 2076 6172 282d 2d70 7974 6f72 6368 2d72   var(--pytorch-r
+0003f130: 6564 293b 0a7d 0a23 7370 6869 6e78 2d74  ed);.}.#sphinx-t
+0003f140: 656d 706c 6174 652d 7269 6768 742d 6d65  emplate-right-me
+0003f150: 6e75 2075 6c20 6c69 2075 6c20 6c69 2075  nu ul li ul li u
+0003f160: 6c20 6c69 202e 7369 6465 2d73 6372 6f6c  l li .side-scrol
+0003f170: 6c2d 6869 6768 6c69 6768 7420 7b0a 2020  l-highlight {.  
+0003f180: 636f 6c6f 723a 2076 6172 282d 2d6c 6967  color: var(--lig
+0003f190: 6874 6e69 6e67 293b 0a7d 0a23 7370 6869  htning);.}.#sphi
+0003f1a0: 6e78 2d74 656d 706c 6174 652d 7269 6768  nx-template-righ
+0003f1b0: 742d 6d65 6e75 2075 6c20 6c69 2075 6c20  t-menu ul li ul 
+0003f1c0: 6c69 2075 6c20 6c69 2075 6c20 6c69 202e  li ul li ul li .
+0003f1d0: 7369 6465 2d73 6372 6f6c 6c2d 6869 6768  side-scroll-high
+0003f1e0: 6c69 6768 7420 7b0a 2020 636f 6c6f 723a  light {.  color:
+0003f1f0: 2076 6172 282d 2d67 6f6f 676c 652d 6772   var(--google-gr
+0003f200: 6565 6e29 3b0a 7d0a 2373 7068 696e 782d  een);.}.#sphinx-
+0003f210: 7465 6d70 6c61 7465 2d72 6967 6874 2d6d  template-right-m
+0003f220: 656e 7520 756c 206c 6920 756c 206c 6920  enu ul li ul li 
+0003f230: 756c 206c 6920 756c 206c 6920 756c 206c  ul li ul li ul l
+0003f240: 6920 2e73 6964 652d 7363 726f 6c6c 2d68  i .side-scroll-h
+0003f250: 6967 686c 6967 6874 207b 0a20 2063 6f6c  ighlight {.  col
+0003f260: 6f72 3a20 7661 7228 2d2d 7265 6164 7468  or: var(--readth
+0003f270: 6564 6f63 293b 0a7d 0a0a 2e68 6561 6465  edoc);.}...heade
+0003f280: 722d 636f 6e74 6169 6e65 7220 7b0a 2020  r-container {.  
+0003f290: 6d61 782d 7769 6474 683a 206e 6f6e 653b  max-width: none;
+0003f2a0: 0a20 206d 6172 6769 6e2d 746f 703a 2034  .  margin-top: 4
+0003f2b0: 7078 3b0a 7d0a 406d 6564 6961 2073 6372  px;.}.@media scr
+0003f2c0: 6565 6e20 616e 6420 286d 696e 2d77 6964  een and (min-wid
+0003f2d0: 7468 3a20 3131 3031 7078 2920 7b0a 2020  th: 1101px) {.  
+0003f2e0: 2e68 6561 6465 722d 636f 6e74 6169 6e65  .header-containe
+0003f2f0: 7220 7b0a 2020 2020 6d61 7267 696e 2d74  r {.    margin-t
+0003f300: 6f70 3a20 303b 0a20 207d 0a7d 0a40 6d65  op: 0;.  }.}.@me
+0003f310: 6469 6120 7363 7265 656e 2061 6e64 2028  dia screen and (
+0003f320: 6d69 6e2d 7769 6474 683a 2031 3630 3070  min-width: 1600p
+0003f330: 7829 207b 0a20 202e 6865 6164 6572 2d63  x) {.  .header-c
+0003f340: 6f6e 7461 696e 6572 207b 0a20 2020 206d  ontainer {.    m
+0003f350: 6172 6769 6e2d 746f 703a 2030 3b0a 2020  argin-top: 0;.  
+0003f360: 7d0a 7d0a 0a2e 636f 6e74 6169 6e65 722d  }.}...container-
+0003f370: 666c 7569 642e 6865 6164 6572 2d68 6f6c  fluid.header-hol
+0003f380: 6465 7220 7b0a 2020 7061 6464 696e 672d  der {.  padding-
+0003f390: 7269 6768 743a 2030 3b0a 2020 7061 6464  right: 0;.  padd
+0003f3a0: 696e 672d 6c65 6674 3a20 303b 0a7d 0a0a  ing-left: 0;.}..
+0003f3b0: 2e68 6561 6465 722d 686f 6c64 6572 202e  .header-holder .
+0003f3c0: 636f 6e74 6169 6e65 7220 7b0a 2020 6d61  container {.  ma
+0003f3d0: 782d 7769 6474 683a 206e 6f6e 653b 0a20  x-width: none;. 
+0003f3e0: 2070 6164 6469 6e67 2d72 6967 6874 3a20   padding-right: 
+0003f3f0: 312e 3837 3572 656d 3b0a 2020 7061 6464  1.875rem;.  padd
+0003f400: 696e 672d 6c65 6674 3a20 312e 3837 3572  ing-left: 1.875r
+0003f410: 656d 3b0a 7d0a 406d 6564 6961 2073 6372  em;.}.@media scr
+0003f420: 6565 6e20 616e 6420 286d 696e 2d77 6964  een and (min-wid
+0003f430: 7468 3a20 3131 3031 7078 2920 7b0a 2020  th: 1101px) {.  
+0003f440: 2e68 6561 6465 722d 686f 6c64 6572 202e  .header-holder .
+0003f450: 636f 6e74 6169 6e65 7220 7b0a 2020 2020  container {.    
+0003f460: 7061 6464 696e 672d 7269 6768 743a 2031  padding-right: 1
+0003f470: 2e38 3735 7265 6d3b 0a20 2020 2070 6164  .875rem;.    pad
+0003f480: 6469 6e67 2d6c 6566 743a 2031 2e38 3735  ding-left: 1.875
+0003f490: 7265 6d3b 0a20 207d 0a7d 0a0a 2e68 6561  rem;.  }.}...hea
+0003f4a0: 6465 722d 686f 6c64 6572 202e 6d61 696e  der-holder .main
+0003f4b0: 2d6d 656e 7520 7b0a 2020 2d77 6562 6b69  -menu {.  -webki
+0003f4c0: 742d 626f 782d 7061 636b 3a20 756e 7365  t-box-pack: unse
+0003f4d0: 743b 0a20 2020 2020 202d 6d73 2d66 6c65  t;.      -ms-fle
+0003f4e0: 782d 7061 636b 3a20 756e 7365 743b 0a20  x-pack: unset;. 
+0003f4f0: 2020 2020 2020 2020 206a 7573 7469 6679           justify
+0003f500: 2d63 6f6e 7465 6e74 3a20 756e 7365 743b  -content: unset;
+0003f510: 0a20 2070 6f73 6974 696f 6e3a 2072 656c  .  position: rel
+0003f520: 6174 6976 653b 0a7d 0a40 6d65 6469 6120  ative;.}.@media 
+0003f530: 7363 7265 656e 2061 6e64 2028 6d69 6e2d  screen and (min-
+0003f540: 7769 6474 683a 2031 3130 3170 7829 207b  width: 1101px) {
+0003f550: 0a20 202e 6865 6164 6572 2d68 6f6c 6465  .  .header-holde
+0003f560: 7220 2e6d 6169 6e2d 6d65 6e75 2075 6c20  r .main-menu ul 
+0003f570: 7b0a 2020 2020 7061 6464 696e 672d 6c65  {.    padding-le
+0003f580: 6674 3a20 303b 0a20 2020 206d 6172 6769  ft: 0;.    margi
+0003f590: 6e2d 6c65 6674 3a20 3236 253b 0a20 207d  n-left: 26%;.  }
+0003f5a0: 0a7d 0a40 6d65 6469 6120 7363 7265 656e  .}.@media screen
+0003f5b0: 2061 6e64 2028 6d69 6e2d 7769 6474 683a   and (min-width:
+0003f5c0: 2031 3630 3070 7829 207b 0a20 202e 6865   1600px) {.  .he
+0003f5d0: 6164 6572 2d68 6f6c 6465 7220 2e6d 6169  ader-holder .mai
+0003f5e0: 6e2d 6d65 6e75 2075 6c20 7b0a 2020 2020  n-menu ul {.    
+0003f5f0: 7061 6464 696e 672d 6c65 6674 3a20 3338  padding-left: 38
+0003f600: 7078 3b0a 2020 2020 6d61 7267 696e 2d6c  px;.    margin-l
+0003f610: 6566 743a 2033 3130 7078 3b0a 2020 7d0a  eft: 310px;.  }.
+0003f620: 7d0a 0a2e 7370 6869 6e78 2d74 656d 706c  }...sphinx-templ
+0003f630: 6174 652d 7061 6765 2d6c 6576 656c 2d62  ate-page-level-b
+0003f640: 6172 207b 0a20 2064 6973 706c 6179 3a20  ar {.  display: 
+0003f650: 6e6f 6e65 3b0a 2020 2d77 6562 6b69 742d  none;.  -webkit-
+0003f660: 626f 782d 616c 6967 6e3a 2063 656e 7465  box-align: cente
+0003f670: 723b 0a20 2020 2020 202d 6d73 2d66 6c65  r;.      -ms-fle
+0003f680: 782d 616c 6967 6e3a 2063 656e 7465 723b  x-align: center;
+0003f690: 0a20 2020 2020 2020 2020 2061 6c69 676e  .          align
+0003f6a0: 2d69 7465 6d73 3a20 6365 6e74 6572 3b0a  -items: center;.
+0003f6b0: 2020 6261 636b 6772 6f75 6e64 2d63 6f6c    background-col
+0003f6c0: 6f72 3a20 2366 6666 6666 663b 0a20 2062  or: #ffffff;.  b
+0003f6d0: 6f72 6465 722d 626f 7474 6f6d 3a20 3170  order-bottom: 1p
+0003f6e0: 7820 736f 6c69 6420 2365 3265 3265 323b  x solid #e2e2e2;
+0003f6f0: 0a20 2077 6964 7468 3a20 3130 3025 3b0a  .  width: 100%;.
+0003f700: 2020 7a2d 696e 6465 783a 2032 3031 3b0a    z-index: 201;.
+0003f710: 7d0a 406d 6564 6961 2073 6372 6565 6e20  }.@media screen 
+0003f720: 616e 6420 286d 696e 2d77 6964 7468 3a20  and (min-width: 
+0003f730: 3131 3031 7078 2920 7b0a 2020 2e73 7068  1101px) {.  .sph
+0003f740: 696e 782d 7465 6d70 6c61 7465 2d70 6167  inx-template-pag
+0003f750: 652d 6c65 7665 6c2d 6261 7220 7b0a 2020  e-level-bar {.  
+0003f760: 2020 6c65 6674 3a20 303b 0a20 2020 2064    left: 0;.    d
+0003f770: 6973 706c 6179 3a20 2d77 6562 6b69 742d  isplay: -webkit-
+0003f780: 626f 783b 0a20 2020 2064 6973 706c 6179  box;.    display
+0003f790: 3a20 2d6d 732d 666c 6578 626f 783b 0a20  : -ms-flexbox;. 
+0003f7a0: 2020 2064 6973 706c 6179 3a20 666c 6578     display: flex
+0003f7b0: 3b0a 2020 2020 6865 6967 6874 3a20 3435  ;.    height: 45
+0003f7c0: 7078 3b0a 2020 2020 7061 6464 696e 672d  px;.    padding-
+0003f7d0: 6c65 6674 3a20 303b 0a20 2020 2077 6964  left: 0;.    wid
+0003f7e0: 7468 3a20 3130 3025 3b0a 2020 2020 706f  th: 100%;.    po
+0003f7f0: 7369 7469 6f6e 3a20 6162 736f 6c75 7465  sition: absolute
+0003f800: 3b0a 2020 2020 7a2d 696e 6465 783a 2031  ;.    z-index: 1
+0003f810: 3b0a 2020 7d0a 2020 2e73 7068 696e 782d  ;.  }.  .sphinx-
+0003f820: 7465 6d70 6c61 7465 2d70 6167 652d 6c65  template-page-le
+0003f830: 7665 6c2d 6261 722e 6c65 6674 2d6d 656e  vel-bar.left-men
+0003f840: 752d 6973 2d66 6978 6564 207b 0a20 2020  u-is-fixed {.   
+0003f850: 2070 6f73 6974 696f 6e3a 2066 6978 6564   position: fixed
+0003f860: 3b0a 2020 2020 746f 703a 2030 3b0a 2020  ;.    top: 0;.  
+0003f870: 2020 6c65 6674 3a20 3235 253b 0a20 2020    left: 25%;.   
+0003f880: 2070 6164 6469 6e67 2d6c 6566 743a 2030   padding-left: 0
+0003f890: 3b0a 2020 2020 7269 6768 743a 2030 3b0a  ;.    right: 0;.
+0003f8a0: 2020 2020 7769 6474 683a 2037 3525 3b0a      width: 75%;.
+0003f8b0: 2020 7d0a 7d0a 406d 6564 6961 2073 6372    }.}.@media scr
+0003f8c0: 6565 6e20 616e 6420 286d 696e 2d77 6964  een and (min-wid
+0003f8d0: 7468 3a20 3136 3030 7078 2920 7b0a 2020  th: 1600px) {.  
+0003f8e0: 2e73 7068 696e 782d 7465 6d70 6c61 7465  .sphinx-template
+0003f8f0: 2d70 6167 652d 6c65 7665 6c2d 6261 7220  -page-level-bar 
+0003f900: 7b0a 2020 2020 6c65 6674 3a20 303b 0a20  {.    left: 0;. 
+0003f910: 2020 2072 6967 6874 3a20 303b 0a20 2020     right: 0;.   
+0003f920: 2077 6964 7468 3a20 6175 746f 3b0a 2020   width: auto;.  
+0003f930: 2020 7a2d 696e 6465 783a 2031 3b0a 2020    z-index: 1;.  
+0003f940: 7d0a 2020 2e73 7068 696e 782d 7465 6d70  }.  .sphinx-temp
+0003f950: 6c61 7465 2d70 6167 652d 6c65 7665 6c2d  late-page-level-
+0003f960: 6261 722e 6c65 6674 2d6d 656e 752d 6973  bar.left-menu-is
+0003f970: 2d66 6978 6564 207b 0a20 2020 206c 6566  -fixed {.    lef
+0003f980: 743a 2033 3530 7078 3b0a 2020 2020 7269  t: 350px;.    ri
+0003f990: 6768 743a 2030 3b0a 2020 2020 7769 6474  ght: 0;.    widt
+0003f9a0: 683a 2061 7574 6f3b 0a20 207d 0a7d 0a2e  h: auto;.  }.}..
+0003f9b0: 7370 6869 6e78 2d74 656d 706c 6174 652d  sphinx-template-
+0003f9c0: 7061 6765 2d6c 6576 656c 2d62 6172 2075  page-level-bar u
+0003f9d0: 6c2c 202e 7370 6869 6e78 2d74 656d 706c  l, .sphinx-templ
+0003f9e0: 6174 652d 7061 6765 2d6c 6576 656c 2d62  ate-page-level-b
+0003f9f0: 6172 206c 6920 7b0a 2020 6d61 7267 696e  ar li {.  margin
+0003fa00: 3a20 303b 0a7d 0a0a 2e73 7068 696e 782d  : 0;.}...sphinx-
+0003fa10: 7465 6d70 6c61 7465 2d73 686f 7274 6375  template-shortcu
+0003fa20: 7473 2d77 7261 7070 6572 207b 0a20 2064  ts-wrapper {.  d
+0003fa30: 6973 706c 6179 3a20 6e6f 6e65 3b0a 7d0a  isplay: none;.}.
+0003fa40: 406d 6564 6961 2073 6372 6565 6e20 616e  @media screen an
+0003fa50: 6420 286d 696e 2d77 6964 7468 3a20 3131  d (min-width: 11
+0003fa60: 3031 7078 2920 7b0a 2020 2e73 7068 696e  01px) {.  .sphin
+0003fa70: 782d 7465 6d70 6c61 7465 2d73 686f 7274  x-template-short
+0003fa80: 6375 7473 2d77 7261 7070 6572 207b 0a20  cuts-wrapper {. 
+0003fa90: 2020 2066 6f6e 742d 7369 7a65 3a20 302e     font-size: 0.
+0003faa0: 3837 3572 656d 3b0a 2020 2020 666c 6f61  875rem;.    floa
+0003fab0: 743a 206c 6566 743b 0a20 2020 206d 6172  t: left;.    mar
+0003fac0: 6769 6e2d 6c65 6674 3a20 3225 3b0a 2020  gin-left: 2%;.  
+0003fad0: 7d0a 7d0a 406d 6564 6961 2073 6372 6565  }.}.@media scree
+0003fae0: 6e20 616e 6420 286d 696e 2d77 6964 7468  n and (min-width
+0003faf0: 3a20 3136 3030 7078 2920 7b0a 2020 2e73  : 1600px) {.  .s
+0003fb00: 7068 696e 782d 7465 6d70 6c61 7465 2d73  phinx-template-s
+0003fb10: 686f 7274 6375 7473 2d77 7261 7070 6572  hortcuts-wrapper
+0003fb20: 207b 0a20 2020 206d 6172 6769 6e2d 6c65   {.    margin-le
+0003fb30: 6674 3a20 312e 3837 3572 656d 3b0a 2020  ft: 1.875rem;.  
+0003fb40: 7d0a 7d0a 0a2e 636f 6f6b 6965 2d62 616e  }.}...cookie-ban
+0003fb50: 6e65 722d 7772 6170 7065 7220 7b0a 2020  ner-wrapper {.  
+0003fb60: 6469 7370 6c61 793a 206e 6f6e 653b 0a7d  display: none;.}
+0003fb70: 0a2e 636f 6f6b 6965 2d62 616e 6e65 722d  ..cookie-banner-
+0003fb80: 7772 6170 7065 7220 2e63 6f6e 7461 696e  wrapper .contain
+0003fb90: 6572 207b 0a20 2070 6164 6469 6e67 2d6c  er {.  padding-l
+0003fba0: 6566 743a 2031 2e38 3735 7265 6d3b 0a20  eft: 1.875rem;. 
+0003fbb0: 2070 6164 6469 6e67 2d72 6967 6874 3a20   padding-right: 
+0003fbc0: 312e 3837 3572 656d 3b0a 2020 6d61 782d  1.875rem;.  max-
+0003fbd0: 7769 6474 683a 2031 3234 3070 783b 0a7d  width: 1240px;.}
+0003fbe0: 0a2e 636f 6f6b 6965 2d62 616e 6e65 722d  ..cookie-banner-
+0003fbf0: 7772 6170 7065 722e 6973 2d76 6973 6962  wrapper.is-visib
+0003fc00: 6c65 207b 0a20 2064 6973 706c 6179 3a20  le {.  display: 
+0003fc10: 626c 6f63 6b3b 0a20 2070 6f73 6974 696f  block;.  positio
+0003fc20: 6e3a 2066 6978 6564 3b0a 2020 626f 7474  n: fixed;.  bott
+0003fc30: 6f6d 3a20 303b 0a20 2062 6163 6b67 726f  om: 0;.  backgro
+0003fc40: 756e 642d 636f 6c6f 723a 2023 6633 6634  und-color: #f3f4
+0003fc50: 6637 3b0a 2020 6d69 6e2d 6865 6967 6874  f7;.  min-height
+0003fc60: 3a20 3130 3070 783b 0a20 2077 6964 7468  : 100px;.  width
+0003fc70: 3a20 3130 3025 3b0a 2020 7a2d 696e 6465  : 100%;.  z-inde
+0003fc80: 783a 2034 3031 3b0a 2020 626f 7264 6572  x: 401;.  border
+0003fc90: 2d74 6f70 3a20 3370 7820 736f 6c69 6420  -top: 3px solid 
+0003fca0: 2365 6465 6465 653b 0a7d 0a2e 636f 6f6b  #ededee;.}..cook
+0003fcb0: 6965 2d62 616e 6e65 722d 7772 6170 7065  ie-banner-wrappe
+0003fcc0: 7220 2e67 6470 722d 6e6f 7469 6365 207b  r .gdpr-notice {
+0003fcd0: 0a20 2063 6f6c 6f72 3a20 2336 6336 6336  .  color: #6c6c6
+0003fce0: 643b 0a20 206d 6172 6769 6e2d 746f 703a  d;.  margin-top:
+0003fcf0: 2031 2e35 3632 3572 656d 3b0a 2020 7465   1.5625rem;.  te
+0003fd00: 7874 2d61 6c69 676e 3a20 6c65 6674 3b0a  xt-align: left;.
+0003fd10: 2020 6d61 782d 7769 6474 683a 2031 3434    max-width: 144
+0003fd20: 3070 783b 0a7d 0a40 6d65 6469 6120 7363  0px;.}.@media sc
+0003fd30: 7265 656e 2061 6e64 2028 6d69 6e2d 7769  reen and (min-wi
+0003fd40: 6474 683a 2037 3638 7078 2920 7b0a 2020  dth: 768px) {.  
+0003fd50: 2e63 6f6f 6b69 652d 6261 6e6e 6572 2d77  .cookie-banner-w
+0003fd60: 7261 7070 6572 202e 6764 7072 2d6e 6f74  rapper .gdpr-not
+0003fd70: 6963 6520 7b0a 2020 2020 7769 6474 683a  ice {.    width:
+0003fd80: 2037 3725 3b0a 2020 7d0a 7d0a 406d 6564   77%;.  }.}.@med
+0003fd90: 6961 2028 6d69 6e2d 7769 6474 683a 2037  ia (min-width: 7
+0003fda0: 3638 7078 2920 616e 6420 286d 6178 2d77  68px) and (max-w
+0003fdb0: 6964 7468 3a20 3132 3339 7078 2920 7b0a  idth: 1239px) {.
+0003fdc0: 2020 2e63 6f6f 6b69 652d 6261 6e6e 6572    .cookie-banner
+0003fdd0: 2d77 7261 7070 6572 202e 6764 7072 2d6e  -wrapper .gdpr-n
+0003fde0: 6f74 6963 6520 7b0a 2020 2020 7769 6474  otice {.    widt
+0003fdf0: 683a 2069 6e68 6572 6974 3b0a 2020 7d0a  h: inherit;.  }.
+0003fe00: 7d0a 2e63 6f6f 6b69 652d 6261 6e6e 6572  }..cookie-banner
+0003fe10: 2d77 7261 7070 6572 202e 6764 7072 2d6e  -wrapper .gdpr-n
+0003fe20: 6f74 6963 6520 2e63 6f6f 6b69 652d 706f  otice .cookie-po
+0003fe30: 6c69 6379 2d6c 696e 6b20 7b0a 2020 636f  licy-link {.  co
+0003fe40: 6c6f 723a 2023 3334 3334 3334 3b0a 7d0a  lor: #343434;.}.
+0003fe50: 2e63 6f6f 6b69 652d 6261 6e6e 6572 2d77  .cookie-banner-w
+0003fe60: 7261 7070 6572 202e 636c 6f73 652d 6275  rapper .close-bu
+0003fe70: 7474 6f6e 207b 0a20 202d 7765 626b 6974  tton {.  -webkit
+0003fe80: 2d61 7070 6561 7261 6e63 653a 206e 6f6e  -appearance: non
+0003fe90: 653b 0a20 2020 2020 2d6d 6f7a 2d61 7070  e;.     -moz-app
+0003fea0: 6561 7261 6e63 653a 206e 6f6e 653b 0a20  earance: none;. 
+0003feb0: 2020 2020 2020 2020 2061 7070 6561 7261           appeara
+0003fec0: 6e63 653a 206e 6f6e 653b 0a20 2062 6163  nce: none;.  bac
+0003fed0: 6b67 726f 756e 643a 2074 7261 6e73 7061  kground: transpa
+0003fee0: 7265 6e74 3b0a 2020 626f 7264 6572 3a20  rent;.  border: 
+0003fef0: 3170 7820 736f 6c69 6420 2366 3366 3466  1px solid #f3f4f
+0003ff00: 373b 0a20 2068 6569 6768 743a 2031 2e33  7;.  height: 1.3
+0003ff10: 3132 3572 656d 3b0a 2020 706f 7369 7469  125rem;.  positi
+0003ff20: 6f6e 3a20 6162 736f 6c75 7465 3b0a 2020  on: absolute;.  
+0003ff30: 626f 7474 6f6d 3a20 3432 7078 3b0a 2020  bottom: 42px;.  
+0003ff40: 7269 6768 743a 2030 3b0a 2020 746f 703a  right: 0;.  top:
+0003ff50: 2030 3b0a 2020 6375 7273 6f72 3a20 706f   0;.  cursor: po
+0003ff60: 696e 7465 723b 0a20 206f 7574 6c69 6e65  inter;.  outline
+0003ff70: 3a20 6e6f 6e65 3b0a 7d0a 406d 6564 6961  : none;.}.@media
+0003ff80: 2073 6372 6565 6e20 616e 6420 286d 696e   screen and (min
+0003ff90: 2d77 6964 7468 3a20 3736 3870 7829 207b  -width: 768px) {
+0003ffa0: 0a20 202e 636f 6f6b 6965 2d62 616e 6e65  .  .cookie-banne
+0003ffb0: 722d 7772 6170 7065 7220 2e63 6c6f 7365  r-wrapper .close
+0003ffc0: 2d62 7574 746f 6e20 7b0a 2020 2020 7269  -button {.    ri
+0003ffd0: 6768 743a 2032 3025 3b0a 2020 2020 746f  ght: 20%;.    to
+0003ffe0: 703a 2069 6e68 6572 6974 3b0a 2020 7d0a  p: inherit;.  }.
+0003fff0: 7d0a 406d 6564 6961 2028 6d69 6e2d 7769  }.@media (min-wi
+00040000: 6474 683a 2037 3638 7078 2920 616e 6420  dth: 768px) and 
+00040010: 286d 6178 2d77 6964 7468 3a20 3132 3339  (max-width: 1239
+00040020: 7078 2920 7b0a 2020 2e63 6f6f 6b69 652d  px) {.  .cookie-
+00040030: 6261 6e6e 6572 2d77 7261 7070 6572 202e  banner-wrapper .
+00040040: 636c 6f73 652d 6275 7474 6f6e 207b 0a20  close-button {. 
+00040050: 2020 2072 6967 6874 3a20 303b 0a20 2020     right: 0;.   
+00040060: 2074 6f70 3a20 303b 0a20 207d 0a7d 0a0a   top: 0;.  }.}..
+00040070: 2e6d 6169 6e2d 6d65 6e75 2075 6c20 6c69  .main-menu ul li
+00040080: 202e 7265 736f 7572 6365 732d 6472 6f70   .resources-drop
+00040090: 646f 776e 2061 207b 0a20 2063 7572 736f  down a {.  curso
+000400a0: 723a 2070 6f69 6e74 6572 3b0a 7d0a 2e6d  r: pointer;.}..m
+000400b0: 6169 6e2d 6d65 6e75 2075 6c20 6c69 202e  ain-menu ul li .
+000400c0: 6472 6f70 646f 776e 2d6d 656e 7520 7b0a  dropdown-menu {.
+000400d0: 2020 626f 7264 6572 2d72 6164 6975 733a    border-radius:
+000400e0: 2030 3b0a 2020 7061 6464 696e 673a 2030   0;.  padding: 0
+000400f0: 3b0a 7d0a 2e6d 6169 6e2d 6d65 6e75 2075  ;.}..main-menu u
+00040100: 6c20 6c69 202e 6472 6f70 646f 776e 2d6d  l li .dropdown-m
+00040110: 656e 7520 2e64 726f 7064 6f77 6e2d 6974  enu .dropdown-it
+00040120: 656d 207b 0a20 2063 6f6c 6f72 3a20 2336  em {.  color: #6
+00040130: 6336 6336 643b 0a20 2062 6f72 6465 722d  c6c6d;.  border-
+00040140: 626f 7474 6f6d 3a20 3170 7820 736f 6c69  bottom: 1px soli
+00040150: 6420 2365 3265 3265 323b 0a7d 0a2e 6d61  d #e2e2e2;.}..ma
+00040160: 696e 2d6d 656e 7520 756c 206c 6920 2e64  in-menu ul li .d
+00040170: 726f 7064 6f77 6e2d 6d65 6e75 202e 6472  ropdown-menu .dr
+00040180: 6f70 646f 776e 2d69 7465 6d3a 6c61 7374  opdown-item:last
+00040190: 2d6f 662d 7479 7065 207b 0a20 2062 6f72  -of-type {.  bor
+000401a0: 6465 722d 626f 7474 6f6d 2d63 6f6c 6f72  der-bottom-color
+000401b0: 3a20 7472 616e 7370 6172 656e 743b 0a7d  : transparent;.}
+000401c0: 0a2e 6d61 696e 2d6d 656e 7520 756c 206c  ..main-menu ul l
+000401d0: 6920 2e64 726f 7064 6f77 6e2d 6d65 6e75  i .dropdown-menu
+000401e0: 202e 6472 6f70 646f 776e 2d69 7465 6d3a   .dropdown-item:
+000401f0: 686f 7665 7220 7b0a 2020 6261 636b 6772  hover {.  backgr
+00040200: 6f75 6e64 2d63 6f6c 6f72 3a20 7661 7228  ound-color: var(
+00040210: 2d2d 7079 746f 7263 6829 3b0a 7d0a 2e6d  --pytorch);.}..m
+00040220: 6169 6e2d 6d65 6e75 2075 6c20 6c69 202e  ain-menu ul li .
+00040230: 6472 6f70 646f 776e 2d6d 656e 7520 2e64  dropdown-menu .d
+00040240: 726f 7064 6f77 6e2d 6974 656d 2070 207b  ropdown-item p {
+00040250: 0a20 2066 6f6e 742d 7369 7a65 3a20 3172  .  font-size: 1r
+00040260: 656d 3b0a 2020 636f 6c6f 723a 2023 3937  em;.  color: #97
+00040270: 3937 3937 3b0a 7d0a 2e6d 6169 6e2d 6d65  9797;.}..main-me
+00040280: 6e75 2075 6c20 6c69 202e 6472 6f70 646f  nu ul li .dropdo
+00040290: 776e 2d6d 656e 7520 612e 6472 6f70 646f  wn-menu a.dropdo
+000402a0: 776e 2d69 7465 6d3a 686f 7665 7220 7b0a  wn-item:hover {.
+000402b0: 2020 636f 6c6f 723a 2023 6666 6666 6666    color: #ffffff
+000402c0: 3b0a 7d0a 2e6d 6169 6e2d 6d65 6e75 2075  ;.}..main-menu u
+000402d0: 6c20 6c69 202e 6472 6f70 646f 776e 2d6d  l li .dropdown-m
+000402e0: 656e 7520 612e 6472 6f70 646f 776e 2d69  enu a.dropdown-i
+000402f0: 7465 6d3a 686f 7665 7220 7020 7b0a 2020  tem:hover p {.  
+00040300: 636f 6c6f 723a 2023 6666 6666 6666 3b0a  color: #ffffff;.
+00040310: 7d0a 0a2e 7265 736f 7572 6365 732d 6472  }...resources-dr
+00040320: 6f70 646f 776e 2d6d 656e 7520 7b0a 2020  opdown-menu {.  
+00040330: 6c65 6674 3a20 2d37 3570 783b 0a20 2077  left: -75px;.  w
+00040340: 6964 7468 3a20 3232 3670 783b 0a20 2064  idth: 226px;.  d
+00040350: 6973 706c 6179 3a20 6e6f 6e65 3b0a 2020  isplay: none;.  
+00040360: 706f 7369 7469 6f6e 3a20 6162 736f 6c75  position: absolu
+00040370: 7465 3b0a 2020 7a2d 696e 6465 783a 2031  te;.  z-index: 1
+00040380: 3030 303b 0a20 2064 6973 706c 6179 3a20  000;.  display: 
+00040390: 6e6f 6e65 3b0a 2020 666c 6f61 743a 206c  none;.  float: l
+000403a0: 6566 743b 0a20 206d 696e 2d77 6964 7468  eft;.  min-width
+000403b0: 3a20 3130 7265 6d3b 0a20 2070 6164 6469  : 10rem;.  paddi
+000403c0: 6e67 3a20 302e 3572 656d 2030 3b0a 2020  ng: 0.5rem 0;.  
+000403d0: 666f 6e74 2d73 697a 653a 2031 7265 6d3b  font-size: 1rem;
+000403e0: 0a20 2063 6f6c 6f72 3a20 2332 3132 3532  .  color: #21252
+000403f0: 393b 0a20 2074 6578 742d 616c 6967 6e3a  9;.  text-align:
+00040400: 206c 6566 743b 0a20 206c 6973 742d 7374   left;.  list-st
+00040410: 796c 653a 206e 6f6e 653b 0a20 2062 6163  yle: none;.  bac
+00040420: 6b67 726f 756e 642d 636f 6c6f 723a 2023  kground-color: #
+00040430: 6666 6666 6666 3b0a 2020 6261 636b 6772  ffffff;.  backgr
+00040440: 6f75 6e64 2d63 6c69 703a 2070 6164 6469  ound-clip: paddi
+00040450: 6e67 2d62 6f78 3b0a 2020 626f 7264 6572  ng-box;.  border
+00040460: 3a20 3170 7820 736f 6c69 6420 7267 6261  : 1px solid rgba
+00040470: 2830 2c20 302c 2030 2c20 302e 3135 293b  (0, 0, 0, 0.15);
+00040480: 0a20 2062 6f72 6465 722d 7261 6469 7573  .  border-radius
+00040490: 3a20 302e 3235 7265 6d3b 0a7d 0a0a 2e72  : 0.25rem;.}...r
+000404a0: 6573 6f75 7263 6573 2d64 726f 7064 6f77  esources-dropdow
+000404b0: 6e3a 686f 7665 7220 2e72 6573 6f75 7263  n:hover .resourc
+000404c0: 6573 2d64 726f 7064 6f77 6e2d 6d65 6e75  es-dropdown-menu
+000404d0: 207b 0a20 2064 6973 706c 6179 3a20 626c   {.  display: bl
+000404e0: 6f63 6b3b 0a7d 0a0a 2e6d 6169 6e2d 6d65  ock;.}...main-me
+000404f0: 6e75 2075 6c20 6c69 202e 7265 736f 7572  nu ul li .resour
+00040500: 6365 732d 6472 6f70 646f 776e 2d6d 656e  ces-dropdown-men
+00040510: 7520 7b0a 2020 626f 7264 6572 2d72 6164  u {.  border-rad
+00040520: 6975 733a 2030 3b0a 2020 7061 6464 696e  ius: 0;.  paddin
+00040530: 673a 2030 3b0a 7d0a 2e6d 6169 6e2d 6d65  g: 0;.}..main-me
+00040540: 6e75 2075 6c20 6c69 2e61 6374 6976 653a  nu ul li.active:
+00040550: 686f 7665 7220 2e72 6573 6f75 7263 6573  hover .resources
+00040560: 2d64 726f 7064 6f77 6e2d 6d65 6e75 207b  -dropdown-menu {
+00040570: 0a20 2064 6973 706c 6179 3a20 626c 6f63  .  display: bloc
+00040580: 6b3b 0a7d 0a0a 2e6d 6169 6e2d 6d65 6e75  k;.}...main-menu
+00040590: 2075 6c20 6c69 202e 7265 736f 7572 6365   ul li .resource
+000405a0: 732d 6472 6f70 646f 776e 2d6d 656e 7520  s-dropdown-menu 
+000405b0: 2e64 726f 7064 6f77 6e2d 6974 656d 207b  .dropdown-item {
+000405c0: 0a20 2063 6f6c 6f72 3a20 2336 6336 6336  .  color: #6c6c6
+000405d0: 643b 0a20 2062 6f72 6465 722d 626f 7474  d;.  border-bott
+000405e0: 6f6d 3a20 3170 7820 736f 6c69 6420 2365  om: 1px solid #e
+000405f0: 3265 3265 323b 0a7d 0a0a 2e72 6573 6f75  2e2e2;.}...resou
+00040600: 7263 6573 2d64 726f 7064 6f77 6e20 2e77  rces-dropdown .w
+00040610: 6974 682d 646f 776e 2d6f 7261 6e67 652d  ith-down-orange-
+00040620: 6172 726f 7720 7b0a 2020 7061 6464 696e  arrow {.  paddin
+00040630: 672d 7269 6768 743a 2032 7265 6d3b 0a20  g-right: 2rem;. 
+00040640: 2070 6f73 6974 696f 6e3a 2072 656c 6174   position: relat
+00040650: 6976 653b 0a20 2062 6163 6b67 726f 756e  ive;.  backgroun
+00040660: 643a 2075 726c 2822 2e2e 2f69 6d61 6765  d: url("../image
+00040670: 732f 6368 6576 726f 6e2d 646f 776e 2d6f  s/chevron-down-o
+00040680: 7261 6e67 652e 7376 6722 293b 0a20 2062  range.svg");.  b
+00040690: 6163 6b67 726f 756e 642d 7369 7a65 3a20  ackground-size: 
+000406a0: 3134 7078 2031 3870 783b 0a20 2062 6163  14px 18px;.  bac
+000406b0: 6b67 726f 756e 642d 706f 7369 7469 6f6e  kground-position
+000406c0: 3a20 746f 7020 3770 7820 7269 6768 7420  : top 7px right 
+000406d0: 3130 7078 3b0a 2020 6261 636b 6772 6f75  10px;.  backgrou
+000406e0: 6e64 2d72 6570 6561 743a 206e 6f2d 7265  nd-repeat: no-re
+000406f0: 7065 6174 3b0a 7d0a 0a2e 7769 7468 2d64  peat;.}...with-d
+00040700: 6f77 6e2d 6172 726f 7720 7b0a 2020 7061  own-arrow {.  pa
+00040710: 6464 696e 672d 7269 6768 743a 2032 7265  dding-right: 2re
+00040720: 6d3b 0a20 2070 6f73 6974 696f 6e3a 2072  m;.  position: r
+00040730: 656c 6174 6976 653b 0a20 2062 6163 6b67  elative;.  backg
+00040740: 726f 756e 642d 696d 6167 653a 2075 726c  round-image: url
+00040750: 2822 2e2e 2f69 6d61 6765 732f 6368 6576  ("../images/chev
+00040760: 726f 6e2d 646f 776e 2d62 6c61 636b 2e73  ron-down-black.s
+00040770: 7667 2229 3b0a 2020 6261 636b 6772 6f75  vg");.  backgrou
+00040780: 6e64 2d73 697a 653a 2031 3470 7820 3138  nd-size: 14px 18
+00040790: 7078 3b0a 2020 6261 636b 6772 6f75 6e64  px;.  background
+000407a0: 2d70 6f73 6974 696f 6e3a 2074 6f70 2037  -position: top 7
+000407b0: 7078 2072 6967 6874 2031 3070 783b 0a20  px right 10px;. 
+000407c0: 2062 6163 6b67 726f 756e 642d 7265 7065   background-repe
+000407d0: 6174 3a20 6e6f 2d72 6570 6561 743b 0a7d  at: no-repeat;.}
+000407e0: 0a2e 7769 7468 2d64 6f77 6e2d 6172 726f  ..with-down-arro
+000407f0: 773a 686f 7665 7220 7b0a 2020 6261 636b  w:hover {.  back
+00040800: 6772 6f75 6e64 2d69 6d61 6765 3a20 7572  ground-image: ur
+00040810: 6c28 222e 2e2f 696d 6167 6573 2f63 6865  l("../images/che
+00040820: 7672 6f6e 2d64 6f77 6e2d 6f72 616e 6765  vron-down-orange
+00040830: 2e73 7667 2229 3b0a 2020 6261 636b 6772  .svg");.  backgr
+00040840: 6f75 6e64 2d72 6570 6561 743a 206e 6f2d  ound-repeat: no-
+00040850: 7265 7065 6174 3b0a 7d0a 0a2e 6865 6164  repeat;.}...head
+00040860: 6572 2d68 6f6c 6465 7220 2e6d 6169 6e2d  er-holder .main-
+00040870: 6d65 6e75 2075 6c20 6c69 202e 7265 736f  menu ul li .reso
+00040880: 7572 6365 732d 6472 6f70 646f 776e 202e  urces-dropdown .
+00040890: 646f 632d 6472 6f70 646f 776e 2d6f 7074  doc-dropdown-opt
+000408a0: 696f 6e20 7b0a 2020 7061 6464 696e 672d  ion {.  padding-
+000408b0: 746f 703a 2031 7265 6d3b 0a7d 0a0a 2e68  top: 1rem;.}...h
+000408c0: 6561 6465 722d 686f 6c64 6572 202e 6d61  eader-holder .ma
+000408d0: 696e 2d6d 656e 7520 756c 206c 6920 612e  in-menu ul li a.
+000408e0: 6e61 762d 6472 6f70 646f 776e 2d69 7465  nav-dropdown-ite
+000408f0: 6d20 7b0a 2020 6469 7370 6c61 793a 2062  m {.  display: b
+00040900: 6c6f 636b 3b0a 2020 666f 6e74 2d73 697a  lock;.  font-siz
+00040910: 653a 2031 7265 6d3b 0a20 206c 696e 652d  e: 1rem;.  line-
+00040920: 6865 6967 6874 3a20 312e 3331 3235 7265  height: 1.3125re
+00040930: 6d3b 0a20 2077 6964 7468 3a20 3130 3025  m;.  width: 100%
+00040940: 3b0a 2020 7061 6464 696e 673a 2030 2e32  ;.  padding: 0.2
+00040950: 3572 656d 2031 2e35 7265 6d3b 0a20 2063  5rem 1.5rem;.  c
+00040960: 6c65 6172 3a20 626f 7468 3b0a 2020 666f  lear: both;.  fo
+00040970: 6e74 2d77 6569 6768 743a 2034 3030 3b0a  nt-weight: 400;.
+00040980: 2020 636f 6c6f 723a 2023 3937 3937 3937    color: #979797
+00040990: 3b0a 2020 7465 7874 2d61 6c69 676e 3a20  ;.  text-align: 
+000409a0: 6365 6e74 6572 3b0a 2020 6261 636b 6772  center;.  backgr
+000409b0: 6f75 6e64 2d63 6f6c 6f72 3a20 7472 616e  ound-color: tran
+000409c0: 7370 6172 656e 743b 0a20 2062 6f72 6465  sparent;.  borde
+000409d0: 722d 626f 7474 6f6d 3a20 3170 7820 736f  r-bottom: 1px so
+000409e0: 6c69 6420 2365 3265 3265 323b 0a7d 0a2e  lid #e2e2e2;.}..
+000409f0: 6865 6164 6572 2d68 6f6c 6465 7220 2e6d  header-holder .m
+00040a00: 6169 6e2d 6d65 6e75 2075 6c20 6c69 2061  ain-menu ul li a
+00040a10: 2e6e 6176 2d64 726f 7064 6f77 6e2d 6974  .nav-dropdown-it
+00040a20: 656d 2e61 6374 6976 653a 6265 666f 7265  em.active:before
+00040a30: 207b 0a20 2063 6f6e 7465 6e74 3a20 225c   {.  content: "\
+00040a40: 4630 4133 223b 0a20 2066 6f6e 742d 6661  F0A3";.  font-fa
+00040a50: 6d69 6c79 3a20 466f 6e74 4177 6573 6f6d  mily: FontAwesom
+00040a60: 653b 0a20 2063 6f6c 6f72 3a20 7661 7228  e;.  color: var(
+00040a70: 2d2d 6c69 6768 746e 696e 6729 3b0a 2020  --lightning);.  
+00040a80: 7061 6464 696e 673a 2030 2e35 7265 6d20  padding: 0.5rem 
+00040a90: 3072 656d 3b0a 2020 666f 6e74 2d73 697a  0rem;.  font-siz
+00040aa0: 653a 2031 2e33 7265 6d3b 0a20 206c 6566  e: 1.3rem;.  lef
+00040ab0: 743a 2033 7078 3b0a 2020 706f 7369 7469  t: 3px;.  positi
+00040ac0: 6f6e 3a20 6162 736f 6c75 7465 3b0a 2020  on: absolute;.  
+00040ad0: 7465 7874 2d61 6c69 676e 3a20 6c65 6674  text-align: left
+00040ae0: 3b0a 7d0a 2e68 6561 6465 722d 686f 6c64  ;.}..header-hold
+00040af0: 6572 202e 6d61 696e 2d6d 656e 7520 756c  er .main-menu ul
+00040b00: 206c 6920 612e 6e61 762d 6472 6f70 646f   li a.nav-dropdo
+00040b10: 776e 2d69 7465 6d2e 6163 7469 7665 3a68  wn-item.active:h
+00040b20: 6f76 6572 3a62 6566 6f72 6520 7b0a 2020  over:before {.  
+00040b30: 636f 6c6f 723a 2076 6172 282d 2d67 6f6f  color: var(--goo
+00040b40: 676c 652d 6772 6565 6e29 3b0a 7d0a 2e68  gle-green);.}..h
+00040b50: 6561 6465 722d 686f 6c64 6572 202e 6d61  eader-holder .ma
+00040b60: 696e 2d6d 656e 7520 756c 206c 6920 612e  in-menu ul li a.
+00040b70: 6e61 762d 6472 6f70 646f 776e 2d69 7465  nav-dropdown-ite
+00040b80: 6d3a 6c61 7374 2d6f 662d 7479 7065 207b  m:last-of-type {
+00040b90: 0a20 2062 6f72 6465 722d 626f 7474 6f6d  .  border-bottom
+00040ba0: 2d63 6f6c 6f72 3a20 7472 616e 7370 6172  -color: transpar
+00040bb0: 656e 743b 0a7d 0a2e 6865 6164 6572 2d68  ent;.}..header-h
+00040bc0: 6f6c 6465 7220 2e6d 6169 6e2d 6d65 6e75  older .main-menu
+00040bd0: 2075 6c20 6c69 2061 2e6e 6176 2d64 726f   ul li a.nav-dro
+00040be0: 7064 6f77 6e2d 6974 656d 3a68 6f76 6572  pdown-item:hover
+00040bf0: 207b 0a20 2062 6163 6b67 726f 756e 642d   {.  background-
+00040c00: 636f 6c6f 723a 2076 6172 282d 2d70 7974  color: var(--pyt
+00040c10: 6f72 6368 293b 0a20 2063 6f6c 6f72 3a20  orch);.  color: 
+00040c20: 7768 6974 653b 0a7d 0a2e 6865 6164 6572  white;.}..header
+00040c30: 2d68 6f6c 6465 7220 2e6d 6169 6e2d 6d65  -holder .main-me
+00040c40: 6e75 2075 6c20 6c69 2061 2e6e 6176 2d64  nu ul li a.nav-d
+00040c50: 726f 7064 6f77 6e2d 6974 656d 202e 6472  ropdown-item .dr
+00040c60: 6f70 646f 776e 2d74 6974 6c65 207b 0a20  opdown-title {. 
+00040c70: 2066 6f6e 742d 7369 7a65 3a20 312e 3132   font-size: 1.12
+00040c80: 3572 656d 3b0a 2020 636f 6c6f 723a 2023  5rem;.  color: #
+00040c90: 3663 3663 3664 3b0a 2020 6c65 7474 6572  6c6c6d;.  letter
+00040ca0: 2d73 7061 6369 6e67 3a20 303b 0a20 206c  -spacing: 0;.  l
+00040cb0: 696e 652d 6865 6967 6874 3a20 3334 7078  ine-height: 34px
+00040cc0: 3b0a 7d0a 0a2e 6865 6164 6572 2d68 6f6c  ;.}...header-hol
+00040cd0: 6465 7220 2e6d 6169 6e2d 6d65 6e75 2075  der .main-menu u
+00040ce0: 6c20 6c69 2061 2e6e 6176 2d64 726f 7064  l li a.nav-dropd
+00040cf0: 6f77 6e2d 6974 656d 3a68 6f76 6572 202e  own-item:hover .
+00040d00: 6472 6f70 646f 776e 2d74 6974 6c65 207b  dropdown-title {
+00040d10: 0a20 2062 6163 6b67 726f 756e 642d 636f  .  background-co
+00040d20: 6c6f 723a 2076 6172 282d 2d70 7974 6f72  lor: var(--pytor
+00040d30: 6368 293b 0a20 2063 6f6c 6f72 3a20 7768  ch);.  color: wh
+00040d40: 6974 653b 0a7d 0a0a 2e66 613a 6265 666f  ite;.}...fa:befo
+00040d50: 7265 207b 0a20 2066 6f6e 742d 6661 6d69  re {.  font-fami
+00040d60: 6c79 3a20 466f 6e74 4177 6573 6f6d 653b  ly: FontAwesome;
+00040d70: 0a20 2064 6973 706c 6179 3a20 696e 6c69  .  display: inli
+00040d80: 6e65 2d62 6c6f 636b 3b0a 2020 666f 6e74  ne-block;.  font
+00040d90: 2d73 7479 6c65 3a20 6e6f 726d 616c 3b0a  -style: normal;.
+00040da0: 2020 666f 6e74 2d77 6569 6768 743a 2034    font-weight: 4
+00040db0: 3030 3b0a 2020 666f 6e74 2d73 697a 653a  00;.  font-size:
+00040dc0: 2069 6e68 6572 6974 3b0a 2020 6c69 6e65   inherit;.  line
+00040dd0: 2d68 6569 6768 743a 2031 3b0a 2020 7061  -height: 1;.  pa
+00040de0: 6464 696e 672d 7269 6768 743a 2032 7078  dding-right: 2px
+00040df0: 3b0a 7d0a 2e66 612d 626c 6163 6b3a 6265  ;.}..fa-black:be
+00040e00: 666f 7265 207b 0a20 2063 6f6c 6f72 3a20  fore {.  color: 
+00040e10: 2762 6c61 636b 273b 0a7d 0a2e 6661 2d62  'black';.}..fa-b
+00040e20: 6c75 653a 6265 666f 7265 207b 0a20 2063  lue:before {.  c
+00040e30: 6f6c 6f72 3a20 7661 7228 2d2d 7265 6164  olor: var(--read
+00040e40: 7468 6564 6f63 293b 0a7d 0a2e 6661 2d6c  thedoc);.}..fa-l
+00040e50: 6172 6765 3a62 6566 6f72 6520 7b0a 2020  arge:before {.  
+00040e60: 666f 6e74 2d73 697a 653a 206c 6172 6765  font-size: large
+00040e70: 3b0a 7d0a 2e66 612e 6661 2d68 6f6d 653a  ;.}..fa.fa-home:
+00040e80: 6265 666f 7265 207b 0a20 2063 6f6e 7465  before {.  conte
+00040e90: 6e74 3a20 225c 4630 3135 223b 0a7d 0a2e  nt: "\F015";.}..
+00040ea0: 6661 2e66 612d 6769 7468 7562 3a62 6566  fa.fa-github:bef
+00040eb0: 6f72 6520 7b0a 2020 636f 6e74 656e 743a  ore {.  content:
+00040ec0: 2022 5c46 3039 4222 3b0a 7d0a 2e66 612e   "\F09B";.}..fa.
+00040ed0: 6661 2d61 7272 6f77 2d63 6972 636c 652d  fa-arrow-circle-
+00040ee0: 6c65 6674 3a62 6566 6f72 6520 7b0a 2020  left:before {.  
+00040ef0: 636f 6e74 656e 743a 2022 5c46 3041 3822  content: "\F0A8"
+00040f00: 3b0a 7d0a 2e66 612e 6661 2d61 7272 6f77  ;.}..fa.fa-arrow
+00040f10: 2d63 6972 636c 652d 7269 6768 743a 6265  -circle-right:be
+00040f20: 666f 7265 207b 0a20 2063 6f6e 7465 6e74  fore {.  content
+00040f30: 3a20 225c 4630 4139 223b 0a7d 0a0a 2e74  : "\F0A9";.}...t
+00040f40: 6f63 7472 6565 2d77 7261 7070 6572 202e  octree-wrapper .
+00040f50: 746f 6374 7265 652d 6c32 2061 207b 0a20  toctree-l2 a {. 
+00040f60: 2063 6f6c 6f72 3a20 7661 7228 2d2d 6c69   color: var(--li
+00040f70: 6768 746e 696e 6729 3b0a 7d0a 2e74 6f63  ghtning);.}..toc
+00040f80: 7472 6565 2d77 7261 7070 6572 202e 746f  tree-wrapper .to
+00040f90: 6374 7265 652d 6c32 202e 746f 6374 7265  ctree-l2 .toctre
+00040fa0: 652d 6c33 2061 207b 0a20 2063 6f6c 6f72  e-l3 a {.  color
+00040fb0: 3a20 7661 7228 2d2d 676f 6f67 6c65 2d67  : var(--google-g
+00040fc0: 7265 656e 293b 0a7d 0a2e 746f 6374 7265  reen);.}..toctre
+00040fd0: 652d 7772 6170 7065 7220 2e74 6f63 7472  e-wrapper .toctr
+00040fe0: 6565 2d6c 3220 2e74 6f63 7472 6565 2d6c  ee-l2 .toctree-l
+00040ff0: 3320 2e74 6f63 7472 6565 2d6c 3420 6120  3 .toctree-l4 a 
+00041000: 7b0a 2020 636f 6c6f 723a 2076 6172 282d  {.  color: var(-
+00041010: 2d72 6561 6474 6865 646f 6329 3b0a 7d0a  -readthedoc);.}.
+00041020: 0a2f 2a23 2073 6f75 7263 654d 6170 7069  ./*# sourceMappi
+00041030: 6e67 5552 4c3d 7468 656d 652e 6373 732e  ngURL=theme.css.
+00041040: 6d61 7020 2a2f 0a                        map */.
```

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.eot` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.ttf` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff2` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/arrow-down-orange.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/arrow-down-orange.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/arrow-right-with-tail.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/arrow-right-with-tail.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-black.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/chevron-down-black.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-grey.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/chevron-down-grey.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-orange.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/chevron-down-orange.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-white.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/chevron-down-white.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-right-orange.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/chevron-right-orange.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-right-white.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/chevron-right-white.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/home-footer-background.jpg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/home-footer-background.jpg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/icon-close.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/icon-close.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/search-icon.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/search-icon.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/versions.html` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme/versions.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/PKG-INFO` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trojanzoo-sphinx-theme
-Version: 0.1.5
+Version: 1.0.0
 Summary: TrojanZoo Sphinx Theme
 Home-page: https://github.com/ain-soph/trojanzoo_sphinx_theme
 Author: Ren Pang
 Author-email: rbp5354@psu.edu
 License: GPL-3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Sphinx :: Theme
@@ -19,16 +19,19 @@
 Classifier: Topic :: Software Development :: Documentation
 Requires-Python: >3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TrojanZoo Sphinx Theme
 
+
+![sphinx>=7.0](https://img.shields.io/badge/sphinx->=7.0-informational.svg)
+
 [![demo](https://github.com/ain-soph/trojanzoo_sphinx_theme/workflows/demo/badge.svg)](https://ain-soph.github.io/trojanzoo_sphinx_theme/)
-[![release](https://img.shields.io/github/v/release/ain-soph/trojanzoo_sphinx_theme)](https://github.com/ain-soph/trojanzoo/releases)
+[![release](https://img.shields.io/github/v/release/ain-soph/trojanzoo_sphinx_theme)](https://github.com/ain-soph/trojanzoo_sphinx_theme/releases)
 [![pypi](https://img.shields.io/pypi/v/trojanzoo_sphinx_theme)](https://pypi.org/project/trojanzoo_sphinx_theme/)
 
 Sphinx theme for [TrojanZoo Docs](https://ain-soph.github.io/trojanzoo) based on the [Read the Docs Sphinx Theme](https://sphinx-rtd-theme.readthedocs.io/en/latest). Forked from [Pytorch Sphinx Theme](https://github.com/pytorch/pytorch_sphinx_theme) with commit `b4d0005` at 09/24/2021.
 
 ## Difference from pytorch_sphinx_theme
 This work removes all pytorch-related things and support many customizations. It also removes all other unnecessary items to make it a pure doc template.  
 See demos at:
```

### Comparing `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/SOURCES.txt` & `trojanzoo_sphinx_theme-1.0.0/trojanzoo_sphinx_theme.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -85,8 +85,10 @@
 trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg
 trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg
 trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg
 trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg
 trojanzoo_sphinx_theme/static/images/search-icon.svg
 trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg
 trojanzoo_sphinx_theme/static/js/theme.js
-trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js
+trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js
+trojanzoo_sphinx_theme/static/js/vendor/bootstrap.min.js
+trojanzoo_sphinx_theme/static/js/vendor/popper.min.js
```

