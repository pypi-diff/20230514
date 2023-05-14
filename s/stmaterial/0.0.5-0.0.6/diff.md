# Comparing `tmp/stmaterial-0.0.5.tar.gz` & `tmp/stmaterial-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stmaterial-0.0.5.tar", last modified: Wed May 10 05:46:17 2023, max compression
+gzip compressed data, was "stmaterial-0.0.6.tar", last modified: Sun May 14 03:21:24 2023, max compression
```

## Comparing `stmaterial-0.0.5.tar` & `stmaterial-0.0.6.tar`

### file list

```diff
@@ -1,210 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:46:17.492102 stmaterial-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-10 05:45:45.148052 stmaterial-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 05:45:45.148052 stmaterial-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-10 05:45:45.148052 stmaterial-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.152052 stmaterial-0.0.5/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-10 05:45:45.148052 stmaterial-0.0.5/docs/_images/a.png
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-10 05:45:45.148052 stmaterial-0.0.5/docs/_images/b.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.152052 stmaterial-0.0.5/docs/_images/books/
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-05-10 05:45:45.152052 stmaterial-0.0.5/docs/_images/books/benders分解.png
--rw-r--r--   0 runner    (1001) docker     (123)   394770 2023-05-10 05:45:45.152052 stmaterial-0.0.5/docs/_images/books/内点法.png
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-10 05:45:45.152052 stmaterial-0.0.5/docs/_images/c.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.152052 stmaterial-0.0.5/docs/_images/links/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_images/links/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)   164525 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_images/links/gallery/jupyter_book.png
--rw-r--r--   0 runner    (1001) docker     (123)    93132 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_images/links/gallery/matplotlib.png
--rw-r--r--   0 runner    (1001) docker     (123)   112977 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_images/links/gallery/pandas.png
--rw-r--r--   0 runner    (1001) docker     (123)   204727 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_images/links/gallery/sphinx_design.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_static/links/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_static/links/gallery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_static/logo-.png
--rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 05:45:45.156052 stmaterial-0.0.5/docs/blog.md
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/kitchen-sink/typography.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/examples/reference/text-formatting.md
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/posts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/posts/plangs/
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/posts/plangs/2021-python-pathlib.md
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/posts/plangs/2022-pytest-tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/posts/plangs/2022-python-setup.md
--rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/posts/plangs/2022-python-typing.md
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide/header.md
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide/sidenav.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/edit-button.md
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/fonts.md
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/header.md
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/index1.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/landing-page.md
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/logo.md
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/sidebar-title.md
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/sidebar.md
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/user_guide_tmp/toc.md
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-10 05:45:45.160052 stmaterial-0.0.5/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-10 05:45:45.160052 stmaterial-0.0.5/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   220389 2023-05-10 05:45:45.160052 stmaterial-0.0.5/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-10 05:45:45.160052 stmaterial-0.0.5/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 05:45:45.160052 stmaterial-0.0.5/postcss.config.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-05-10 05:45:45.160052 stmaterial-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.160052 stmaterial-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/_navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/_translations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/scripts/gumshoe-patched.js
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/scripts/materialize.js
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/scripts/stmaterial.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/base/_theme.sass
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/base/_typography.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_brand-logo.scss
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_breadcrumb.sass
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_edit-update-meta.scss
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_searchbox.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/components/_table-of-contents.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_admonitions.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_api.sass
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_code.sass
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_gui-labels.sass
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_lists.sass
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_spans.scss
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_ablog.scss
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_myst-nb.scss
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_tippy.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/patch/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/patch/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/patch/_legacy.sass
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/patch/_patch.scss
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/patch/_test.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_article.sass
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_headnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_stm-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/stmaterial.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_colors.scss
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/stmaterial theme.json
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/demo/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/directives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3333 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/brand-logo.html
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/headnav-items.html
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/license.html
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/postnav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-10 05:45:45.164052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/static/images/github.svg
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/theme/stmaterial/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-10 05:45:45.168052 stmaterial-0.0.5/src/stmaterial/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:45:45.168052 stmaterial-0.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-10 05:45:45.168052 stmaterial-0.0.5/webpack.config.js
--rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 stmaterial-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:24.695963 stmaterial-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-14 03:21:07.611593 stmaterial-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-14 03:21:07.611593 stmaterial-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-14 03:21:07.611593 stmaterial-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-14 03:21:07.611593 stmaterial-0.0.6/docs/_images/a.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-14 03:21:07.611593 stmaterial-0.0.6/docs/_images/b.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.611593 stmaterial-0.0.6/docs/_images/books/
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-05-14 03:21:07.611593 stmaterial-0.0.6/docs/_images/books/benders分解.png
+-rw-r--r--   0 runner    (1001) docker     (123)   394770 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/books/内点法.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/c.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/links/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/links/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)   164525 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/links/gallery/jupyter_book.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93132 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/links/gallery/matplotlib.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112977 2023-05-14 03:21:07.615594 stmaterial-0.0.6/docs/_images/links/gallery/pandas.png
+-rw-r--r--   0 runner    (1001) docker     (123)   204727 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_images/links/gallery/sphinx_design.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_static/links/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_static/links/gallery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_static/logo-.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/blog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/develop.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/kitchen-sink/typography.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/examples/reference/text-formatting.md
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/posts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/posts/plangs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/posts/plangs/2021-python-pathlib.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/posts/plangs/2022-pytest-tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/posts/plangs/2022-python-setup.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/posts/plangs/2022-python-typing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide/header.md
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide/sidenav.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide/source-buttons.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/edit-button.md
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/fonts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/header.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/index1.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/landing-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/logo.md
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/sidebar-title.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/sidebar.md
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/user_guide_tmp/toc.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-14 03:21:07.619594 stmaterial-0.0.6/docs/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-14 03:21:07.619594 stmaterial-0.0.6/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220389 2023-05-14 03:21:07.619594 stmaterial-0.0.6/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-14 03:21:07.619594 stmaterial-0.0.6/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-14 03:21:07.619594 stmaterial-0.0.6/postcss.config.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1507 2023-05-14 03:21:07.619594 stmaterial-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.619594 stmaterial-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-05-14 03:21:07.619594 stmaterial-0.0.6/src/stmaterial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-05-14 03:21:07.619594 stmaterial-0.0.6/src/stmaterial/_navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-14 03:21:07.619594 stmaterial-0.0.6/src/stmaterial/_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/_translations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/scripts/gumshoe-patched.js
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/scripts/materialize.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/scripts/stmaterial.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/base/_theme.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/base/_typography.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_article-metadata-info.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_breadcrumb.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_scrollbar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_searchbox.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_sidenav-icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/components/_table-of-contents.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_admonitions.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_api.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_code.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_gui-labels.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_lists.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_math.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_spans.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_ablog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_myst-nb.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_tippy.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/patch/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/patch/_legacy.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/patch/_patch.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/patch/_test.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_article.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_headnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_stm-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/stmaterial.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_colors.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/stmaterial theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/directives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3418 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/brand-logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/headnav-items.html
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/license.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/postnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/partials/_icon_links_declaration.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/static/images/github.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/theme/stmaterial/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-14 03:21:07.623594 stmaterial-0.0.6/src/stmaterial/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 03:21:07.623594 stmaterial-0.0.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-14 03:21:07.623594 stmaterial-0.0.6/webpack.config.js
+-rw-r--r--   0        0        0     4163 1970-01-01 00:00:00.000000 stmaterial-0.0.6/PKG-INFO
```

### Comparing `stmaterial-0.0.5/LICENSE` & `stmaterial-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_images/a.png` & `stmaterial-0.0.6/docs/_images/a.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_images/b.png` & `stmaterial-0.0.6/docs/_images/b.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_images/books/benders分解.png` & `stmaterial-0.0.6/docs/_images/books/benders分解.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_images/books/内点法.png` & `stmaterial-0.0.6/docs/_images/books/内点法.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_images/c.png` & `stmaterial-0.0.6/docs/_images/c.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_images/links/gallery/jupyter_book.png` & `stmaterial-0.0.6/docs/_images/links/gallery/jupyter_book.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_images/links/gallery/matplotlib.png` & `stmaterial-0.0.6/docs/_images/links/gallery/matplotlib.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_images/links/gallery/pandas.png` & `stmaterial-0.0.6/docs/_images/links/gallery/pandas.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_images/links/gallery/sphinx_design.png` & `stmaterial-0.0.6/docs/_images/links/gallery/sphinx_design.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_static/favicon.png` & `stmaterial-0.0.6/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_static/links/gallery.yaml` & `stmaterial-0.0.6/docs/_static/links/gallery.yaml`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_static/logo-.png` & `stmaterial-0.0.6/docs/_static/logo-.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/_static/logo.png` & `stmaterial-0.0.6/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/conf.py` & `stmaterial-0.0.6/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,40 +21,40 @@
     "ablog",
     "myst_parser",
     "sphinx_inline_tabs",
     "sphinx_design",
     "sphinx_copybutton",
     "sphinx_togglebutton",
     "sphinx_subfigure",
-    "sphinx_tippy"
 ]
 
 
 myst_enable_extensions = ["colon_fence", "deflist"]
 exclude_patterns = [
     "_build", 
     "Thumbs.db", 
     ".DS_Store",
     "contributing",
     "user_guide_tmp/*"
 ]
 
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/3.7", None),
+    "python": ("https://docs.python.org/3.9", None),
     "sphinx": ("https://www.sphinx-doc.org/en/master", None),
     "markdown_it": ("https://markdown-it-py.readthedocs.io/en/latest", None),
 }
 
 templates_path = ["_templates"]
 html_static_path = ["_static"]
 html_theme = "stmaterial"
 html_title = "sphinx theme of material"
 html_favicon = "_static/favicon.png"
 html_last_updated_fmt = ""
 html_logo = "_static/logo-.png"
+html_show_sourcelink = False
 
 todo_include_todos = True
 
 
 html_theme_options = {
     "header_links_before_dropdown": 4,
     "source_repository": "https://github.com/zclab/stmaterial",
@@ -70,18 +70,20 @@
         {"name": "Furo", "url": "https://pradyunsg.me/furo/quickstart/"},
         {"name": "Sphinx book theme", "url": "https://sphinx-book-theme.readthedocs.io/en/latest/"},
         {"name": "Pydata sphinx theme", "url": "https://pydata-sphinx-theme.readthedocs.io/"},
     ],
     "show_toc_level": 1,
     "header_icons": [
         {"name":"Github", "url": "http://github.com/zclab/stmaterial", "fontawesome":"fa-brands fa-github"},
-        # {"name":"Email", "url": "example@example.com", "material_icons":"email"},
+    ],
+    "sidenav_icons": [
+        {"name":"pypistats", "url": "https://pypistats.org/packages/stmaterial", "image":"https://img.shields.io/pypi/dm/stmaterial.svg?style=flat-square"},
+        {"name":"Github Stars", "url": "https://github.com/zclab/stmaterial", "image":"https://img.shields.io/github/stars/zclab/stmaterial?style=flat-square&logo=github"},
     ],
     "footer_icons": [
-        {"name":"PyPi", "url": "https://pypi.org/project/stmaterial/", "image":"https://img.shields.io/pypi/dw/stmaterial"},
         {"name":"Licence", "url": "https://github.com/zclab/stmaterial/blob/main/LICENSE", "fontawesome":"fa-solid fa-file"},
         {"name":"Github", "url": "http://github.com/zclab/stmaterial", "fontawesome":"fa-brands fa-github"},
     ],
     "use_edit_page_button": True,
     "toc_title": "On this page",
     "custom_fonts": {
         "name": 'LXGWWenKaiLite',
```

### Comparing `stmaterial-0.0.5/docs/develop.md` & `stmaterial-0.0.6/docs/develop.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/kitchen-sink/admonitions.rst` & `stmaterial-0.0.6/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/kitchen-sink/api.rst` & `stmaterial-0.0.6/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/kitchen-sink/blocks.rst` & `stmaterial-0.0.6/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/kitchen-sink/generic.rst` & `stmaterial-0.0.6/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/kitchen-sink/images.rst` & `stmaterial-0.0.6/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/kitchen-sink/index.md` & `stmaterial-0.0.6/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/kitchen-sink/lists.rst` & `stmaterial-0.0.6/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/kitchen-sink/really-long.md` & `stmaterial-0.0.6/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/kitchen-sink/sphinx-design.md` & `stmaterial-0.0.6/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/kitchen-sink/structure.rst` & `stmaterial-0.0.6/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/kitchen-sink/tables.rst` & `stmaterial-0.0.6/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/kitchen-sink/typography.rst` & `stmaterial-0.0.6/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/reference/admonitions.md` & `stmaterial-0.0.6/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/reference/api.md` & `stmaterial-0.0.6/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/reference/code-blocks.md` & `stmaterial-0.0.6/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/reference/hyperlinks.md` & `stmaterial-0.0.6/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/reference/images.md` & `stmaterial-0.0.6/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/reference/index.md` & `stmaterial-0.0.6/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/reference/lists.md` & `stmaterial-0.0.6/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/reference/tables.md` & `stmaterial-0.0.6/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/reference/tabs.md` & `stmaterial-0.0.6/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/examples/reference/text-formatting.md` & `stmaterial-0.0.6/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/posts/plangs/2021-python-pathlib.md` & `stmaterial-0.0.6/docs/posts/plangs/2021-python-pathlib.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/posts/plangs/2022-pytest-tutorial.md` & `stmaterial-0.0.6/docs/posts/plangs/2022-pytest-tutorial.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/posts/plangs/2022-python-setup.md` & `stmaterial-0.0.6/docs/posts/plangs/2022-python-setup.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/posts/plangs/2022-python-typing.md` & `stmaterial-0.0.6/docs/posts/plangs/2022-python-typing.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/user_guide/header.md` & `stmaterial-0.0.6/docs/user_guide/header.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/user_guide/sidenav.md` & `stmaterial-0.0.6/docs/user_guide/sidenav.md`

 * *Files 16% similar despite different names*

```diff
@@ -35,8 +35,21 @@
 hide-sidenav: true
 ---
 
 [page contents]
 ```
 ````
 
+
+## Set up sidenav icons
+
+Stmaterial allows set up the icons that are presented in the sidenav, there is no sidenav icons by default. To add custom sidenav icons, you need to provide the `sidenav_icons` configuration value to Stmaterial. 
+
+```python
+html_theme_options = {
+    "sidenav_icons": [
+        {"name":"Gitlab", "url": "http://gitlabcom/zclab/stmaterial", "fontawesome":"fa-brands fa-gitlab"},
+    ],
+}
+```
+
 [sphinx-file-wide-metadata]: https://www.sphinx-doc.org/en/master/usage/restructuredtext/field-lists.html#metadata
```

### Comparing `stmaterial-0.0.5/docs/user_guide_tmp/edit-button.md` & `stmaterial-0.0.6/docs/user_guide_tmp/edit-button.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/user_guide_tmp/fonts.md` & `stmaterial-0.0.6/docs/user_guide_tmp/fonts.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/user_guide_tmp/header.md` & `stmaterial-0.0.6/docs/user_guide_tmp/header.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/user_guide_tmp/index1.md` & `stmaterial-0.0.6/docs/user_guide_tmp/index1.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/user_guide_tmp/landing-page.md` & `stmaterial-0.0.6/docs/user_guide_tmp/landing-page.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/user_guide_tmp/logo.md` & `stmaterial-0.0.6/docs/user_guide_tmp/logo.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/user_guide_tmp/sidebar.md` & `stmaterial-0.0.6/docs/user_guide_tmp/sidebar.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/user_guide_tmp/toc.md` & `stmaterial-0.0.6/docs/user_guide_tmp/toc.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/docs/web-components.rst` & `stmaterial-0.0.6/docs/web-components.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/noxfile.py` & `stmaterial-0.0.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/package-lock.json` & `stmaterial-0.0.6/package-lock.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/package.json` & `stmaterial-0.0.6/package.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/pyproject.toml` & `stmaterial-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,14 @@
   "Development Status :: 2 - Pre-Alpha",
   "Framework :: Sphinx",
   "Framework :: Sphinx :: Theme",
   "License :: OSI Approved :: MIT License",
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: OS Independent",
   "Topic :: Documentation",
   "Topic :: Software Development :: Documentation",
@@ -50,8 +49,8 @@
 dev = ['sphinx-theme-builder[cli] >= 0.2.0b2']
 
 [project.entry-points]
 "sphinx.html_themes" = { stmaterial = "stmaterial" }
 
 [project.urls]
 Repository = "https://github.com/zclab/stmaterial"
-Documentation = "https://zclab.github.io/stmaterial/"
+Documentation = "https://stmaterial.readthedocs.io/en/latest/"
```

### Comparing `stmaterial-0.0.5/src/stmaterial/__init__.py` & `stmaterial-0.0.6/src/stmaterial/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from sphinx.locale import get_translation
 from ._navigation import add_toctree_functions
 from ._transforms import ShortenLinkTransform, WrapTableAndMathInAContainerTransform
 from .utils import get_theme_options, config_provided_by_user
 from .directives import GalleryDirective
 
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 logger = logging.getLogger(__name__)
 
 MESSAGE_CATALOG_NAME = "stmaterial"
 _KNOWN_STYLES_IN_USE: Dict[str, Optional[Style]] = {
     "light": None,
     "dark": None,
 }
```

### Comparing `stmaterial-0.0.5/src/stmaterial/_navigation.py` & `stmaterial-0.0.6/src/stmaterial/_navigation.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/_transforms.py` & `stmaterial-0.0.6/src/stmaterial/_transforms.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/_translations.py` & `stmaterial-0.0.6/src/stmaterial/_translations.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/scripts/gumshoe-patched.js` & `stmaterial-0.0.6/src/stmaterial/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/scripts/stmaterial.js` & `stmaterial-0.0.6/src/stmaterial/assets/scripts/stmaterial.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/base/_typography.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/base/_typography.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/components/_back-to-top.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/components/_back-to-top.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/components/_brand-logo.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/components/_brand-logo.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/components/_prev-next.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/components/_searchbox.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/components/_searchbox.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/components/_table-of-contents.sass` & `stmaterial-0.0.6/src/stmaterial/assets/styles/components/_table-of-contents.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_admonitions.sass` & `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_admonitions.sass`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     margin-top: 0
 
   // Last item should have no margin, since we'll control that w/ padding
   > :last-child
     margin-bottom: 0
 
 p.admonition-title, p.topic-title
+  display: flex
+  align-items: center
   position: relative
   margin: 0 -0.5rem 0.5rem
   padding-left: 2rem
   padding-right: .5rem
   padding-top: .4rem
   padding-bottom: .4rem
```

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_api.sass` & `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_api.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_code.sass` & `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_code.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_footnotes.sass` & `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_images.sass` & `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_lists.sass` & `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_lists.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_misc.sass` & `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_sidebar.sass` & `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_tables.sass` & `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/content/_target.sass` & `stmaterial-0.0.6/src/stmaterial/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_ablog.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_ablog.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/extensions/_timeline.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/extensions/_timeline.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/patch/_legacy.sass` & `stmaterial-0.0.6/src/stmaterial/assets/styles/patch/_legacy.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/patch/_test.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/patch/_test.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_footer.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_footer.scss`

 * *Files 5% similar despite different names*

```diff
@@ -32,21 +32,24 @@
 .stm-bottom-footer {
   display: flex;
   align-items: center;
   justify-content: space-between;
 }
 
 .stm-right-footer {
-  display: flex;
-  align-items: center;
-  gap: 1.2rem;
   font-size: 24px;
 
   a {
-    display: contents;
     color: var(--font-color-medium);
   }
 
   i.material-icons {
     font-size: 28px;
   }
+
+  ul {
+    display: flex;
+    align-items: center;
+    gap: 1.2rem;
+    margin: 0;
+  }
 }
```

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_headnav.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_headnav.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/sections/_stm-sidenav.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/sections/_stm-sidenav.scss`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
       height: 100%;
       // width: $sidenav-width;
 
       .sidenav-menu {
         flex-grow: 1;
         padding: 0 0 0 var(--header-horizontal-spacing);
         overflow: auto;
+        margin-top: 1.0rem;
 
         .sidenav-menulist {
           list-style: none;
           margin: 0;
           padding-left: 0;
 
           p {
```

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_admonitions.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_colors.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_colors.scss`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 
   // GUI Labels
   --color-guilabel-background: #ddeeff80;
   --color-guilabel-border: #bedaf580;
   --color-guilabel-text: var(--font-color-main);
   // Dropdown colors
   --dropdown-color: var(--primary-color);
+
+  --input-focus-color: var(--secondary-color-focus-solid);
 }
 
 @mixin colors-dark {
   // primary and secondary color
   --primary-color: #B39DDB;
   --primary-color-dark: #9575CD;
   --primary-color-numeric: 179, 157, 219;
```

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/styles/variables/_icons.scss` & `stmaterial-0.0.6/src/stmaterial/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/translations/README.md` & `stmaterial-0.0.6/src/stmaterial/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/Edit this page.json` & `stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/assets/translations/jsons/On this page.json` & `stmaterial-0.0.6/src/stmaterial/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/demo/module.py` & `stmaterial-0.0.6/src/stmaterial/demo/module.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/demo/sphinxext.py` & `stmaterial-0.0.6/src/stmaterial/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/directives.py` & `stmaterial-0.0.6/src/stmaterial/directives.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/base.html` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/base.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 <!doctype html>
 <html class="no-js" {% if language is not none %} lang="{{ language }}" {% endif %}>
 {%- import "static/webpack-macros.html" as _webpack with context %}
+{%- import "partials/_icon_links_declaration.html" as _icon_declare with context %}
 
 <head>
     {%- block site_meta -%}
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width,initial-scale=1" />
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="msapplication-tap-highlight" content="no">
@@ -105,8 +106,8 @@
     {%- block theme_scripts -%}
     {{ _webpack.body_post() }}
     {%- endblock -%}
 
     {%- endblock scripts -%}
 </body>
 
-</html>
+</html>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 
 % if language is not none %} lang="{{ language }}" {% endif %}> {%- import
-"static/webpack-macros.html" as _webpack with context %}
+"static/webpack-macros.html" as _webpack with context %} {%- import "partials/
+_icon_links_declaration.html" as _icon_declare with context %}
 {%- block site_meta -%}
 
 
 
 
  {%- if metatags %}{{ metatags }}{% endif -%} {%- block linktags %} {%- if
 hasdoc('about') %}
```

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/breadcrumbs.html` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/edit-this-page.html` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/edit-this-page.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% extends "basic-ng/components/edit-this-page.html" %}
 {% from "basic-ng/components/edit-this-page.html" import determine_page_edit_link with context %}
 
 {%- macro page_edit_button(url) -%}
 <a class="edit-this-page" href="{{ url }}" title="{{ translate('Edit this page') }}">
-    <i class="material-icons">mode_edit</i> {{ translate('Edit this page') }}
+    <i class="material-icons">mode_edit</i> {% if not show_source %} {{ translate('Edit this page') }} {% endif %}
 </a>
 {%- endmacro -%}
 
 {% block link_available -%}
 {{ page_edit_button(determine_page_edit_link()) }}
 {%- endblock %}
 
@@ -15,8 +15,8 @@
 {# Make nice things happen, on Read the Docs #}
 {%- if READTHEDOCS and conf_py_path and page_source_suffix and github_user != "None" and github_repo != "None" and
 github_version and pagename and page_source_suffix %}
 {% set url = "https://github.com/" + github_user + "/" + github_repo + "/edit/" + github_version + conf_py_path +
 pagename + page_source_suffix %}
 {{ page_edit_button(url) }}
 {%- endif -%}
-{% endblock %}
+{% endblock %}
```

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/postnav.html` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/postnav.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/prev-next.html` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/components/search-field.html` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/components/search-field.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/domainindex.html` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/domainindex.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/genindex.html` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/genindex.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/layout.html` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/layout.html`

 * *Files 5% similar despite different names*

```diff
@@ -109,208 +109,190 @@
 000006c0: 2020 7b25 2062 6c6f 636b 2062 6f64 7920    {% block body 
 000006d0: 257d 7b7b 2062 6f64 7920 7d7d 7b25 2065  %}{{ body }}{% e
 000006e0: 6e64 626c 6f63 6b20 257d 0a20 2020 2020  ndblock %}.     
 000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000700: 2020 203c 2f61 7274 6963 6c65 3e0a 0a20     </article>.. 
 00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000720: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00000730: 733d 2273 746d 2d65 6469 742d 7570 6461  s="stm-edit-upda
-00000740: 7465 2d6d 6574 6122 3e0a 2020 2020 2020  te-meta">.      
+00000730: 733d 2273 746d 2d61 7274 6963 6c65 2d6d  s="stm-article-m
+00000740: 6574 6164 6174 612d 696e 666f 223e 0a20  etadata-info">. 
 00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000760: 2020 2020 2020 7b25 2069 6e63 6c75 6465        {% include
-00000770: 2022 636f 6d70 6f6e 656e 7473 2f6c 6173   "components/las
-00000780: 742d 7570 6461 7465 642e 6874 6d6c 2220  t-updated.html" 
-00000790: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-000007a0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000007b0: 2520 6966 2074 6865 6d65 5f75 7365 5f65  % if theme_use_e
-000007c0: 6469 745f 7061 6765 5f62 7574 746f 6e20  dit_page_button 
-000007d0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-000007e0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000007f0: 2520 696e 636c 7564 6520 2263 6f6d 706f  % include "compo
-00000800: 6e65 6e74 732f 6564 6974 2d74 6869 732d  nents/edit-this-
-00000810: 7061 6765 2e68 746d 6c22 2025 7d0a 2020  page.html" %}.  
+00000760: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00000770: 636c 6173 733d 226d 6574 6164 6174 612d  class="metadata-
+00000780: 696e 666f 2d61 7265 6122 3e0a 2020 2020  info-area">.    
+00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007a0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000007b0: 2063 6c61 7373 3d22 6d65 7461 6461 7461   class="metadata
+000007c0: 2d6c 6566 7422 3e0a 2020 2020 2020 2020  -left">.        
+000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007e0: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
+000007f0: 6e63 6c75 6465 2022 636f 6d70 6f6e 656e  nclude "componen
+00000800: 7473 2f6c 6173 742d 7570 6461 7465 642e  ts/last-updated.
+00000810: 6874 6d6c 2220 257d 0a20 2020 2020 2020  html" %}.       
 00000820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000830: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-00000840: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-00000850: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00000860: 6469 763e 0a0a 2020 2020 2020 2020 2020  div>..          
-00000870: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00000880: 6976 2063 6c61 7373 3d22 7374 6d2d 6172  iv class="stm-ar
-00000890: 7469 636c 652d 666f 6f74 6572 223e 0a20  ticle-footer">. 
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008b0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-000008c0: 636c 6173 733d 2270 7265 762d 6e65 7874  class="prev-next
-000008d0: 2d61 7265 6122 3e0a 2020 2020 2020 2020  -area">.        
+00000830: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000860: 3c64 6976 2063 6c61 7373 3d22 6d65 7461  <div class="meta
+00000870: 6461 7461 2d72 6967 6874 223e 0a20 2020  data-right">.   
+00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008a0: 207b 2520 696e 636c 7564 6520 2263 6f6d   {% include "com
+000008b0: 706f 6e65 6e74 732f 736f 7572 6365 6c69  ponents/sourceli
+000008c0: 6e6b 2e68 746d 6c22 2025 7d0a 2020 2020  nk.html" %}.    
+000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008f0: 2020 2020 2020 2020 7b25 2069 6620 7468          {% if th
-00000900: 656d 655f 7368 6f77 5f70 7265 765f 6e65  eme_show_prev_ne
-00000910: 7874 2025 7d0a 2020 2020 2020 2020 2020  xt %}.          
+000008f0: 7b25 2069 6620 7468 656d 655f 7573 655f  {% if theme_use_
+00000900: 6564 6974 5f70 6167 655f 6275 7474 6f6e  edit_page_button
+00000910: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
 00000920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000930: 2020 2020 2020 7b25 2069 6e63 6c75 6465        {% include
-00000940: 2022 636f 6d70 6f6e 656e 7473 2f70 7265   "components/pre
-00000950: 762d 6e65 7874 2e68 746d 6c22 2025 7d0a  v-next.html" %}.
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000930: 2020 2020 2020 2020 7b25 2069 6e63 6c75          {% inclu
+00000940: 6465 2022 636f 6d70 6f6e 656e 7473 2f65  de "components/e
+00000950: 6469 742d 7468 6973 2d70 6167 652e 6874  dit-this-page.ht
+00000960: 6d6c 2220 257d 0a20 2020 2020 2020 2020  ml" %}.         
 00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000980: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-00000990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009a0: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-000009b0: 6e63 6c75 6465 2022 636f 6d70 6f6e 656e  nclude "componen
-000009c0: 7473 2f70 6f73 746e 6176 2e68 746d 6c22  ts/postnav.html"
-000009d0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009f0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00000a00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000a10: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00000a20: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00000a30: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000a40: 2020 2020 2020 7b25 2069 6620 6e6f 7420        {% if not 
-00000a50: 6869 6465 5f74 6f63 6e61 7620 257d 0a20  hide_tocnav %}. 
-00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a70: 2020 207b 2520 7365 7420 7061 6765 5f74     {% set page_t
-00000a80: 6f63 203d 2067 656e 6572 6174 655f 746f  oc = generate_to
-00000a90: 635f 6874 6d6c 2829 2025 7d0a 2020 2020  c_html() %}.    
-00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ab0: 7b25 2d20 6966 2070 6167 655f 746f 6320  {%- if page_toc 
-00000ac0: 7c20 6c65 6e67 7468 203e 3d20 3120 257d  | length >= 1 %}
-00000ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ae0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00000af0: 2273 746d 2d74 6f63 2063 6f6c 206d 3220  "stm-toc col m2 
-00000b00: 786c 3320 7b25 2069 6620 6869 6465 5f74  xl3 {% if hide_t
-00000b10: 6f63 2025 7d20 6869 6465 207b 2520 656c  oc %} hide {% el
-00000b20: 7365 2025 7d20 6869 6465 2d6f 6e2d 736d  se %} hide-on-sm
-00000b30: 616c 6c2d 6f6e 6c79 207b 2520 656e 6469  all-only {% endi
-00000b40: 6620 257d 223e 0a20 2020 2020 2020 2020  f %}">.         
-00000b50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000b60: 6469 7620 636c 6173 733d 2274 6f63 2d77  div class="toc-w
-00000b70: 7261 7070 6572 2074 6f63 2d73 6372 6f6c  rapper toc-scrol
-00000b80: 6c22 3e0a 2020 2020 2020 2020 2020 2020  l">.            
-00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ba0: 7b25 2069 6620 7468 656d 655f 746f 635f  {% if theme_toc_
-00000bb0: 7469 746c 6520 257d 0a20 2020 2020 2020  title %}.       
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00000be0: 2274 6f63 2d74 6974 6c65 223e 0a20 2020  "toc-title">.   
-00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c00: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
-00000c10: 616e 2063 6c61 7373 3d22 6d61 7465 7269  an class="materi
-00000c20: 616c 2d69 636f 6e73 223e 6c69 7374 3c2f  al-icons">list</
-00000c30: 7370 616e 3e20 7b7b 2074 6865 6d65 5f74  span> {{ theme_t
-00000c40: 6f63 5f74 6974 6c65 207d 7d0a 2020 2020  oc_title }}.    
-00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c60: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000980: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+00000990: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
+000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009b0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009d0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+000009e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000009f0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00000a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a10: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00000a20: 6173 733d 2273 746d 2d61 7274 6963 6c65  ass="stm-article
+00000a30: 2d66 6f6f 7465 7222 3e0a 2020 2020 2020  -footer">.      
+00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a50: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000a60: 3d22 7072 6576 2d6e 6578 742d 6172 6561  ="prev-next-area
+00000a70: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a90: 2020 207b 2520 6966 2074 6865 6d65 5f73     {% if theme_s
+00000aa0: 686f 775f 7072 6576 5f6e 6578 7420 257d  how_prev_next %}
+00000ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ad0: 207b 2520 696e 636c 7564 6520 2263 6f6d   {% include "com
+00000ae0: 706f 6e65 6e74 732f 7072 6576 2d6e 6578  ponents/prev-nex
+00000af0: 742e 6874 6d6c 2220 257d 0a20 2020 2020  t.html" %}.     
+00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b10: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+00000b20: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
+00000b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b40: 2020 2020 2020 207b 2520 696e 636c 7564         {% includ
+00000b50: 6520 2263 6f6d 706f 6e65 6e74 732f 706f  e "components/po
+00000b60: 7374 6e61 762e 6874 6d6c 2220 257d 0a20  stnav.html" %}. 
+00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b80: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00000b90: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000ba0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00000bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000bc0: 2020 2020 203c 2f64 6976 3e0a 0a20 2020       </div>..   
+00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000be0: 207b 2520 6966 206e 6f74 2068 6964 655f   {% if not hide_
+00000bf0: 746f 636e 6176 2025 7d0a 2020 2020 2020  tocnav %}.      
+00000c00: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00000c10: 2073 6574 2070 6167 655f 746f 6320 3d20   set page_toc = 
+00000c20: 6765 6e65 7261 7465 5f74 6f63 5f68 746d  generate_toc_htm
+00000c30: 6c28 2920 257d 0a20 2020 2020 2020 2020  l() %}.         
+00000c40: 2020 2020 2020 2020 2020 207b 252d 2069             {%- i
+00000c50: 6620 7061 6765 5f74 6f63 207c 206c 656e  f page_toc | len
+00000c60: 6774 6820 3e3d 2031 2025 7d0a 2020 2020  gth >= 1 %}.    
 00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00000c90: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
-00000ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cb0: 2020 207b 7b20 7061 6765 5f74 6f63 207d     {{ page_toc }
-00000cc0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000cd0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00000ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000cf0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d10: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00000c80: 3c64 6976 2063 6c61 7373 3d22 7374 6d2d  <div class="stm-
+00000c90: 746f 6320 636f 6c20 6d32 2078 6c33 207b  toc col m2 xl3 {
+00000ca0: 2520 6966 2068 6964 655f 746f 6320 257d  % if hide_toc %}
+00000cb0: 2068 6964 6520 7b25 2065 6c73 6520 257d   hide {% else %}
+00000cc0: 2068 6964 652d 6f6e 2d73 6d61 6c6c 2d6f   hide-on-small-o
+00000cd0: 6e6c 7920 7b25 2065 6e64 6966 2025 7d22  nly {% endif %}"
+00000ce0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000cf0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00000d00: 6c61 7373 3d22 746f 632d 7772 6170 7065  lass="toc-wrappe
+00000d10: 7220 746f 632d 7363 726f 6c6c 223e 0a20  r toc-scroll">. 
 00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d30: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-00000d40: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00000d50: 763e 0a20 2020 2020 2020 2020 2020 203c  v>.            <
-00000d60: 2f64 6976 3e0a 0a20 2020 2020 2020 2020  /div>..         
-00000d70: 2020 207b 2520 6966 2074 6865 6d65 5f66     {% if theme_f
-00000d80: 6f6f 7465 725f 636f 6e74 656e 7420 257d  ooter_content %}
-00000d90: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
-00000da0: 7620 636c 6173 733d 2273 746d 2d63 6f6e  v class="stm-con
-00000db0: 7465 6e74 2d66 6f6f 7465 7222 3e0a 2020  tent-footer">.  
-00000dc0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00000dd0: 6976 2063 6c61 7373 3d22 7374 6d2d 626f  iv class="stm-bo
-00000de0: 7474 6f6d 2d66 6f6f 7465 7222 3e0a 2020  ttom-footer">.  
+00000d30: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+00000d40: 2074 6865 6d65 5f74 6f63 5f74 6974 6c65   theme_toc_title
+00000d50: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d70: 3c64 6976 2063 6c61 7373 3d22 746f 632d  <div class="toc-
+00000d80: 7469 746c 6522 3e0a 2020 2020 2020 2020  title">.        
+00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000da0: 2020 2020 2020 2020 3c73 7061 6e20 636c          <span cl
+00000db0: 6173 733d 226d 6174 6572 6961 6c2d 6963  ass="material-ic
+00000dc0: 6f6e 7322 3e6c 6973 743c 2f73 7061 6e3e  ons">list</span>
+00000dd0: 207b 7b20 7468 656d 655f 746f 635f 7469   {{ theme_toc_ti
+00000de0: 746c 6520 7d7d 0a20 2020 2020 2020 2020  tle }}.         
 00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e00: 2020 3c64 6976 2063 6c61 7373 3d22 7374    <div class="st
-00000e10: 6d2d 6c65 6674 2d66 6f6f 7465 7222 3e0a  m-left-footer">.
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 2020 2020 2020 2020 7b25 2d20 666f 7220          {%- for 
-00000e40: 666f 6f74 6572 5f69 7465 6d20 696e 2074  footer_item in t
-00000e50: 6865 6d65 5f66 6f6f 7465 725f 636f 6e74  heme_footer_cont
-00000e60: 656e 7420 257d 0a20 2020 2020 2020 2020  ent %}.         
-00000e70: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00000e80: 252d 2069 6e63 6c75 6465 2066 6f6f 7465  %- include foote
-00000e90: 725f 6974 656d 2025 7d0a 2020 2020 2020  r_item %}.      
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000eb0: 2020 7b25 2d20 656e 6466 6f72 2025 7d0a    {%- endfor %}.
-00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ed0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00000ee0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000ef0: 6469 7620 636c 6173 733d 2273 746d 2d72  div class="stm-r
-00000f00: 6967 6874 2d66 6f6f 7465 7222 3e0a 2020  ight-footer">.  
-00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f20: 2020 2020 2020 7b25 2069 6620 7468 656d        {% if them
-00000f30: 655f 666f 6f74 6572 5f69 636f 6e73 202d  e_footer_icons -
-00000f40: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00000f50: 2020 2020 2020 2020 2020 207b 2520 666f             {% fo
-00000f60: 7220 6963 6f6e 5f64 6963 7420 696e 2074  r icon_dict in t
-00000f70: 6865 6d65 5f66 6f6f 7465 725f 6963 6f6e  heme_footer_icon
-00000f80: 7320 2d25 7d0a 2020 2020 2020 2020 2020  s -%}.          
-00000f90: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
-00000fa0: 2068 7265 663d 227b 7b20 6963 6f6e 5f64   href="{{ icon_d
-00000fb0: 6963 742e 7572 6c20 7d7d 2220 7461 7267  ict.url }}" targ
-00000fc0: 6574 3d22 5f62 6c61 6e6b 2220 7469 746c  et="_blank" titl
-00000fd0: 653d 227b 7b20 6963 6f6e 5f64 6963 742e  e="{{ icon_dict.
-00000fe0: 6e61 6d65 207d 7d22 2063 6c61 7373 3d22  name }}" class="
-00000ff0: 6578 742d 6c69 6e6b 223e 0a20 2020 2020  ext-link">.     
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 2020 2020 2020 207b 2520 6966 2069 636f         {% if ico
-00001020: 6e5f 6469 6374 2e63 6c61 7373 2025 7d0a  n_dict.class %}.
-00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001040: 2020 2020 2020 2020 2020 2020 3c69 2063              <i c
-00001050: 6c61 7373 3d22 7b7b 2069 636f 6e5f 6469  lass="{{ icon_di
-00001060: 6374 2e63 6c61 7373 207d 7d22 3e3c 2f69  ct.class }}"></i
-00001070: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001080: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00001090: 2065 6c69 6620 6963 6f6e 5f64 6963 742e   elif icon_dict.
-000010a0: 6d61 7465 7269 616c 5f69 636f 6e73 2025  material_icons %
-000010b0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-000010c0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-000010d0: 2063 6c61 7373 3d22 6d61 7465 7269 616c   class="material
-000010e0: 2d69 636f 6e73 223e 7b7b 2069 636f 6e5f  -icons">{{ icon_
-000010f0: 6469 6374 2e6d 6174 6572 6961 6c5f 6963  dict.material_ic
-00001100: 6f6e 7320 7d7d 3c2f 693e 0a20 2020 2020  ons }}</i>.     
-00001110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001120: 2020 2020 2020 207b 2520 656c 6966 2069         {% elif i
-00001130: 636f 6e5f 6469 6374 2e66 6f6e 7461 7765  con_dict.fontawe
-00001140: 736f 6d65 2025 7d0a 2020 2020 2020 2020  some %}.        
-00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001160: 2020 2020 3c69 2063 6c61 7373 3d22 7b7b      <i class="{{
-00001170: 2069 636f 6e5f 6469 6374 2e66 6f6e 7461   icon_dict.fonta
-00001180: 7765 736f 6d65 207d 7d22 3e3c 2f69 3e0a  wesome }}"></i>.
-00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011a0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-000011b0: 6c69 6620 6963 6f6e 5f64 6963 742e 696d  lif icon_dict.im
-000011c0: 6167 6520 257d 0a20 2020 2020 2020 2020  age %}.         
-000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011e0: 2020 203c 696d 6720 7372 633d 227b 7b20     <img src="{{ 
-000011f0: 6963 6f6e 5f64 6963 742e 696d 6167 6520  icon_dict.image 
-00001200: 7d7d 2220 636c 6173 733d 2273 746d 2d69  }}" class="stm-i
-00001210: 636f 6e2d 696d 6167 6522 3e0a 2020 2020  con-image">.    
-00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001230: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00001240: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00001250: 2020 2020 2020 2020 2020 2020 3c2f 613e              </a>
-00001260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001270: 2020 2020 2020 2020 207b 2520 656e 6466           {% endf
-00001280: 6f72 2025 7d0a 2020 2020 2020 2020 2020  or %}.          
-00001290: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-000012a0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-000012b0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000012c0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-000012d0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-000012e0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-000012f0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00001300: 6469 6620 257d 0a0a 2020 2020 2020 2020  dif %}..        
-00001310: 3c2f 6d61 696e 3e0a 2020 2020 3c2f 6469  </main>.    </di
-00001320: 763e 0a3c 2f64 6976 3e0a 0a7b 2520 626c  v>.</div>..{% bl
-00001330: 6f63 6b20 666f 6f74 6572 2025 7d0a 7b25  ock footer %}.{%
-00001340: 2069 6620 7468 656d 655f 666f 6f74 6572   if theme_footer
-00001350: 2025 7d0a 7b25 2069 6e63 6c75 6465 2022   %}.{% include "
-00001360: 7365 6374 696f 6e73 2f66 6f6f 7465 722e  sections/footer.
-00001370: 6874 6d6c 2220 257d 0a7b 2520 656e 6469  html" %}.{% endi
-00001380: 6620 257d 0a7b 2520 656e 6462 6c6f 636b  f %}.{% endblock
-00001390: 2025 7d0a 0a7b 252d 2065 6e64 626c 6f63   %}..{%- endbloc
-000013a0: 6b20 257d 0a7b 252d 2065 6e64 626c 6f63  k %}.{%- endbloc
-000013b0: 6b20 257d 0a                             k %}.
+00000e00: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e20: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00000e30: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00000e40: 2020 2020 2020 2020 2020 2020 2020 7b7b                {{
+00000e50: 2070 6167 655f 746f 6320 7d7d 0a20 2020   page_toc }}.   
+00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e70: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e90: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00000ea0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+00000eb0: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
+00000ec0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+00000ed0: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
+00000ee0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00000ef0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00000f00: 0a0a 2020 2020 2020 2020 2020 2020 7b25  ..            {%
+00000f10: 2069 6620 7468 656d 655f 666f 6f74 6572   if theme_footer
+00000f20: 5f63 6f6e 7465 6e74 2025 7d0a 2020 2020  _content %}.    
+00000f30: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00000f40: 7373 3d22 7374 6d2d 636f 6e74 656e 742d  ss="stm-content-
+00000f50: 666f 6f74 6572 223e 0a20 2020 2020 2020  footer">.       
+00000f60: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00000f70: 6173 733d 2273 746d 2d62 6f74 746f 6d2d  ass="stm-bottom-
+00000f80: 666f 6f74 6572 223e 0a20 2020 2020 2020  footer">.       
+00000f90: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00000fa0: 7620 636c 6173 733d 2273 746d 2d6c 6566  v class="stm-lef
+00000fb0: 742d 666f 6f74 6572 223e 0a20 2020 2020  t-footer">.     
+00000fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fd0: 2020 207b 252d 2066 6f72 2066 6f6f 7465     {%- for foote
+00000fe0: 725f 6974 656d 2069 6e20 7468 656d 655f  r_item in theme_
+00000ff0: 666f 6f74 6572 5f63 6f6e 7465 6e74 2025  footer_content %
+00001000: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00001010: 2020 2020 2020 2020 2020 7b25 2d20 696e            {%- in
+00001020: 636c 7564 6520 666f 6f74 6572 5f69 7465  clude footer_ite
+00001030: 6d20 257d 0a20 2020 2020 2020 2020 2020  m %}.           
+00001040: 2020 2020 2020 2020 2020 2020 207b 252d               {%-
+00001050: 2065 6e64 666f 7220 257d 0a20 2020 2020   endfor %}.     
+00001060: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001070: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00001080: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00001090: 6c61 7373 3d22 7374 6d2d 7269 6768 742d  lass="stm-right-
+000010a0: 666f 6f74 6572 223e 0a20 2020 2020 2020  footer">.       
+000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010c0: 207b 2520 6966 2074 6865 6d65 5f66 6f6f   {% if theme_foo
+000010d0: 7465 725f 6963 6f6e 7320 257d 0a20 2020  ter_icons %}.   
+000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010f0: 2020 2020 203c 756c 3e0a 2020 2020 2020       <ul>.      
+00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001110: 2020 2020 2020 7b7b 205f 6963 6f6e 5f64        {{ _icon_d
+00001120: 6563 6c61 7265 2e64 6563 6c61 7265 5f69  eclare.declare_i
+00001130: 636f 6e5f 6c69 6e6b 7328 7468 656d 655f  con_links(theme_
+00001140: 666f 6f74 6572 5f69 636f 6e73 2920 7d7d  footer_icons) }}
+00001150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001160: 2020 2020 2020 2020 203c 2f75 6c3e 0a20           </ul>. 
+00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001180: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+00001190: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+000011a0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+000011b0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000011c0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+000011d0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+000011e0: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
+000011f0: 0a20 2020 2020 2020 203c 2f6d 6169 6e3e  .        </main>
+00001200: 0a20 2020 203c 2f64 6976 3e0a 3c2f 6469  .    </div>.</di
+00001210: 763e 0a0a 7b25 2062 6c6f 636b 2066 6f6f  v>..{% block foo
+00001220: 7465 7220 257d 0a7b 2520 6966 2074 6865  ter %}.{% if the
+00001230: 6d65 5f66 6f6f 7465 7220 257d 0a7b 2520  me_footer %}.{% 
+00001240: 696e 636c 7564 6520 2273 6563 7469 6f6e  include "section
+00001250: 732f 666f 6f74 6572 2e68 746d 6c22 2025  s/footer.html" %
+00001260: 7d0a 7b25 2065 6e64 6966 2025 7d0a 7b25  }.{% endif %}.{%
+00001270: 2065 6e64 626c 6f63 6b20 257d 0a0a 7b25   endblock %}..{%
+00001280: 2d20 656e 6462 6c6f 636b 2025 7d0a 7b25  - endblock %}.{%
+00001290: 2d20 656e 6462 6c6f 636b 2025 7d0a       - endblock %}.
```

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/search.html` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/search.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/static/images/github.svg` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/static/images/github.svg`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/src/stmaterial/theme/stmaterial/theme.conf` & `stmaterial-0.0.6/src/stmaterial/theme/stmaterial/theme.conf`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 show_nav_level = 1
 show_toc_level = 1
 logo = 
 header_links_before_dropdown = 4
 external_links = 
 header_icons =
 footer_icons = 
+sidenav_icons =
 use_edit_page_button=
 source_repository=
 source_branch =
 source_directory =
 source_edit_link =
 custom_fonts =
 show_prev_next = True
```

### Comparing `stmaterial-0.0.5/src/stmaterial/utils.py` & `stmaterial-0.0.6/src/stmaterial/utils.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/webpack.config.js` & `stmaterial-0.0.6/webpack.config.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.5/PKG-INFO` & `stmaterial-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7374 6d61  : 2.1.Name: stma
 00000020: 7465 7269 616c 0a56 6572 7369 6f6e 3a20  terial.Version: 
-00000030: 302e 302e 350a 5375 6d6d 6172 793a 2041  0.0.5.Summary: A
+00000030: 302e 302e 360a 5375 6d6d 6172 793a 2041  0.0.6.Summary: A
 00000040: 2073 7068 696e 7820 7468 656d 6520 6f66   sphinx theme of
 00000050: 206d 6174 6572 6961 6c69 7a65 6373 732e   materializecss.
 00000060: 0a41 7574 686f 722d 456d 6169 6c3a 207a  .Author-Email: z
 00000070: 636c 6162 203c 7379 6668 7562 4068 6f74  clab <syfhub@hot
 00000080: 6d61 696c 2e63 6f6d 3e0a 4c69 6365 6e73  mail.com>.Licens
 00000090: 653a 204d 4954 204c 6963 656e 7365 0a20  e: MIT License. 
 000000a0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
@@ -101,113 +101,161 @@
 00000640: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
 00000650: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
 00000660: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
 00000670: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
 00000680: 686f 6e20 3a3a 2033 0a43 6c61 7373 6966  hon :: 3.Classif
 00000690: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
 000006a0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000006b0: 686f 6e20 3a3a 2033 2e37 0a43 6c61 7373  hon :: 3.7.Class
+000006b0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
 000006c0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
 000006d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000006e0: 7974 686f 6e20 3a3a 2033 2e38 0a43 6c61  ython :: 3.8.Cla
+000006e0: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
 000006f0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
 00000700: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000710: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
-00000720: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000730: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000740: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000750: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
-00000760: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000770: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000780: 332e 3131 0a43 6c61 7373 6966 6965 723a  3.11.Classifier:
-00000790: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-000007a0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-000007b0: 656e 740a 436c 6173 7369 6669 6572 3a20  ent.Classifier: 
-000007c0: 546f 7069 6320 3a3a 2044 6f63 756d 656e  Topic :: Documen
-000007d0: 7461 7469 6f6e 0a43 6c61 7373 6966 6965  tation.Classifie
-000007e0: 723a 2054 6f70 6963 203a 3a20 536f 6674  r: Topic :: Soft
-000007f0: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
-00000800: 203a 3a20 446f 6375 6d65 6e74 6174 696f   :: Documentatio
-00000810: 6e0a 5072 6f6a 6563 742d 5552 4c3a 2052  n.Project-URL: R
-00000820: 6570 6f73 6974 6f72 792c 2068 7474 7073  epository, https
-00000830: 3a2f 2f67 6974 6875 622e 636f 6d2f 7a63  ://github.com/zc
-00000840: 6c61 622f 7374 6d61 7465 7269 616c 0a50  lab/stmaterial.P
-00000850: 726f 6a65 6374 2d55 524c 3a20 446f 6375  roject-URL: Docu
-00000860: 6d65 6e74 6174 696f 6e2c 2068 7474 7073  mentation, https
-00000870: 3a2f 2f7a 636c 6162 2e67 6974 6875 622e  ://zclab.github.
-00000880: 696f 2f73 746d 6174 6572 6961 6c2f 0a52  io/stmaterial/.R
-00000890: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-000008a0: 3e3d 332e 380a 5265 7175 6972 6573 2d44  >=3.8.Requires-D
-000008b0: 6973 743a 2062 6561 7574 6966 756c 736f  ist: beautifulso
-000008c0: 7570 340a 5265 7175 6972 6573 2d44 6973  up4.Requires-Dis
-000008d0: 743a 2073 7068 696e 783c 372e 302c 3e3d  t: sphinx<7.0,>=
-000008e0: 352e 300a 5265 7175 6972 6573 2d44 6973  5.0.Requires-Dis
-000008f0: 743a 2073 7068 696e 782d 6261 7369 632d  t: sphinx-basic-
-00000900: 6e67 0a52 6571 7569 7265 732d 4469 7374  ng.Requires-Dist
-00000910: 3a20 7079 676d 656e 7473 3e3d 322e 370a  : pygments>=2.7.
-00000920: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
-00000930: 7068 696e 782d 7468 656d 652d 6275 696c  phinx-theme-buil
-00000940: 6465 725b 636c 695d 3e3d 302e 322e 3062  der[cli]>=0.2.0b
-00000950: 323b 2065 7874 7261 203d 3d20 2264 6576  2; extra == "dev
-00000960: 220a 5072 6f76 6964 6573 2d45 7874 7261  ".Provides-Extra
-00000970: 3a20 6465 760a 4465 7363 7269 7074 696f  : dev.Descriptio
-00000980: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-00000990: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a3c  text/markdown..<
-000009a0: 6831 2061 6c69 676e 3d22 6365 6e74 6572  h1 align="center
-000009b0: 223e 0a20 203c 696d 6720 7372 633d 2264  ">.  <img src="d
-000009c0: 6f63 732f 5f73 7461 7469 632f 6c6f 676f  ocs/_static/logo
-000009d0: 2e70 6e67 2220 7769 6474 683d 2234 3030  .png" width="400
-000009e0: 223e 0a3c 2f68 313e 0a0a 5b21 5b50 7950  ">.</h1>..[![PyP
-000009f0: 495d 2868 7474 7073 3a2f 2f69 6d67 2e73  I](https://img.s
-00000a00: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-00000a10: 2f73 746d 6174 6572 6961 6c3f 6c6f 676f  /stmaterial?logo
-00000a20: 3d70 7974 686f 6e26 6c6f 676f 436f 6c6f  =python&logoColo
-00000a30: 723d 7768 6974 6526 636f 6c6f 723d 6f72  r=white&color=or
-00000a40: 616e 6765 295d 2868 7474 7073 3a2f 2f70  ange)](https://p
-00000a50: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000a60: 7374 6d61 7465 7269 616c 2f29 0a5b 215b  stmaterial/).[![
-00000a70: 6465 706c 6f79 5d28 6874 7470 733a 2f2f  deploy](https://
-00000a80: 6769 7468 7562 2e63 6f6d 2f7a 636c 6162  github.com/zclab
-00000a90: 2f73 746d 6174 6572 6961 6c2f 6163 7469  /stmaterial/acti
-00000aa0: 6f6e 732f 776f 726b 666c 6f77 732f 6465  ons/workflows/de
-00000ab0: 706c 6f79 2d64 6f63 732e 796d 6c2f 6261  ploy-docs.yml/ba
-00000ac0: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
-00000ad0: 2f2f 7a63 6c61 622e 6769 7468 7562 2e69  //zclab.github.i
-00000ae0: 6f2f 7374 6d61 7465 7269 616c 2f29 0a5b  o/stmaterial/).[
-00000af0: 215b 7265 6c65 6173 655d 2868 7474 7073  ![release](https
-00000b00: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000b10: 6f2f 6769 7468 7562 2f72 656c 6561 7365  o/github/release
-00000b20: 2f7a 636c 6162 2f73 746d 6174 6572 6961  /zclab/stmateria
-00000b30: 6c2e 7376 6729 5d28 6874 7470 733a 2f2f  l.svg)](https://
-00000b40: 6769 7468 7562 2e63 6f6d 2f7a 636c 6162  github.com/zclab
-00000b50: 2f73 746d 6174 6572 6961 6c2f 7265 6c65  /stmaterial/rele
-00000b60: 6173 6573 290a 0a0a 4120 4d61 7465 7269  ases)...A Materi
-00000b70: 616c 697a 6520 6261 7365 6420 7370 6869  alize based sphi
-00000b80: 6e78 2074 6865 6d65 0a0a 0a23 2320 496e  nx theme...## In
-00000b90: 7374 616c 6c61 7469 6f6e 2061 6e64 2075  stallation and u
-00000ba0: 7361 6765 0a0a 3c21 2d2d 2073 7461 7274  sage..<!-- start
-00000bb0: 2071 7569 636b 7374 6172 7420 2d2d 3e0a   quickstart -->.
-00000bc0: 0a54 6f20 7573 6520 7468 6973 2074 6865  .To use this the
-00000bd0: 6d65 2069 6e20 7468 6520 7265 706f 7369  me in the reposi
-00000be0: 746f 7279 2c20 666f 6c6c 6f77 2074 6865  tory, follow the
-00000bf0: 7365 2073 7465 7073 3a0a 0a31 2e20 496e  se steps:..1. In
-00000c00: 7374 616c 6c20 7468 6520 6073 746d 6174  stall the `stmat
-00000c10: 6572 6961 6c60 2069 6e20 796f 7572 2064  erial` in your d
-00000c20: 6f63 2062 7569 6c64 2065 6e76 6972 6f6e  oc build environ
-00000c30: 6d65 6e74 3a0a 2020 200a 2020 2020 6060  ment:.   .    ``
-00000c40: 600a 2020 2020 7069 7020 696e 7374 616c  `.    pip instal
-00000c50: 6c20 7374 6d61 7465 7269 616c 0a20 2020  l stmaterial.   
-00000c60: 2060 6060 0a0a 322e 2043 6f6e 6669 6775   ```..2. Configu
-00000c70: 7265 2074 6865 2053 7068 696e 7820 646f  re the Sphinx do
-00000c80: 6373 2074 6f20 7573 6520 7468 6520 7468  cs to use the th
-00000c90: 656d 6520 6279 2065 6469 7469 6e67 2060  eme by editing `
-00000ca0: 636f 6e66 2e70 7960 0a0a 2020 2020 6060  conf.py`..    ``
-00000cb0: 6070 7974 686f 6e0a 2020 2020 6874 6d6c  `python.    html
-00000cc0: 5f74 6865 6d65 203d 2022 7374 6d61 7465  _theme = "stmate
-00000cd0: 7269 616c 220a 2020 2020 6060 600a 0a33  rial".    ```..3
-00000ce0: 2e20 596f 7572 2053 7068 696e 7820 646f  . Your Sphinx do
-00000cf0: 6375 6d65 6e74 6174 696f 6e27 7320 4854  cumentation's HT
-00000d00: 4d4c 2070 6167 6573 2077 696c 6c20 6e6f  ML pages will no
-00000d10: 7720 6265 2067 656e 6572 6174 6564 2077  w be generated w
-00000d20: 6974 6820 7468 6973 2074 6865 6d65 2120  ith this theme! 
-00000d30: f09f 8e89 0a0a 3c21 2d2d 2065 6e64 2071  ......<!-- end q
-00000d40: 7569 636b 7374 6172 7420 2d2d 3e0a       uickstart -->.
+00000710: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+00000720: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000730: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000740: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000750: 3131 0a43 6c61 7373 6966 6965 723a 204f  11.Classifier: O
+00000760: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000770: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+00000780: 740a 436c 6173 7369 6669 6572 3a20 546f  t.Classifier: To
+00000790: 7069 6320 3a3a 2044 6f63 756d 656e 7461  pic :: Documenta
+000007a0: 7469 6f6e 0a43 6c61 7373 6966 6965 723a  tion.Classifier:
+000007b0: 2054 6f70 6963 203a 3a20 536f 6674 7761   Topic :: Softwa
+000007c0: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
+000007d0: 3a20 446f 6375 6d65 6e74 6174 696f 6e0a  : Documentation.
+000007e0: 5072 6f6a 6563 742d 5552 4c3a 2052 6570  Project-URL: Rep
+000007f0: 6f73 6974 6f72 792c 2068 7474 7073 3a2f  ository, https:/
+00000800: 2f67 6974 6875 622e 636f 6d2f 7a63 6c61  /github.com/zcla
+00000810: 622f 7374 6d61 7465 7269 616c 0a50 726f  b/stmaterial.Pro
+00000820: 6a65 6374 2d55 524c 3a20 446f 6375 6d65  ject-URL: Docume
+00000830: 6e74 6174 696f 6e2c 2068 7474 7073 3a2f  ntation, https:/
+00000840: 2f73 746d 6174 6572 6961 6c2e 7265 6164  /stmaterial.read
+00000850: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00000860: 7465 7374 2f0a 5265 7175 6972 6573 2d50  test/.Requires-P
+00000870: 7974 686f 6e3a 203e 3d33 2e38 0a52 6571  ython: >=3.8.Req
+00000880: 7569 7265 732d 4469 7374 3a20 6265 6175  uires-Dist: beau
+00000890: 7469 6675 6c73 6f75 7034 0a52 6571 7569  tifulsoup4.Requi
+000008a0: 7265 732d 4469 7374 3a20 7370 6869 6e78  res-Dist: sphinx
+000008b0: 3c37 2e30 2c3e 3d35 2e30 0a52 6571 7569  <7.0,>=5.0.Requi
+000008c0: 7265 732d 4469 7374 3a20 7370 6869 6e78  res-Dist: sphinx
+000008d0: 2d62 6173 6963 2d6e 670a 5265 7175 6972  -basic-ng.Requir
+000008e0: 6573 2d44 6973 743a 2070 7967 6d65 6e74  es-Dist: pygment
+000008f0: 733e 3d32 2e37 0a52 6571 7569 7265 732d  s>=2.7.Requires-
+00000900: 4469 7374 3a20 7370 6869 6e78 2d74 6865  Dist: sphinx-the
+00000910: 6d65 2d62 7569 6c64 6572 5b63 6c69 5d3e  me-builder[cli]>
+00000920: 3d30 2e32 2e30 6232 3b20 6578 7472 6120  =0.2.0b2; extra 
+00000930: 3d3d 2022 6465 7622 0a50 726f 7669 6465  == "dev".Provide
+00000940: 732d 4578 7472 613a 2064 6576 0a44 6573  s-Extra: dev.Des
+00000950: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000960: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000970: 646f 776e 0a0a 3c68 3120 616c 6967 6e3d  down..<h1 align=
+00000980: 2263 656e 7465 7222 3e0a 2020 3c69 6d67  "center">.  <img
+00000990: 2073 7263 3d22 6874 7470 733a 2f2f 6364   src="https://cd
+000009a0: 6e2e 6a73 6465 6c69 7672 2e6e 6574 2f67  n.jsdelivr.net/g
+000009b0: 682f 7a63 6c61 622f 7374 6d61 7465 7269  h/zclab/stmateri
+000009c0: 616c 2f64 6f63 732f 5f73 7461 7469 632f  al/docs/_static/
+000009d0: 6c6f 676f 2e70 6e67 2220 7769 6474 683d  logo.png" width=
+000009e0: 2234 3030 223e 0a3c 2f68 313e 0a0a 3c70  "400">.</h1>..<p
+000009f0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000a00: 0a20 203c 7374 726f 6e67 3e0a 2020 2020  .  <strong>.    
+00000a10: 4120 0a20 2020 203c 6120 6872 6566 3d22  A .    <a href="
+00000a20: 6874 7470 733a 2f2f 6d61 7465 7269 616c  https://material
+00000a30: 697a 6577 6562 2e63 6f6d 2f22 3e4d 6174  izeweb.com/">Mat
+00000a40: 6572 6961 6c69 7a65 3c2f 613e 2062 6173  erialize</a> bas
+00000a50: 6564 203c 6120 6872 6566 3d22 6874 7470  ed <a href="http
+00000a60: 733a 2f2f 7777 772e 7370 6869 6e78 2d64  s://www.sphinx-d
+00000a70: 6f63 2e6f 7267 2f65 6e2f 6d61 7374 6572  oc.org/en/master
+00000a80: 2f22 3e73 7068 696e 783c 2f61 3e20 7468  /">sphinx</a> th
+00000a90: 656d 652e 0a20 203c 2f73 7472 6f6e 673e  eme..  </strong>
+00000aa0: 0a3c 2f70 3e0a 0a3c 212d 2d20 5b21 5b64  .</p>..<!-- [![d
+00000ab0: 6570 6c6f 795d 2868 7474 7073 3a2f 2f67  eploy](https://g
+00000ac0: 6974 6875 622e 636f 6d2f 7a63 6c61 622f  ithub.com/zclab/
+00000ad0: 7374 6d61 7465 7269 616c 2f61 6374 696f  stmaterial/actio
+00000ae0: 6e73 2f77 6f72 6b66 6c6f 7773 2f64 6570  ns/workflows/dep
+00000af0: 6c6f 792d 646f 6373 2e79 6d6c 2f62 6164  loy-docs.yml/bad
+00000b00: 6765 2e73 7667 295d 2868 7474 7073 3a2f  ge.svg)](https:/
+00000b10: 2f7a 636c 6162 2e67 6974 6875 622e 696f  /zclab.github.io
+00000b20: 2f73 746d 6174 6572 6961 6c2f 2920 2d2d  /stmaterial/) --
+00000b30: 3e0a 5b21 5b64 6570 6c6f 795d 2868 7474  >.[![deploy](htt
+00000b40: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000b50: 2e69 6f2f 7265 6164 7468 6564 6f63 732f  .io/readthedocs/
+00000b60: 7374 6d61 7465 7269 616c 3f73 7479 6c65  stmaterial?style
+00000b70: 3d66 6c61 742d 7371 7561 7265 266c 6f67  =flat-square&log
+00000b80: 6f3d 7265 6164 7468 6564 6f63 7326 6c6f  o=readthedocs&lo
+00000b90: 676f 436f 6c6f 723d 7768 6974 6529 5d28  goColor=white)](
+00000ba0: 6874 7470 733a 2f2f 7374 6d61 7465 7269  https://stmateri
+00000bb0: 616c 2e72 6561 6474 6865 646f 6373 2e69  al.readthedocs.i
+00000bc0: 6f2f 656e 2f6c 6174 6573 742f 290a 5b21  o/en/latest/).[!
+00000bd0: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
+00000be0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000bf0: 696f 2f70 7970 692f 646d 2f73 746d 6174  io/pypi/dm/stmat
+00000c00: 6572 6961 6c2e 7376 673f 7374 796c 653d  erial.svg?style=
+00000c10: 666c 6174 2d73 7175 6172 6529 5d28 6874  flat-square)](ht
+00000c20: 7470 733a 2f2f 7079 7069 7374 6174 732e  tps://pypistats.
+00000c30: 6f72 672f 7061 636b 6167 6573 2f73 746d  org/packages/stm
+00000c40: 6174 6572 6961 6c29 0a5b 215b 7079 7468  aterial).[![pyth
+00000c50: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
+00000c60: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000c70: 7079 7665 7273 696f 6e73 2f73 746d 6174  pyversions/stmat
+00000c80: 6572 6961 6c2e 7376 673f 7374 796c 653d  erial.svg?style=
+00000c90: 666c 6174 2d73 7175 6172 6529 5d28 6874  flat-square)](ht
+00000ca0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000cb0: 726f 6a65 6374 2f73 746d 6174 6572 6961  roject/stmateria
+00000cc0: 6c2f 290a 5b21 5b50 7950 495d 2868 7474  l/).[![PyPI](htt
+00000cd0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000ce0: 2e69 6f2f 7079 7069 2f76 2f73 746d 6174  .io/pypi/v/stmat
+00000cf0: 6572 6961 6c3f 7374 796c 653d 666c 6174  erial?style=flat
+00000d00: 2d73 7175 6172 6526 6c6f 676f 3d70 7974  -square&logo=pyt
+00000d10: 686f 6e26 6c6f 676f 436f 6c6f 723d 7768  hon&logoColor=wh
+00000d20: 6974 6526 636f 6c6f 723d 6f72 616e 6765  ite&color=orange
+00000d30: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
+00000d40: 6f72 672f 7072 6f6a 6563 742f 7374 6d61  org/project/stma
+00000d50: 7465 7269 616c 2f29 0a5b 215b 7374 6174  terial/).[![stat
+00000d60: 7573 5d28 6874 7470 733a 2f2f 696d 672e  us](https://img.
+00000d70: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000d80: 7374 6174 7573 2f73 746d 6174 6572 6961  status/stmateria
+00000d90: 6c2e 7376 673f 7374 796c 653d 666c 6174  l.svg?style=flat
+00000da0: 2d73 7175 6172 6529 5d28 6874 7470 733a  -square)](https:
+00000db0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000dc0: 6374 2f73 746d 6174 6572 6961 6c2f 290a  ct/stmaterial/).
+00000dd0: 5b21 5b6c 6963 656e 7365 5d28 6874 7470  [![license](http
+00000de0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000df0: 696f 2f70 7970 692f 6c2f 7374 6d61 7465  io/pypi/l/stmate
+00000e00: 7269 616c 2e73 7667 3f73 7479 6c65 3d66  rial.svg?style=f
+00000e10: 6c61 742d 7371 7561 7265 266c 6f67 6f3d  lat-square&logo=
+00000e20: 6f70 656e 736f 7572 6365 696e 6974 6961  opensourceinitia
+00000e30: 7469 7665 266c 6f67 6f43 6f6c 6f72 3d77  tive&logoColor=w
+00000e40: 6869 7465 295d 2868 7474 7073 3a2f 2f67  hite)](https://g
+00000e50: 6974 6875 622e 636f 6d2f 7a63 6c61 622f  ithub.com/zclab/
+00000e60: 7374 6d61 7465 7269 616c 2f62 6c6f 622f  stmaterial/blob/
+00000e70: 6d61 696e 2f4c 4943 454e 5345 290a 0a0a  main/LICENSE)...
+00000e80: 2323 2049 6e73 7461 6c6c 6174 696f 6e20  ## Installation 
+00000e90: 616e 6420 7573 6167 650a 0a3c 212d 2d20  and usage..<!-- 
+00000ea0: 7374 6172 7420 7175 6963 6b73 7461 7274  start quickstart
+00000eb0: 202d 2d3e 0a0a 546f 2075 7365 2074 6869   -->..To use thi
+00000ec0: 7320 7468 656d 6520 696e 2074 6865 2072  s theme in the r
+00000ed0: 6570 6f73 6974 6f72 792c 2066 6f6c 6c6f  epository, follo
+00000ee0: 7720 7468 6573 6520 7374 6570 733a 0a0a  w these steps:..
+00000ef0: 312e 2049 6e73 7461 6c6c 2074 6865 2060  1. Install the `
+00000f00: 7374 6d61 7465 7269 616c 6020 696e 2079  stmaterial` in y
+00000f10: 6f75 7220 646f 6320 6275 696c 6420 656e  our doc build en
+00000f20: 7669 726f 6e6d 656e 743a 0a20 2020 0a20  vironment:.   . 
+00000f30: 2020 2060 6060 0a20 2020 2070 6970 2069     ```.    pip i
+00000f40: 6e73 7461 6c6c 2073 746d 6174 6572 6961  nstall stmateria
+00000f50: 6c0a 2020 2020 6060 600a 0a32 2e20 436f  l.    ```..2. Co
+00000f60: 6e66 6967 7572 6520 7468 6520 5370 6869  nfigure the Sphi
+00000f70: 6e78 2064 6f63 7320 746f 2075 7365 2074  nx docs to use t
+00000f80: 6865 2074 6865 6d65 2062 7920 6564 6974  he theme by edit
+00000f90: 696e 6720 6063 6f6e 662e 7079 600a 0a20  ing `conf.py`.. 
+00000fa0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+00000fb0: 2068 746d 6c5f 7468 656d 6520 3d20 2273   html_theme = "s
+00000fc0: 746d 6174 6572 6961 6c22 0a20 2020 2060  tmaterial".    `
+00000fd0: 6060 0a0a 332e 2059 6f75 7220 5370 6869  ``..3. Your Sphi
+00000fe0: 6e78 2064 6f63 756d 656e 7461 7469 6f6e  nx documentation
+00000ff0: 2773 2048 544d 4c20 7061 6765 7320 7769  's HTML pages wi
+00001000: 6c6c 206e 6f77 2062 6520 6765 6e65 7261  ll now be genera
+00001010: 7465 6420 7769 7468 2074 6869 7320 7468  ted with this th
+00001020: 656d 6521 20f0 9f8e 890a 0a3c 212d 2d20  eme! ......<!-- 
+00001030: 656e 6420 7175 6963 6b73 7461 7274 202d  end quickstart -
+00001040: 2d3e 0a                                  ->.
```

