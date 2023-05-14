# Comparing `tmp/trojanzoo_sphinx_theme-1.0.1.tar.gz` & `tmp/trojanzoo_sphinx_theme-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trojanzoo_sphinx_theme-1.0.1.tar", last modified: Sun May 14 09:49:52 2023, max compression
+gzip compressed data, was "trojanzoo_sphinx_theme-1.0.2.tar", last modified: Sun May 14 20:54:31 2023, max compression
```

## Comparing `trojanzoo_sphinx_theme-1.0.1.tar` & `trojanzoo_sphinx_theme-1.0.2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.436724 trojanzoo_sphinx_theme-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-14 09:49:52.436724 trojanzoo_sphinx_theme-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.416724 trojanzoo_sphinx_theme-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.416724 trojanzoo_sphinx_theme-1.0.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/configuring.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.420724 trojanzoo_sphinx_theme-1.0.1/docs/source/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/demo/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/demo/demo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/demo/lists_tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/demo/long.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/demo/structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.420724 trojanzoo_sphinx_theme-1.0.1/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/images/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.420724 trojanzoo_sphinx_theme-1.0.1/docs/source/images/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/images/logo/trojanzoo-logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/images/logo/trojanzoo-logo-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/images/logo/trojanzoo-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/images/yi_jing_01_chien.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/installing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.420724 trojanzoo_sphinx_theme-1.0.1/docs/source/test_py_module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/test_py_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/docs/source/test_py_module/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-14 09:49:52.436724 trojanzoo_sphinx_theme-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.424724 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/fonts.html
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/linkcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.412724 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.428724 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   266311 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/css/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.412724 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.432724 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FontAwesome/
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.432724 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/
--rw-r--r--   0 runner    (1001) docker     (123)    39560 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    31812 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    32396 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    25672 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33944 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    26832 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff
--rw-r--r--   0 runner    (1001) docker     (123)    25120 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    29304 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26908 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff
--rw-r--r--   0 runner    (1001) docker     (123)    21012 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    19420 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    32072 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff
--rw-r--r--   0 runner    (1001) docker     (123)    25460 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.432724 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/
--rw-r--r--   0 runner    (1001) docker     (123)    50680 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff
--rw-r--r--   0 runner    (1001) docker     (123)    35916 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff
--rw-r--r--   0 runner    (1001) docker     (123)    36648 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    50664 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    35536 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    52936 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    37592 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.436724 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/arrow-down-orange.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/arrow-right-with-tail.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/chevron-down-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/chevron-down-grey.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/chevron-down-orange.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/chevron-down-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/chevron-right-orange.svg
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/chevron-right-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)    38907 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/home-footer-background.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/icon-close.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/search-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.436724 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/js/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.436724 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    58072 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/js/vendor/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/js/vendor/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-14 09:49:43.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:49:52.428724 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-14 09:49:52.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-14 09:49:52.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:49:52.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 09:49:52.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:49:52.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-14 09:49:52.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 09:49:52.000000 trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.323410 trojanzoo_sphinx_theme-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-14 20:54:31.323410 trojanzoo_sphinx_theme-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.315410 trojanzoo_sphinx_theme-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.315410 trojanzoo_sphinx_theme-1.0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/configuring.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.315410 trojanzoo_sphinx_theme-1.0.2/docs/source/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/demo/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/demo/demo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/demo/lists_tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/demo/long.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/demo/structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.315410 trojanzoo_sphinx_theme-1.0.2/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/images/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.315410 trojanzoo_sphinx_theme-1.0.2/docs/source/images/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/images/logo/trojanzoo-logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/images/logo/trojanzoo-logo-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/images/logo/trojanzoo-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/images/yi_jing_01_chien.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/installing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.315410 trojanzoo_sphinx_theme-1.0.2/docs/source/test_py_module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/test_py_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/docs/source/test_py_module/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-14 20:54:31.327410 trojanzoo_sphinx_theme-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.315410 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/fonts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/linkcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.311410 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.319409 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   266311 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/css/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.311410 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.319409 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FontAwesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.323410 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/
+-rw-r--r--   0 runner    (1001) docker     (123)    39560 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    31812 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    32396 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    25672 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33944 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    26832 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    25120 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    29304 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26908 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21012 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    19420 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    32072 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    25460 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.323410 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/
+-rw-r--r--   0 runner    (1001) docker     (123)    50680 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35916 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    36648 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    50664 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35536 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    52936 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    37592 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.323410 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/arrow-down-orange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/arrow-right-with-tail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/chevron-down-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/chevron-down-grey.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/chevron-down-orange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/chevron-down-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/chevron-right-orange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/chevron-right-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38907 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/home-footer-background.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/icon-close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/search-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.323410 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/js/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.323410 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58072 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/js/vendor/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/js/vendor/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-14 20:54:21.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:54:31.319409 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-14 20:54:31.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-14 20:54:31.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:54:31.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 20:54:31.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:54:31.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-14 20:54:31.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 20:54:31.000000 trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme.egg-info/top_level.txt
```

### Comparing `trojanzoo_sphinx_theme-1.0.1/LICENSE` & `trojanzoo_sphinx_theme-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/PKG-INFO` & `trojanzoo_sphinx_theme-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trojanzoo_sphinx_theme
-Version: 1.0.1
+Version: 1.0.2
 Summary: TrojanZoo Sphinx Theme
 Home-page: https://github.com/ain-soph/trojanzoo_sphinx_theme
 Author: Ren Pang
 Author-email: rbp5354@psu.edu
 License: GPL-3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Sphinx :: Theme
```

### Comparing `trojanzoo_sphinx_theme-1.0.1/README.md` & `trojanzoo_sphinx_theme-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/make.bat` & `trojanzoo_sphinx_theme-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/conf.py` & `trojanzoo_sphinx_theme-1.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/configuring.rst` & `trojanzoo_sphinx_theme-1.0.2/docs/source/configuring.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/demo/api.rst` & `trojanzoo_sphinx_theme-1.0.2/docs/source/demo/api.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/demo/demo.rst` & `trojanzoo_sphinx_theme-1.0.2/docs/source/demo/demo.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/demo/lists_tables.rst` & `trojanzoo_sphinx_theme-1.0.2/docs/source/demo/lists_tables.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/demo/long.rst` & `trojanzoo_sphinx_theme-1.0.2/docs/source/demo/long.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/demo/structure.rst` & `trojanzoo_sphinx_theme-1.0.2/docs/source/demo/structure.rst`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/images/favicon.ico` & `trojanzoo_sphinx_theme-1.0.2/docs/source/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/images/logo/trojanzoo-logo-dark.svg` & `trojanzoo_sphinx_theme-1.0.2/docs/source/images/logo/trojanzoo-logo-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/images/logo/trojanzoo-logo-icon.svg` & `trojanzoo_sphinx_theme-1.0.2/docs/source/images/logo/trojanzoo-logo-icon.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/images/logo/trojanzoo-logo.svg` & `trojanzoo_sphinx_theme-1.0.2/docs/source/images/logo/trojanzoo-logo.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/images/yi_jing_01_chien.jpg` & `trojanzoo_sphinx_theme-1.0.2/docs/source/images/yi_jing_01_chien.jpg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/docs/source/test_py_module/test.py` & `trojanzoo_sphinx_theme-1.0.2/docs/source/test_py_module/test.py`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/setup.cfg` & `trojanzoo_sphinx_theme-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/__init__.py` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/breadcrumbs.html` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/fonts.html` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/fonts.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/footer.html` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/footer.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/layout.html` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/layout.html`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,14 @@
   <link rel="search" type="application/opensearchdescription+xml"
     title="{% trans docstitle=docstitle|e %}Search within {{ docstitle }}{% endtrans %}"
     href="{{ pathto('_static/opensearch.xml', 1) }}" />
   {% endif %}
 
   {% endif %}
 
-  <link rel="stylesheet" href="{{ pathto('_static/' + styles[-1], 1) }}" type="text/css" />
-  <!-- <link rel="stylesheet" href="{{ pathto('_static/pygments.css', 1) }}" type="text/css" /> -->
   {%- for css in css_files %}
   {%- if css|attr("rel") %}
   <link rel="{{ css.rel }}" href="{{ pathto(css.filename, 1) }}" type="text/css" {% if css.title is not none %}
     title="{{ css.title }}" {% endif %} />
   {%- else %}
   <link rel="stylesheet" href="{{ pathto(css, 1) }}" type="text/css" />
   {%- endif %}
```

#### html2text {}

```diff
@@ -6,16 +6,15 @@
 
  {{ metatags }}
  {% block htmltitle %}
 {% endblock %} {# FAVICON #} {% if favicon %}
  {% endif %} {# CANONICAL URL #} {% if html_baseurl %}
  {% endif %} {# CSS #} {# OPENSEARCH #} {% if not embedded %} {% if
 use_opensearch %}
- {% endif %} {% endif %}
-  {%- for css in css_files %} {%- if css|attr("rel") %}
+ {% endif %} {% endif %} {%- for css in css_files %} {%- if css|attr("rel") %}
 % if css.title is not none %} title="{{ css.title }}" {% endif %} /> {%- else
 %}
  {%- endif %} {%- endfor %} {%- for cssfile in extra_css_files %}
  {%- endfor %} {%- block linktags %} {%- if hasdoc('about') %}
  {%- endif %} {%- if hasdoc('genindex') %}
  {%- endif %} {%- if hasdoc('search') %}
  {%- endif %} {%- if hasdoc('copyright') %}
```

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/linkcode.py` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/linkcode.py`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/search.html` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/css/theme.css` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.eot` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.ttf` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FontAwesome/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-bold.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book-italic.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-book.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light-italic.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-light.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium-italic.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/FreightSans/freight-sans-medium.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Light.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Medium.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-Regular.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff2` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/fonts/IBMPlexMono/IBMPlexMono-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/arrow-down-orange.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/arrow-down-orange.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/arrow-right-with-tail.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/arrow-right-with-tail.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/chevron-down-black.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/chevron-down-black.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/chevron-down-grey.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/chevron-down-grey.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/chevron-down-orange.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/chevron-down-orange.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/chevron-down-white.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/chevron-down-white.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/chevron-right-orange.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/chevron-right-orange.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/chevron-right-white.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/chevron-right-white.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/home-footer-background.jpg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/home-footer-background.jpg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/icon-close.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/icon-close.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/icon-menu-dots-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/logo-facebook-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/logo-twitter-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/logo-youtube-dark.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/search-icon.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/search-icon.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/images/view-page-source-icon.svg`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/js/theme.js` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/js/vendor/anchor.min.js`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/js/vendor/bootstrap.min.js` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/js/vendor/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/static/js/vendor/popper.min.js` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/static/js/vendor/popper.min.js`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme/versions.html` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme/versions.html`

 * *Files identical despite different names*

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme.egg-info/PKG-INFO` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trojanzoo-sphinx-theme
-Version: 1.0.1
+Version: 1.0.2
 Summary: TrojanZoo Sphinx Theme
 Home-page: https://github.com/ain-soph/trojanzoo_sphinx_theme
 Author: Ren Pang
 Author-email: rbp5354@psu.edu
 License: GPL-3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Sphinx :: Theme
```

### Comparing `trojanzoo_sphinx_theme-1.0.1/trojanzoo_sphinx_theme.egg-info/SOURCES.txt` & `trojanzoo_sphinx_theme-1.0.2/trojanzoo_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

