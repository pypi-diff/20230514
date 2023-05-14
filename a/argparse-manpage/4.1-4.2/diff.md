# Comparing `tmp/argparse-manpage-4.1.tar.gz` & `tmp/argparse-manpage-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse-manpage-4.1.tar", last modified: Sat Apr 15 19:13:25 2023, max compression
+gzip compressed data, was "argparse-manpage-4.2.tar", last modified: Sun May 14 10:58:16 2023, max compression
```

## Comparing `argparse-manpage-4.1.tar` & `argparse-manpage-4.2.tar`

### file list

```diff
@@ -1,106 +1,111 @@
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.044954 argparse-manpage-4.1/
--rw-rw-r--   0 twine    (17125) twine    (17125)      136 2019-09-07 00:39:54.000000 argparse-manpage-4.1/AUTHORS
--rw-rw-r--   0 twine    (17125) twine    (17125)    11357 2019-09-07 00:39:54.000000 argparse-manpage-4.1/LICENSE
--rw-r--r--   0 twine    (17125) twine    (17125)      601 2023-04-15 19:13:21.000000 argparse-manpage-4.1/MANIFEST.in
--rw-r--r--   0 twine    (17125) twine    (17125)     4345 2023-04-15 19:13:21.000000 argparse-manpage-4.1/NEWS
--rw-r--r--   0 twine    (17125) twine    (17125)     8490 2023-04-15 19:13:25.044954 argparse-manpage-4.1/PKG-INFO
--rw-r--r--   0 twine    (17125) twine    (17125)     8047 2023-04-15 19:13:21.000000 argparse-manpage-4.1/README.md
--rwxr-xr-x   0 twine    (17125) twine    (17125)      357 2022-10-31 08:33:07.000000 argparse-manpage-4.1/argparse-manpage
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.034954 argparse-manpage-4.1/argparse_manpage/
--rw-r--r--   0 twine    (17125) twine    (17125)       54 2023-04-15 19:13:21.000000 argparse-manpage-4.1/argparse_manpage/__init__.py
--rw-r--r--   0 twine    (17125) twine    (17125)     3492 2023-04-15 19:13:21.000000 argparse-manpage-4.1/argparse_manpage/cli.py
--rw-r--r--   0 twine    (17125) twine    (17125)     1637 2022-10-31 08:33:07.000000 argparse-manpage-4.1/argparse_manpage/compat.py
--rw-r--r--   0 twine    (17125) twine    (17125)    21030 2023-04-15 19:13:21.000000 argparse-manpage-4.1/argparse_manpage/manpage.py
--rw-r--r--   0 twine    (17125) twine    (17125)     2326 2022-10-31 08:33:07.000000 argparse-manpage-4.1/argparse_manpage/tooling.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.035954 argparse-manpage-4.1/argparse_manpage.egg-info/
--rw-rw-r--   0 twine    (17125) twine    (17125)     8490 2023-04-15 19:13:24.000000 argparse-manpage-4.1/argparse_manpage.egg-info/PKG-INFO
--rw-rw-r--   0 twine    (17125) twine    (17125)     2471 2023-04-15 19:13:24.000000 argparse-manpage-4.1/argparse_manpage.egg-info/SOURCES.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)        1 2023-04-15 19:13:24.000000 argparse-manpage-4.1/argparse_manpage.egg-info/dependency_links.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)       63 2023-04-15 19:13:24.000000 argparse-manpage-4.1/argparse_manpage.egg-info/entry_points.txt
--rw-r--r--   0 twine    (17125) twine    (17125)       25 2023-04-15 19:13:24.000000 argparse-manpage-4.1/argparse_manpage.egg-info/requires.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)       32 2023-04-15 19:13:24.000000 argparse-manpage-4.1/argparse_manpage.egg-info/top_level.txt
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.035954 argparse-manpage-4.1/build_manpages/
--rw-r--r--   0 twine    (17125) twine    (17125)      169 2022-10-31 08:33:07.000000 argparse-manpage-4.1/build_manpages/__init__.py
--rw-r--r--   0 twine    (17125) twine    (17125)     7364 2023-04-15 19:13:21.000000 argparse-manpage-4.1/build_manpages/build_manpage.py
--rw-r--r--   0 twine    (17125) twine    (17125)     5205 2022-10-31 08:33:07.000000 argparse-manpage-4.1/build_manpages/build_manpages.py
--rw-r--r--   0 twine    (17125) twine    (17125)      980 2022-10-31 08:33:07.000000 argparse-manpage-4.1/build_manpages/compat.py
--rw-r--r--   0 twine    (17125) twine    (17125)      157 2022-10-31 08:33:07.000000 argparse-manpage-4.1/build_manpages/manpage.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.032954 argparse-manpage-4.1/examples/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.036954 argparse-manpage-4.1/examples/argument_groups/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.036954 argparse-manpage-4.1/examples/argument_groups/bin/
--rwxr-xr-x   0 twine    (17125) twine    (17125)     2250 2021-11-28 22:10:08.000000 argparse-manpage-4.1/examples/argument_groups/bin/test
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.036954 argparse-manpage-4.1/examples/argument_groups/expected/
--rw-r--r--   0 twine    (17125) twine    (17125)     2125 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/argument_groups/expected/test.1
--rw-r--r--   0 twine    (17125) twine    (17125)      115 2022-10-31 08:33:07.000000 argparse-manpage-4.1/examples/argument_groups/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)      984 2021-11-28 22:10:08.000000 argparse-manpage-4.1/examples/argument_groups/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.036954 argparse-manpage-4.1/examples/copr/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.037954 argparse-manpage-4.1/examples/copr/copr_cli/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/copr_cli/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1067 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/copr_cli/build_config.py
--rw-r--r--   0 twine    (17125) twine    (17125)    49234 2022-10-31 08:33:07.000000 argparse-manpage-4.1/examples/copr/copr_cli/main.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     1067 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/copr_cli/util.py
--rw-r--r--   0 twine    (17125) twine    (17125)    26531 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/copr/expected-output.1
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.037954 argparse-manpage-4.1/examples/copr/fake-deps/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/HACK
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.038954 argparse-manpage-4.1/examples/copr/fake-deps/copr/
--rw-rw-r--   0 twine    (17125) twine    (17125)       35 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/copr/README
--rw-rw-r--   0 twine    (17125) twine    (17125)       43 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/copr/__init__.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.038954 argparse-manpage-4.1/examples/copr/fake-deps/copr/client/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/copr/client/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       29 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/copr/client/responses.py
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/copr/exceptions.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       28 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/jinja2.py
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/fake-deps/simplejson.py
--rw-r--r--   0 twine    (17125) twine    (17125)      113 2022-10-31 08:33:07.000000 argparse-manpage-4.1/examples/copr/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)      965 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/copr/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.039954 argparse-manpage-4.1/examples/old_format/
--rw-r--r--   0 twine    (17125) twine    (17125)      917 2022-01-12 01:47:25.000000 argparse-manpage-4.1/examples/old_format/README.md
--rw-rw-r--   0 twine    (17125) twine    (17125)      519 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/old_format/example.py
--rw-r--r--   0 twine    (17125) twine    (17125)      503 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/old_format/expected-output.1
--rw-rw-r--   0 twine    (17125) twine    (17125)       59 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/old_format/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)      789 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/old_format/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.040954 argparse-manpage-4.1/examples/old_format_file_name/
--rw-r--r--   0 twine    (17125) twine    (17125)      585 2022-01-12 01:47:25.000000 argparse-manpage-4.1/examples/old_format_file_name/README.md
--rw-r--r--   0 twine    (17125) twine    (17125)      519 2022-01-12 01:47:25.000000 argparse-manpage-4.1/examples/old_format_file_name/example.py
--rw-r--r--   0 twine    (17125) twine    (17125)      503 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/old_format_file_name/expected-output.1
--rw-r--r--   0 twine    (17125) twine    (17125)       82 2022-01-12 01:47:25.000000 argparse-manpage-4.1/examples/old_format_file_name/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)      789 2022-01-12 01:47:25.000000 argparse-manpage-4.1/examples/old_format_file_name/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.040954 argparse-manpage-4.1/examples/osc/
--rw-r--r--   0 twine    (17125) twine    (17125)     2246 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/osc/expected-output.1
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.041954 argparse-manpage-4.1/examples/osc/osc/
--rw-r--r--   0 twine    (17125) twine    (17125)        0 2022-04-27 06:51:30.000000 argparse-manpage-4.1/examples/osc/osc/__init__.py
--rwxr-xr-x   0 twine    (17125) twine    (17125)     4636 2022-10-31 08:33:07.000000 argparse-manpage-4.1/examples/osc/osc/main.py
--rw-r--r--   0 twine    (17125) twine    (17125)      251 2022-10-31 08:33:07.000000 argparse-manpage-4.1/examples/osc/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)      772 2022-04-27 06:51:30.000000 argparse-manpage-4.1/examples/osc/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.041954 argparse-manpage-4.1/examples/raw-description/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.041954 argparse-manpage-4.1/examples/raw-description/bin/
--rwxrwxr-x   0 twine    (17125) twine    (17125)     4455 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/raw-description/bin/dg
--rw-r--r--   0 twine    (17125) twine    (17125)     2035 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/raw-description/expected-output.1
--rw-rw-r--   0 twine    (17125) twine    (17125)       69 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/raw-description/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)      982 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/raw-description/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.042954 argparse-manpage-4.1/examples/resalloc/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.042954 argparse-manpage-4.1/examples/resalloc/bin/
--rwxrwxr-x   0 twine    (17125) twine    (17125)     3076 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/bin/resalloc
--rwxrwxr-x   0 twine    (17125) twine    (17125)     2070 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/bin/resalloc-maint
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.032954 argparse-manpage-4.1/examples/resalloc/expected/
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.043954 argparse-manpage-4.1/examples/resalloc/expected/man/
--rw-r--r--   0 twine    (17125) twine    (17125)     1123 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/resalloc/expected/man/resalloc-maint.1
--rw-r--r--   0 twine    (17125) twine    (17125)     1351 2023-04-15 19:13:21.000000 argparse-manpage-4.1/examples/resalloc/expected/man/resalloc.1
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/requirements.txt
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.043954 argparse-manpage-4.1/examples/resalloc/resalloc/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/resalloc/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       51 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/resalloc/client.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       23 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/resalloc/version.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.043954 argparse-manpage-4.1/examples/resalloc/resallocserver/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/resallocserver/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)       27 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/resallocserver/maint.py
--rw-rw-r--   0 twine    (17125) twine    (17125)      146 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)     2241 2019-09-07 00:39:54.000000 argparse-manpage-4.1/examples/resalloc/setup.py
--rw-r--r--   0 twine    (17125) twine    (17125)      133 2023-04-15 19:13:25.045954 argparse-manpage-4.1/setup.cfg
--rw-r--r--   0 twine    (17125) twine    (17125)     1390 2022-10-31 08:33:07.000000 argparse-manpage-4.1/setup.py
-drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-04-15 19:13:25.044954 argparse-manpage-4.1/tests/
--rw-r--r--   0 twine    (17125) twine    (17125)      660 2022-04-27 06:51:30.000000 argparse-manpage-4.1/tests/argparse_testlib.py
--rw-r--r--   0 twine    (17125) twine    (17125)       80 2023-04-15 19:13:21.000000 argparse-manpage-4.1/tests/extra.man
--rw-r--r--   0 twine    (17125) twine    (17125)     2010 2022-10-31 08:33:07.000000 argparse-manpage-4.1/tests/test_basic.py
--rw-r--r--   0 twine    (17125) twine    (17125)     7014 2022-10-31 08:33:07.000000 argparse-manpage-4.1/tests/test_examples.py
--rw-r--r--   0 twine    (17125) twine    (17125)     4165 2023-04-15 19:13:21.000000 argparse-manpage-4.1/tests/test_script.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.389906 argparse-manpage-4.2/
+-rw-rw-r--   0 twine    (17125) twine    (17125)      136 2019-09-07 00:39:54.000000 argparse-manpage-4.2/AUTHORS
+-rw-rw-r--   0 twine    (17125) twine    (17125)    11357 2019-09-07 00:39:54.000000 argparse-manpage-4.2/LICENSE
+-rw-r--r--   0 twine    (17125) twine    (17125)      649 2023-05-14 10:57:58.000000 argparse-manpage-4.2/MANIFEST.in
+-rw-r--r--   0 twine    (17125) twine    (17125)     4774 2023-05-14 10:57:58.000000 argparse-manpage-4.2/NEWS
+-rw-r--r--   0 twine    (17125) twine    (17125)     8915 2023-05-14 10:58:16.389906 argparse-manpage-4.2/PKG-INFO
+-rw-r--r--   0 twine    (17125) twine    (17125)     8472 2023-05-14 10:57:58.000000 argparse-manpage-4.2/README.md
+-rwxr-xr-x   0 twine    (17125) twine    (17125)      357 2022-10-31 08:33:07.000000 argparse-manpage-4.2/argparse-manpage
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.379906 argparse-manpage-4.2/argparse_manpage/
+-rw-r--r--   0 twine    (17125) twine    (17125)       54 2023-05-14 10:57:58.000000 argparse-manpage-4.2/argparse_manpage/__init__.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     3589 2023-05-14 10:57:58.000000 argparse-manpage-4.2/argparse_manpage/cli.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     1669 2023-05-14 10:57:58.000000 argparse-manpage-4.2/argparse_manpage/compat.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    21556 2023-05-14 10:57:58.000000 argparse-manpage-4.2/argparse_manpage/manpage.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     2326 2022-10-31 08:33:07.000000 argparse-manpage-4.2/argparse_manpage/tooling.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.380906 argparse-manpage-4.2/argparse_manpage.egg-info/
+-rw-rw-r--   0 twine    (17125) twine    (17125)     8915 2023-05-14 10:58:16.000000 argparse-manpage-4.2/argparse_manpage.egg-info/PKG-INFO
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2605 2023-05-14 10:58:16.000000 argparse-manpage-4.2/argparse_manpage.egg-info/SOURCES.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)        1 2023-05-14 10:58:16.000000 argparse-manpage-4.2/argparse_manpage.egg-info/dependency_links.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)       63 2023-05-14 10:58:16.000000 argparse-manpage-4.2/argparse_manpage.egg-info/entry_points.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)       58 2023-05-14 10:58:16.000000 argparse-manpage-4.2/argparse_manpage.egg-info/requires.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)       32 2023-05-14 10:58:16.000000 argparse-manpage-4.2/argparse_manpage.egg-info/top_level.txt
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.381906 argparse-manpage-4.2/build_manpages/
+-rw-r--r--   0 twine    (17125) twine    (17125)      169 2022-10-31 08:33:07.000000 argparse-manpage-4.2/build_manpages/__init__.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     7364 2023-04-15 19:13:21.000000 argparse-manpage-4.2/build_manpages/build_manpage.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     6248 2023-05-14 10:57:58.000000 argparse-manpage-4.2/build_manpages/build_manpages.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      980 2022-10-31 08:33:07.000000 argparse-manpage-4.2/build_manpages/compat.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      157 2022-10-31 08:33:07.000000 argparse-manpage-4.2/build_manpages/manpage.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.378906 argparse-manpage-4.2/examples/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.381906 argparse-manpage-4.2/examples/argument_groups/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.381906 argparse-manpage-4.2/examples/argument_groups/bin/
+-rwxr-xr-x   0 twine    (17125) twine    (17125)     2250 2021-11-28 22:10:08.000000 argparse-manpage-4.2/examples/argument_groups/bin/test
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.381906 argparse-manpage-4.2/examples/argument_groups/expected/
+-rw-r--r--   0 twine    (17125) twine    (17125)     2125 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/argument_groups/expected/test.1
+-rw-r--r--   0 twine    (17125) twine    (17125)      115 2022-10-31 08:33:07.000000 argparse-manpage-4.2/examples/argument_groups/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)      984 2021-11-28 22:10:08.000000 argparse-manpage-4.2/examples/argument_groups/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.382906 argparse-manpage-4.2/examples/copr/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.383906 argparse-manpage-4.2/examples/copr/copr_cli/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/copr_cli/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1067 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/copr_cli/build_config.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    49234 2022-10-31 08:33:07.000000 argparse-manpage-4.2/examples/copr/copr_cli/main.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)     1067 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/copr_cli/util.py
+-rw-r--r--   0 twine    (17125) twine    (17125)    26531 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/copr/expected-output.1
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.383906 argparse-manpage-4.2/examples/copr/fake-deps/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/HACK
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.384906 argparse-manpage-4.2/examples/copr/fake-deps/copr/
+-rw-rw-r--   0 twine    (17125) twine    (17125)       35 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/copr/README
+-rw-rw-r--   0 twine    (17125) twine    (17125)       43 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/copr/__init__.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.384906 argparse-manpage-4.2/examples/copr/fake-deps/copr/client/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/copr/client/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       29 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/copr/client/responses.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/copr/exceptions.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       28 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/jinja2.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/fake-deps/simplejson.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      113 2022-10-31 08:33:07.000000 argparse-manpage-4.2/examples/copr/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)      965 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/copr/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.385906 argparse-manpage-4.2/examples/old_format/
+-rw-r--r--   0 twine    (17125) twine    (17125)      917 2022-01-12 01:47:25.000000 argparse-manpage-4.2/examples/old_format/README.md
+-rw-rw-r--   0 twine    (17125) twine    (17125)      519 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/old_format/example.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      503 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/old_format/expected-output.1
+-rw-rw-r--   0 twine    (17125) twine    (17125)       59 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/old_format/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)      789 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/old_format/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.385906 argparse-manpage-4.2/examples/old_format_file_name/
+-rw-r--r--   0 twine    (17125) twine    (17125)      585 2022-01-12 01:47:25.000000 argparse-manpage-4.2/examples/old_format_file_name/README.md
+-rw-r--r--   0 twine    (17125) twine    (17125)      519 2022-01-12 01:47:25.000000 argparse-manpage-4.2/examples/old_format_file_name/example.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      503 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/old_format_file_name/expected-output.1
+-rw-r--r--   0 twine    (17125) twine    (17125)       82 2022-01-12 01:47:25.000000 argparse-manpage-4.2/examples/old_format_file_name/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)      789 2022-01-12 01:47:25.000000 argparse-manpage-4.2/examples/old_format_file_name/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.386906 argparse-manpage-4.2/examples/osc/
+-rw-r--r--   0 twine    (17125) twine    (17125)     2246 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/osc/expected-output.1
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.386906 argparse-manpage-4.2/examples/osc/osc/
+-rw-r--r--   0 twine    (17125) twine    (17125)        0 2022-04-27 06:51:30.000000 argparse-manpage-4.2/examples/osc/osc/__init__.py
+-rwxr-xr-x   0 twine    (17125) twine    (17125)     4636 2022-10-31 08:33:07.000000 argparse-manpage-4.2/examples/osc/osc/main.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      251 2022-10-31 08:33:07.000000 argparse-manpage-4.2/examples/osc/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)      772 2022-04-27 06:51:30.000000 argparse-manpage-4.2/examples/osc/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.387906 argparse-manpage-4.2/examples/pre-written-man-page/
+-rw-r--r--   0 twine    (17125) twine    (17125)      871 2023-05-14 10:57:58.000000 argparse-manpage-4.2/examples/pre-written-man-page/psutils.1
+-rw-r--r--   0 twine    (17125) twine    (17125)       60 2023-05-14 10:57:58.000000 argparse-manpage-4.2/examples/pre-written-man-page/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)      272 2023-05-14 10:57:58.000000 argparse-manpage-4.2/examples/pre-written-man-page/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.387906 argparse-manpage-4.2/examples/raw-description/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.387906 argparse-manpage-4.2/examples/raw-description/bin/
+-rwxrwxr-x   0 twine    (17125) twine    (17125)     4455 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/raw-description/bin/dg
+-rw-r--r--   0 twine    (17125) twine    (17125)     2035 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/raw-description/expected-output.1
+-rw-rw-r--   0 twine    (17125) twine    (17125)       69 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/raw-description/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)      982 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/raw-description/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.388906 argparse-manpage-4.2/examples/resalloc/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.388906 argparse-manpage-4.2/examples/resalloc/bin/
+-rwxrwxr-x   0 twine    (17125) twine    (17125)     3076 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/bin/resalloc
+-rwxrwxr-x   0 twine    (17125) twine    (17125)     2070 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/bin/resalloc-maint
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.378906 argparse-manpage-4.2/examples/resalloc/expected/
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.388906 argparse-manpage-4.2/examples/resalloc/expected/man/
+-rw-r--r--   0 twine    (17125) twine    (17125)     1123 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/resalloc/expected/man/resalloc-maint.1
+-rw-r--r--   0 twine    (17125) twine    (17125)     1351 2023-04-15 19:13:21.000000 argparse-manpage-4.2/examples/resalloc/expected/man/resalloc.1
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/requirements.txt
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.388906 argparse-manpage-4.2/examples/resalloc/resalloc/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/resalloc/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       51 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/resalloc/client.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       23 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/resalloc/version.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.389906 argparse-manpage-4.2/examples/resalloc/resallocserver/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/resallocserver/__init__.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)       27 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/resallocserver/maint.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)      146 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/setup.cfg
+-rw-rw-r--   0 twine    (17125) twine    (17125)     2241 2019-09-07 00:39:54.000000 argparse-manpage-4.2/examples/resalloc/setup.py
+-rw-r--r--   0 twine    (17125) twine    (17125)      193 2023-05-14 10:57:58.000000 argparse-manpage-4.2/pyproject.toml
+-rw-r--r--   0 twine    (17125) twine    (17125)      133 2023-05-14 10:58:16.390906 argparse-manpage-4.2/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)     1551 2023-05-14 10:57:58.000000 argparse-manpage-4.2/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2023-05-14 10:58:16.389906 argparse-manpage-4.2/tests/
+-rw-r--r--   0 twine    (17125) twine    (17125)      849 2023-05-14 10:57:58.000000 argparse-manpage-4.2/tests/argparse_testlib.py
+-rw-r--r--   0 twine    (17125) twine    (17125)       80 2023-04-15 19:13:21.000000 argparse-manpage-4.2/tests/extra.man
+-rw-r--r--   0 twine    (17125) twine    (17125)     2010 2022-10-31 08:33:07.000000 argparse-manpage-4.2/tests/test_basic.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     7299 2023-05-14 10:57:58.000000 argparse-manpage-4.2/tests/test_examples.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     6098 2023-05-14 10:57:58.000000 argparse-manpage-4.2/tests/test_script.py
```

### Comparing `argparse-manpage-4.1/LICENSE` & `argparse-manpage-4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/MANIFEST.in` & `argparse-manpage-4.2/MANIFEST.in`

 * *Files 10% similar despite different names*

```diff
@@ -6,11 +6,12 @@
 recursive-include tests *.py
 recursive-include unittests *.py
 include examples/argument_groups/bin/test
 include examples/resalloc/expected/man/resalloc-maint.1
 include examples/resalloc/expected/man/resalloc.1
 include examples/copr/fake-deps/HACK
 include examples/copr/fake-deps/copr/README
+include examples/pre-written-man-page/psutils.1
 include examples/raw-description/bin/dg
 include examples/resalloc/bin/resalloc
 include examples/resalloc/bin/resalloc-maint
 include tests/extra.man
```

### Comparing `argparse-manpage-4.1/NEWS` & `argparse-manpage-4.2/NEWS`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 WARNING: The 'build_manpage' setup.py command will be removed v5
 WARNING: We'll drop the Python 2.7 support in v5
 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+News in v4.2
+
+* Support for pyproject.toml specification of manpages added.
+
+* Support for pre-written man pages (the --manfile option)
+
+Bugfixes in version 4.2
+
+* Incorrect dict access for --include support fixed.
+
+* Provide useful AUTHORS section with e-mail from
+  Distribution.get_author_email() even if Distribution.get_author() returns
+  None.
+
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
 News in v4.1
 
 * A new `--include` feature, inspired by `help2man --include`.
 
 * Allow overriding build date with SOURCE_DATE_EPOCH environment variable
   in order to make builds reproducible.  See this link for more info:
   https://reproducible-builds.org/specs/source-date-epoch/
```

### Comparing `argparse-manpage-4.1/PKG-INFO` & `argparse-manpage-4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-manpage
-Version: 4.1
+Version: 4.2
 Summary: Build manual page from python's ArgumentParser object.
 Home-page: https://github.com/praiskup/argparse-manpage
 Author: Gabriele Giammatteo
 Author-email: gabriele.giammatteo@eng.it
 Maintainer: Pavel Raiskup
 Maintainer-email: praiskup@redhat.com
 License: Apache 2.0
@@ -95,25 +95,36 @@
       # are automatically re-generated and installed
       'build_py': get_build_py_cmd(),
       'install': get_install_cmd(),
   }
 )
 ```
 
-And in the `setup.cfg` configure the manual pages you want to automatically
+And in `setup.cfg` configure the manual pages you want to automatically
 generate and install:
 
 ```
 [build_manpages]
 manpages =
     man/foo.1:object=parser:pyfile=bin/foo.py
     man/bar.1:function=get_parser:pyfile=bin/bar
     man/baz.1:function=get_parser:pyfile=bin/bar:prog=baz
 ```
 
+Or in `pyproject.toml` (requires setuptools >= 62.2.0):
+
+```toml
+[build_manpages]
+manpages = [
+    "man/foo.1:object=parser:pyfile=bin/foo.py",
+    "man/bar.1:function=get_parser:pyfile=bin/bar",
+    "man/baz.1:function=get_parser:pyfile=bin/bar:prog=baz",
+]
+```
+
 The format of those lines is a colon separated list of arguments/options.  The
 first argument determines the filename of the generated manual page.  Then
 follows a list of options of format `option=value`.  Supported values are:
 
 - pyfile - what python file the argparse object resides in
 - object - the name of arparse object in "pyfile" to import
 - function - the name of function in pyfile to call to get the argparse object
@@ -126,16 +137,18 @@
 - prog - value that substitutes %prog in ArgumentParser's usage
 - url - link to project download page
 - manual_section - section of the manual, by default 1, see man (7) man-pages
     for more info about existing sections
 - manual_title - the title of the manual, by default "Generated Python Manual",
     see man (7) man-pages for more instructions
 - include - a file of extra material to include; see below for the format
+- manfile - a file containing a complete man page that just needs to be installed
 
-The values from setup.cfg override values from setup.py's setup().
+The values from setup.cfg override values from setup.py's setup(). Note that
+when `manfile` is set for a particular page, no other option is allowed.
 
 Then run `setup.py build_manpages` to build a manpages for your project.  Also,
 if you used `get_build_py` helper, `setup.py build` then transitively builds the
 manual pages.
 
 ## Include file format
```

### Comparing `argparse-manpage-4.1/README.md` & `argparse-manpage-4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -80,25 +80,36 @@
       # are automatically re-generated and installed
       'build_py': get_build_py_cmd(),
       'install': get_install_cmd(),
   }
 )
 ```
 
-And in the `setup.cfg` configure the manual pages you want to automatically
+And in `setup.cfg` configure the manual pages you want to automatically
 generate and install:
 
 ```
 [build_manpages]
 manpages =
     man/foo.1:object=parser:pyfile=bin/foo.py
     man/bar.1:function=get_parser:pyfile=bin/bar
     man/baz.1:function=get_parser:pyfile=bin/bar:prog=baz
 ```
 
+Or in `pyproject.toml` (requires setuptools >= 62.2.0):
+
+```toml
+[build_manpages]
+manpages = [
+    "man/foo.1:object=parser:pyfile=bin/foo.py",
+    "man/bar.1:function=get_parser:pyfile=bin/bar",
+    "man/baz.1:function=get_parser:pyfile=bin/bar:prog=baz",
+]
+```
+
 The format of those lines is a colon separated list of arguments/options.  The
 first argument determines the filename of the generated manual page.  Then
 follows a list of options of format `option=value`.  Supported values are:
 
 - pyfile - what python file the argparse object resides in
 - object - the name of arparse object in "pyfile" to import
 - function - the name of function in pyfile to call to get the argparse object
@@ -111,16 +122,18 @@
 - prog - value that substitutes %prog in ArgumentParser's usage
 - url - link to project download page
 - manual_section - section of the manual, by default 1, see man (7) man-pages
     for more info about existing sections
 - manual_title - the title of the manual, by default "Generated Python Manual",
     see man (7) man-pages for more instructions
 - include - a file of extra material to include; see below for the format
+- manfile - a file containing a complete man page that just needs to be installed
 
-The values from setup.cfg override values from setup.py's setup().
+The values from setup.cfg override values from setup.py's setup(). Note that
+when `manfile` is set for a particular page, no other option is allowed.
 
 Then run `setup.py build_manpages` to build a manpages for your project.  Also,
 if you used `get_build_py` helper, `setup.py build` then transitively builds the
 manual pages.
 
 ## Include file format
```

### Comparing `argparse-manpage-4.1/argparse_manpage/cli.py` & `argparse-manpage-4.2/argparse_manpage/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     "Section of the manual, by default 1.  See man (7) man-pages for more "
     "info about existing sections."))
 ap.add_argument("--manual-title", help=(
     "The title of the manual, by default \"Generated Python Manual\". "
     "See man (7) man-pages for more instructions."))
 ap.add_argument("--include", metavar="FILE", help=(
     "File that contains extra material for the man page."))
+ap.add_argument("--manfile", metavar="FILE", help=(
+    "File containing a complete man page."))
 
 
 def args_to_manpage_data(args):
     data = {}
     for attr in MANPAGE_DATA_ATTRS:
         value = getattr(args, attr)
         data[attr] = value
```

### Comparing `argparse-manpage-4.1/argparse_manpage/compat.py` & `argparse-manpage-4.2/argparse_manpage/compat.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 
 import sys
 
 # Drop once Python 2.7 is dropped
 # pylint: disable=unused-import
 try:
-    from configparser import ConfigParser
+    from configparser import ConfigParser, NoSectionError
 except ImportError:
-    from ConfigParser import SafeConfigParser as ConfigParser  # type: ignore
+    from ConfigParser import SafeConfigParser as ConfigParser, NoSectionError  # type: ignore
 
 if sys.version_info < (3, 0):
     import imp  # pylint: disable=deprecated-module
     def load_py_file(filename):
         """ Small wrapper having the same call arg list as runpy.run_path() """
         return imp.load_source("argparse_manpage_loaded_file", filename)
 else:
```

### Comparing `argparse-manpage-4.1/argparse_manpage/manpage.py` & `argparse-manpage-4.2/argparse_manpage/manpage.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "prog",
     "url",
     "version",
     "format",
     "manual_section",
     "manual_title",
     "include",
+    "manfile",
 )
 
 # manpage sections that are handled specially, so need special treatment
 # when --include'ing extra material; see Manpage.add_section.
 SPECIAL_MANPAGE_SECTIONS = (
     "author",
     "comments",
@@ -67,18 +68,23 @@
 
 def get_manpage_data_from_distribution(distribution, data):
     """
     Update `data` with values from `distribution`.
     """
     # authors
     if not "authors" in data:
-        author = distribution.get_author()
-        if distribution.get_author_email():
-            author += " <{}>".format(distribution.get_author_email())
-        data["authors"] = [author]
+        author = None
+        if distribution.get_author():
+            author = distribution.get_author()
+            if distribution.get_author_email():
+                author += " <{}>".format(distribution.get_author_email())
+        elif distribution.get_author_email():
+            author = distribution.get_author_email()
+        if author:
+            data["authors"] = [author]
 
     attrs = list(MANPAGE_DATA_ATTRS)
     attrs.remove("authors")
     attrs.remove("prog")  # not available, copied from 'project_name' later
     attrs.remove("format")  # not available, must be set in setup.cfg
     # we want the utility description, not the project description
     attrs.remove("description")
@@ -151,14 +157,20 @@
         self.parser = parser
         self.format = format
         self._data = _data or {}
         self._match_texts = []
         if not getattr(parser, '_manpage', None):
             self.parser._manpage = []
 
+        self.manfile = self._data.get("manfile")
+        if self.manfile:
+            if len(self._data) > 1:
+                raise ValueError("manfile set, so no other key is allowed")
+            return
+
         self.formatter = self.parser._get_formatter()
         self.mf = _ManpageFormatter(self.prog, self.formatter, format=self.format)
         self.synopsis = self.parser.format_usage().split(':')[-1].split()
 
         self.date = self._data.get("date")
         if not self.date:
             builddate = datetime.datetime.utcfromtimestamp(
@@ -189,14 +201,18 @@
             self.parse_include(include)
 
     def format_text(self, text):
         # Wrap by parser formatter and convert to manpage format
         return self.mf.format_text(self.formatter._format_text(text)).strip('\n')
 
     def __str__(self):
+        if self.manfile:
+            with open(self.manfile) as fd:
+                return fd.read()
+
         lines = []
 
         # Header
         # per man (7) man-pages: .TH title section date source manual
         header = '.TH {title} "{section}" "{date}" "{source}" "{manual}"'
         lines.append(header.format(
             title=_markup(self.prog.upper()),
@@ -222,31 +238,31 @@
         lines.append(_markup(line))
 
         # Synopsis
         synopsis_section = self.get_extra_section("synopsis")
         if self.synopsis or synopsis_section:
             lines.append('.SH SYNOPSIS')
             if synopsis_section:
-                lines.append(synopsis_section.content)
+                lines.append(synopsis_section["content"])
             else:
                 lines.append('.B {}'.format(_markup(self.synopsis[0])))
                 lines.append(' '.join(self.synopsis[1:]))
 
         extra_description = None
         description_section = self.get_extra_section("description")
         if description_section:
-            extra_description = description_section.content
+            extra_description = description_section["content"]
         lines.extend(self.mf.format_parser(self.parser, extra_description=extra_description))
 
         comments_section = self.get_extra_section("comments")
         if self.parser.epilog or comments_section:
             lines.append("")
             lines.append('.SH COMMENTS')
             if comments_section:
-                lines.append(comments_section.content)
+                lines.append(comments_section["content"])
             else:
                 lines.append(self.format_text(self.parser.epilog))
 
         # Additional sections
         for section in self.parser._manpage: # pylint: disable=protected-access
             if section["heading"] not in SPECIAL_MANPAGE_SECTIONS:
                 lines.append('.SH {}'.format(section['heading'].upper()))
```

### Comparing `argparse-manpage-4.1/argparse_manpage/tooling.py` & `argparse-manpage-4.2/argparse_manpage/tooling.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/argparse_manpage.egg-info/PKG-INFO` & `argparse-manpage-4.2/argparse_manpage.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-manpage
-Version: 4.1
+Version: 4.2
 Summary: Build manual page from python's ArgumentParser object.
 Home-page: https://github.com/praiskup/argparse-manpage
 Author: Gabriele Giammatteo
 Author-email: gabriele.giammatteo@eng.it
 Maintainer: Pavel Raiskup
 Maintainer-email: praiskup@redhat.com
 License: Apache 2.0
@@ -95,25 +95,36 @@
       # are automatically re-generated and installed
       'build_py': get_build_py_cmd(),
       'install': get_install_cmd(),
   }
 )
 ```
 
-And in the `setup.cfg` configure the manual pages you want to automatically
+And in `setup.cfg` configure the manual pages you want to automatically
 generate and install:
 
 ```
 [build_manpages]
 manpages =
     man/foo.1:object=parser:pyfile=bin/foo.py
     man/bar.1:function=get_parser:pyfile=bin/bar
     man/baz.1:function=get_parser:pyfile=bin/bar:prog=baz
 ```
 
+Or in `pyproject.toml` (requires setuptools >= 62.2.0):
+
+```toml
+[build_manpages]
+manpages = [
+    "man/foo.1:object=parser:pyfile=bin/foo.py",
+    "man/bar.1:function=get_parser:pyfile=bin/bar",
+    "man/baz.1:function=get_parser:pyfile=bin/bar:prog=baz",
+]
+```
+
 The format of those lines is a colon separated list of arguments/options.  The
 first argument determines the filename of the generated manual page.  Then
 follows a list of options of format `option=value`.  Supported values are:
 
 - pyfile - what python file the argparse object resides in
 - object - the name of arparse object in "pyfile" to import
 - function - the name of function in pyfile to call to get the argparse object
@@ -126,16 +137,18 @@
 - prog - value that substitutes %prog in ArgumentParser's usage
 - url - link to project download page
 - manual_section - section of the manual, by default 1, see man (7) man-pages
     for more info about existing sections
 - manual_title - the title of the manual, by default "Generated Python Manual",
     see man (7) man-pages for more instructions
 - include - a file of extra material to include; see below for the format
+- manfile - a file containing a complete man page that just needs to be installed
 
-The values from setup.cfg override values from setup.py's setup().
+The values from setup.cfg override values from setup.py's setup(). Note that
+when `manfile` is set for a particular page, no other option is allowed.
 
 Then run `setup.py build_manpages` to build a manpages for your project.  Also,
 if you used `get_build_py` helper, `setup.py build` then transitively builds the
 manual pages.
 
 ## Include file format
```

### Comparing `argparse-manpage-4.1/argparse_manpage.egg-info/SOURCES.txt` & `argparse-manpage-4.2/argparse_manpage.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 NEWS
 README.md
 argparse-manpage
+pyproject.toml
 setup.cfg
 setup.py
 argparse_manpage/__init__.py
 argparse_manpage/cli.py
 argparse_manpage/compat.py
 argparse_manpage/manpage.py
 argparse_manpage/tooling.py
@@ -52,14 +53,17 @@
 examples/old_format_file_name/setup.cfg
 examples/old_format_file_name/setup.py
 examples/osc/expected-output.1
 examples/osc/setup.cfg
 examples/osc/setup.py
 examples/osc/osc/__init__.py
 examples/osc/osc/main.py
+examples/pre-written-man-page/psutils.1
+examples/pre-written-man-page/setup.cfg
+examples/pre-written-man-page/setup.py
 examples/raw-description/expected-output.1
 examples/raw-description/setup.cfg
 examples/raw-description/setup.py
 examples/raw-description/bin/dg
 examples/resalloc/requirements.txt
 examples/resalloc/setup.cfg
 examples/resalloc/setup.py
```

### Comparing `argparse-manpage-4.1/build_manpages/build_manpage.py` & `argparse-manpage-4.2/build_manpages/build_manpage.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/build_manpages/build_manpages.py` & `argparse-manpage-4.2/build_manpages/build_manpages.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,22 @@
 build_manpages command -- generate set of manual pages by the setup()
 command.
 """
 
 import os
 import shutil
 
-from argparse_manpage.compat import ConfigParser
+try:
+    import tomllib
+    from tomllib import TOMLDecodeError
+except ImportError:
+    import toml as tomllib
+    from toml import TomlDecodeError as TOMLDecodeError
+
+from argparse_manpage.compat import ConfigParser, NoSectionError
 from argparse_manpage.tooling import get_parser, write_to_filename
 from argparse_manpage.manpage import (
     Manpage,
     MANPAGE_DATA_ATTRS,
     get_manpage_data_from_distribution,
 )
 
@@ -62,37 +69,55 @@
             else:
                 raise ValueError("Unknown manpage configuration option: {}".format(oname))
 
         manpages_data[outputfile] = manpagedata
 
     return manpages_data
 
+def get_pyproject_settings():
+    """Parse and handle errors of a toml configuration file."""
+    try:
+        with open("pyproject.toml", mode="r") as fp:
+            content = tomllib.loads(fp.read())
+    except TOMLDecodeError:
+        return None
+
+    try:
+        value = content["tool"][DEFAULT_CMD_NAME]["manpages"]
+        if isinstance(value, list):
+            value = "\n".join(value)
+        return str(value)
+    except KeyError:
+        return None
 
 class build_manpages(Command):
     description = 'Generate set of man pages from setup().'
     user_options = [
         ('manpages=', 'O', 'list man pages specifications'),
     ]
 
     def initialize_options(self):
         self.manpages = None
 
 
     def finalize_options(self):
-        if not self.manpages:
+        manpages = self.manpages or get_pyproject_settings()
+        if not manpages:
             raise DistutilsOptionError('\'manpages\' option is required')
-
-        self.manpages_data = parse_manpages_spec(self.manpages)
+        self.manpages_data = parse_manpages_spec(manpages)
 
         # if a value wasn't set in setup.cfg, use the value from setup.py
         for page, data in self.manpages_data.items():
             get_manpage_data_from_distribution(self.distribution, data)
 
     def run(self):
         for page, data in self.manpages_data.items():
+            if data.get('manfile'):
+                print ("using pre-written " + page)
+                return
             print ("generating " + page)
             parser = get_parser(data['import_type'], data['import_from'], data['objname'], data['objtype'], data.get('prog', None))
             format = data.get('format', 'pretty')
             if format in ('pretty', 'single-commands-section'):
                 manpage = Manpage(parser, format=format, _data=data)
                 write_to_filename(str(manpage), page)
             elif format == 'old':
@@ -131,15 +156,21 @@
     class _build_manpages_install(command):
         def install_manual_pages(self):
             """
             Additional logic for installing the generated manual pages
             """
             config = ConfigParser()
             config.read('setup.cfg')
-            spec = config.get(DEFAULT_CMD_NAME, 'manpages')
+            try:
+                spec = config.get(DEFAULT_CMD_NAME, 'manpages')
+            except NoSectionError:
+                spec = get_pyproject_settings()
+            if spec is None:
+                raise ValueError("'manpage' configuration not found in setup.cfg or pyproject.toml")
+
             data = parse_manpages_spec(spec)
 
             mandir = os.path.join(self.install_data, 'share/man/man1')
             if not os.path.exists(mandir):
                 os.makedirs(mandir)
             for key, _ in data.items():
                 print ('installing {0}'.format(key))
```

### Comparing `argparse-manpage-4.1/build_manpages/compat.py` & `argparse-manpage-4.2/build_manpages/compat.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/argument_groups/bin/test` & `argparse-manpage-4.2/examples/argument_groups/bin/test`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/argument_groups/expected/test.1` & `argparse-manpage-4.2/examples/argument_groups/expected/test.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/argument_groups/setup.py` & `argparse-manpage-4.2/examples/argument_groups/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/copr/copr_cli/build_config.py` & `argparse-manpage-4.2/examples/copr/copr_cli/build_config.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/copr/copr_cli/main.py` & `argparse-manpage-4.2/examples/copr/copr_cli/main.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/copr/copr_cli/util.py` & `argparse-manpage-4.2/examples/copr/copr_cli/util.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/copr/expected-output.1` & `argparse-manpage-4.2/examples/copr/expected-output.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/copr/setup.py` & `argparse-manpage-4.2/examples/copr/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/old_format/README.md` & `argparse-manpage-4.2/examples/old_format/README.md`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/old_format/example.py` & `argparse-manpage-4.2/examples/old_format/example.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/old_format/setup.py` & `argparse-manpage-4.2/examples/old_format/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/old_format_file_name/README.md` & `argparse-manpage-4.2/examples/old_format_file_name/README.md`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/old_format_file_name/example.py` & `argparse-manpage-4.2/examples/old_format_file_name/example.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/old_format_file_name/setup.py` & `argparse-manpage-4.2/examples/old_format_file_name/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/osc/expected-output.1` & `argparse-manpage-4.2/examples/osc/expected-output.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/osc/osc/main.py` & `argparse-manpage-4.2/examples/osc/osc/main.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/osc/setup.py` & `argparse-manpage-4.2/examples/osc/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/raw-description/bin/dg` & `argparse-manpage-4.2/examples/raw-description/bin/dg`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/raw-description/expected-output.1` & `argparse-manpage-4.2/examples/raw-description/expected-output.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/raw-description/setup.py` & `argparse-manpage-4.2/examples/raw-description/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/resalloc/bin/resalloc` & `argparse-manpage-4.2/examples/resalloc/bin/resalloc`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/resalloc/bin/resalloc-maint` & `argparse-manpage-4.2/examples/resalloc/bin/resalloc-maint`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/resalloc/expected/man/resalloc-maint.1` & `argparse-manpage-4.2/examples/resalloc/expected/man/resalloc-maint.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/resalloc/expected/man/resalloc.1` & `argparse-manpage-4.2/examples/resalloc/expected/man/resalloc.1`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/examples/resalloc/setup.py` & `argparse-manpage-4.2/examples/resalloc/setup.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/tests/test_basic.py` & `argparse-manpage-4.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `argparse-manpage-4.1/tests/test_examples.py` & `argparse-manpage-4.2/tests/test_examples.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,32 +8,23 @@
 import sysconfig
 from contextlib import contextmanager
 
 import pytest
 
 sys.path = [os.path.join(os.path.dirname(os.path.realpath(__file__)),'..')]+sys.path
 
-from argparse_testlib import skip_on_python_older_than
+from argparse_testlib import skip_on_python_older_than, pushd
 
 
 def _mandir(prefix, num=1):
     data = sysconfig.get_path('data', vars={'base': prefix})
     return os.path.join(data, 'share/man/man' + str(num))
 
 
 @contextmanager
-def pushd(path):
-    old_dir = os.getcwd()
-    os.chdir(path)
-    try:
-        yield
-    finally:
-        os.chdir(old_dir)
-
-@contextmanager
 def change_argv(argv):
     old_argv = sys.argv
     sys.argv = argv
     try:
         yield
     finally:
         sys.argv = old_argv
@@ -60,22 +51,16 @@
         subprocess.call([sys.executable, '-m', 'pip'] + args + ["."], env=environ)
 
 
 def run_setup_py(args):
     environ = os.environ.copy()
     environ['PYTHONPATH'] = ':'.join(sys.path)
     with change_argv(['setup.py'] + args):
-        subprocess.call([sys.executable, 'setup.py'] + args,
-                        env=environ)
-
-def skip_if_older_python(min_version):
-    def _get_int(version):
-        int_v = [int(sv) for sv in version.split(".")]
-
-
+        return subprocess.call([sys.executable, 'setup.py'] + args,
+                               env=environ)
 
 
 def run_one_installer(installer, args):
     """
     Run 'pip <args> .' or 'python setup.py <args>'
     """
 
@@ -108,15 +93,15 @@
                 if filter_string is not None:
                     left = filter_string(left)
                     right = filter_string(right)
 
                 assert left == right
 
 
-class TestAllExapmles:
+class TestAllExamples:
     def test_old_example(self):
         with pushd('examples/old_format'):
             try:
                 os.remove('example.1')
             except OSError:
                 pass
             run_setup_py(['build_manpage'])
@@ -202,10 +187,22 @@
             mandir = os.path.join(idir, _mandir("usr/"))
             _rmtree(idir)
             run_one_installer(installer, ['install', '--root', idir, '--prefix', prefix])
 
             file_cmp(os.path.join(mandir, os.path.basename(name)), 'expected-output.1')
             file_cmp(name, 'expected-output.1')
 
+    @pytest.mark.parametrize("installer", ["pip", "setuppy"])
+    def test_pre_written_man_page(self, installer):
+        with pushd('examples/pre-written-man-page'):
+            name = 'psutils.1'
+            prefix = '/usr'
+            idir = os.path.join(os.getcwd(), installer + "_install_dir")
+            mandir = os.path.join(idir, _mandir("usr/"))
+            _rmtree(idir)
+            run_one_installer(installer, ['install', '--root', idir, '--prefix', prefix])
+
+            file_cmp(os.path.join(mandir, name), name)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `argparse-manpage-4.1/tests/test_script.py` & `argparse-manpage-4.2/tests/test_script.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,30 +5,41 @@
 import datetime
 import os
 import shutil
 import sys
 import subprocess
 import tempfile
 import time
+import warnings
 
-SIMPLE_FILE_CONTENTS = """
+from packaging import version
+
+import setuptools
+
+from test_examples import run_setup_py
+from argparse_testlib import pushd
+
+SIMPLE_FILE_CONTENTS = """\
 import argparse
 
 def get_parser():
         parser = argparse.ArgumentParser({ap_arguments})
         parser.add_argument("test")
         return parser
 
-if __name__ == "__main__":
+def main():
         print("here")
         get_parser().parse_args()
+
+if __name__ == "__main__":
+        main()
 """
 
 SIMPLE_OUTPUT = """\
-.TH {NAME} "1" "{DATE}" "{name}" "Generated Python Manual"
+.TH {NAME} "1" "{DATE}" "{name}{version}" "Generated Python Manual"
 .SH NAME
 {name}
 .SH SYNOPSIS
 .B {name}
 [-h] test
 
 .TP
@@ -54,22 +65,43 @@
 Developer extraordinaire.
 .fi
 .nf
 Mr. Foo <mfoo@example.com> and friends
 .fi
 """
 
+SETUP_PY_FILE_CONTENTS = """\
+from build_manpages import build_manpages, get_install_cmd, get_build_py_cmd
+from setuptools import setup
+
+setup(
+    cmdclass={
+        'build_manpages': build_manpages,
+        'build_py': get_build_py_cmd(),
+        'install': get_install_cmd(),
+    }
+)
+"""
+
+PYPROJECT_TOML_FILE_CONTENTS = """\
+[tool.build_manpages]
+manpages = [
+    "some-file.1:project_name=some-file:module=somefile:function=get_parser",
+]
+"""
+
 DATE = datetime.datetime.utcfromtimestamp(
            int(os.environ.get('SOURCE_DATE_EPOCH', time.time()))
        ).strftime("%Y\\-%m\\-%d")
 
 class TestsArgparseManpageScript:
     def setup_method(self, _):
         self.workdir = tempfile.mkdtemp(prefix="argparse-manpage-tests-")
         os.environ["PYTHON"] = sys.executable
+        os.environ["PYTHONPATH"] = os.getcwd()
 
     def teardown_method(self, _):
         shutil.rmtree(self.workdir)
 
     @staticmethod
     def _get_am_executable():
         testdir = os.path.dirname(__file__)
@@ -88,15 +120,15 @@
 
         cmd = [
             self._get_am_executable(),
             "--pyfile", tested_executable,
             "--function", "get_parser",
         ]
         output = subprocess.check_output(cmd).decode("utf-8")
-        assert output == SIMPLE_OUTPUT.format(name=expname,
+        assert output == SIMPLE_OUTPUT.format(name=expname, version="",
                                               NAME=expname.upper(), DATE=DATE)
 
     def test_filepath_prog(self):
         """
         Test --pyfile --function with prog explicitly specified in
         ArgumentParser name.
         """
@@ -109,15 +141,15 @@
         cmd = [
             self._get_am_executable(),
             "--pyfile", tested_executable,
             "--function", "get_parser",
         ]
         output = subprocess.check_output(cmd).decode("utf-8")
         name="progname"
-        assert output == SIMPLE_OUTPUT.format(name=expname,
+        assert output == SIMPLE_OUTPUT.format(name=expname, version="",
                                               NAME=expname.upper(), DATE=DATE)
 
     def test_full_args(self):
         """
         Submit as many commandline arguments as possible.
         """
         name = "full_name"
@@ -139,7 +171,33 @@
             "--long-description", "Some long description.",  # unused
             "--include", "tests/extra.man",
         ]
         output = subprocess.check_output(cmd).decode("utf-8")
         name="progname"
         assert output == FULL_OUTPUT.format(name=name, NAME=name.upper(),
                                             DATE=DATE)
+
+    def test_pyproject_toml(self):
+        """
+        Test that we can read information from pyproject.toml.
+        """
+        current_dir = os.getcwd()
+        with pushd(self.workdir):
+            with open("pyproject.toml", "w+") as script_fd:
+                script_fd.write(PYPROJECT_TOML_FILE_CONTENTS.format(gitdir=current_dir))
+            with open("setup.py", "w+") as script_fd:
+                script_fd.write(SETUP_PY_FILE_CONTENTS)
+
+            modname = "somefile"
+            name = r"some\-file"
+            os.mkdir(modname)
+            with open(os.path.join(modname, "__init__.py"), "w+") as script_fd:
+                script_fd.write(SIMPLE_FILE_CONTENTS.format(ap_arguments=""))
+
+            assert 0 == run_setup_py(["build"])
+            if version.parse(setuptools.__version__) >= version.parse("62.2.0"):
+                with open("some-file.1") as script_fd:
+                    output = script_fd.read()
+                    assert output == SIMPLE_OUTPUT.format(name=name, version=" 0.0.0",
+                                                          NAME=name.upper(), DATE=DATE)
+            else:
+                warnings.warn("setuptools >= 62.2.0 required to generate man pages with pyprojects.toml")
```

