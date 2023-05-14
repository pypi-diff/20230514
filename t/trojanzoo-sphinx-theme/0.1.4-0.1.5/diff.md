# Comparing `tmp/trojanzoo_sphinx_theme-0.1.4.tar.gz` & `tmp/trojanzoo_sphinx_theme-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trojanzoo_sphinx_theme-0.1.4.tar", last modified: Mon Aug  1 19:21:11 2022, max compression
+gzip compressed data, was "trojanzoo_sphinx_theme-0.1.5.tar", last modified: Wed Jan 11 12:19:11 2023, max compression
```

## Comparing `trojanzoo_sphinx_theme-0.1.4.tar` & `trojanzoo_sphinx_theme-0.1.5.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.668915 trojanzoo_sphinx_theme-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-08-01 19:21:11.668915 trojanzoo_sphinx_theme-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.656914 trojanzoo_sphinx_theme-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.656914 trojanzoo_sphinx_theme-0.1.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4700 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4399 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/configuring.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.656914 trojanzoo_sphinx_theme-0.1.4/docs/source/demo/
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/demo/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13932 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/demo/demo.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8935 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/demo/lists_tables.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/demo/long.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6226 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/demo/structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.656914 trojanzoo_sphinx_theme-0.1.4/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/images/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.656914 trojanzoo_sphinx_theme-0.1.4/docs/source/images/logo/
--rw-r--r--   0 runner    (1001) docker     (121)     8520 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/images/logo/trojanzoo-logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5671 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/images/logo/trojanzoo-logo-icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7587 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/images/logo/trojanzoo-logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6614 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/images/yi_jing_01_chien.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/installing.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.656914 trojanzoo_sphinx_theme-0.1.4/docs/source/test_py_module/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/test_py_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3145 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/docs/source/test_py_module/test.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-08-01 19:21:11.668915 trojanzoo_sphinx_theme-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.660914 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4352 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/fonts.html
--rw-r--r--   0 runner    (1001) docker     (121)     2170 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)    12349 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/linkcode.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/search.html
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.652914 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.660914 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)   266305 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/css/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.652914 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.660914 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FontAwesome/
--rw-r--r--   0 runner    (1001) docker     (121)   165742 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (121)   444379 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (121)   165548 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    98024 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (121)    77160 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.664914 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/
--rw-r--r--   0 runner    (1001) docker     (121)    39560 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (121)    31812 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    32396 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25672 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    33944 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff
--rw-r--r--   0 runner    (1001) docker     (121)    26832 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    31612 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25120 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    29304 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff
--rw-r--r--   0 runner    (1001) docker     (121)    22720 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    26908 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff
--rw-r--r--   0 runner    (1001) docker     (121)    21012 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    19420 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff
--rw-r--r--   0 runner    (1001) docker     (121)    16000 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    32072 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff
--rw-r--r--   0 runner    (1001) docker     (121)    25460 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.664914 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/
--rw-r--r--   0 runner    (1001) docker     (121)    50680 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff
--rw-r--r--   0 runner    (1001) docker     (121)    35916 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    51872 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff
--rw-r--r--   0 runner    (1001) docker     (121)    36648 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    50664 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    35536 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    52936 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff
--rw-r--r--   0 runner    (1001) docker     (121)    37592 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.668915 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/arrow-down-orange.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/arrow-right-with-tail.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/chevron-down-black.svg
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/chevron-down-grey.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/chevron-down-orange.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/chevron-down-white.svg
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/chevron-right-orange.svg
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/chevron-right-white.svg
--rw-r--r--   0 runner    (1001) docker     (121)    38907 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/home-footer-background.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/icon-close.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3284 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1703 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/search-icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.668915 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)    36099 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/js/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.668915 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (121)     6039 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-08-01 19:21:00.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:21:11.660914 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-08-01 19:21:11.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4635 2022-08-01 19:21:11.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 19:21:11.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-08-01 19:21:11.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 19:21:11.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-01 19:21:11.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-01 19:21:11.000000 trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.434750 trojanzoo_sphinx_theme-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-01-11 12:19:11.434750 trojanzoo_sphinx_theme-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.418749 trojanzoo_sphinx_theme-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.418749 trojanzoo_sphinx_theme-0.1.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/configuring.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.418749 trojanzoo_sphinx_theme-0.1.5/docs/source/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/demo/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/demo/demo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/demo/lists_tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/demo/long.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/demo/structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.422749 trojanzoo_sphinx_theme-0.1.5/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/images/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.422749 trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/trojanzoo-logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/trojanzoo-logo-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/trojanzoo-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/images/yi_jing_01_chien.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/installing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.422749 trojanzoo_sphinx_theme-0.1.5/docs/source/test_py_module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/test_py_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/docs/source/test_py_module/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-01-11 12:19:11.434750 trojanzoo_sphinx_theme-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.422749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/fonts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/linkcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.418749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.422749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   266305 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/css/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.418749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.426749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.426749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/
+-rw-r--r--   0 runner    (1001) docker     (123)    39560 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    31812 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    32396 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    25672 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33944 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    26832 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    25120 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    29304 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26908 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21012 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    19420 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    32072 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    25460 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.430750 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/
+-rw-r--r--   0 runner    (1001) docker     (123)    50680 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35916 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    36648 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    50664 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35536 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    52936 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    37592 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.434750 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/arrow-down-orange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/arrow-right-with-tail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-grey.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-orange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-right-orange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-right-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38907 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/home-footer-background.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/icon-close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/search-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.434750 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    36099 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/js/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.434750 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-01-11 12:19:00.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 12:19:11.422749 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-11 12:19:11.000000 trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/top_level.txt
```

### Comparing `trojanzoo_sphinx_theme-0.1.4/LICENSE` & `trojanzoo_sphinx_theme-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/PKG-INFO` & `trojanzoo_sphinx_theme-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trojanzoo_sphinx_theme
-Version: 0.1.4
+Version: 0.1.5
 Summary: TrojanZoo Sphinx Theme
 Home-page: https://github.com/ain-soph/trojanzoo_sphinx_theme
 Author: Ren Pang
 Author-email: rbp5354@psu.edu
 License: GPL-3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Sphinx :: Theme
```

### Comparing `trojanzoo_sphinx_theme-0.1.4/README.md` & `trojanzoo_sphinx_theme-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/make.bat` & `trojanzoo_sphinx_theme-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/conf.py` & `trojanzoo_sphinx_theme-0.1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/configuring.rst` & `trojanzoo_sphinx_theme-0.1.5/docs/source/configuring.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/demo/api.rst` & `trojanzoo_sphinx_theme-0.1.5/docs/source/demo/api.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/demo/demo.rst` & `trojanzoo_sphinx_theme-0.1.5/docs/source/demo/demo.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/demo/lists_tables.rst` & `trojanzoo_sphinx_theme-0.1.5/docs/source/demo/lists_tables.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/demo/long.rst` & `trojanzoo_sphinx_theme-0.1.5/docs/source/demo/long.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/demo/structure.rst` & `trojanzoo_sphinx_theme-0.1.5/docs/source/demo/structure.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/images/favicon.ico` & `trojanzoo_sphinx_theme-0.1.5/docs/source/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/images/logo/trojanzoo-logo-dark.svg` & `trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/trojanzoo-logo-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/images/logo/trojanzoo-logo-icon.svg` & `trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/trojanzoo-logo-icon.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/images/logo/trojanzoo-logo.svg` & `trojanzoo_sphinx_theme-0.1.5/docs/source/images/logo/trojanzoo-logo.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/images/yi_jing_01_chien.jpg` & `trojanzoo_sphinx_theme-0.1.5/docs/source/images/yi_jing_01_chien.jpg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/docs/source/test_py_module/test.py` & `trojanzoo_sphinx_theme-0.1.5/docs/source/test_py_module/test.py`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/setup.cfg` & `trojanzoo_sphinx_theme-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 universal = 1
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = trojanzoo_sphinx_theme
 install_requires = 
-	sphinx>=4.2.0
+	sphinx>=4.2.0,<5.2.0
 	docutils>=0.17.1
 python_requires = >3
 
 [options.package_data]
 trojanzoo_sphinx_theme = 
 	theme.conf
 	*.html
```

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/__init__.py` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/breadcrumbs.html` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/fonts.html` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/fonts.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/footer.html` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/footer.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/layout.html` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/linkcode.py` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/linkcode.py`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/search.html` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/css/theme.css` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.eot` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.ttf` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff2` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/arrow-down-orange.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/arrow-down-orange.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/arrow-right-with-tail.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/arrow-right-with-tail.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/chevron-down-black.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-black.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/chevron-down-grey.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-grey.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/chevron-down-orange.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-orange.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/chevron-down-white.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-down-white.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/chevron-right-orange.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-right-orange.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/chevron-right-white.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/chevron-right-white.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/home-footer-background.jpg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/home-footer-background.jpg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/icon-close.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/icon-close.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/search-icon.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/search-icon.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/js/theme.js` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme/versions.html` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme/versions.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme.egg-info/PKG-INFO` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trojanzoo-sphinx-theme
-Version: 0.1.4
+Version: 0.1.5
 Summary: TrojanZoo Sphinx Theme
 Home-page: https://github.com/ain-soph/trojanzoo_sphinx_theme
 Author: Ren Pang
 Author-email: rbp5354@psu.edu
 License: GPL-3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Sphinx :: Theme
```

### Comparing `trojanzoo_sphinx_theme-0.1.4/trojanzoo_sphinx_theme.egg-info/SOURCES.txt` & `trojanzoo_sphinx_theme-0.1.5/trojanzoo_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

