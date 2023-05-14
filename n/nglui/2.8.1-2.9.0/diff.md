# Comparing `tmp/nglui-2.8.1.tar.gz` & `tmp/nglui-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nglui-2.8.1.tar", last modified: Sat Jan 22 00:23:55 2022, max compression
+gzip compressed data, was "nglui-2.9.0.tar", last modified: Mon Jan 24 16:34:24 2022, max compression
```

## Comparing `nglui-2.8.1.tar` & `nglui-2.9.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-22 00:23:55.682959 nglui-2.8.1/
--rw-r--r--   0 caseys     (502) staff       (20)      105 2022-01-22 00:23:43.000000 nglui-2.8.1/.bumpversion.cfg
--rw-r--r--   0 caseys     (502) staff       (20)     1268 2020-07-18 02:30:34.000000 nglui-2.8.1/.gitignore
--rw-r--r--   0 caseys     (502) staff       (20)      246 2020-07-18 02:30:34.000000 nglui-2.8.1/.travis.yaml
--rw-r--r--   0 caseys     (502) staff       (20)     5970 2021-06-14 07:51:38.000000 nglui-2.8.1/CHANGELOG.md
--rw-r--r--   0 caseys     (502) staff       (20)      561 2020-07-18 02:30:34.000000 nglui-2.8.1/Dockerfile
--rw-r--r--   0 caseys     (502) staff       (20)    11356 2020-07-18 02:30:34.000000 nglui-2.8.1/LICENSE.license
--rw-r--r--   0 caseys     (502) staff       (20)       73 2020-07-18 02:30:34.000000 nglui-2.8.1/MANIFEST.in
--rw-r--r--   0 caseys     (502) staff       (20)     1830 2022-01-22 00:23:55.683481 nglui-2.8.1/PKG-INFO
--rw-r--r--   0 caseys     (502) staff       (20)     1440 2020-07-18 02:30:34.000000 nglui-2.8.1/README.md
--rw-r--r--   0 caseys     (502) staff       (20)      540 2020-07-18 02:30:34.000000 nglui-2.8.1/cloudbuild.yaml
-drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-22 00:23:55.651649 nglui-2.8.1/examples/
--rw-r--r--   0 caseys     (502) staff       (20)  1130416 2020-07-18 02:30:34.000000 nglui-2.8.1/examples/dash_example_data.h5
--rw-r--r--   0 caseys     (502) staff       (20)     1867 2020-07-18 02:30:34.000000 nglui-2.8.1/examples/dash_with_statebuilder.py
--rw-r--r--   0 caseys     (502) staff       (20)  3747792 2020-07-18 02:30:34.000000 nglui-2.8.1/examples/example_data.h5
--rw-r--r--   0 caseys     (502) staff       (20)    27274 2020-07-18 02:30:34.000000 nglui-2.8.1/examples/statebuilder_examples.ipynb
--rw-r--r--   0 caseys     (502) staff       (20)       40 2021-01-15 19:39:08.000000 nglui-2.8.1/requirements.txt
--rw-r--r--   0 caseys     (502) staff       (20)      126 2022-01-22 00:23:55.685560 nglui-2.8.1/setup.cfg
--rw-r--r--   0 caseys     (502) staff       (20)     1406 2020-07-18 02:30:34.000000 nglui-2.8.1/setup.py
-drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-22 00:23:55.621185 nglui-2.8.1/src/
-drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-22 00:23:55.655792 nglui-2.8.1/src/nglui/
--rw-r--r--   0 caseys     (502) staff       (20)      144 2022-01-22 00:23:43.000000 nglui-2.8.1/src/nglui/__init__.py
-drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-22 00:23:55.660576 nglui-2.8.1/src/nglui/easyviewer/
--rw-r--r--   0 caseys     (502) staff       (20)       54 2021-07-02 16:38:58.000000 nglui-2.8.1/src/nglui/easyviewer/__init__.py
--rw-r--r--   0 caseys     (502) staff       (20)     4898 2021-12-17 22:22:48.000000 nglui-2.8.1/src/nglui/easyviewer/annotation.py
--rw-r--r--   0 caseys     (502) staff       (20)    21123 2022-01-18 02:15:42.000000 nglui-2.8.1/src/nglui/easyviewer/base.py
--rw-r--r--   0 caseys     (502) staff       (20)      500 2022-01-18 02:15:42.000000 nglui-2.8.1/src/nglui/easyviewer/utils.py
-drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-22 00:23:55.665991 nglui-2.8.1/src/nglui/nglite/
--rw-r--r--   0 caseys     (502) staff       (20)      884 2020-07-18 02:30:34.000000 nglui-2.8.1/src/nglui/nglite/__init__.py
--rw-r--r--   0 caseys     (502) staff       (20)     6226 2020-07-18 02:30:34.000000 nglui-2.8.1/src/nglui/nglite/equivalence_map.py
--rw-r--r--   0 caseys     (502) staff       (20)     1623 2021-06-11 21:45:42.000000 nglui-2.8.1/src/nglui/nglite/json_utils.py
--rw-r--r--   0 caseys     (502) staff       (20)     9861 2021-06-11 21:45:42.000000 nglui-2.8.1/src/nglui/nglite/json_wrappers.py
--rw-r--r--   0 caseys     (502) staff       (20)      753 2020-07-18 02:30:34.000000 nglui-2.8.1/src/nglui/nglite/random_token.py
--rw-r--r--   0 caseys     (502) staff       (20)     2958 2021-06-11 21:45:42.000000 nglui-2.8.1/src/nglui/nglite/skeleton.py
--rw-r--r--   0 caseys     (502) staff       (20)     4758 2021-06-11 21:45:42.000000 nglui-2.8.1/src/nglui/nglite/trackable_state.py
--rw-r--r--   0 caseys     (502) staff       (20)     3944 2021-06-11 21:45:42.000000 nglui-2.8.1/src/nglui/nglite/url_state.py
--rw-r--r--   0 caseys     (502) staff       (20)     1574 2021-06-11 21:45:42.000000 nglui-2.8.1/src/nglui/nglite/viewer.py
--rw-r--r--   0 caseys     (502) staff       (20)     6920 2021-06-11 21:45:42.000000 nglui-2.8.1/src/nglui/nglite/viewer_base.py
--rw-r--r--   0 caseys     (502) staff       (20)     6866 2021-06-11 21:45:42.000000 nglui-2.8.1/src/nglui/nglite/viewer_config_state.py
--rw-r--r--   0 caseys     (502) staff       (20)    30192 2021-06-11 22:28:05.000000 nglui-2.8.1/src/nglui/nglite/viewer_state.py
-drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-22 00:23:55.666881 nglui-2.8.1/src/nglui/nglite_compatibility/
--rw-r--r--   0 caseys     (502) staff       (20)      350 2022-01-18 02:15:42.000000 nglui-2.8.1/src/nglui/nglite_compatibility/__init__.py
--rw-r--r--   0 caseys     (502) staff       (20)     1961 2022-01-18 02:15:42.000000 nglui-2.8.1/src/nglui/nglite_compatibility/annotation_compatibility.py
-drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-22 00:23:55.668578 nglui-2.8.1/src/nglui/parser/
--rw-r--r--   0 caseys     (502) staff       (20)       20 2020-09-04 19:01:36.000000 nglui-2.8.1/src/nglui/parser/__init__.py
--rw-r--r--   0 caseys     (502) staff       (20)    13683 2021-06-11 21:45:42.000000 nglui-2.8.1/src/nglui/parser/base.py
-drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-22 00:23:55.672505 nglui-2.8.1/src/nglui/statebuilder/
--rw-r--r--   0 caseys     (502) staff       (20)      320 2021-06-11 22:16:54.000000 nglui-2.8.1/src/nglui/statebuilder/__init__.py
--rw-r--r--   0 caseys     (502) staff       (20)     1574 2021-06-11 22:16:55.000000 nglui-2.8.1/src/nglui/statebuilder/helpers.py
--rw-r--r--   0 caseys     (502) staff       (20)    13816 2022-01-22 00:19:34.000000 nglui-2.8.1/src/nglui/statebuilder/layers.py
--rw-r--r--   0 caseys     (502) staff       (20)    24137 2022-01-21 23:16:12.000000 nglui-2.8.1/src/nglui/statebuilder/mappers.py
--rw-r--r--   0 caseys     (502) staff       (20)     8157 2022-01-18 02:15:42.000000 nglui-2.8.1/src/nglui/statebuilder/statebuilder.py
--rw-r--r--   0 caseys     (502) staff       (20)     1291 2021-06-11 22:17:02.000000 nglui-2.8.1/src/nglui/statebuilder/utils.py
-drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-22 00:23:55.658296 nglui-2.8.1/src/nglui.egg-info/
--rw-r--r--   0 caseys     (502) staff       (20)     1830 2022-01-22 00:23:55.000000 nglui-2.8.1/src/nglui.egg-info/PKG-INFO
--rw-r--r--   0 caseys     (502) staff       (20)     1515 2022-01-22 00:23:55.000000 nglui-2.8.1/src/nglui.egg-info/SOURCES.txt
--rw-r--r--   0 caseys     (502) staff       (20)        1 2022-01-22 00:23:55.000000 nglui-2.8.1/src/nglui.egg-info/dependency_links.txt
--rw-r--r--   0 caseys     (502) staff       (20)       40 2022-01-22 00:23:55.000000 nglui-2.8.1/src/nglui.egg-info/requires.txt
--rw-r--r--   0 caseys     (502) staff       (20)        6 2022-01-22 00:23:55.000000 nglui-2.8.1/src/nglui.egg-info/top_level.txt
--rw-r--r--   0 caseys     (502) staff       (20)      124 2021-01-15 19:48:51.000000 nglui-2.8.1/test_requirements.txt
-drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-22 00:23:55.676034 nglui-2.8.1/tests/
--rw-r--r--   0 caseys     (502) staff       (20)     1936 2022-01-18 02:15:42.000000 nglui-2.8.1/tests/conftest.py
--rw-r--r--   0 caseys     (502) staff       (20)     1423 2020-09-04 19:01:36.000000 nglui-2.8.1/tests/test_parser.py
--rw-r--r--   0 caseys     (502) staff       (20)     8282 2022-01-18 02:15:42.000000 nglui-2.8.1/tests/test_statebuilder.py
--rw-r--r--   0 caseys     (502) staff       (20)     2891 2022-01-18 02:15:42.000000 nglui-2.8.1/tests/test_viewer.py
-drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-22 00:23:55.682552 nglui-2.8.1/tests/testdata/
--rw-r--r--   0 caseys     (502) staff       (20)  3747792 2020-07-18 02:30:34.000000 nglui-2.8.1/tests/testdata/test_data.h5
--rw-r--r--   0 caseys     (502) staff       (20)     3784 2020-09-04 19:01:36.000000 nglui-2.8.1/tests/testdata/test_state.json
+drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-24 16:34:24.991964 nglui-2.9.0/
+-rw-r--r--   0 caseys     (502) staff       (20)      105 2022-01-24 16:34:14.000000 nglui-2.9.0/.bumpversion.cfg
+-rw-r--r--   0 caseys     (502) staff       (20)     1268 2020-07-18 02:30:34.000000 nglui-2.9.0/.gitignore
+-rw-r--r--   0 caseys     (502) staff       (20)      246 2020-07-18 02:30:34.000000 nglui-2.9.0/.travis.yaml
+-rw-r--r--   0 caseys     (502) staff       (20)     5970 2021-06-14 07:51:38.000000 nglui-2.9.0/CHANGELOG.md
+-rw-r--r--   0 caseys     (502) staff       (20)      561 2020-07-18 02:30:34.000000 nglui-2.9.0/Dockerfile
+-rw-r--r--   0 caseys     (502) staff       (20)    11356 2020-07-18 02:30:34.000000 nglui-2.9.0/LICENSE.license
+-rw-r--r--   0 caseys     (502) staff       (20)       73 2020-07-18 02:30:34.000000 nglui-2.9.0/MANIFEST.in
+-rw-r--r--   0 caseys     (502) staff       (20)     1830 2022-01-24 16:34:24.992177 nglui-2.9.0/PKG-INFO
+-rw-r--r--   0 caseys     (502) staff       (20)     1440 2020-07-18 02:30:34.000000 nglui-2.9.0/README.md
+-rw-r--r--   0 caseys     (502) staff       (20)      540 2020-07-18 02:30:34.000000 nglui-2.9.0/cloudbuild.yaml
+drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-24 16:34:24.940025 nglui-2.9.0/examples/
+-rw-r--r--   0 caseys     (502) staff       (20)  1130416 2020-07-18 02:30:34.000000 nglui-2.9.0/examples/dash_example_data.h5
+-rw-r--r--   0 caseys     (502) staff       (20)     1867 2020-07-18 02:30:34.000000 nglui-2.9.0/examples/dash_with_statebuilder.py
+-rw-r--r--   0 caseys     (502) staff       (20)  3747792 2020-07-18 02:30:34.000000 nglui-2.9.0/examples/example_data.h5
+-rw-r--r--   0 caseys     (502) staff       (20)    27274 2020-07-18 02:30:34.000000 nglui-2.9.0/examples/statebuilder_examples.ipynb
+-rw-r--r--   0 caseys     (502) staff       (20)       40 2021-01-15 19:39:08.000000 nglui-2.9.0/requirements.txt
+-rw-r--r--   0 caseys     (502) staff       (20)      126 2022-01-24 16:34:24.993272 nglui-2.9.0/setup.cfg
+-rw-r--r--   0 caseys     (502) staff       (20)     1406 2020-07-18 02:30:34.000000 nglui-2.9.0/setup.py
+drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-24 16:34:24.907062 nglui-2.9.0/src/
+drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-24 16:34:24.943810 nglui-2.9.0/src/nglui/
+-rw-r--r--   0 caseys     (502) staff       (20)      144 2022-01-24 16:34:14.000000 nglui-2.9.0/src/nglui/__init__.py
+drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-24 16:34:24.952565 nglui-2.9.0/src/nglui/easyviewer/
+-rw-r--r--   0 caseys     (502) staff       (20)       54 2021-07-02 16:38:58.000000 nglui-2.9.0/src/nglui/easyviewer/__init__.py
+-rw-r--r--   0 caseys     (502) staff       (20)     4937 2022-01-24 16:18:02.000000 nglui-2.9.0/src/nglui/easyviewer/annotation.py
+-rw-r--r--   0 caseys     (502) staff       (20)    21123 2022-01-18 02:15:42.000000 nglui-2.9.0/src/nglui/easyviewer/base.py
+-rw-r--r--   0 caseys     (502) staff       (20)      500 2022-01-18 02:15:42.000000 nglui-2.9.0/src/nglui/easyviewer/utils.py
+drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-24 16:34:24.965969 nglui-2.9.0/src/nglui/nglite/
+-rw-r--r--   0 caseys     (502) staff       (20)      884 2020-07-18 02:30:34.000000 nglui-2.9.0/src/nglui/nglite/__init__.py
+-rw-r--r--   0 caseys     (502) staff       (20)     6226 2020-07-18 02:30:34.000000 nglui-2.9.0/src/nglui/nglite/equivalence_map.py
+-rw-r--r--   0 caseys     (502) staff       (20)     1623 2021-06-11 21:45:42.000000 nglui-2.9.0/src/nglui/nglite/json_utils.py
+-rw-r--r--   0 caseys     (502) staff       (20)     9861 2021-06-11 21:45:42.000000 nglui-2.9.0/src/nglui/nglite/json_wrappers.py
+-rw-r--r--   0 caseys     (502) staff       (20)      753 2020-07-18 02:30:34.000000 nglui-2.9.0/src/nglui/nglite/random_token.py
+-rw-r--r--   0 caseys     (502) staff       (20)     2958 2021-06-11 21:45:42.000000 nglui-2.9.0/src/nglui/nglite/skeleton.py
+-rw-r--r--   0 caseys     (502) staff       (20)     4758 2021-06-11 21:45:42.000000 nglui-2.9.0/src/nglui/nglite/trackable_state.py
+-rw-r--r--   0 caseys     (502) staff       (20)     3944 2021-06-11 21:45:42.000000 nglui-2.9.0/src/nglui/nglite/url_state.py
+-rw-r--r--   0 caseys     (502) staff       (20)     1574 2021-06-11 21:45:42.000000 nglui-2.9.0/src/nglui/nglite/viewer.py
+-rw-r--r--   0 caseys     (502) staff       (20)     6920 2021-06-11 21:45:42.000000 nglui-2.9.0/src/nglui/nglite/viewer_base.py
+-rw-r--r--   0 caseys     (502) staff       (20)     6866 2021-06-11 21:45:42.000000 nglui-2.9.0/src/nglui/nglite/viewer_config_state.py
+-rw-r--r--   0 caseys     (502) staff       (20)    30192 2021-06-11 22:28:05.000000 nglui-2.9.0/src/nglui/nglite/viewer_state.py
+drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-24 16:34:24.968235 nglui-2.9.0/src/nglui/nglite_compatibility/
+-rw-r--r--   0 caseys     (502) staff       (20)      350 2022-01-18 02:15:42.000000 nglui-2.9.0/src/nglui/nglite_compatibility/__init__.py
+-rw-r--r--   0 caseys     (502) staff       (20)     1961 2022-01-18 02:15:42.000000 nglui-2.9.0/src/nglui/nglite_compatibility/annotation_compatibility.py
+drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-24 16:34:24.970107 nglui-2.9.0/src/nglui/parser/
+-rw-r--r--   0 caseys     (502) staff       (20)       20 2020-09-04 19:01:36.000000 nglui-2.9.0/src/nglui/parser/__init__.py
+-rw-r--r--   0 caseys     (502) staff       (20)    13683 2021-06-11 21:45:42.000000 nglui-2.9.0/src/nglui/parser/base.py
+drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-24 16:34:24.975390 nglui-2.9.0/src/nglui/statebuilder/
+-rw-r--r--   0 caseys     (502) staff       (20)      320 2021-06-11 22:16:54.000000 nglui-2.9.0/src/nglui/statebuilder/__init__.py
+-rw-r--r--   0 caseys     (502) staff       (20)     1574 2021-06-11 22:16:55.000000 nglui-2.9.0/src/nglui/statebuilder/helpers.py
+-rw-r--r--   0 caseys     (502) staff       (20)    13816 2022-01-22 00:19:34.000000 nglui-2.9.0/src/nglui/statebuilder/layers.py
+-rw-r--r--   0 caseys     (502) staff       (20)    24668 2022-01-24 16:31:47.000000 nglui-2.9.0/src/nglui/statebuilder/mappers.py
+-rw-r--r--   0 caseys     (502) staff       (20)     8157 2022-01-18 02:15:42.000000 nglui-2.9.0/src/nglui/statebuilder/statebuilder.py
+-rw-r--r--   0 caseys     (502) staff       (20)     1291 2021-06-11 22:17:02.000000 nglui-2.9.0/src/nglui/statebuilder/utils.py
+drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-24 16:34:24.947692 nglui-2.9.0/src/nglui.egg-info/
+-rw-r--r--   0 caseys     (502) staff       (20)     1830 2022-01-24 16:34:24.000000 nglui-2.9.0/src/nglui.egg-info/PKG-INFO
+-rw-r--r--   0 caseys     (502) staff       (20)     1515 2022-01-24 16:34:24.000000 nglui-2.9.0/src/nglui.egg-info/SOURCES.txt
+-rw-r--r--   0 caseys     (502) staff       (20)        1 2022-01-24 16:34:24.000000 nglui-2.9.0/src/nglui.egg-info/dependency_links.txt
+-rw-r--r--   0 caseys     (502) staff       (20)       40 2022-01-24 16:34:24.000000 nglui-2.9.0/src/nglui.egg-info/requires.txt
+-rw-r--r--   0 caseys     (502) staff       (20)        6 2022-01-24 16:34:24.000000 nglui-2.9.0/src/nglui.egg-info/top_level.txt
+-rw-r--r--   0 caseys     (502) staff       (20)      124 2021-01-15 19:48:51.000000 nglui-2.9.0/test_requirements.txt
+drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-24 16:34:24.979668 nglui-2.9.0/tests/
+-rw-r--r--   0 caseys     (502) staff       (20)     1936 2022-01-18 02:15:42.000000 nglui-2.9.0/tests/conftest.py
+-rw-r--r--   0 caseys     (502) staff       (20)     1423 2020-09-04 19:01:36.000000 nglui-2.9.0/tests/test_parser.py
+-rw-r--r--   0 caseys     (502) staff       (20)     8282 2022-01-18 02:15:42.000000 nglui-2.9.0/tests/test_statebuilder.py
+-rw-r--r--   0 caseys     (502) staff       (20)     2891 2022-01-18 02:15:42.000000 nglui-2.9.0/tests/test_viewer.py
+drwxr-xr-x   0 caseys     (502) staff       (20)        0 2022-01-24 16:34:24.990782 nglui-2.9.0/tests/testdata/
+-rw-r--r--   0 caseys     (502) staff       (20)  3747792 2020-07-18 02:30:34.000000 nglui-2.9.0/tests/testdata/test_data.h5
+-rw-r--r--   0 caseys     (502) staff       (20)     3784 2020-09-04 19:01:36.000000 nglui-2.9.0/tests/testdata/test_state.json
```

### Comparing `nglui-2.8.1/.gitignore` & `nglui-2.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/CHANGELOG.md` & `nglui-2.9.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/Dockerfile` & `nglui-2.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/LICENSE.license` & `nglui-2.9.0/LICENSE.license`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/PKG-INFO` & `nglui-2.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nglui
-Version: 2.8.1
+Version: 2.9.0
 Summary: Framework for data-driven generation of neuroglancer states.
 Home-page: https://github.com/seung-lab/NeuroglancerAnnotationUI
 Author: Derrick Brittain, Casey Schneider-Mizell, Forrest Collman
 Author-email: caseysm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `nglui-2.8.1/README.md` & `nglui-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/cloudbuild.yaml` & `nglui-2.9.0/cloudbuild.yaml`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/examples/dash_example_data.h5` & `nglui-2.9.0/examples/dash_example_data.h5`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/examples/dash_with_statebuilder.py` & `nglui-2.9.0/examples/dash_with_statebuilder.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/examples/example_data.h5` & `nglui-2.9.0/examples/example_data.h5`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/examples/statebuilder_examples.ipynb` & `nglui-2.9.0/examples/statebuilder_examples.ipynb`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/setup.py` & `nglui-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/easyviewer/annotation.py` & `nglui-2.9.0/src/nglui/easyviewer/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
 def group_annotations(
     annotations,
     source=None,
     id=None,
     return_all=True,
     gather_linked_segmentations=True,
     share_linked_segmentations=False,
+    children_visible=True,
 ):
     if len(annotations) == 0:
         return []
     if id is None:
         id = random_token.make_random_token()
     if source is None:
         if annotations[0].type == "point":
@@ -161,15 +162,15 @@
         linked_segs = []
 
     collection_anno = CollectionAnnotation(
         source=source,
         entries=entries,
         id=id,
         segments=omit_nones(seg_in_group),
-        children_visible=True,
+        children_visible=children_visible,
     )
 
     for anno in annotations:
         anno.parent_id = collection_anno.id
         if share_linked_segmentations:
             anno.segments = seg_in_group
     if return_all:
```

### Comparing `nglui-2.8.1/src/nglui/easyviewer/base.py` & `nglui-2.9.0/src/nglui/easyviewer/base.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite/__init__.py` & `nglui-2.9.0/src/nglui/nglite/__init__.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite/equivalence_map.py` & `nglui-2.9.0/src/nglui/nglite/equivalence_map.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite/json_utils.py` & `nglui-2.9.0/src/nglui/nglite/json_utils.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite/json_wrappers.py` & `nglui-2.9.0/src/nglui/nglite/json_wrappers.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite/random_token.py` & `nglui-2.9.0/src/nglui/nglite/random_token.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite/skeleton.py` & `nglui-2.9.0/src/nglui/nglite/skeleton.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite/trackable_state.py` & `nglui-2.9.0/src/nglui/nglite/trackable_state.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite/url_state.py` & `nglui-2.9.0/src/nglui/nglite/url_state.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite/viewer.py` & `nglui-2.9.0/src/nglui/nglite/viewer.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite/viewer_base.py` & `nglui-2.9.0/src/nglui/nglite/viewer_base.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite/viewer_config_state.py` & `nglui-2.9.0/src/nglui/nglite/viewer_config_state.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite/viewer_state.py` & `nglui-2.9.0/src/nglui/nglite/viewer_state.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/nglite_compatibility/annotation_compatibility.py` & `nglui-2.9.0/src/nglui/nglite_compatibility/annotation_compatibility.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/parser/base.py` & `nglui-2.9.0/src/nglui/parser/base.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/statebuilder/helpers.py` & `nglui-2.9.0/src/nglui/statebuilder/helpers.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/statebuilder/layers.py` & `nglui-2.9.0/src/nglui/statebuilder/layers.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/statebuilder/mappers.py` & `nglui-2.9.0/src/nglui/statebuilder/mappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,28 +111,30 @@
         linked_segmentation_column,
         tag_column,
         group_column,
         set_position,
         gather_linked_segmentations,
         share_linked_segmentations,
         multipoint,
+        collapse_groups,
     ):
 
         self._config = dict(
             type=type,
             data_columns=data_columns,
             array_data=False,
             description_column=description_column,
             linked_segmentation_column=linked_segmentation_column,
             tag_column=tag_column,
             group_column=group_column,
             set_position=set_position,
             gather_linked_segmentations=gather_linked_segmentations,
             share_linked_segmentations=share_linked_segmentations,
             multipoint=multipoint,
+            collapse_groups=collapse_groups,
         )
         self._tag_map = None
 
     @property
     def type(self):
         return self._config.get("type", None)
 
@@ -168,14 +170,18 @@
     def set_position(self):
         return self._config.get("set_position", False)
 
     @property
     def multipoint(self):
         return self._config.get("multipoint", False)
 
+    @property
+    def collapse_groups(self):
+        return self._config.get("collapse_groups", False)
+
     def multipoint_reshape(self, data, pt_columns, squeeze_cols=[]):
         if data is None or len(data) == 0:
             return data
         else:
             rows = data.apply(
                 lambda x: _multipoint_transform(
                     x, pt_columns=pt_columns, squeeze_cols=squeeze_cols
@@ -257,14 +263,15 @@
             anno_to_group = [annos[jj] for jj in np.flatnonzero(inverse == ii)]
             group_annos.append(
                 annotation.group_annotations(
                     anno_to_group,
                     return_all=False,
                     gather_linked_segmentations=self.gather_linked_segmentations,
                     share_linked_segmentations=self.share_linked_segmentations,
+                    children_visible=not self.collapse_groups,
                 )
             )
         annos.extend(group_annos)
         return annos
 
     def _get_position(self, data, data_resolution=None, viewer_resolution=None):
         if len(data) > 0 and self.set_position is True:
@@ -310,26 +317,28 @@
         linked_segmentation_column=None,
         tag_column=None,
         group_column=None,
         gather_linked_segmentations=True,
         share_linked_segmentations=False,
         set_position=False,
         multipoint=False,
+        collapse_groups=False,
     ):
         super(PointMapper, self).__init__(
             type="point",
             data_columns=[point_column],
             description_column=description_column,
             linked_segmentation_column=linked_segmentation_column,
             tag_column=tag_column,
             group_column=group_column,
             gather_linked_segmentations=gather_linked_segmentations,
             share_linked_segmentations=share_linked_segmentations,
             set_position=set_position,
             multipoint=multipoint,
+            collapse_groups=collapse_groups,
         )
 
     def _default_array_data_columns(self):
         return ["pt"]
 
     def _render_data(self, data, data_resolution, viewer_resolution):
         if self.array_data:
@@ -395,26 +404,28 @@
         linked_segmentation_column=None,
         tag_column=None,
         group_column=None,
         gather_linked_segmentations=True,
         share_linked_segmentations=False,
         set_position=False,
         multipoint=False,
+        collapse_groups=False,
     ):
         super(LineMapper, self).__init__(
             type="line",
             data_columns=[point_column_a, point_column_b],
             description_column=description_column,
             linked_segmentation_column=linked_segmentation_column,
             tag_column=tag_column,
             group_column=group_column,
             gather_linked_segmentations=gather_linked_segmentations,
             share_linked_segmentations=share_linked_segmentations,
             set_position=set_position,
             multipoint=multipoint,
+            collapse_groups=collapse_groups,
         )
 
     def _default_array_data_columns(self):
         return ["pt_a", "pt_b"]
 
     def _render_data(self, data, data_resolution, viewer_resolution):
         if self.array_data:
@@ -482,26 +493,28 @@
         tag_column=None,
         group_column=None,
         gather_linked_segmentations=True,
         share_linked_segmentations=False,
         z_multiplier=0.1,
         set_position=False,
         multipoint=False,
+        collapse_groups=False,
     ):
         super(SphereMapper, self).__init__(
             type="sphere",
             data_columns=[center_column, radius_column],
             description_column=description_column,
             linked_segmentation_column=linked_segmentation_column,
             tag_column=tag_column,
             group_column=group_column,
             gather_linked_segmentations=gather_linked_segmentations,
             share_linked_segmentations=share_linked_segmentations,
             set_position=set_position,
             multipoint=multipoint,
+            collapse_groups=collapse_groups,
         )
         self._z_multiplier = z_multiplier
 
     def _default_array_data_columns(self):
         return ["ctr_pt", "rad"]
 
     def _render_data(self, data, data_resolution, viewer_resolution):
@@ -556,26 +569,28 @@
         linked_segmentation_column=None,
         tag_column=None,
         group_column=None,
         gather_linked_segmentations=True,
         share_linked_segmentations=False,
         set_position=False,
         multipoint=False,
+        collapse_groups=False,
     ):
         super(BoundingBoxMapper, self).__init__(
             type="axis_aligned_bounding_box",
             data_columns=[point_column_a, point_column_b],
             description_column=description_column,
             linked_segmentation_column=linked_segmentation_column,
             tag_column=tag_column,
             group_column=group_column,
             gather_linked_segmentations=gather_linked_segmentations,
             share_linked_segmentations=share_linked_segmentations,
             set_position=set_position,
             multipoint=multipoint,
+            collapse_groups=False,
         )
 
     def _default_array_data_columns(self):
         return ["pt_a", "pt_b"]
 
     def _render_data(self, data, data_resolution, viewer_resolution):
```

### Comparing `nglui-2.8.1/src/nglui/statebuilder/statebuilder.py` & `nglui-2.9.0/src/nglui/statebuilder/statebuilder.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui/statebuilder/utils.py` & `nglui-2.9.0/src/nglui/statebuilder/utils.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/src/nglui.egg-info/PKG-INFO` & `nglui-2.9.0/src/nglui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nglui
-Version: 2.8.1
+Version: 2.9.0
 Summary: Framework for data-driven generation of neuroglancer states.
 Home-page: https://github.com/seung-lab/NeuroglancerAnnotationUI
 Author: Derrick Brittain, Casey Schneider-Mizell, Forrest Collman
 Author-email: caseysm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `nglui-2.8.1/src/nglui.egg-info/SOURCES.txt` & `nglui-2.9.0/src/nglui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/tests/conftest.py` & `nglui-2.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/tests/test_parser.py` & `nglui-2.9.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/tests/test_statebuilder.py` & `nglui-2.9.0/tests/test_statebuilder.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/tests/test_viewer.py` & `nglui-2.9.0/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/tests/testdata/test_data.h5` & `nglui-2.9.0/tests/testdata/test_data.h5`

 * *Files identical despite different names*

### Comparing `nglui-2.8.1/tests/testdata/test_state.json` & `nglui-2.9.0/tests/testdata/test_state.json`

 * *Files identical despite different names*

