# Comparing `tmp/labmate-0.6.0.tar.gz` & `tmp/labmate-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labmate-0.6.0.tar", last modified: Fri May 12 13:19:49 2023, max compression
+gzip compressed data, was "labmate-0.6.1.tar", last modified: Sun May 14 17:35:11 2023, max compression
```

## Comparing `labmate-0.6.0.tar` & `labmate-0.6.1.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-12 13:19:37.000000 labmate-0.6.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-12 13:19:37.000000 labmate-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-12 13:19:49.060316 labmate-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-12 13:19:37.000000 labmate-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.056316 labmate-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/acquisition_notebook.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.056316 labmate-0.6.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   112640 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/acquisition_and_analysis_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.056316 labmate-0.6.0/docs/examples/files/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/files/dummy_config1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/files/dummy_config2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/files/dummy_config3.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/files/init_analyse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.056316 labmate-0.6.0/docs/examples/more/
--rw-r--r--   0 runner    (1001) docker     (123)   111306 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/more/h5nparray.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/more/loop_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/smart_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/h5nparray.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.056316 labmate-0.6.0/docs/releases/
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/releases/0.4.0.md
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/releases/0.5.0.md
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/releases/0.6.0.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.056316 labmate-0.6.0/labmate/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/acquisition/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/acquisition_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/acquisition_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/acquisition_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/analysis_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/analysis_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/acquisition_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15313 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition_notebook/acquisition_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition_notebook/acquisition_magic_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/attrdict/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/attrdict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/attrdict/attrdict_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/json/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/json/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/json/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/json/open.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/json_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/path/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/path/path_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/plot_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/plot_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/plot_utils/random_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/plt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/syncdata/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/syncdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/syncdata/h5py_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/syncdata/syncdata_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/syncdata_types/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/syncdata_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/syncdata_types/h5_np_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/utils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/utils/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/utils/random_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-12 13:19:49.000000 labmate-0.6.0/labmate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-12 13:19:49.000000 labmate-0.6.0/labmate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:19:49.000000 labmate-0.6.0/labmate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 13:19:49.000000 labmate-0.6.0/labmate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 13:19:49.000000 labmate-0.6.0/labmate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 13:19:37.000000 labmate-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:19:49.060316 labmate-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-12 13:19:37.000000 labmate-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.763683 labmate-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-14 17:34:57.000000 labmate-0.6.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-14 17:34:57.000000 labmate-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-14 17:35:11.763683 labmate-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-14 17:34:57.000000 labmate-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.755683 labmate-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/acquisition_notebook.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   112640 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/acquisition_and_analysis_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/docs/examples/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/files/dummy_config1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/files/dummy_config2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/files/dummy_config3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/files/init_analyse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/docs/examples/more/
+-rw-r--r--   0 runner    (1001) docker     (123)   111306 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/more/h5nparray.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/more/loop_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/examples/smart_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/h5nparray.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/docs/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/releases/0.4.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/releases/0.5.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/releases/0.6.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-14 17:34:57.000000 labmate-0.6.1/docs/releases/0.6.1.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/acquisition_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/acquisition_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/acquisition_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/analysis_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/analysis_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/acquisition_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15313 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition_notebook/acquisition_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/acquisition_notebook/acquisition_magic_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/attrdict/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/attrdict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/attrdict/attrdict_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/json/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/json/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/json/open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/json_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/path/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/path/path_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/plot_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/plot_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/plot_utils/random_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/plt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/syncdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/syncdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/syncdata/h5py_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/syncdata/syncdata_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate/syncdata_types/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/syncdata_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/syncdata_types/h5_np_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.763683 labmate-0.6.1/labmate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/utils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/utils/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-14 17:34:57.000000 labmate-0.6.1/labmate/utils/random_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:35:11.759683 labmate-0.6.1/labmate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-14 17:35:11.000000 labmate-0.6.1/labmate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-14 17:35:11.000000 labmate-0.6.1/labmate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:35:11.000000 labmate-0.6.1/labmate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-14 17:35:11.000000 labmate-0.6.1/labmate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 17:35:11.000000 labmate-0.6.1/labmate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-14 17:34:57.000000 labmate-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 17:35:11.763683 labmate-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-14 17:34:57.000000 labmate-0.6.1/setup.py
```

### Comparing `labmate-0.6.0/LICENCE` & `labmate-0.6.1/LICENCE`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/docs/examples/acquisition_and_analysis_notebook.ipynb` & `labmate-0.6.1/docs/examples/acquisition_and_analysis_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/docs/examples/files/init_analyse.py` & `labmate-0.6.1/docs/examples/files/init_analyse.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb` & `labmate-0.6.1/docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/docs/examples/more/h5nparray.ipynb` & `labmate-0.6.1/docs/examples/more/h5nparray.ipynb`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/docs/examples/more/loop_example.ipynb` & `labmate-0.6.1/docs/examples/more/loop_example.ipynb`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/docs/h5nparray.md` & `labmate-0.6.1/docs/h5nparray.md`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/docs/releases/0.4.0.md` & `labmate-0.6.1/docs/releases/0.4.0.md`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/docs/releases/0.5.0.md` & `labmate-0.6.1/docs/releases/0.5.0.md`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/docs/releases/0.6.0.md` & `labmate-0.6.1/docs/releases/0.6.0.md`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/acquisition/acquisition_data.py` & `labmate-0.6.1/labmate/acquisition/acquisition_data.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/acquisition/acquisition_loop.py` & `labmate-0.6.1/labmate/acquisition/acquisition_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,19 @@
                                 self[key].shape)))
                     )
                     self[key][iteration] = value
                     # data = self.data[key]
                     # self.data[key] = np.zeros(shape)
                     # self.data[key][:, :data.shape[-1]] = data
             else:
-                self[key] = SyncNp(np.zeros(key_shape))
+                if isinstance(value, (complex, np.complex_)):  # type: ignore
+                    self[key] = SyncNp(np.zeros(key_shape, dtype=np.complex128))
+                else:
+                    self[key] = SyncNp(np.zeros(key_shape))
+
                 self[key][iteration] = value
 
     def iter(self, iterable: Iterable, level=None):
         if not hasattr(iterable, "__len__"):
             iterable = list(iterable)
 
         length = len(iterable)  # type: ignore
@@ -138,14 +142,18 @@
             if len(self._iteration)-1 > level:
                 self._iteration.pop()
             self._level -= 1
 
         return GenerToIter(
             loop_iter(iterable, level=level), length)
 
+    def enum(self, iterable: Iterable, level=None):
+        return enumerate(self.iter(
+            iterable=iterable, level=level))
+
 
 class AcquisitionLoopOld:
     """Acquisition loop allow to save data during for loops.
 
     - Example 1 that saves list of squares till 10:
     ```
     sd.test_loop = loop = AcquisitionLoop()
```

### Comparing `labmate-0.6.0/labmate/acquisition/acquisition_manager.py` & `labmate-0.6.1/labmate/acquisition/acquisition_manager.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/acquisition/analysis_data.py` & `labmate-0.6.1/labmate/acquisition/analysis_data.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/acquisition/analysis_loop.py` & `labmate-0.6.1/labmate/acquisition/analysis_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,16 @@
         for index in range(self._loop_shape[0]):
             child_kwds = {}
             for key, value in self._data.items():
                 if key[:1] == '_':
                     continue
 
                 # if not isinstance(value, Iterable) or isinstance(value, (str, bytes)):
-                if not hasattr(value, "__getitem__") or isinstance(value, (int, float)):
+                if not hasattr(value, "__getitem__") or \
+                        isinstance(value, (str, bytes, int, float)):
                     child_kwds[key] = value
                 elif len(value) == 1:
                     child_kwds[key] = value[0]
                 else:
                     child_kwds[key] = value[index]
 
                 val = child_kwds[key]
```

### Comparing `labmate-0.6.0/labmate/acquisition/lint.py` & `labmate-0.6.1/labmate/acquisition/lint.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/acquisition_notebook/acquisition_analysis_manager.py` & `labmate-0.6.1/labmate/acquisition_notebook/acquisition_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/acquisition_notebook/acquisition_magic_class.py` & `labmate-0.6.1/labmate/acquisition_notebook/acquisition_magic_class.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/json/decoders.py` & `labmate-0.6.1/labmate/json/decoders.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/json/open.py` & `labmate-0.6.1/labmate/json/open.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/json_utils.py` & `labmate-0.6.1/labmate/json_utils.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/path/path_class.py` & `labmate-0.6.1/labmate/path/path_class.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/plt.py` & `labmate-0.6.1/labmate/plt.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/syncdata/h5py_utils.py` & `labmate-0.6.1/labmate/syncdata/h5py_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,24 +70,39 @@
     if isinstance(data, dict):
         for key, value in data.items():
             data[key] = transform_to_possible_formats(value)
         return data
     if isinstance(data, (tuple, set)):
         data = list(data)
     if isinstance(data, list):
-        return np.array(data)
+        data_array = np.array(data)
+        if 'U' in str(data_array.dtype) or \
+                'object' in str(data_array.dtype):
+            return data
+        return data_array
     return data
 
 
 def transform_on_open(value):
     if isinstance(value, bytes):
-        return value.decode()
+        value = value.decode()
+    if isinstance(value, str) and value.startswith('__json__'):
+        return json.loads(value[8:])
+
     return value
 
 
+def transform_list_on_save(value):
+    value_np = np.array(value)
+    if 'U' in str(value_np.dtype) or \
+            'object' in str(value_np.dtype):
+        return '__json__' + json.dumps(value)
+    return value_np
+
+
 def save_sub_dict(
     group: Union[h5py.File, h5py.Group],
     data: Union[dict, list, np.ndarray, ClassWithAsdict],
     key: str,
     use_compression: Optional[Union[Literal[True], str]] = None
 ):
     if hasattr(data, 'asdict'):
@@ -97,14 +112,15 @@
     if isinstance(data, dict):
         g = group.create_group(key)
         for k, v in data.items():
             save_sub_dict(g, v, k, use_compression=use_compression)
     elif (key is not None) and (data is not None):
         if isinstance(data, (np.ndarray, list)):
             use_compression = "gzip" if use_compression is True else use_compression
+            data = transform_list_on_save(data)  # type: ignore
             group.create_dataset(key, data=data, compression=use_compression)  # compression="gzip"
         else:
             group.create_dataset(key, data=data)
 
 
 def save_dict(
     filename: str,
@@ -210,16 +226,16 @@
             else:
                 structure[k] = "variable of type dict"
 
         elif isinstance(v, (np.ndarray, list)):
             structure[k] = f"shape: {np.shape(v)} (type: {type(v).__name__})"
         elif isinstance(v, (int, np.int_)):  # type: ignore
             structure[k] = f"{v:.0f} (type : {type(v).__name__})"
-        elif isinstance(v, (float, np.float_)):  # type: ignore
-            str_value = f"{v:.3f}" if .1 <= v <= 100. else f"{v:.3e}"
+        elif isinstance(v, (float, np.float_, complex, np.complex_)):  # type: ignore
+            str_value = f"{v:.3f}" if .1 <= abs(v) <= 100. else f"{v:.3e}"
             structure[k] = f"{str_value} (type : {type(v).__name__})"
         else:
             structure[k] = f"variable of type {type(v).__name__}"
     return structure
 
 
 def get_keys_structure(data) -> dict:
```

### Comparing `labmate-0.6.0/labmate/syncdata/syncdata_class.py` & `labmate-0.6.1/labmate/syncdata/syncdata_class.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/syncdata_types/h5_np_array.py` & `labmate-0.6.1/labmate/syncdata_types/h5_np_array.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/utils/parse.py` & `labmate-0.6.1/labmate/utils/parse.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate/utils/random_utils.py` & `labmate-0.6.1/labmate/utils/random_utils.py`

 * *Files identical despite different names*

### Comparing `labmate-0.6.0/labmate.egg-info/SOURCES.txt` & `labmate-0.6.1/labmate.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 docs/examples/files/init_analyse.py
 docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb
 docs/examples/more/h5nparray.ipynb
 docs/examples/more/loop_example.ipynb
 docs/releases/0.4.0.md
 docs/releases/0.5.0.md
 docs/releases/0.6.0.md
+docs/releases/0.6.1.md
 labmate/__init__.py
 labmate/json_utils.py
 labmate/plt.py
 labmate.egg-info/PKG-INFO
 labmate.egg-info/SOURCES.txt
 labmate.egg-info/dependency_links.txt
 labmate.egg-info/requires.txt
```

### Comparing `labmate-0.6.0/setup.py` & `labmate-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='labmate',
-    version="0.6.0",
+    version="0.6.1",
     author="LKB-OMQ",
     author_email="cryo.paris.su@gmail.com",
     description="Data management library to save data and plots to hdf5 files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kyrylo-gr/labmate",
     packages=setuptools.find_packages(exclude=['tests', 'tests.*']),
```

