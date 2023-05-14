# Comparing `tmp/dash-connectivity-viewer-2.0.4.tar.gz` & `tmp/dash-connectivity-viewer-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-connectivity-viewer-2.0.4.tar", last modified: Sat May 13 00:19:11 2023, max compression
+gzip compressed data, was "dash-connectivity-viewer-2.0.5.tar", last modified: Sun May 14 21:44:17 2023, max compression
```

## Comparing `dash-connectivity-viewer-2.0.4.tar` & `dash-connectivity-viewer-2.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-13 00:19:11.207229 dash-connectivity-viewer-2.0.4/
--rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash-connectivity-viewer-2.0.4/LICENSE.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.4/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-13 00:19:11.206631 dash-connectivity-viewer-2.0.4/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.4/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-13 00:19:11.185507 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/
--rw-r--r--   0 caseysm    (501) staff       (20)       22 2023-05-13 00:18:50.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/__init__.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-13 00:19:11.192928 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/
--rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    24594 2023-05-13 00:17:14.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6156 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
--rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    20418 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/layout.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4439 2023-05-12 23:41:48.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-13 00:19:11.195050 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14456 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_table/ct_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14861 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-13 00:19:11.199231 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/
--rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5184 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/dash_url_helper.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-13 00:19:11.201161 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/data/
--rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/data/height_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)    10088 2023-05-12 23:38:21.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/dataframe_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    13477 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/link_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4043 2023-04-25 19:19:28.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/lookup_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)    11370 2023-05-12 23:38:23.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/neuron_data_base.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3756 2023-04-25 19:21:22.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/schema_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3950 2023-05-12 22:52:58.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/table_lookup.py
--rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/transform_utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-13 00:19:11.205509 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/connectivity_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/connectivity_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    13817 2023-05-13 00:16:13.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/connectivity_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/connectivity_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     9093 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/connectivity_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-13 00:19:11.188637 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-13 00:19:11.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     1990 2023-05-13 00:19:11.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-05-13 00:19:11.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      174 2023-05-13 00:19:11.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       25 2023-05-13 00:19:11.000000 dash-connectivity-viewer-2.0.4/dash_connectivity_viewer.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      173 2023-05-12 20:41:16.000000 dash-connectivity-viewer-2.0.4/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-05-13 00:19:11.207358 dash-connectivity-viewer-2.0.4/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.4/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-14 21:44:17.725775 dash-connectivity-viewer-2.0.5/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash-connectivity-viewer-2.0.5/LICENSE.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.5/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-14 21:44:17.725420 dash-connectivity-viewer-2.0.5/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.5/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-14 21:44:17.708732 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/
+-rw-r--r--   0 caseysm    (501) staff       (20)       22 2023-05-14 20:19:19.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/__init__.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-14 21:44:17.713408 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/
+-rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    24594 2023-05-13 00:17:14.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6156 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
+-rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    20408 2023-05-14 19:13:50.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/layout.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4439 2023-05-12 23:41:48.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-14 21:44:17.715011 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    14472 2023-05-14 19:13:28.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_table/ct_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    14841 2023-05-14 19:13:16.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-14 21:44:17.721182 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/
+-rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5184 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/dash_url_helper.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-14 21:44:17.722160 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/data/
+-rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/data/height_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)    10088 2023-05-12 23:38:21.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/dataframe_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    13477 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/link_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3942 2023-05-14 20:42:12.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/lookup_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    11370 2023-05-12 23:38:23.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/neuron_data_base.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3756 2023-04-25 19:21:22.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/schema_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3950 2023-05-14 19:10:55.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/table_lookup.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/transform_utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-14 21:44:17.724149 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/connectivity_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/connectivity_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    13817 2023-05-14 19:07:55.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/connectivity_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/connectivity_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9093 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/connectivity_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-14 21:44:17.710142 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-14 21:44:17.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     1990 2023-05-14 21:44:17.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-05-14 21:44:17.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      179 2023-05-14 21:44:17.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       25 2023-05-14 21:44:17.000000 dash-connectivity-viewer-2.0.5/dash_connectivity_viewer.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      178 2023-05-14 19:37:50.000000 dash-connectivity-viewer-2.0.5/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-05-14 21:44:17.725843 dash-connectivity-viewer-2.0.5/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.5/setup.py
```

### Comparing `dash-connectivity-viewer-2.0.4/LICENSE.txt` & `dash-connectivity-viewer-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/PKG-INFO` & `dash-connectivity-viewer-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-connectivity-viewer
-Version: 2.0.4
+Version: 2.0.5
 Summary: Dash connectivity viewer for CAVE data
 Home-page: https://github.com/ceesem/dash-connectivity-viewer
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/__init__.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/callbacks.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/config.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/layout.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                 ],
                 justify="start",
             ),
             dbc.Row(
                 [
                     dbc.Col(
                         [
-                            html.Div("Cell Type Table:"),
+                            html.Div("Table:"),
                             dcc.Dropdown(
                                 **create_component_kwargs(
                                     state,
                                     id_inner="cell-type-table-dropdown",
                                     options=[],
                                     value="",
                                     clearable=True,
```

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_table/__init__.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_table/callbacks.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_table/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             client = make_client(datastack, c.server_address)
             info_cache = client.info.get_datastack_info()
             info_cache["global_server"] = client.server_address
         except Exception as e:
             return [], str(e), "", EMPTY_INFO_CACHE, "danger", c.data_resolution
 
         if cell_type_table is None:
-            return [], "No Cell Type Table Selected", "", info_cache, "info", c.data_resolution
+            return [], "No Table Selected", "", info_cache, "info", c.data_resolution
 
         if len(anno_id) == 0:
             anno_id = None
         else:
             anno_id = [int(x) for x in anno_id.split(",")]
 
         live_query = len(live_query_toggle) == 1
@@ -230,18 +230,19 @@
                 cell_type_table,
                 client,
                 c,
                 id_query=anno_id,
                 id_query_type=anno_type_lookup[id_type],
                 column_query=annotation_filter,
                 timestamp=timestamp,
+                is_live=live_query,
             )
             df = tv.table_data()
             if live_query:
-                output_report = f"Current state of cell type table {cell_type_table}"
+                output_report = f"Current state of table {cell_type_table}"
             else:
                 output_report = f"Table {cell_type_table} materialized on {timestamp_ngl:%m/%d/%Y} (v{client.materialize.version})"
             output_color = "success"
         except Exception as e:
             df = pd.DataFrame(columns=c.ct_table_columns)
             output_report = str(e)
             output_color = "danger"
```

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_table/config.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_table/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/cell_type_table/layout.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/cell_type_table/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                     dbc.Col(
                         [
                             html.Div("Annotation Table:"),
                             dcc.Dropdown(
                                 **create_component_kwargs(
                                     state,
                                     id_inner="cell-type-table-menu",
-                                    placeholder="Select a Cell Type Table",
+                                    placeholder="Select a Table",
                                     options=[],
                                     value=None,
                                 ),
                             ),
                         ],
                         width={"size": 3, "offset": 1},
                         align="end",
@@ -369,15 +369,15 @@
             ),
         ),
     )
 
     title_row = dbc.Row(
         [
             dbc.Col(
-                html.H3("Cell Type Table Lookup"),
+                html.H3("Table Viewer"),
                 width={"size": 6, "offset": 1},
             ),
         ],
     )
 
     layout = html.Div(
         children=[
```

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/config.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/dash_url_helper.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/dash_url_helper.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/dataframe_utilities.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/dataframe_utilities.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/link_utilities.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/link_utilities.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/lookup_utilities.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/lookup_utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,27 +18,27 @@
     datastack,
     config,
 ):
     client = make_client(datastack, config.server_address)
     tables = client.materialize.get_tables()
     populate_metadata_cache(tables, client)
     schema_tables = []
-    # exe = ThreadPoolExecutor(max_workers=10)
-    # is_val_source = {t: exe.submit(table_is_value_source, t, client) for t in tables if t not in config.omit_cell_type_tables}
     is_val_source = {t: table_is_value_source(t, client) for t in tables if t not in config.omit_cell_type_tables}
     schema_tables = [k for k, v in is_val_source.items() if v]
     return [{"label": t, "value": t} for t in sorted(schema_tables)]
 
 def get_type_tables(datastack, config):
     tables = get_all_schema_tables(datastack, config)
 
     named_options = config.cell_type_dropdown_options
     if named_options is None:
         return tables
     else:
+        if len(named_options) == 0:
+            named_option_dict = dict()
         named_option_dict = {r["value"]: r["label"] for r in named_options[::-1]}
 
     new_tables = []
     for t in tables:
         if t["value"] in named_option_dict:
             new_tables = [
                 {"label": named_option_dict.get(t["value"]), "value": t["value"]}
```

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/neuron_data_base.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/neuron_data_base.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/schema_utils.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/table_lookup.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/table_lookup.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/common/transform_utils.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/common/transform_utils.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/connectivity_table/__init__.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/connectivity_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/connectivity_table/callbacks.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/connectivity_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/connectivity_table/config.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/connectivity_table/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer/connectivity_table/layout.py` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer/connectivity_table/layout.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer.egg-info/PKG-INFO` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-connectivity-viewer
-Version: 2.0.4
+Version: 2.0.5
 Summary: Dash connectivity viewer for CAVE data
 Home-page: https://github.com/ceesem/dash-connectivity-viewer
 Author: Casey Schneider-Mizell
 Author-email: caseysm@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dash-connectivity-viewer-2.0.4/dash_connectivity_viewer.egg-info/SOURCES.txt` & `dash-connectivity-viewer-2.0.5/dash_connectivity_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.4/setup.py` & `dash-connectivity-viewer-2.0.5/setup.py`

 * *Files identical despite different names*

