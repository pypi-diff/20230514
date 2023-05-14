# Comparing `tmp/cellpy-1.0.0a7.tar.gz` & `tmp/cellpy-1.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellpy-1.0.0a7.tar", last modified: Sun May 14 16:53:21 2023, max compression
+gzip compressed data, was "cellpy-1.0.0a8.tar", last modified: Sun May 14 17:53:18 2023, max compression
```

## Comparing `cellpy-1.0.0a7.tar` & `cellpy-1.0.0a8.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.172419 cellpy-1.0.0a7/
--rw-rw-rw-   0        0        0      503 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/AUTHORS.rst
--rw-rw-rw-   0        0        0     3086 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     3908 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-1.0.0a7/LICENSE
--rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-1.0.0a7/MANIFEST.in
--rw-rw-rw-   0        0        0     6518 2023-05-14 16:53:21.171392 cellpy-1.0.0a7/PKG-INFO
--rw-rw-rw-   0        0        0     1872 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.761471 cellpy-1.0.0a7/cellpy/
--rw-rw-rw-   0        0        0      805 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/__init__.py
--rw-rw-rw-   0        0        0       25 2023-05-14 16:52:54.000000 cellpy-1.0.0a7/cellpy/_version.py
--rw-rw-rw-   0        0        0    53597 2023-05-06 21:51:58.000000 cellpy-1.0.0a7/cellpy/cli.py
--rw-rw-rw-   0        0        0     1228 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.778750 cellpy-1.0.0a7/cellpy/internals/
--rw-rw-rw-   0        0        0        0 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/internals/__init__.py
--rw-rw-rw-   0        0        0    27994 2023-05-06 21:51:58.000000 cellpy-1.0.0a7/cellpy/internals/core.py
--rw-rw-rw-   0        0        0     4838 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/log.py
--rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.0a7/cellpy/logging.json
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.789352 cellpy-1.0.0a7/cellpy/parameters/
--rw-rw-rw-   0        0        0     3183 2023-05-02 11:51:31.000000 cellpy-1.0.0a7/cellpy/parameters/.cellpy_prms_default.conf
--rw-rw-rw-   0        0        0        2 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/parameters/__init__.py
--rw-rw-rw-   0        0        0    23784 2023-05-06 21:51:58.000000 cellpy-1.0.0a7/cellpy/parameters/internal_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.793348 cellpy-1.0.0a7/cellpy/parameters/legacy/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a7/cellpy/parameters/legacy/__init__.py
--rw-rw-rw-   0        0        0    24146 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/parameters/legacy/update_headers.py
--rw-rw-rw-   0        0        0    12142 2023-05-02 11:42:19.000000 cellpy-1.0.0a7/cellpy/parameters/prmreader.py
--rw-rw-rw-   0        0        0    12220 2023-05-02 11:49:22.000000 cellpy-1.0.0a7/cellpy/parameters/prms.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.808421 cellpy-1.0.0a7/cellpy/readers/
--rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.0a7/cellpy/readers/__init__.py
--rw-rw-rw-   0        0        0   230333 2023-05-12 19:06:24.000000 cellpy-1.0.0a7/cellpy/readers/cellreader.py
--rw-rw-rw-   0        0        0    39537 2023-05-06 21:51:58.000000 cellpy-1.0.0a7/cellpy/readers/core.py
--rw-rw-rw-   0        0        0    22998 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/dbreader.py
--rw-rw-rw-   0        0        0    13825 2023-05-06 21:51:58.000000 cellpy-1.0.0a7/cellpy/readers/filefinder.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.843034 cellpy-1.0.0a7/cellpy/readers/instruments/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a7/cellpy/readers/instruments/__init__.py
--rw-rw-rw-   0        0        0    49052 2023-05-12 17:21:48.000000 cellpy-1.0.0a7/cellpy/readers/instruments/arbin_res.py
--rw-rw-rw-   0        0        0    19381 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/arbin_sql.py
--rw-rw-rw-   0        0        0    21062 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/arbin_sql_7.py
--rw-rw-rw-   0        0        0    11134 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/arbin_sql_csv.py
--rw-rw-rw-   0        0        0     7126 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/arbin_sql_h5.py
--rw-rw-rw-   0        0        0     9883 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/arbin_sql_xlsx.py
--rw-rw-rw-   0        0        0    27324 2023-05-09 19:57:46.000000 cellpy-1.0.0a7/cellpy/readers/instruments/base.py
--rw-rw-rw-   0        0        0    22693 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/biologics_mpr.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.858546 cellpy-1.0.0a7/cellpy/readers/instruments/configurations/
--rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-1.0.0a7/cellpy/readers/instruments/configurations/__init__.py
--rw-rw-rw-   0        0        0     1700 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/configurations/maccor_txt_four.py
--rw-rw-rw-   0        0        0     4084 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/configurations/maccor_txt_one.py
--rw-rw-rw-   0        0        0     1990 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/configurations/maccor_txt_three.py
--rw-rw-rw-   0        0        0     1788 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/configurations/maccor_txt_two.py
--rw-rw-rw-   0        0        0     3549 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/configurations/maccor_txt_zero.py
--rw-rw-rw-   0        0        0     2132 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/configurations/neware_txt_zero.py
--rw-rw-rw-   0        0        0    10327 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/custom.py
--rw-rw-rw-   0        0        0     3760 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/ext_nda_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.863068 cellpy-1.0.0a7/cellpy/readers/instruments/loader_specific_modules/
--rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.0a7/cellpy/readers/instruments/loader_specific_modules/__init__.py
--rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-1.0.0a7/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
--rw-rw-rw-   0        0        0     1067 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/local_instrument.py
--rw-rw-rw-   0        0        0    12886 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/maccor_txt.py
--rw-rw-rw-   0        0        0     3488 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/neware_txt.py
--rw-rw-rw-   0        0        0    16769 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/pec_csv.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.869068 cellpy-1.0.0a7/cellpy/readers/instruments/processors/
--rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.0a7/cellpy/readers/instruments/processors/__init__.py
--rw-rw-rw-   0        0        0    15265 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/processors/post_processors.py
--rw-rw-rw-   0        0        0     1450 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/instruments/processors/pre_processors.py
--rw-rw-rw-   0        0        0    26852 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/readers/sql_dbreader.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.901142 cellpy-1.0.0a7/cellpy/utils/
--rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.0a7/cellpy/utils/__init__.py
--rw-rw-rw-   0        0        0    48182 2023-05-03 09:31:40.000000 cellpy-1.0.0a7/cellpy/utils/batch.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.927789 cellpy-1.0.0a7/cellpy/utils/batch_tools/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a7/cellpy/utils/batch_tools/__init__.py
--rw-rw-rw-   0        0        0     7578 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_analyzers.py
--rw-rw-rw-   0        0        0    19566 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_core.py
--rw-rw-rw-   0        0        0    41058 2023-05-06 21:51:58.000000 cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_experiments.py
--rw-rw-rw-   0        0        0     2931 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_exporters.py
--rw-rw-rw-   0        0        0    14090 2023-05-06 21:51:58.000000 cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_helpers.py
--rw-rw-rw-   0        0        0    27683 2023-05-02 13:39:36.000000 cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_journals.py
--rw-rw-rw-   0        0        0    29066 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_plotters.py
--rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_reporters.py
--rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-1.0.0a7/cellpy/utils/batch_tools/dumpers.py
--rw-rw-rw-   0        0        0     9872 2023-05-02 10:20:24.000000 cellpy-1.0.0a7/cellpy/utils/batch_tools/engines.py
--rw-rw-rw-   0        0        0     5294 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/batch_tools/sqlite_from_excel_db.py
--rw-rw-rw-   0        0        0    63308 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/collectors.py
--rw-rw-rw-   0        0        0    45461 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/collectors_old.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.930785 cellpy-1.0.0a7/cellpy/utils/data/
--rw-rw-rw-   0        0        0  3700143 2023-05-12 19:07:44.000000 cellpy-1.0.0a7/cellpy/utils/data/20160805_test001_45_cc.h5
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.944124 cellpy-1.0.0a7/cellpy/utils/data/raw/
--rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-1.0.0a7/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
--rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.0a7/cellpy/utils/diagnostics.py
--rw-rw-rw-   0        0        0    79016 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/easyplot.py
--rw-rw-rw-   0        0        0     1576 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/example_data.py
--rw-rw-rw-   0        0        0    39446 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/helpers.py
--rw-rw-rw-   0        0        0    38991 2023-05-06 21:51:58.000000 cellpy-1.0.0a7/cellpy/utils/ica.py
--rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.0a7/cellpy/utils/live.py
--rw-rw-rw-   0        0        0    24037 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/ocv_rlx.py
--rw-rw-rw-   0        0        0    45397 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/plotutils.py
--rw-rw-rw-   0        0        0     1787 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/cellpy/utils/processor.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.775083 cellpy-1.0.0a7/cellpy.egg-info/
--rw-rw-rw-   0        0        0     6518 2023-05-14 16:53:20.000000 cellpy-1.0.0a7/cellpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7846 2023-05-14 16:53:20.000000 cellpy-1.0.0a7/cellpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 16:53:20.000000 cellpy-1.0.0a7/cellpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 16:53:20.000000 cellpy-1.0.0a7/cellpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-14 16:53:19.000000 cellpy-1.0.0a7/cellpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      337 2023-05-14 16:53:20.000000 cellpy-1.0.0a7/cellpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-14 16:53:20.000000 cellpy-1.0.0a7/cellpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.963472 cellpy-1.0.0a7/docs/
--rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-1.0.0a7/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.731383 cellpy-1.0.0a7/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.730382 cellpy-1.0.0a7/docs/_build/.doctrees/
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.973399 cellpy-1.0.0a7/docs/_build/.doctrees/nbsphinx/
--rw-rw-rw-   0        0        0    15014 2023-04-30 13:53:57.000000 cellpy-1.0.0a7/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-04-30 13:53:57.000000 cellpy-1.0.0a7/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-04-30 13:53:57.000000 cellpy-1.0.0a7/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    25669 2023-04-30 13:54:02.000000 cellpy-1.0.0a7/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.023134 cellpy-1.0.0a7/docs/_build/_images/
--rw-rw-rw-   0        0        0    15014 2023-04-27 15:02:55.000000 cellpy-1.0.0a7/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-04-27 15:02:55.000000 cellpy-1.0.0a7/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-04-27 15:02:55.000000 cellpy-1.0.0a7/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    25669 2023-04-27 15:03:02.000000 cellpy-1.0.0a7/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
--rw-rw-rw-   0        0        0    11678 2023-04-29 14:19:31.000000 cellpy-1.0.0a7/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png
--rw-rw-rw-   0        0        0    22040 2023-04-29 14:33:27.000000 cellpy-1.0.0a7/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png
--rw-rw-rw-   0        0        0    21790 2023-04-29 14:26:00.000000 cellpy-1.0.0a7/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png
--rw-rw-rw-   0        0        0    32991 2023-04-29 14:26:01.000000 cellpy-1.0.0a7/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png
--rw-rw-rw-   0        0        0    32991 2023-04-30 20:02:23.000000 cellpy-1.0.0a7/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png
--rw-rw-rw-   0        0        0     7231 2023-04-29 14:12:31.000000 cellpy-1.0.0a7/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png
--rw-rw-rw-   0        0        0    13360 2023-04-29 14:36:26.000000 cellpy-1.0.0a7/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png
--rw-rw-rw-   0        0        0    21790 2023-04-30 20:02:22.000000 cellpy-1.0.0a7/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png
--rw-rw-rw-   0        0        0     5391 2023-04-29 14:10:02.000000 cellpy-1.0.0a7/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png
--rw-rw-rw-   0        0        0    20826 2023-04-29 14:29:06.000000 cellpy-1.0.0a7/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png
--rw-rw-rw-   0        0        0    88743 2023-04-19 13:49:30.000000 cellpy-1.0.0a7/docs/_build/_images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-1.0.0a7/docs/_build/_images/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-1.0.0a7/docs/_build/_images/tutorials_utils_plotting_fig2.png
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.030137 cellpy-1.0.0a7/docs/_build/_static/
--rw-rw-rw-   0        0        0      286 2023-04-25 11:20:36.000000 cellpy-1.0.0a7/docs/_build/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a7/docs/_build/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a7/docs/_build/_static/plus.png
--rw-rw-rw-   0        0        0     1695 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/adapted_readme.rst
--rw-rw-rw-   0        0        0    10731 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.052132 cellpy-1.0.0a7/docs/developers_guide/
--rw-rw-rw-   0        0        0     1334 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/developers_guide/dev_cellpy_data_structure.rst
--rw-rw-rw-   0        0        0     5904 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/developers_guide/dev_cellpy_folder_structure.rst
--rw-rw-rw-   0        0        0      935 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/developers_guide/dev_cellpy_packaging_pypi.rst
--rw-rw-rw-   0        0        0     3009 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/developers_guide/dev_cellpy_setup.rst
--rw-rw-rw-   0        0        0     1821 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/developers_guide/dev_conda_package.rst
--rw-rw-rw-   0        0        0     2136 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/developers_guide/dev_docs.rst
--rw-rw-rw-   0        0        0     5218 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/developers_guide/dev_loaders_and_instruments.rst
--rw-rw-rw-   0        0        0     1768 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/developers_guide/dev_various.rst
--rw-rw-rw-   0        0        0      326 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/developers_guide/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.065897 cellpy-1.0.0a7/docs/examples_and_tutorials/
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.083285 cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/
--rw-rw-rw-   0        0        0    15786 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst
--rw-rw-rw-   0        0        0     3909 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst
--rw-rw-rw-   0        0        0     5485 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst
--rw-rw-rw-   0        0        0     4465 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst
--rw-rw-rw-   0        0        0     5908 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/05_configuring.rst
--rw-rw-rw-   0        0        0     1052 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/06_pandas.rst
--rw-rw-rw-   0        0        0     1102 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst
--rw-rw-rw-   0        0        0     8224 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst
--rw-rw-rw-   0        0        0      484 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/basics.rst
--rw-rw-rw-   0        0        0      366 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/examples.rst
--rw-rw-rw-   0        0        0      174 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.094352 cellpy-1.0.0a7/docs/examples_and_tutorials/loaders/
--rw-rw-rw-   0        0        0       49 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/loaders/01_arbin.rst
--rw-rw-rw-   0        0        0       52 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/loaders/02_maccor.rst
--rw-rw-rw-   0        0        0       43 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/loaders/03_PEC.rst
--rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/loaders/04_Neware.rst
--rw-rw-rw-   0        0        0       62 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/loaders/05_biologics.rst
--rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/loaders/06_custom.rst
--rw-rw-rw-   0        0        0      260 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/loaders.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:20.733393 cellpy-1.0.0a7/docs/examples_and_tutorials/notebooks/
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.099359 cellpy-1.0.0a7/docs/examples_and_tutorials/notebooks/images/
--rw-rw-rw-   0        0        0    88743 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0    95663 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png
--rw-rw-rw-   0        0        0      231 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/notebooks.rst
--rw-rw-rw-   0        0        0     1797 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/tips_and_tricks.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.114389 cellpy-1.0.0a7/docs/examples_and_tutorials/utils/
--rw-rw-rw-   0        0        0     4388 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/utils/batch.rst
--rw-rw-rw-   0        0        0       59 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/utils/collectors.rst
--rw-rw-rw-   0        0        0       53 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/utils/easyplot.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.119939 cellpy-1.0.0a7/docs/examples_and_tutorials/utils/figures/
--rw-rw-rw-   0        0        0   296908 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png
--rw-rw-rw-   0        0        0     1219 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/utils/ica.rst
--rw-rw-rw-   0        0        0     2063 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/utils/plotting.rst
--rw-rw-rw-   0        0        0      338 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/utils/templates.rst
--rw-rw-rw-   0        0        0     1379 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst
--rw-rw-rw-   0        0        0      371 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/examples_and_tutorials/utils.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.125014 cellpy-1.0.0a7/docs/figures/
--rw-rw-rw-   0        0        0     9981 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/figures/cellpy-icon-bw.png
--rw-rw-rw-   0        0        0    10302 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/figures/cellpy-logo-v1.png
--rw-rw-rw-   0        0        0      593 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.138394 cellpy-1.0.0a7/docs/main_description/
--rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/main_description/authors.rst
--rw-rw-rw-   0        0        0       37 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/main_description/contributing.rst
--rw-rw-rw-   0        0        0    16327 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/main_description/formats.rst
--rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/main_description/history.rst
--rw-rw-rw-   0        0        0      182 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/main_description/index.rst
--rw-rw-rw-   0        0        0     4288 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/main_description/installation.rst
--rw-rw-rw-   0        0        0     3444 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/main_description/usage.rst
--rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-1.0.0a7/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-14 16:53:21.169386 cellpy-1.0.0a7/docs/source/
--rw-rw-rw-   0        0        0      367 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/source/cellpy.internals.rst
--rw-rw-rw-   0        0        0      447 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/source/cellpy.parameters.legacy.rst
--rw-rw-rw-   0        0        0      847 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/source/cellpy.parameters.rst
--rw-rw-rw-   0        0        0     1911 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/source/cellpy.readers.instruments.configurations.rst
--rw-rw-rw-   0        0        0      631 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/source/cellpy.readers.instruments.loader_specific_modules.rst
--rw-rw-rw-   0        0        0      783 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/source/cellpy.readers.instruments.processors.rst
--rw-rw-rw-   0        0        0     3413 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/source/cellpy.readers.instruments.rst
--rw-rw-rw-   0        0        0     1139 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/source/cellpy.readers.rst
--rw-rw-rw-   0        0        0      721 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/source/cellpy.rst
--rw-rw-rw-   0        0        0     2610 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/source/cellpy.utils.batch_tools.rst
--rw-rw-rw-   0        0        0     2222 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/docs/source/cellpy.utils.rst
--rw-rw-rw-   0        0        0       62 2023-05-01 10:14:23.000000 cellpy-1.0.0a7/docs/source/modules.rst
--rw-rw-rw-   0        0        0      281 2023-05-01 18:24:45.000000 cellpy-1.0.0a7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 16:53:21.172419 cellpy-1.0.0a7/setup.cfg
--rw-rw-rw-   0        0        0     2922 2023-05-12 17:21:47.000000 cellpy-1.0.0a7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.397303 cellpy-1.0.0a8/
+-rw-rw-rw-   0        0        0      503 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3086 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     3908 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/LICENSE
+-rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-1.0.0a8/MANIFEST.in
+-rw-rw-rw-   0        0        0     6518 2023-05-14 17:53:18.397303 cellpy-1.0.0a8/PKG-INFO
+-rw-rw-rw-   0        0        0     1872 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.117245 cellpy-1.0.0a8/cellpy/
+-rw-rw-rw-   0        0        0      805 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/__init__.py
+-rw-rw-rw-   0        0        0       25 2023-05-14 17:52:59.000000 cellpy-1.0.0a8/cellpy/_version.py
+-rw-rw-rw-   0        0        0    53597 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/cli.py
+-rw-rw-rw-   0        0        0     1228 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.129456 cellpy-1.0.0a8/cellpy/internals/
+-rw-rw-rw-   0        0        0        0 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/internals/__init__.py
+-rw-rw-rw-   0        0        0    27994 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/internals/core.py
+-rw-rw-rw-   0        0        0     4838 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/log.py
+-rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/logging.json
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.139109 cellpy-1.0.0a8/cellpy/parameters/
+-rw-rw-rw-   0        0        0     3183 2023-05-02 11:51:31.000000 cellpy-1.0.0a8/cellpy/parameters/.cellpy_prms_default.conf
+-rw-rw-rw-   0        0        0        2 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/parameters/__init__.py
+-rw-rw-rw-   0        0        0    23452 2023-05-14 17:34:31.000000 cellpy-1.0.0a8/cellpy/parameters/internal_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.142108 cellpy-1.0.0a8/cellpy/parameters/legacy/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/parameters/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24146 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/parameters/legacy/update_headers.py
+-rw-rw-rw-   0        0        0    12142 2023-05-02 11:42:19.000000 cellpy-1.0.0a8/cellpy/parameters/prmreader.py
+-rw-rw-rw-   0        0        0    12220 2023-05-02 11:49:22.000000 cellpy-1.0.0a8/cellpy/parameters/prms.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.151689 cellpy-1.0.0a8/cellpy/readers/
+-rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/readers/__init__.py
+-rw-rw-rw-   0        0        0   230654 2023-05-14 17:41:37.000000 cellpy-1.0.0a8/cellpy/readers/cellreader.py
+-rw-rw-rw-   0        0        0    39537 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/readers/core.py
+-rw-rw-rw-   0        0        0    22998 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/dbreader.py
+-rw-rw-rw-   0        0        0    13825 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/readers/filefinder.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.179208 cellpy-1.0.0a8/cellpy/readers/instruments/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/readers/instruments/__init__.py
+-rw-rw-rw-   0        0        0    49052 2023-05-12 17:21:48.000000 cellpy-1.0.0a8/cellpy/readers/instruments/arbin_res.py
+-rw-rw-rw-   0        0        0    19381 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql.py
+-rw-rw-rw-   0        0        0    21062 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_7.py
+-rw-rw-rw-   0        0        0    11134 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_csv.py
+-rw-rw-rw-   0        0        0     7126 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_h5.py
+-rw-rw-rw-   0        0        0     9883 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_xlsx.py
+-rw-rw-rw-   0        0        0    27324 2023-05-09 19:57:46.000000 cellpy-1.0.0a8/cellpy/readers/instruments/base.py
+-rw-rw-rw-   0        0        0    22693 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/biologics_mpr.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.190716 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/
+-rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1700 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_four.py
+-rw-rw-rw-   0        0        0     4084 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_one.py
+-rw-rw-rw-   0        0        0     1990 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_three.py
+-rw-rw-rw-   0        0        0     1788 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_two.py
+-rw-rw-rw-   0        0        0     3549 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_zero.py
+-rw-rw-rw-   0        0        0     2132 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/neware_txt_zero.py
+-rw-rw-rw-   0        0        0    10327 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/custom.py
+-rw-rw-rw-   0        0        0     3760 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/ext_nda_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.193716 cellpy-1.0.0a8/cellpy/readers/instruments/loader_specific_modules/
+-rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.0a8/cellpy/readers/instruments/loader_specific_modules/__init__.py
+-rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-1.0.0a8/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
+-rw-rw-rw-   0        0        0     1067 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/local_instrument.py
+-rw-rw-rw-   0        0        0    12886 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/maccor_txt.py
+-rw-rw-rw-   0        0        0     3488 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/neware_txt.py
+-rw-rw-rw-   0        0        0    16769 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/pec_csv.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.199716 cellpy-1.0.0a8/cellpy/readers/instruments/processors/
+-rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.0a8/cellpy/readers/instruments/processors/__init__.py
+-rw-rw-rw-   0        0        0    15265 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/processors/post_processors.py
+-rw-rw-rw-   0        0        0     1450 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/processors/pre_processors.py
+-rw-rw-rw-   0        0        0    26852 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/sql_dbreader.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.223716 cellpy-1.0.0a8/cellpy/utils/
+-rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    48182 2023-05-03 09:31:40.000000 cellpy-1.0.0a8/cellpy/utils/batch.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.242716 cellpy-1.0.0a8/cellpy/utils/batch_tools/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/__init__.py
+-rw-rw-rw-   0        0        0     7578 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_analyzers.py
+-rw-rw-rw-   0        0        0    19566 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_core.py
+-rw-rw-rw-   0        0        0    41058 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_experiments.py
+-rw-rw-rw-   0        0        0     2931 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_exporters.py
+-rw-rw-rw-   0        0        0    14090 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_helpers.py
+-rw-rw-rw-   0        0        0    27683 2023-05-02 13:39:36.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_journals.py
+-rw-rw-rw-   0        0        0    29066 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_plotters.py
+-rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_reporters.py
+-rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/dumpers.py
+-rw-rw-rw-   0        0        0     9872 2023-05-02 10:20:24.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/engines.py
+-rw-rw-rw-   0        0        0     5294 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/sqlite_from_excel_db.py
+-rw-rw-rw-   0        0        0    63308 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/collectors.py
+-rw-rw-rw-   0        0        0    45461 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/collectors_old.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.244716 cellpy-1.0.0a8/cellpy/utils/data/
+-rw-rw-rw-   0        0        0  3700143 2023-05-14 17:50:44.000000 cellpy-1.0.0a8/cellpy/utils/data/20160805_test001_45_cc.h5
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.249716 cellpy-1.0.0a8/cellpy/utils/data/raw/
+-rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
+-rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.0a8/cellpy/utils/diagnostics.py
+-rw-rw-rw-   0        0        0    79016 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/easyplot.py
+-rw-rw-rw-   0        0        0     1576 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/example_data.py
+-rw-rw-rw-   0        0        0    39446 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/helpers.py
+-rw-rw-rw-   0        0        0    38991 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/utils/ica.py
+-rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.0a8/cellpy/utils/live.py
+-rw-rw-rw-   0        0        0    24037 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/ocv_rlx.py
+-rw-rw-rw-   0        0        0    45397 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/plotutils.py
+-rw-rw-rw-   0        0        0     1787 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/processor.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.127456 cellpy-1.0.0a8/cellpy.egg-info/
+-rw-rw-rw-   0        0        0     6518 2023-05-14 17:53:17.000000 cellpy-1.0.0a8/cellpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7846 2023-05-14 17:53:18.000000 cellpy-1.0.0a8/cellpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 17:53:17.000000 cellpy-1.0.0a8/cellpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 17:53:17.000000 cellpy-1.0.0a8/cellpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 17:53:16.000000 cellpy-1.0.0a8/cellpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      337 2023-05-14 17:53:17.000000 cellpy-1.0.0a8/cellpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-14 17:53:17.000000 cellpy-1.0.0a8/cellpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.259228 cellpy-1.0.0a8/docs/
+-rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-1.0.0a8/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.089754 cellpy-1.0.0a8/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.088754 cellpy-1.0.0a8/docs/_build/.doctrees/
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.266226 cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/
+-rw-rw-rw-   0        0        0    15014 2023-04-30 13:53:57.000000 cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-04-30 13:53:57.000000 cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-04-30 13:53:57.000000 cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    25669 2023-04-30 13:54:02.000000 cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.295735 cellpy-1.0.0a8/docs/_build/_images/
+-rw-rw-rw-   0        0        0    15014 2023-04-27 15:02:55.000000 cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-04-27 15:02:55.000000 cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-04-27 15:02:55.000000 cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    25669 2023-04-27 15:03:02.000000 cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
+-rw-rw-rw-   0        0        0    11678 2023-04-29 14:19:31.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png
+-rw-rw-rw-   0        0        0    22040 2023-04-29 14:33:27.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png
+-rw-rw-rw-   0        0        0    21790 2023-04-29 14:26:00.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png
+-rw-rw-rw-   0        0        0    32991 2023-04-29 14:26:01.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png
+-rw-rw-rw-   0        0        0    32991 2023-04-30 20:02:23.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png
+-rw-rw-rw-   0        0        0     7231 2023-04-29 14:12:31.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png
+-rw-rw-rw-   0        0        0    13360 2023-04-29 14:36:26.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png
+-rw-rw-rw-   0        0        0    21790 2023-04-30 20:02:22.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png
+-rw-rw-rw-   0        0        0     5391 2023-04-29 14:10:02.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png
+-rw-rw-rw-   0        0        0    20826 2023-04-29 14:29:06.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png
+-rw-rw-rw-   0        0        0    88743 2023-04-19 13:49:30.000000 cellpy-1.0.0a8/docs/_build/_images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-1.0.0a8/docs/_build/_images/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-1.0.0a8/docs/_build/_images/tutorials_utils_plotting_fig2.png
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.300268 cellpy-1.0.0a8/docs/_build/_static/
+-rw-rw-rw-   0        0        0      286 2023-04-25 11:20:36.000000 cellpy-1.0.0a8/docs/_build/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a8/docs/_build/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a8/docs/_build/_static/plus.png
+-rw-rw-rw-   0        0        0     1695 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/adapted_readme.rst
+-rw-rw-rw-   0        0        0    10731 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.313794 cellpy-1.0.0a8/docs/developers_guide/
+-rw-rw-rw-   0        0        0     1334 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_data_structure.rst
+-rw-rw-rw-   0        0        0     5904 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_folder_structure.rst
+-rw-rw-rw-   0        0        0      935 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_packaging_pypi.rst
+-rw-rw-rw-   0        0        0     3009 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_setup.rst
+-rw-rw-rw-   0        0        0     1821 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_conda_package.rst
+-rw-rw-rw-   0        0        0     2136 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_docs.rst
+-rw-rw-rw-   0        0        0     5218 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_loaders_and_instruments.rst
+-rw-rw-rw-   0        0        0     1768 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_various.rst
+-rw-rw-rw-   0        0        0      326 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.322793 cellpy-1.0.0a8/docs/examples_and_tutorials/
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.334793 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/
+-rw-rw-rw-   0        0        0    15786 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst
+-rw-rw-rw-   0        0        0     3909 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst
+-rw-rw-rw-   0        0        0     5485 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst
+-rw-rw-rw-   0        0        0     4465 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst
+-rw-rw-rw-   0        0        0     5908 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/05_configuring.rst
+-rw-rw-rw-   0        0        0     1052 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/06_pandas.rst
+-rw-rw-rw-   0        0        0     1102 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst
+-rw-rw-rw-   0        0        0     8224 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst
+-rw-rw-rw-   0        0        0      484 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basics.rst
+-rw-rw-rw-   0        0        0      366 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/examples.rst
+-rw-rw-rw-   0        0        0      174 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.343793 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/
+-rw-rw-rw-   0        0        0       49 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/01_arbin.rst
+-rw-rw-rw-   0        0        0       52 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/02_maccor.rst
+-rw-rw-rw-   0        0        0       43 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/03_PEC.rst
+-rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/04_Neware.rst
+-rw-rw-rw-   0        0        0       62 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/05_biologics.rst
+-rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/06_custom.rst
+-rw-rw-rw-   0        0        0      260 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.091754 cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks/
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.347793 cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks/images/
+-rw-rw-rw-   0        0        0    88743 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0    95663 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png
+-rw-rw-rw-   0        0        0      231 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks.rst
+-rw-rw-rw-   0        0        0     1797 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/tips_and_tricks.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.358792 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/
+-rw-rw-rw-   0        0        0     4388 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/batch.rst
+-rw-rw-rw-   0        0        0       59 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/collectors.rst
+-rw-rw-rw-   0        0        0       53 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/easyplot.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.362793 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/figures/
+-rw-rw-rw-   0        0        0   296908 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png
+-rw-rw-rw-   0        0        0     1219 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/ica.rst
+-rw-rw-rw-   0        0        0     2063 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/plotting.rst
+-rw-rw-rw-   0        0        0      338 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/templates.rst
+-rw-rw-rw-   0        0        0     1379 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst
+-rw-rw-rw-   0        0        0      371 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.366794 cellpy-1.0.0a8/docs/figures/
+-rw-rw-rw-   0        0        0     9981 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/figures/cellpy-icon-bw.png
+-rw-rw-rw-   0        0        0    10302 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/figures/cellpy-logo-v1.png
+-rw-rw-rw-   0        0        0      593 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.376793 cellpy-1.0.0a8/docs/main_description/
+-rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/authors.rst
+-rw-rw-rw-   0        0        0       37 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/contributing.rst
+-rw-rw-rw-   0        0        0    16327 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/formats.rst
+-rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/history.rst
+-rw-rw-rw-   0        0        0      182 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/index.rst
+-rw-rw-rw-   0        0        0     4288 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/installation.rst
+-rw-rw-rw-   0        0        0     3444 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/usage.rst
+-rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-1.0.0a8/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.396303 cellpy-1.0.0a8/docs/source/
+-rw-rw-rw-   0        0        0      367 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.internals.rst
+-rw-rw-rw-   0        0        0      447 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.parameters.legacy.rst
+-rw-rw-rw-   0        0        0      847 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.parameters.rst
+-rw-rw-rw-   0        0        0     1911 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.configurations.rst
+-rw-rw-rw-   0        0        0      631 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.loader_specific_modules.rst
+-rw-rw-rw-   0        0        0      783 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.processors.rst
+-rw-rw-rw-   0        0        0     3413 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.rst
+-rw-rw-rw-   0        0        0     1139 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.readers.rst
+-rw-rw-rw-   0        0        0      721 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.rst
+-rw-rw-rw-   0        0        0     2610 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.utils.batch_tools.rst
+-rw-rw-rw-   0        0        0     2222 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.utils.rst
+-rw-rw-rw-   0        0        0       62 2023-05-01 10:14:23.000000 cellpy-1.0.0a8/docs/source/modules.rst
+-rw-rw-rw-   0        0        0      281 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 17:53:18.398304 cellpy-1.0.0a8/setup.cfg
+-rw-rw-rw-   0        0        0     2922 2023-05-12 17:21:47.000000 cellpy-1.0.0a8/setup.py
```

### Comparing `cellpy-1.0.0a7/CONTRIBUTING.rst` & `cellpy-1.0.0a8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/HISTORY.rst` & `cellpy-1.0.0a8/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/LICENSE` & `cellpy-1.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/MANIFEST.in` & `cellpy-1.0.0a8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/PKG-INFO` & `cellpy-1.0.0a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cellpy-1.0.0a7/README.rst` & `cellpy-1.0.0a8/README.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/__init__.py` & `cellpy-1.0.0a8/cellpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/cli.py` & `cellpy-1.0.0a8/cellpy/cli.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/exceptions.py` & `cellpy-1.0.0a8/cellpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/internals/core.py` & `cellpy-1.0.0a8/cellpy/internals/core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/log.py` & `cellpy-1.0.0a8/cellpy/log.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/logging.json` & `cellpy-1.0.0a8/cellpy/logging.json`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/parameters/.cellpy_prms_default.conf` & `cellpy-1.0.0a8/cellpy/parameters/.cellpy_prms_default.conf`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/parameters/internal_settings.py` & `cellpy-1.0.0a8/cellpy/parameters/internal_settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,711 +1,724 @@
-"""Internal settings and definitions and functions for getting them."""
-import logging
-import warnings
-from collections import UserDict
-from dataclasses import dataclass, fields, asdict
-from typing import List, Optional
-
-import pandas as pd
-
-from cellpy import prms
-
-CELLPY_FILE_VERSION = 8
-MINIMUM_CELLPY_FILE_VERSION = 4
-STEP_TABLE_VERSION = 5
-RAW_TABLE_VERSION = 5
-SUMMARY_TABLE_VERSION = 7
-# if you change this, remember that both loading and saving uses this
-# constant at the moment, and check that loading old files still works
-# - and possibly refactor so that the old-file loaders contain the
-# appropriate pickle protocol:
-PICKLE_PROTOCOL = 4
-
-# For creating the sqlite database from Excel:
-TABLE_NAME_SQLITE = "cells"
-COLUMNS_EXCEL_PK = "id"
-COLUMNS_RENAMER = {
-    COLUMNS_EXCEL_PK: "pk",
-    "batch": "comment_history",
-    "cell_name": "name",
-    "exists": "cell_exists",
-    "group": "cell_group",
-    "raw_file_names": "raw_data",
-    "argument": "cell_spec",
-    "nom_cap": "nominal_capacity",
-    "freeze": "frozen",
-}
-ATTRS_TO_IMPORT_FROM_EXCEL_SQLITE = [
-    "name",
-    "label",
-    "project",
-    "cell_group",
-    "cellpy_file_name",
-    "instrument",
-    "cell_type",
-    "cell_design",
-    "channel",
-    "experiment_type",
-    "mass_active",
-    "area",
-    "mass_total",
-    "loading_active",
-    "nominal_capacity",
-    "comment_slurry",
-    "comment_cell",
-    "comment_general",
-    "comment_history",
-    "selected",
-    "freeze",
-    "cell_exists",
-]
-BATCH_ATTRS_TO_IMPORT_FROM_EXCEL_SQLITE = [
-    "comment_history",
-    "sub_batch_01",
-    "sub_batch_02",
-    "sub_batch_03",
-    "sub_batch_04",
-    "sub_batch_05",
-    "sub_batch_06",
-    "sub_batch_07",
-]
-
-
-OTHERPATHS = ["rawdatadir", "cellpydatadir"]
-
-
-@dataclass
-class CellpyMeta:
-    def update(self, as_list: bool = False, **kwargs):
-        """Updates from dictionary of form {key: [values]}
-
-        Args:
-            as_list (bool): pick only first scalar if True.
-            **kwargs (dict): key word attributes to update.
-
-        Returns:
-            None
-        """
-
-        for k, v in kwargs.items():
-            if not as_list:
-                v = v[0]
-            if hasattr(self, k):
-                logging.debug(f"{k} -> {v}")
-                setattr(self, k, v)
-            else:
-                logging.debug(f"[NOT-VALID]{k}:{v}")
-
-    def digest(self, as_list: bool = False, **kwargs):
-        """Pops from dictionary of form {key: [values]}
-
-        Args:
-            as_list (bool): pick only first scalar if True.
-            **kwargs (dict): key word attributes to pick.
-
-        Returns:
-            Dictionary containing the non-digested part.
-        """
-        not_digested = {}
-        for k, v in kwargs.items():
-            if not as_list:
-                v = v[0]
-            if hasattr(self, k):
-                logging.debug(f"{k} -> {v}")
-                setattr(self, k, v)
-            else:
-                logging.debug(f"{k}:{v} ->")
-                not_digested[k] = v
-        return not_digested
-
-    def to_frame(self):
-        """Converts to pandas dataframe"""
-        df = pd.DataFrame.from_dict(asdict(self), orient="index")
-        df.index.name = "key"
-        n_rows, n_cols = df.shape
-        if n_cols == 1:
-            columns = ["value"]
-        else:
-            columns = [f"value_{i:02}" for i in range(n_cols)]
-        df.columns = columns
-
-        return df
-
-
-@dataclass
-class CellpyMetaCommon(CellpyMeta):
-    # about test
-    cell_name: Optional[str] = None  # used as property
-    start_datetime: Optional[str] = None
-    time_zone: Optional[str] = None
-    comment: Optional[prms.CellPyDataConfig] = prms.CellInfo.comment
-    file_errors: Optional[str] = None  # not in use at the moment
-    raw_id: Optional[str] = None  # used as property
-    cellpy_file_version: int = CELLPY_FILE_VERSION
-
-    # about tester
-    tester_ID: Optional[prms.CellPyDataConfig] = None
-    tester_server_software_version: Optional[prms.CellPyDataConfig] = None
-    tester_client_software_version: Optional[prms.CellPyDataConfig] = None
-    tester_calibration_date: Optional[prms.CellPyDataConfig] = None
-
-    # about cell
-    material: Optional[prms.CellPyDataConfig] = prms.Materials.default_material
-    # TODO @jepe: Maybe we should use values with units here instead (pint)?
-    mass: Optional[
-        prms.CellPyDataConfig
-    ] = prms.Materials.default_mass  # active material
-    tot_mass: Optional[
-        prms.CellPyDataConfig
-    ] = prms.Materials.default_mass  # total material
-    nom_cap: Optional[
-        prms.CellPyDataConfig
-    ] = prms.Materials.default_nom_cap  # nominal capacity   # used as property
-    nom_cap_specifics: Optional[
-        prms.CellPyDataConfig
-    ] = (
-        prms.Materials.default_nom_cap_specifics
-    )  # nominal capacity type  # used as property
-
-    active_electrode_area: Optional[
-        prms.CellPyDataConfig
-    ] = prms.CellInfo.active_electrode_area
-    active_electrode_thickness: Optional[
-        prms.CellPyDataConfig
-    ] = prms.CellInfo.active_electrode_thickness
-    electrolyte_volume: Optional[
-        prms.CellPyDataConfig
-    ] = prms.CellInfo.electrolyte_volume
-
-    electrolyte_type: Optional[prms.CellPyDataConfig] = prms.CellInfo.electrolyte_type
-    active_electrode_type: Optional[
-        prms.CellPyDataConfig
-    ] = prms.CellInfo.active_electrode_type
-    counter_electrode_type: Optional[
-        prms.CellPyDataConfig
-    ] = prms.CellInfo.counter_electrode_type
-    reference_electrode_type: Optional[
-        prms.CellPyDataConfig
-    ] = prms.CellInfo.reference_electrode_type
-    experiment_type: Optional[prms.CellPyDataConfig] = prms.CellInfo.experiment_type
-    cell_type: Optional[prms.CellPyDataConfig] = prms.CellInfo.cell_type
-    separator_type: Optional[prms.CellPyDataConfig] = prms.CellInfo.separator_type
-    active_electrode_current_collector: Optional[
-        prms.CellPyDataConfig
-    ] = prms.CellInfo.active_electrode_current_collector
-    reference_electrode_current_collector: Optional[
-        prms.CellPyDataConfig
-    ] = prms.CellInfo.reference_electrode_current_collector
-
-
-@dataclass
-class CellpyMetaIndividualTest(CellpyMeta):
-    # ---------------- test dependent -------------------------------
-    channel_index: Optional[prms.CellPyDataConfig] = None
-    creator: Optional[str] = None
-    schedule_file_name = None
-    test_type: Optional[
-        prms.CellPyDataConfig
-    ] = None  # Not used (and might be put inside test_ID)
-    voltage_lim_low: Optional[prms.CellPyDataConfig] = prms.CellInfo.voltage_lim_low
-    voltage_lim_high: Optional[prms.CellPyDataConfig] = prms.CellInfo.voltage_lim_high
-    cycle_mode: Optional[prms.CellPyDataConfig] = prms.Reader.cycle_mode
-    test_ID: Optional[
-        prms.CellPyDataConfig
-    ] = None  # id for the test - currently just a number; could become a list or more in the future
-
-
-# TODO: remove import of this
-class HeaderDict(UserDict):
-    """Sub-classing dict to allow for tab-completion."""
-
-    def __setitem__(self, key: str, value: str) -> None:
-        if key == "data":
-            raise KeyError("protected key")
-        super().__setitem__(key, value)
-        self.__dict__[key] = value
-
-
-@dataclass
-class DictLikeClass:
-    """Add some dunder-methods so that it does not break old code that used
-    dictionaries for storing settings
-
-    Remarks: it is not a complete dictionary experience - for example,
-    setting new attributes (new keys) is not supported (raises ``KeyError``
-    if using the typical dict setting method) since it uses the
-    ``dataclasses.fields`` method to find its members.
-
-    """
-
-    def __getitem__(self, key):
-        if key not in self._field_names:
-            logging.debug(f"{key} not in fields")
-        try:
-            return getattr(self, key)
-        except AttributeError:
-            raise KeyError(f"missing key: {key}")
-
-    def __setitem__(self, key, value):
-        if key not in self._field_names:
-            raise KeyError(f"creating new key not allowed: {key}")
-        setattr(self, key, value)
-
-    def __missing__(self, key):
-        raise KeyError
-
-    @property
-    def _field_names(self):
-        return [field.name for field in fields(self)]
-
-    def __iter__(self):
-        for field in self._field_names:
-            yield field
-
-    def _value_iter(self):
-        for field in self._field_names:
-            yield getattr(self, field)
-
-    def keys(self):
-        return [key for key in self.__iter__()]
-
-    def values(self):
-        return [v for v in self._value_iter()]
-
-    def items(self):
-        return zip(self.keys(), self.values())
-
-
-@dataclass
-class BaseSettings(DictLikeClass):
-    """Base class for internal cellpy settings.
-
-    Usage::
-
-         @dataclass
-         class MyCoolCellpySetting(BaseSetting):
-             var1: str = "first var"
-             var2: int = 12
-
-    """
-
-    def get(self, key):
-        """Get the value (postfixes not supported)."""
-        if key not in self.keys():
-            logging.critical(f"the column header '{key}' not found")
-            return
-        else:
-            return self[key]
-
-
-@dataclass
-class BaseHeaders(BaseSettings):
-    """Extending BaseSetting so that it's allowed to add postfixes.
-
-    Example:
-         >>> header["key_postfix"]  # returns "value_postfix"
-    """
-
-    postfixes = []
-
-    def __getitem__(self, key):
-        postfix = ""
-        if key not in self._field_names:
-            # check postfix:
-            subs = key.split("_")
-            _key = "_".join(subs[:-1])
-            _postfix = subs[-1]
-            if _postfix in self.postfixes:
-                postfix = f"_{_postfix}"
-                key = _key
-        try:
-            v = getattr(self, key)
-            return f"{v}{postfix}"
-        except AttributeError:
-            raise KeyError(f"missing key: {key}")
-
-
-@dataclass
-class InstrumentSettings(DictLikeClass):
-    """Base class for instrument settings.
-
-    Usage::
-
-        @dataclass
-        class MyCoolInstrumentSetting(InstrumentSettings):
-            var1: str = "first var"
-            var2: int = 12
-
-    Remark! Try to use it as you would use a normal dataclass.
-
-    """
-
-    ...
-
-
-@dataclass
-class CellpyUnits(BaseSettings):
-    """These are the units used inside Cellpy.
-
-    At least two sets of units needs to be defined; `cellpy_units` and `raw_units`.
-    The `data.raw` dataframe is given in `raw_units` where the units are defined
-    inside the instrument loader used. Since the `data.steps` dataframe is a summary of
-    the step statistics from the `data.raw` dataframe, this also uses the `raw_units`.
-    The `data.summary` dataframe contains columns with values directly from the `data.raw` dataframe
-    given in `raw_units` as well as calculated columns given in `cellpy_units`.
-
-    Remark that all input to cellpy through user interaction (or utils) should be in `cellpy_units`.
-    This is also true for meta-data collected from the raw files. The instrument loader needs to
-    take care of the translation from its raw units to `cellpy_units` during loading the raw data
-    file for the meta-data (remark that this is not necessary and not recommended for the actual
-    "raw" data that is going to be stored in the `data.raw` dataframe).
-
-    As of 2022.09.29, cellpy does not automatically ensure unit conversion for input of meta-data,
-    but has an internal method (`CellPyData.to_cellpy_units`) that can be used.
-
-    These are the different attributes currently supported for data in the dataframes::
-
-        current: str = "A"
-        charge: str = "mAh"
-        voltage: str = "V"
-        time: str = "sec"
-        resistance: str = "Ohms"
-        power: str = "W"
-        energy: str = "Wh"
-        frequency: str = "hz"
-
-    And here are the different attributes currently supported for meta-data::
-
-        # output-units for specific capacity etc.
-        specific_gravimetric: str = "g"
-        specific_areal: str = "cm**2"  # used for calculating specific capacity etc.
-        specific_volumetric: str = "cm**3"  # used for calculating specific capacity etc.
-
-        # other meta-data
-        nominal_capacity: str = "mAh/g"  # used for calculating rates etc.
-        mass: str = "mg"
-        length: str = "cm"
-        area: str = "cm**2"
-        volume: str = "cm**3"
-        temperature: str = "C"
-
-    """
-
-    current: str = "A"
-    charge: str = "mAh"
-    voltage: str = "V"
-    time: str = "sec"
-    resistance: str = "ohm"
-    power: str = "W"
-    energy: str = "Wh"
-    frequency: str = "hz"
-    mass: str = "mg"  # for mass
-    nominal_capacity: str = "mAh/g"
-    specific_gravimetric: str = "g"  # g in specific capacity etc
-    specific_areal: str = "cm**2"  # m2 in specific capacity etc
-    specific_volumetric: str = "cm**3"  # m3 in specific capacity etc
-
-    length: str = "cm"
-    area: str = "cm**2"
-    volume: str = "cm**3"
-    temperature: str = "C"
-    pressure: str = "bar"
-
-    def update(self, new_units: dict):
-        """Update the units."""
-
-        logging.debug(f"{new_units=}")
-        for k in new_units:
-            if k in self.keys():
-                self[k] = new_units[k]
-
-
-@dataclass
-class CellpyLimits(BaseSettings):
-    """These are the limits used inside ``cellpy`` for finding step types.
-
-    Since all instruments have an inherent inaccuracy, it is naive to assume that
-    for example the voltage within a constant voltage step does not change at all.
-    Therefore, we need to define some limits for what we consider to be a constant and
-    what we assume to be zero.
-
-    """
-
-    current_hard: float = 1e-13
-    current_soft: float = 1e-05
-    stable_current_hard: float = 2.0
-    stable_current_soft: float = 4.0
-    stable_voltage_hard: float = 2.0
-    stable_voltage_soft: float = 4.0
-    stable_charge_hard: float = 0.9
-    stable_charge_soft: float = 5.0
-    ir_change: float = 1e-05
-
-
-@dataclass
-class HeadersNormal(BaseHeaders):
-    aci_phase_angle_txt: str = "aci_phase_angle"
-    ref_aci_phase_angle_txt: str = "ref_aci_phase_angle"
-    ac_impedance_txt: str = "ac_impedance"
-    ref_ac_impedance_txt: str = "ref_ac_impedance"
-    charge_capacity_txt: str = "charge_capacity"
-    charge_energy_txt: str = "charge_energy"
-    current_txt: str = "current"
-    cycle_index_txt: str = "cycle_index"
-    data_point_txt: str = "data_point"
-    datetime_txt: str = "date_time"
-    discharge_capacity_txt: str = "discharge_capacity"
-    discharge_energy_txt: str = "discharge_energy"
-    internal_resistance_txt: str = "internal_resistance"
-    power_txt: str = "power"
-    is_fc_data_txt: str = "is_fc_data"
-    step_index_txt: str = "step_index"
-    sub_step_index_txt: str = "sub_step_index"
-    step_time_txt: str = "step_time"
-    sub_step_time_txt: str = "sub_step_time"
-    test_id_txt: str = "test_id"
-    test_time_txt: str = "test_time"
-    voltage_txt: str = "voltage"
-    ref_voltage_txt: str = "reference_voltage"
-    dv_dt_txt: str = "dv_dt"
-    frequency_txt: str = "frequency"
-    amplitude_txt: str = "amplitude"
-    channel_id_txt: str = "channel_id"
-    data_flag_txt: str = "data_flag"
-    test_name_txt: str = "test_name"
-
-
-@dataclass
-class HeadersSummary(BaseHeaders):
-    """In addition to the headers defined here, the summary might also contain
-    specific headers (ending in _gravimetric or _areal).
-    """
-
-    postfixes = ["gravimetric", "areal"]
-
-    cycle_index: str = "cycle_index"
-    data_point: str = "data_point"
-    test_time: str = "test_time"
-    datetime: str = "date_time"
-    discharge_capacity_raw: str = "discharge_capacity"
-    charge_capacity_raw: str = "charge_capacity"
-    test_name: str = "test_name"
-    data_flag: str = "data_flag"
-    channel_id: str = "channel_id"
-
-    coulombic_efficiency: str = "coulombic_efficiency"
-    cumulated_coulombic_efficiency: str = "cumulated_coulombic_efficiency"
-
-    discharge_capacity: str = "discharge_capacity"
-    charge_capacity: str = "charge_capacity"
-    cumulated_charge_capacity: str = "cumulated_charge_capacity"
-    cumulated_discharge_capacity: str = "cumulated_discharge_capacity"
-
-    coulombic_difference: str = "coulombic_difference"
-    cumulated_coulombic_difference: str = "cumulated_coulombic_difference"
-    discharge_capacity_loss: str = "discharge_capacity_loss"
-    charge_capacity_loss: str = "charge_capacity_loss"
-    cumulated_discharge_capacity_loss: str = "cumulated_discharge_capacity_loss"
-    cumulated_charge_capacity_loss: str = "cumulated_charge_capacity_loss"
-
-    normalized_charge_capacity: str = "normalized_charge_capacity"
-    normalized_discharge_capacity: str = "normalized_discharge_capacity"
-
-    shifted_charge_capacity: str = "shifted_charge_capacity"
-    shifted_discharge_capacity: str = "shifted_discharge_capacity"
-
-    ir_discharge: str = "ir_discharge"
-    ir_charge: str = "ir_charge"
-    ocv_first_min: str = "ocv_first_min"
-    ocv_second_min: str = "ocv_second_min"
-    ocv_first_max: str = "ocv_first_max"
-    ocv_second_max: str = "ocv_second_max"
-    end_voltage_discharge: str = "end_voltage_discharge"
-    end_voltage_charge: str = "end_voltage_charge"
-    cumulated_ric_disconnect: str = "cumulated_ric_disconnect"
-    cumulated_ric_sei: str = "cumulated_ric_sei"
-    cumulated_ric: str = "cumulated_ric"
-    normalized_cycle_index: str = "normalized_cycle_index"
-    low_level: str = "low_level"
-    high_level: str = "high_level"
-
-    temperature_last: str = "temperature_last"
-    temperature_mean: str = "temperature_mean"
-
-    charge_c_rate: str = "charge_c_rate"
-    discharge_c_rate: str = "discharge_c_rate"
-    pre_aux: str = "aux_"
-
-    @property
-    def areal_charge_capacity(self) -> str:
-        warnings.warn(
-            "using old-type look-up (areal_charge_capacity) -> will be deprecated soon",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return f"{self.charge_capacity}_areal"
-
-    @property
-    def areal_discharge_capacity(self) -> str:
-        warnings.warn(
-            "using old-type look-up (areal_discharge_capacity) -> will be deprecated soon",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return f"{self.discharge_capacity}_areal"
-
-    @property
-    def specific_columns(self) -> List[str]:
-        return [
-            self.discharge_capacity,
-            self.charge_capacity,
-            self.cumulated_charge_capacity,
-            self.cumulated_discharge_capacity,
-            self.coulombic_difference,
-            self.cumulated_coulombic_difference,
-            self.discharge_capacity_loss,
-            self.charge_capacity_loss,
-            self.cumulated_discharge_capacity_loss,
-            self.cumulated_charge_capacity_loss,
-            self.shifted_charge_capacity,
-            self.shifted_discharge_capacity,
-            # self.cumulated_ric_disconnect,
-            # self.cumulated_ric_sei,
-            # self.cumulated_ric,
-            # self.normalized_cycle_index,
-        ]
-
-
-@dataclass
-class HeadersStepTable(BaseHeaders):
-    test: str = "test"
-    ustep: str = "ustep"
-    cycle: str = "cycle"
-    step: str = "step"
-    test_time: str = "test_time"
-    step_time: str = "step_time"
-    sub_step: str = "sub_step"
-    type: str = "type"
-    sub_type: str = "sub_type"
-    info: str = "info"
-    voltage: str = "voltage"
-    current: str = "current"
-    charge: str = "charge"
-    discharge: str = "discharge"
-    point: str = "point"
-    internal_resistance: str = "ir"
-    internal_resistance_change: str = "ir_pct_change"
-    rate_avr: str = "rate_avr"
-
-
-@dataclass
-class HeadersJournal(BaseHeaders):
-    filename: str = "filename"
-    mass: str = "mass"
-    total_mass: str = "total_mass"
-    loading: str = "loading"
-    area: str = "area"
-    nom_cap: str = "nom_cap"
-    experiment: str = "experiment"
-    fixed: str = "fixed"
-    label: str = "label"
-    cell_type: str = "cell_type"
-    instrument: str = "instrument"
-    raw_file_names: str = "raw_file_names"
-    cellpy_file_name: str = "cellpy_file_name"
-    group: str = "group"
-    sub_group: str = "sub_group"
-    comment: str = "comment"
-    argument: str = "argument"
-
-
-keys_journal_session = ["starred", "bad_cells", "bad_cycles", "notes"]
-
-headers_step_table = HeadersStepTable()
-headers_journal = HeadersJournal()
-headers_summary = HeadersSummary()
-headers_normal = HeadersNormal()
-cellpy_units = CellpyUnits()
-
-base_columns_float = [
-    headers_normal.test_time_txt,
-    headers_normal.step_time_txt,
-    headers_normal.current_txt,
-    headers_normal.voltage_txt,
-    headers_normal.ref_voltage_txt,
-    headers_normal.charge_capacity_txt,
-    headers_normal.discharge_capacity_txt,
-    headers_normal.internal_resistance_txt,
-]
-
-base_columns_int = [
-    headers_normal.data_point_txt,
-    headers_normal.step_index_txt,
-    headers_normal.cycle_index_txt,
-]
-
-
-def get_cellpy_units(*args, **kwargs) -> CellpyUnits:
-    """Returns an augmented global dictionary with units"""
-    return cellpy_units
-
-
-def get_default_output_units(*args, **kwargs) -> CellpyUnits:
-    """Returns an augmented dictionary with units to use as default."""
-    return CellpyUnits()
-
-
-def get_default_cellpy_file_raw_units(*args, **kwargs) -> CellpyUnits:
-    """Returns a dictionary with units to use as default for old versions of cellpy files"""
-    return CellpyUnits(
-        charge="Ah",
-        mass="mg",
-    )
-
-
-def get_default_raw_units(*args, **kwargs) -> CellpyUnits:
-    """Returns a dictionary with units as default for raw data"""
-    return CellpyUnits(
-        charge="Ah",
-        mass="mg",
-    )
-
-
-def get_default_raw_limits() -> CellpyLimits:
-    """Returns an augmented dictionary with units as default for raw data"""
-    return CellpyLimits()
-
-
-def get_headers_normal() -> HeadersNormal:
-    """Returns an augmented global dictionary containing the header-strings for the normal data
-    (used as column headers for the main data pandas DataFrames)"""
-    return headers_normal
-
-
-def get_headers_step_table() -> HeadersStepTable:
-    """Returns an augmented global dictionary containing the header-strings for the steps table
-    (used as column headers for the steps pandas DataFrames)"""
-    return headers_step_table
-
-
-def get_headers_journal() -> HeadersJournal:
-    """Returns an augmented global dictionary containing the header-strings for the journal (batch)
-    (used as column headers for the journal pandas DataFrames)"""
-    return headers_journal
-
-
-def get_headers_summary() -> HeadersSummary:
-    """Returns an augmented global dictionary containing the header-strings for the summary
-    (used as column headers for the summary pandas DataFrames)"""
-    return headers_summary
-
-
-def get_default_custom_headers_summary() -> HeadersSummary:
-    """Returns an augmented dictionary that can be used to create custom header-strings for the summary
-    (used as column headers for the summary pandas DataFrames)
-
-    This function is mainly implemented to provide an example.
-
-    """
-    # maybe I can do some tricks in here so that tab completion works in pycharm?
-    # solution: ctrl + space works
-    return HeadersSummary()
+"""Internal settings and definitions and functions for getting them."""
+import logging
+import warnings
+from collections import UserDict
+from dataclasses import dataclass, fields, asdict
+from typing import List, Optional
+
+import pandas as pd
+
+from cellpy import prms
+
+CELLPY_FILE_VERSION = 8
+MINIMUM_CELLPY_FILE_VERSION = 4
+STEP_TABLE_VERSION = 5
+RAW_TABLE_VERSION = 5
+SUMMARY_TABLE_VERSION = 7
+# if you change this, remember that both loading and saving uses this
+# constant at the moment, and check that loading old files still works
+# - and possibly refactor so that the old-file loaders contain the
+# appropriate pickle protocol:
+PICKLE_PROTOCOL = 4
+
+# For creating the sqlite database from Excel:
+TABLE_NAME_SQLITE = "cells"
+COLUMNS_EXCEL_PK = "id"
+COLUMNS_RENAMER = {
+    COLUMNS_EXCEL_PK: "pk",
+    "batch": "comment_history",
+    "cell_name": "name",
+    "exists": "cell_exists",
+    "group": "cell_group",
+    "raw_file_names": "raw_data",
+    "argument": "cell_spec",
+    "nom_cap": "nominal_capacity",
+    "freeze": "frozen",
+}
+ATTRS_TO_IMPORT_FROM_EXCEL_SQLITE = [
+    "name",
+    "label",
+    "project",
+    "cell_group",
+    "cellpy_file_name",
+    "instrument",
+    "cell_type",
+    "cell_design",
+    "channel",
+    "experiment_type",
+    "mass_active",
+    "area",
+    "mass_total",
+    "loading_active",
+    "nominal_capacity",
+    "comment_slurry",
+    "comment_cell",
+    "comment_general",
+    "comment_history",
+    "selected",
+    "freeze",
+    "cell_exists",
+]
+BATCH_ATTRS_TO_IMPORT_FROM_EXCEL_SQLITE = [
+    "comment_history",
+    "sub_batch_01",
+    "sub_batch_02",
+    "sub_batch_03",
+    "sub_batch_04",
+    "sub_batch_05",
+    "sub_batch_06",
+    "sub_batch_07",
+]
+
+
+OTHERPATHS = ["rawdatadir", "cellpydatadir"]
+
+
+@dataclass
+class CellpyMeta:
+    def update(self, as_list: bool = False, **kwargs):
+        """Updates from dictionary of form {key: [values]}
+
+        Args:
+            as_list (bool): pick only first scalar if True.
+            **kwargs (dict): key word attributes to update.
+
+        Returns:
+            None
+        """
+
+        for k, v in kwargs.items():
+            if not as_list:
+                v = v[0]
+            if hasattr(self, k):
+                logging.debug(f"{k} -> {v}")
+                setattr(self, k, v)
+            else:
+                logging.debug(f"[NOT-VALID]{k}:{v}")
+
+    def digest(self, as_list: bool = False, **kwargs):
+        """Pops from dictionary of form {key: [values]}
+
+        Args:
+            as_list (bool): pick only first scalar if True.
+            **kwargs (dict): key word attributes to pick.
+
+        Returns:
+            Dictionary containing the non-digested part.
+        """
+        not_digested = {}
+        for k, v in kwargs.items():
+            if not as_list:
+                v = v[0]
+            if hasattr(self, k):
+                logging.debug(f"{k} -> {v}")
+                setattr(self, k, v)
+            else:
+                logging.debug(f"{k}:{v} ->")
+                not_digested[k] = v
+        return not_digested
+
+    def to_frame(self):
+        """Converts to pandas dataframe"""
+        df = pd.DataFrame.from_dict(asdict(self), orient="index")
+        df.index.name = "key"
+        n_rows, n_cols = df.shape
+        if n_cols == 1:
+            columns = ["value"]
+        else:
+            columns = [f"value_{i:02}" for i in range(n_cols)]
+        df.columns = columns
+
+        return df
+
+
+@dataclass
+class CellpyMetaCommon(CellpyMeta):
+    # about test
+    cell_name: Optional[str] = None  # used as property
+    start_datetime: Optional[str] = None
+    time_zone: Optional[str] = None
+    comment: Optional[prms.CellPyDataConfig] = prms.CellInfo.comment
+    file_errors: Optional[str] = None  # not in use at the moment
+    raw_id: Optional[str] = None  # used as property
+    cellpy_file_version: int = CELLPY_FILE_VERSION
+
+    # about tester
+    tester_ID: Optional[prms.CellPyDataConfig] = None
+    tester_server_software_version: Optional[prms.CellPyDataConfig] = None
+    tester_client_software_version: Optional[prms.CellPyDataConfig] = None
+    tester_calibration_date: Optional[prms.CellPyDataConfig] = None
+
+    # about cell
+    material: Optional[prms.CellPyDataConfig] = prms.Materials.default_material
+    # TODO @jepe: Maybe we should use values with units here instead (pint)?
+    mass: Optional[
+        prms.CellPyDataConfig
+    ] = prms.Materials.default_mass  # active material
+    tot_mass: Optional[
+        prms.CellPyDataConfig
+    ] = prms.Materials.default_mass  # total material
+    nom_cap: Optional[
+        prms.CellPyDataConfig
+    ] = prms.Materials.default_nom_cap  # nominal capacity   # used as property
+    nom_cap_specifics: Optional[
+        prms.CellPyDataConfig
+    ] = (
+        prms.Materials.default_nom_cap_specifics
+    )  # nominal capacity type  # used as property
+
+    active_electrode_area: Optional[
+        prms.CellPyDataConfig
+    ] = prms.CellInfo.active_electrode_area
+    active_electrode_thickness: Optional[
+        prms.CellPyDataConfig
+    ] = prms.CellInfo.active_electrode_thickness
+    electrolyte_volume: Optional[
+        prms.CellPyDataConfig
+    ] = prms.CellInfo.electrolyte_volume
+
+    electrolyte_type: Optional[prms.CellPyDataConfig] = prms.CellInfo.electrolyte_type
+    active_electrode_type: Optional[
+        prms.CellPyDataConfig
+    ] = prms.CellInfo.active_electrode_type
+    counter_electrode_type: Optional[
+        prms.CellPyDataConfig
+    ] = prms.CellInfo.counter_electrode_type
+    reference_electrode_type: Optional[
+        prms.CellPyDataConfig
+    ] = prms.CellInfo.reference_electrode_type
+    experiment_type: Optional[prms.CellPyDataConfig] = prms.CellInfo.experiment_type
+    cell_type: Optional[prms.CellPyDataConfig] = prms.CellInfo.cell_type
+    separator_type: Optional[prms.CellPyDataConfig] = prms.CellInfo.separator_type
+    active_electrode_current_collector: Optional[
+        prms.CellPyDataConfig
+    ] = prms.CellInfo.active_electrode_current_collector
+    reference_electrode_current_collector: Optional[
+        prms.CellPyDataConfig
+    ] = prms.CellInfo.reference_electrode_current_collector
+
+
+@dataclass
+class CellpyMetaIndividualTest(CellpyMeta):
+    # ---------------- test dependent -------------------------------
+    channel_index: Optional[prms.CellPyDataConfig] = None
+    creator: Optional[str] = None
+    schedule_file_name = None
+    test_type: Optional[
+        prms.CellPyDataConfig
+    ] = None  # Not used (and might be put inside test_ID)
+    voltage_lim_low: Optional[prms.CellPyDataConfig] = prms.CellInfo.voltage_lim_low
+    voltage_lim_high: Optional[prms.CellPyDataConfig] = prms.CellInfo.voltage_lim_high
+    cycle_mode: Optional[prms.CellPyDataConfig] = prms.Reader.cycle_mode
+    test_ID: Optional[
+        prms.CellPyDataConfig
+    ] = None  # id for the test - currently just a number; could become a list or more in the future
+
+
+# TODO: remove import of this
+class HeaderDict(UserDict):
+    """Sub-classing dict to allow for tab-completion."""
+
+    def __setitem__(self, key: str, value: str) -> None:
+        if key == "data":
+            raise KeyError("protected key")
+        super().__setitem__(key, value)
+        self.__dict__[key] = value
+
+
+@dataclass
+class DictLikeClass:
+    """Add some dunder-methods so that it does not break old code that used
+    dictionaries for storing settings
+
+    Remarks: it is not a complete dictionary experience - for example,
+    setting new attributes (new keys) is not supported (raises ``KeyError``
+    if using the typical dict setting method) since it uses the
+    ``dataclasses.fields`` method to find its members.
+
+    """
+
+    def __getitem__(self, key):
+        if key not in self._field_names:
+            logging.debug(f"{key} not in fields")
+        try:
+            return getattr(self, key)
+        except AttributeError:
+            raise KeyError(f"missing key: {key}")
+
+    def __setitem__(self, key, value):
+        if key not in self._field_names:
+            raise KeyError(f"creating new key not allowed: {key}")
+        setattr(self, key, value)
+
+    def __missing__(self, key):
+        raise KeyError
+
+    @property
+    def _field_names(self):
+        return [field.name for field in fields(self)]
+
+    def __iter__(self):
+        for field in self._field_names:
+            yield field
+
+    def _value_iter(self):
+        for field in self._field_names:
+            yield getattr(self, field)
+
+    def keys(self):
+        return [key for key in self.__iter__()]
+
+    def values(self):
+        return [v for v in self._value_iter()]
+
+    def items(self):
+        return zip(self.keys(), self.values())
+
+
+@dataclass
+class BaseSettings(DictLikeClass):
+    """Base class for internal cellpy settings.
+
+    Usage::
+
+         @dataclass
+         class MyCoolCellpySetting(BaseSetting):
+             var1: str = "first var"
+             var2: int = 12
+
+    """
+
+    def get(self, key):
+        """Get the value (postfixes not supported)."""
+        if key not in self.keys():
+            logging.critical(f"the column header '{key}' not found")
+            return
+        else:
+            return self[key]
+
+    def to_frame(self):
+        """Converts to pandas dataframe"""
+        df = pd.DataFrame.from_dict(asdict(self), orient="index")
+        df.index.name = "key"
+        n_rows, n_cols = df.shape
+        if n_cols == 1:
+            columns = ["value"]
+        else:
+            columns = [f"value_{i:02}" for i in range(n_cols)]
+        df.columns = columns
+
+        return df
+
+
+@dataclass
+class BaseHeaders(BaseSettings):
+    """Extending BaseSetting so that it's allowed to add postfixes.
+
+    Example:
+         >>> header["key_postfix"]  # returns "value_postfix"
+    """
+
+    postfixes = []
+
+    def __getitem__(self, key):
+        postfix = ""
+        if key not in self._field_names:
+            # check postfix:
+            subs = key.split("_")
+            _key = "_".join(subs[:-1])
+            _postfix = subs[-1]
+            if _postfix in self.postfixes:
+                postfix = f"_{_postfix}"
+                key = _key
+        try:
+            v = getattr(self, key)
+            return f"{v}{postfix}"
+        except AttributeError:
+            raise KeyError(f"missing key: {key}")
+
+
+@dataclass
+class InstrumentSettings(DictLikeClass):
+    """Base class for instrument settings.
+
+    Usage::
+
+        @dataclass
+        class MyCoolInstrumentSetting(InstrumentSettings):
+            var1: str = "first var"
+            var2: int = 12
+
+    Remark! Try to use it as you would use a normal dataclass.
+
+    """
+
+    ...
+
+
+@dataclass
+class CellpyUnits(BaseSettings):
+    """These are the units used inside Cellpy.
+
+    At least two sets of units needs to be defined; `cellpy_units` and `raw_units`.
+    The `data.raw` dataframe is given in `raw_units` where the units are defined
+    inside the instrument loader used. Since the `data.steps` dataframe is a summary of
+    the step statistics from the `data.raw` dataframe, this also uses the `raw_units`.
+    The `data.summary` dataframe contains columns with values directly from the `data.raw` dataframe
+    given in `raw_units` as well as calculated columns given in `cellpy_units`.
+
+    Remark that all input to cellpy through user interaction (or utils) should be in `cellpy_units`.
+    This is also true for meta-data collected from the raw files. The instrument loader needs to
+    take care of the translation from its raw units to `cellpy_units` during loading the raw data
+    file for the meta-data (remark that this is not necessary and not recommended for the actual
+    "raw" data that is going to be stored in the `data.raw` dataframe).
+
+    As of 2022.09.29, cellpy does not automatically ensure unit conversion for input of meta-data,
+    but has an internal method (`CellPyData.to_cellpy_units`) that can be used.
+
+    These are the different attributes currently supported for data in the dataframes::
+
+        current: str = "A"
+        charge: str = "mAh"
+        voltage: str = "V"
+        time: str = "sec"
+        resistance: str = "Ohms"
+        power: str = "W"
+        energy: str = "Wh"
+        frequency: str = "hz"
+
+    And here are the different attributes currently supported for meta-data::
+
+        # output-units for specific capacity etc.
+        specific_gravimetric: str = "g"
+        specific_areal: str = "cm**2"  # used for calculating specific capacity etc.
+        specific_volumetric: str = "cm**3"  # used for calculating specific capacity etc.
+
+        # other meta-data
+        nominal_capacity: str = "mAh/g"  # used for calculating rates etc.
+        mass: str = "mg"
+        length: str = "cm"
+        area: str = "cm**2"
+        volume: str = "cm**3"
+        temperature: str = "C"
+
+    """
+
+    current: str = "A"
+    charge: str = "mAh"
+    voltage: str = "V"
+    time: str = "sec"
+    resistance: str = "ohm"
+    power: str = "W"
+    energy: str = "Wh"
+    frequency: str = "hz"
+    mass: str = "mg"  # for mass
+    nominal_capacity: str = "mAh/g"
+    specific_gravimetric: str = "g"  # g in specific capacity etc
+    specific_areal: str = "cm**2"  # m2 in specific capacity etc
+    specific_volumetric: str = "cm**3"  # m3 in specific capacity etc
+
+    length: str = "cm"
+    area: str = "cm**2"
+    volume: str = "cm**3"
+    temperature: str = "C"
+    pressure: str = "bar"
+
+    def update(self, new_units: dict):
+        """Update the units."""
+
+        logging.debug(f"{new_units=}")
+        for k in new_units:
+            if k in self.keys():
+                self[k] = new_units[k]
+
+
+@dataclass
+class CellpyLimits(BaseSettings):
+    """These are the limits used inside ``cellpy`` for finding step types.
+
+    Since all instruments have an inherent inaccuracy, it is naive to assume that
+    for example the voltage within a constant voltage step does not change at all.
+    Therefore, we need to define some limits for what we consider to be a constant and
+    what we assume to be zero.
+
+    """
+
+    current_hard: float = 1e-13
+    current_soft: float = 1e-05
+    stable_current_hard: float = 2.0
+    stable_current_soft: float = 4.0
+    stable_voltage_hard: float = 2.0
+    stable_voltage_soft: float = 4.0
+    stable_charge_hard: float = 0.9
+    stable_charge_soft: float = 5.0
+    ir_change: float = 1e-05
+
+
+@dataclass
+class HeadersNormal(BaseHeaders):
+    aci_phase_angle_txt: str = "aci_phase_angle"
+    ref_aci_phase_angle_txt: str = "ref_aci_phase_angle"
+    ac_impedance_txt: str = "ac_impedance"
+    ref_ac_impedance_txt: str = "ref_ac_impedance"
+    charge_capacity_txt: str = "charge_capacity"
+    charge_energy_txt: str = "charge_energy"
+    current_txt: str = "current"
+    cycle_index_txt: str = "cycle_index"
+    data_point_txt: str = "data_point"
+    datetime_txt: str = "date_time"
+    discharge_capacity_txt: str = "discharge_capacity"
+    discharge_energy_txt: str = "discharge_energy"
+    internal_resistance_txt: str = "internal_resistance"
+    power_txt: str = "power"
+    is_fc_data_txt: str = "is_fc_data"
+    step_index_txt: str = "step_index"
+    sub_step_index_txt: str = "sub_step_index"
+    step_time_txt: str = "step_time"
+    sub_step_time_txt: str = "sub_step_time"
+    test_id_txt: str = "test_id"
+    test_time_txt: str = "test_time"
+    voltage_txt: str = "voltage"
+    ref_voltage_txt: str = "reference_voltage"
+    dv_dt_txt: str = "dv_dt"
+    frequency_txt: str = "frequency"
+    amplitude_txt: str = "amplitude"
+    channel_id_txt: str = "channel_id"
+    data_flag_txt: str = "data_flag"
+    test_name_txt: str = "test_name"
+
+
+@dataclass
+class HeadersSummary(BaseHeaders):
+    """In addition to the headers defined here, the summary might also contain
+    specific headers (ending in _gravimetric or _areal).
+    """
+
+    postfixes = ["gravimetric", "areal"]
+
+    cycle_index: str = "cycle_index"
+    data_point: str = "data_point"
+    test_time: str = "test_time"
+    datetime: str = "date_time"
+    discharge_capacity_raw: str = "discharge_capacity"
+    charge_capacity_raw: str = "charge_capacity"
+    test_name: str = "test_name"
+    data_flag: str = "data_flag"
+    channel_id: str = "channel_id"
+
+    coulombic_efficiency: str = "coulombic_efficiency"
+    cumulated_coulombic_efficiency: str = "cumulated_coulombic_efficiency"
+
+    discharge_capacity: str = "discharge_capacity"
+    charge_capacity: str = "charge_capacity"
+    cumulated_charge_capacity: str = "cumulated_charge_capacity"
+    cumulated_discharge_capacity: str = "cumulated_discharge_capacity"
+
+    coulombic_difference: str = "coulombic_difference"
+    cumulated_coulombic_difference: str = "cumulated_coulombic_difference"
+    discharge_capacity_loss: str = "discharge_capacity_loss"
+    charge_capacity_loss: str = "charge_capacity_loss"
+    cumulated_discharge_capacity_loss: str = "cumulated_discharge_capacity_loss"
+    cumulated_charge_capacity_loss: str = "cumulated_charge_capacity_loss"
+
+    normalized_charge_capacity: str = "normalized_charge_capacity"
+    normalized_discharge_capacity: str = "normalized_discharge_capacity"
+
+    shifted_charge_capacity: str = "shifted_charge_capacity"
+    shifted_discharge_capacity: str = "shifted_discharge_capacity"
+
+    ir_discharge: str = "ir_discharge"
+    ir_charge: str = "ir_charge"
+    ocv_first_min: str = "ocv_first_min"
+    ocv_second_min: str = "ocv_second_min"
+    ocv_first_max: str = "ocv_first_max"
+    ocv_second_max: str = "ocv_second_max"
+    end_voltage_discharge: str = "end_voltage_discharge"
+    end_voltage_charge: str = "end_voltage_charge"
+    cumulated_ric_disconnect: str = "cumulated_ric_disconnect"
+    cumulated_ric_sei: str = "cumulated_ric_sei"
+    cumulated_ric: str = "cumulated_ric"
+    normalized_cycle_index: str = "normalized_cycle_index"
+    low_level: str = "low_level"
+    high_level: str = "high_level"
+
+    temperature_last: str = "temperature_last"
+    temperature_mean: str = "temperature_mean"
+
+    charge_c_rate: str = "charge_c_rate"
+    discharge_c_rate: str = "discharge_c_rate"
+    pre_aux: str = "aux_"
+
+    @property
+    def areal_charge_capacity(self) -> str:
+        warnings.warn(
+            "using old-type look-up (areal_charge_capacity) -> will be deprecated soon",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return f"{self.charge_capacity}_areal"
+
+    @property
+    def areal_discharge_capacity(self) -> str:
+        warnings.warn(
+            "using old-type look-up (areal_discharge_capacity) -> will be deprecated soon",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return f"{self.discharge_capacity}_areal"
+
+    @property
+    def specific_columns(self) -> List[str]:
+        return [
+            self.discharge_capacity,
+            self.charge_capacity,
+            self.cumulated_charge_capacity,
+            self.cumulated_discharge_capacity,
+            self.coulombic_difference,
+            self.cumulated_coulombic_difference,
+            self.discharge_capacity_loss,
+            self.charge_capacity_loss,
+            self.cumulated_discharge_capacity_loss,
+            self.cumulated_charge_capacity_loss,
+            self.shifted_charge_capacity,
+            self.shifted_discharge_capacity,
+            # self.cumulated_ric_disconnect,
+            # self.cumulated_ric_sei,
+            # self.cumulated_ric,
+            # self.normalized_cycle_index,
+        ]
+
+
+@dataclass
+class HeadersStepTable(BaseHeaders):
+    test: str = "test"
+    ustep: str = "ustep"
+    cycle: str = "cycle"
+    step: str = "step"
+    test_time: str = "test_time"
+    step_time: str = "step_time"
+    sub_step: str = "sub_step"
+    type: str = "type"
+    sub_type: str = "sub_type"
+    info: str = "info"
+    voltage: str = "voltage"
+    current: str = "current"
+    charge: str = "charge"
+    discharge: str = "discharge"
+    point: str = "point"
+    internal_resistance: str = "ir"
+    internal_resistance_change: str = "ir_pct_change"
+    rate_avr: str = "rate_avr"
+
+
+@dataclass
+class HeadersJournal(BaseHeaders):
+    filename: str = "filename"
+    mass: str = "mass"
+    total_mass: str = "total_mass"
+    loading: str = "loading"
+    area: str = "area"
+    nom_cap: str = "nom_cap"
+    experiment: str = "experiment"
+    fixed: str = "fixed"
+    label: str = "label"
+    cell_type: str = "cell_type"
+    instrument: str = "instrument"
+    raw_file_names: str = "raw_file_names"
+    cellpy_file_name: str = "cellpy_file_name"
+    group: str = "group"
+    sub_group: str = "sub_group"
+    comment: str = "comment"
+    argument: str = "argument"
+
+
+keys_journal_session = ["starred", "bad_cells", "bad_cycles", "notes"]
+
+headers_step_table = HeadersStepTable()
+headers_journal = HeadersJournal()
+headers_summary = HeadersSummary()
+headers_normal = HeadersNormal()
+cellpy_units = CellpyUnits()
+
+base_columns_float = [
+    headers_normal.test_time_txt,
+    headers_normal.step_time_txt,
+    headers_normal.current_txt,
+    headers_normal.voltage_txt,
+    headers_normal.ref_voltage_txt,
+    headers_normal.charge_capacity_txt,
+    headers_normal.discharge_capacity_txt,
+    headers_normal.internal_resistance_txt,
+]
+
+base_columns_int = [
+    headers_normal.data_point_txt,
+    headers_normal.step_index_txt,
+    headers_normal.cycle_index_txt,
+]
+
+
+def get_cellpy_units(*args, **kwargs) -> CellpyUnits:
+    """Returns an augmented global dictionary with units"""
+    return cellpy_units
+
+
+def get_default_output_units(*args, **kwargs) -> CellpyUnits:
+    """Returns an augmented dictionary with units to use as default."""
+    return CellpyUnits()
+
+
+def get_default_cellpy_file_raw_units(*args, **kwargs) -> CellpyUnits:
+    """Returns a dictionary with units to use as default for old versions of cellpy files"""
+    return CellpyUnits(
+        charge="Ah",
+        mass="mg",
+    )
+
+
+def get_default_raw_units(*args, **kwargs) -> CellpyUnits:
+    """Returns a dictionary with units as default for raw data"""
+    return CellpyUnits(
+        charge="Ah",
+        mass="mg",
+    )
+
+
+def get_default_raw_limits() -> CellpyLimits:
+    """Returns an augmented dictionary with units as default for raw data"""
+    return CellpyLimits()
+
+
+def get_headers_normal() -> HeadersNormal:
+    """Returns an augmented global dictionary containing the header-strings for the normal data
+    (used as column headers for the main data pandas DataFrames)"""
+    return headers_normal
+
+
+def get_headers_step_table() -> HeadersStepTable:
+    """Returns an augmented global dictionary containing the header-strings for the steps table
+    (used as column headers for the steps pandas DataFrames)"""
+    return headers_step_table
+
+
+def get_headers_journal() -> HeadersJournal:
+    """Returns an augmented global dictionary containing the header-strings for the journal (batch)
+    (used as column headers for the journal pandas DataFrames)"""
+    return headers_journal
+
+
+def get_headers_summary() -> HeadersSummary:
+    """Returns an augmented global dictionary containing the header-strings for the summary
+    (used as column headers for the summary pandas DataFrames)"""
+    return headers_summary
+
+
+def get_default_custom_headers_summary() -> HeadersSummary:
+    """Returns an augmented dictionary that can be used to create custom header-strings for the summary
+    (used as column headers for the summary pandas DataFrames)
+
+    This function is mainly implemented to provide an example.
+
+    """
+    # maybe I can do some tricks in here so that tab completion works in pycharm?
+    # solution: ctrl + space works
+    return HeadersSummary()
```

### Comparing `cellpy-1.0.0a7/cellpy/parameters/legacy/update_headers.py` & `cellpy-1.0.0a8/cellpy/parameters/legacy/update_headers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/parameters/prmreader.py` & `cellpy-1.0.0a8/cellpy/parameters/prmreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/parameters/prms.py` & `cellpy-1.0.0a8/cellpy/parameters/prms.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/cellreader.py` & `cellpy-1.0.0a8/cellpy/readers/cellreader.py`

 * *Files 1% similar despite different names*

```diff
@@ -3167,14 +3167,20 @@
             filename = f"{pre}_cellpy.xlsx"
             filename = Path(filename).resolve()
             logging.critical(f"generating filename: {filename}")
 
         summary_frame = self.data.summary
         meta_common_frame = self.data.meta_common.to_frame()
         meta_test_dependent_frame = self.data.meta_test_dependent.to_frame()
+        cellpy_units = self.cellpy_units.to_frame()
+        cellpy_units.index = "cellpy_units_" + cellpy_units.index
+        raw_units = self.raw_units.to_frame()
+        raw_units.index = "raw_units_" + raw_units.index
+
+        meta_common_frame = pd.concat([meta_common_frame, cellpy_units, raw_units])
 
         with pd.ExcelWriter(filename, engine="openpyxl") as writer:
             meta_common_frame.to_excel(
                 writer, sheet_name="meta_common", **to_excel_method_kwargs
             )
             meta_test_dependent_frame.to_excel(
                 writer, sheet_name="meta_test_dependent", **to_excel_method_kwargs
@@ -6078,20 +6084,20 @@
     cellpy_file = Path("../../tmp/20160805_test001_45_cc.h5")
     excel_file = Path("../../tmp/20160805_test001_45_cc.xlsx")
 
     c = get(raw_file, mass=1.0, nominal_capacity=3579)
     print("loaded ...")
     c.to_excel(excel_file)
     print("saved ...")
-
-    c.save(cellpy_file)
-    c2 = get(cellpy_file)
-    print("loaded again ...")
-    c2.to_excel(excel_file, raw=True, cycles=True)
-    print("saved again ...")
+    #
+    # c.save(cellpy_file)
+    # c2 = get(cellpy_file)
+    # print("loaded again ...")
+    # c2.to_excel(excel_file, raw=True, cycles=True)
+    # print("saved again ...")
 
 
 def check_excel():
     import openpyxl
     from openpyxl.styles import Border, Side
     import pandas as pd
```

### Comparing `cellpy-1.0.0a7/cellpy/readers/core.py` & `cellpy-1.0.0a8/cellpy/readers/core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/dbreader.py` & `cellpy-1.0.0a8/cellpy/readers/dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/filefinder.py` & `cellpy-1.0.0a8/cellpy/readers/filefinder.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/arbin_res.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/arbin_res.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/arbin_sql.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/arbin_sql_7.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_7.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/arbin_sql_csv.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/arbin_sql_h5.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_h5.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/arbin_sql_xlsx.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_xlsx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/base.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/base.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/biologics_mpr.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/biologics_mpr.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/configurations/__init__.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/configurations/maccor_txt_four.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_four.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/configurations/maccor_txt_one.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_one.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/configurations/maccor_txt_three.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_three.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/configurations/maccor_txt_two.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_two.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/configurations/maccor_txt_zero.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/configurations/neware_txt_zero.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/neware_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/custom.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/custom.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/ext_nda_reader.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/ext_nda_reader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/local_instrument.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/local_instrument.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/maccor_txt.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/maccor_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/neware_txt.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/neware_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/pec_csv.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/pec_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/processors/post_processors.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/processors/post_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/instruments/processors/pre_processors.py` & `cellpy-1.0.0a8/cellpy/readers/instruments/processors/pre_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/readers/sql_dbreader.py` & `cellpy-1.0.0a8/cellpy/readers/sql_dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/batch.py` & `cellpy-1.0.0a8/cellpy/utils/batch.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_analyzers.py` & `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_analyzers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_core.py` & `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_experiments.py` & `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_experiments.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_exporters.py` & `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_exporters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_helpers.py` & `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_journals.py` & `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_journals.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/batch_tools/batch_plotters.py` & `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_plotters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/batch_tools/dumpers.py` & `cellpy-1.0.0a8/cellpy/utils/batch_tools/dumpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/batch_tools/engines.py` & `cellpy-1.0.0a8/cellpy/utils/batch_tools/engines.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/batch_tools/sqlite_from_excel_db.py` & `cellpy-1.0.0a8/cellpy/utils/batch_tools/sqlite_from_excel_db.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/collectors.py` & `cellpy-1.0.0a8/cellpy/utils/collectors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/collectors_old.py` & `cellpy-1.0.0a8/cellpy/utils/collectors_old.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/data/20160805_test001_45_cc.h5` & `cellpy-1.0.0a8/cellpy/utils/data/20160805_test001_45_cc.h5`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/data/raw/20160805_test001_45_cc_01.res` & `cellpy-1.0.0a8/cellpy/utils/data/raw/20160805_test001_45_cc_01.res`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/easyplot.py` & `cellpy-1.0.0a8/cellpy/utils/easyplot.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/example_data.py` & `cellpy-1.0.0a8/cellpy/utils/example_data.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/helpers.py` & `cellpy-1.0.0a8/cellpy/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/ica.py` & `cellpy-1.0.0a8/cellpy/utils/ica.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/ocv_rlx.py` & `cellpy-1.0.0a8/cellpy/utils/ocv_rlx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/plotutils.py` & `cellpy-1.0.0a8/cellpy/utils/plotutils.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy/utils/processor.py` & `cellpy-1.0.0a8/cellpy/utils/processor.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/cellpy.egg-info/PKG-INFO` & `cellpy-1.0.0a8/cellpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cellpy-1.0.0a7/cellpy.egg-info/SOURCES.txt` & `cellpy-1.0.0a8/cellpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/Makefile` & `cellpy-1.0.0a8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png` & `cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png` & `cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png` & `cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png` & `cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png` & `cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png` & `cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png` & `cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png` & `cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png` & `cellpy-1.0.0a8/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png` & `cellpy-1.0.0a8/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png` & `cellpy-1.0.0a8/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png` & `cellpy-1.0.0a8/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png` & `cellpy-1.0.0a8/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png` & `cellpy-1.0.0a8/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png` & `cellpy-1.0.0a8/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png` & `cellpy-1.0.0a8/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png` & `cellpy-1.0.0a8/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png` & `cellpy-1.0.0a8/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/templates_jupyterlab_001.png` & `cellpy-1.0.0a8/docs/_build/_images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/tutorials_utils_plotting_fig1.png` & `cellpy-1.0.0a8/docs/_build/_images/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/_build/_images/tutorials_utils_plotting_fig2.png` & `cellpy-1.0.0a8/docs/_build/_images/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/adapted_readme.rst` & `cellpy-1.0.0a8/docs/adapted_readme.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/conf.py` & `cellpy-1.0.0a8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/developers_guide/dev_cellpy_data_structure.rst` & `cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_data_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/developers_guide/dev_cellpy_folder_structure.rst` & `cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_folder_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/developers_guide/dev_cellpy_packaging_pypi.rst` & `cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_packaging_pypi.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/developers_guide/dev_cellpy_setup.rst` & `cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_setup.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/developers_guide/dev_conda_package.rst` & `cellpy-1.0.0a8/docs/developers_guide/dev_conda_package.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/developers_guide/dev_docs.rst` & `cellpy-1.0.0a8/docs/developers_guide/dev_docs.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/developers_guide/dev_loaders_and_instruments.rst` & `cellpy-1.0.0a8/docs/developers_guide/dev_loaders_and_instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/developers_guide/dev_various.rst` & `cellpy-1.0.0a8/docs/developers_guide/dev_various.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/05_configuring.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/05_configuring.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/06_pandas.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/06_pandas.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png` & `cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png` & `cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/tips_and_tricks.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/tips_and_tricks.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/utils/batch.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/utils/batch.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png` & `cellpy-1.0.0a8/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png` & `cellpy-1.0.0a8/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/utils/ica.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/utils/ica.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/utils/plotting.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/utils/plotting.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst` & `cellpy-1.0.0a8/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/figures/cellpy-icon-bw.png` & `cellpy-1.0.0a8/docs/figures/cellpy-icon-bw.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/figures/cellpy-logo-v1.png` & `cellpy-1.0.0a8/docs/figures/cellpy-logo-v1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/index.rst` & `cellpy-1.0.0a8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/main_description/formats.rst` & `cellpy-1.0.0a8/docs/main_description/formats.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/main_description/installation.rst` & `cellpy-1.0.0a8/docs/main_description/installation.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/main_description/usage.rst` & `cellpy-1.0.0a8/docs/main_description/usage.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/make.bat` & `cellpy-1.0.0a8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/source/cellpy.parameters.rst` & `cellpy-1.0.0a8/docs/source/cellpy.parameters.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/source/cellpy.readers.instruments.configurations.rst` & `cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.configurations.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/source/cellpy.readers.instruments.loader_specific_modules.rst` & `cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.loader_specific_modules.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/source/cellpy.readers.instruments.processors.rst` & `cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.processors.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/source/cellpy.readers.instruments.rst` & `cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/source/cellpy.readers.rst` & `cellpy-1.0.0a8/docs/source/cellpy.readers.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/source/cellpy.rst` & `cellpy-1.0.0a8/docs/source/cellpy.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/source/cellpy.utils.batch_tools.rst` & `cellpy-1.0.0a8/docs/source/cellpy.utils.batch_tools.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/docs/source/cellpy.utils.rst` & `cellpy-1.0.0a8/docs/source/cellpy.utils.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a7/setup.py` & `cellpy-1.0.0a8/setup.py`

 * *Files identical despite different names*

