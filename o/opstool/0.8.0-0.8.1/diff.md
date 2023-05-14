# Comparing `tmp/opstool-0.8.0.tar.gz` & `tmp/opstool-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opstool-0.8.0.tar", last modified: Sun May  7 06:04:22 2023, max compression
+gzip compressed data, was "opstool-0.8.1.tar", last modified: Sun May 14 11:41:34 2023, max compression
```

## Comparing `opstool-0.8.0.tar` & `opstool-0.8.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.738934 opstool-0.8.0/
--rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 opstool-0.8.0/LICENCE.txt
--rw-rw-rw-   0        0        0     6424 2023-05-07 06:04:22.738934 opstool-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     6005 2023-03-31 11:53:22.000000 opstool-0.8.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-07 06:04:22.738934 opstool-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1013 2023-05-07 06:04:08.000000 opstool-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.691089 opstool-0.8.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.691089 opstool-0.8.0/src/opstool/
--rw-rw-rw-   0        0        0       23 2023-05-07 05:55:41.000000 opstool-0.8.0/src/opstool/__about__.py
--rw-rw-rw-   0        0        0      560 2023-04-29 15:03:24.000000 opstool-0.8.0/src/opstool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.707487 opstool-0.8.0/src/opstool/analysis/
--rw-rw-rw-   0        0        0      147 2023-03-10 09:13:36.000000 opstool-0.8.0/src/opstool/analysis/__init__.py
--rw-rw-rw-   0        0        0    13408 2023-05-02 13:56:05.000000 opstool-0.8.0/src/opstool/analysis/_sec_analysis.py
--rw-rw-rw-   0        0        0    35206 2023-05-02 13:57:14.000000 opstool-0.8.0/src/opstool/analysis/_smart_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.707487 opstool-0.8.0/src/opstool/examples/
--rw-rw-rw-   0        0        0   365987 2022-12-25 13:36:57.000000 opstool-0.8.0/src/opstool/examples/ArchBridge.py
--rw-rw-rw-   0        0        0    96069 2023-01-06 03:19:00.000000 opstool-0.8.0/src/opstool/examples/ArchBridge2.py
--rw-rw-rw-   0        0        0   697240 2022-12-25 13:38:38.000000 opstool-0.8.0/src/opstool/examples/CableStayedBridge.py
--rw-rw-rw-   0        0        0   289022 2022-12-25 13:39:18.000000 opstool-0.8.0/src/opstool/examples/Dam.py
--rw-rw-rw-   0        0        0     1699 2022-12-25 13:39:55.000000 opstool-0.8.0/src/opstool/examples/DamBreak.py
--rw-rw-rw-   0        0        0   241484 2022-12-25 13:40:30.000000 opstool-0.8.0/src/opstool/examples/Frame3D.py
--rw-rw-rw-   0        0        0    15435 2023-05-06 11:58:20.000000 opstool-0.8.0/src/opstool/examples/Frame3D2.py
--rw-rw-rw-   0        0        0    54201 2023-05-06 11:47:25.000000 opstool-0.8.0/src/opstool/examples/GridFrame.py
--rw-rw-rw-   0        0        0   901646 2022-12-25 13:41:16.000000 opstool-0.8.0/src/opstool/examples/Igloo.py
--rw-rw-rw-   0        0        0     2102 2022-12-25 13:41:50.000000 opstool-0.8.0/src/opstool/examples/Pier.py
--rw-rw-rw-   0        0        0     1813 2022-12-25 13:42:23.000000 opstool-0.8.0/src/opstool/examples/SDOF.py
--rw-rw-rw-   0        0        0   110248 2022-12-25 13:43:18.000000 opstool-0.8.0/src/opstool/examples/SuspensionBridge.py
--rw-rw-rw-   0        0        0        2 2022-12-02 13:20:45.000000 opstool-0.8.0/src/opstool/examples/__init__.py
--rw-rw-rw-   0        0        0    16275 2023-05-06 19:15:36.000000 opstool-0.8.0/src/opstool/examples/shell3D.py
-drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.723716 opstool-0.8.0/src/opstool/preprocessing/
--rw-rw-rw-   0        0        0      838 2023-04-02 12:08:20.000000 opstool-0.8.0/src/opstool/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2876 2023-05-02 14:24:57.000000 opstool-0.8.0/src/opstool/preprocessing/geom_transf.py
--rw-rw-rw-   0        0        0     2266 2023-05-02 14:30:35.000000 opstool-0.8.0/src/opstool/preprocessing/load.py
-drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.728233 opstool-0.8.0/src/opstool/preprocessing/section/
--rw-rw-rw-   0        0        0      554 2023-04-02 12:05:56.000000 opstool-0.8.0/src/opstool/preprocessing/section/__init__.py
--rw-rw-rw-   0        0        0     1417 2023-05-02 13:57:22.000000 opstool-0.8.0/src/opstool/preprocessing/section/lib_sec_mesh.py
--rw-rw-rw-   0        0        0    58277 2023-05-02 13:56:50.000000 opstool-0.8.0/src/opstool/preprocessing/section/sec_mesh.py
--rw-rw-rw-   0        0        0    26107 2023-05-02 13:57:35.000000 opstool-0.8.0/src/opstool/preprocessing/section/var_sec_mesh.py
--rw-rw-rw-   0        0        0    53330 2023-03-30 08:56:24.000000 opstool-0.8.0/src/opstool/preprocessing/tcl2py.py
--rw-rw-rw-   0        0        0     5490 2023-03-30 08:58:00.000000 opstool-0.8.0/src/opstool/preprocessing/unit_system.py
--rw-rw-rw-   0        0        0     6848 2023-05-06 15:12:02.000000 opstool-0.8.0/src/opstool/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.728233 opstool-0.8.0/src/opstool/vis/
--rw-rw-rw-   0        0        0      494 2023-05-04 17:23:00.000000 opstool-0.8.0/src/opstool/vis/__init__.py
--rw-rw-rw-   0        0        0    31743 2023-05-06 13:21:15.000000 opstool-0.8.0/src/opstool/vis/_get_model_base.py
--rw-rw-rw-   0        0        0   101317 2023-05-06 12:18:34.000000 opstool-0.8.0/src/opstool/vis/_plotly_base.py
--rw-rw-rw-   0        0        0    59718 2023-05-06 12:19:04.000000 opstool-0.8.0/src/opstool/vis/_pyvista_base.py
--rw-rw-rw-   0        0        0    23046 2023-05-04 17:23:18.000000 opstool-0.8.0/src/opstool/vis/fiber_sec_vis.py
--rw-rw-rw-   0        0        0    32818 2023-05-06 16:41:25.000000 opstool-0.8.0/src/opstool/vis/get_model_data.py
--rw-rw-rw-   0        0        0    28069 2023-05-06 14:31:33.000000 opstool-0.8.0/src/opstool/vis/ops_vis_2d.py
--rw-rw-rw-   0        0        0    24646 2023-05-06 08:18:30.000000 opstool-0.8.0/src/opstool/vis/ops_vis_plotly.py
--rw-rw-rw-   0        0        0    21638 2023-05-03 06:58:59.000000 opstool-0.8.0/src/opstool/vis/ops_vis_pyvista.py
--rw-rw-rw-   0        0        0    10257 2023-05-06 12:44:36.000000 opstool-0.8.0/src/opstool/vis/quick_plot.py
--rw-rw-rw-   0        0        0     9601 2023-04-29 15:01:29.000000 opstool-0.8.0/src/opstool/vis/save_tikz.py
-drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.707487 opstool-0.8.0/src/opstool.egg-info/
--rw-rw-rw-   0        0        0     6424 2023-05-07 06:04:22.000000 opstool-0.8.0/src/opstool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1730 2023-05-07 06:04:22.000000 opstool-0.8.0/src/opstool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 06:04:22.000000 opstool-0.8.0/src/opstool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-05-07 06:04:22.000000 opstool-0.8.0/src/opstool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-07 06:04:22.000000 opstool-0.8.0/src/opstool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.738934 opstool-0.8.0/tests/
--rw-rw-rw-   0        0        0     2002 2023-01-18 14:49:51.000000 opstool-0.8.0/tests/test_dambreak.py
--rw-rw-rw-   0        0        0     1705 2023-03-27 03:00:39.000000 opstool-0.8.0/tests/test_fiber_sec_vis.py
--rw-rw-rw-   0        0        0     2997 2023-05-06 07:58:02.000000 opstool-0.8.0/tests/test_model_vis.py
--rw-rw-rw-   0        0        0     2261 2023-03-29 06:45:30.000000 opstool-0.8.0/tests/test_sec_analysis.py
--rw-rw-rw-   0        0        0    10302 2023-04-03 08:29:31.000000 opstool-0.8.0/tests/test_sec_mesh.py
--rw-rw-rw-   0        0        0     1237 2023-05-06 09:45:10.000000 opstool-0.8.0/tests/test_temp.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.289529 opstool-0.8.1/
+-rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 opstool-0.8.1/LICENCE.txt
+-rw-rw-rw-   0        0        0     6424 2023-05-14 11:41:34.289529 opstool-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6005 2023-03-31 11:53:22.000000 opstool-0.8.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-14 11:41:34.289529 opstool-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-05-07 06:04:08.000000 opstool-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.258862 opstool-0.8.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.258862 opstool-0.8.1/src/opstool/
+-rw-rw-rw-   0        0        0       23 2023-05-14 11:38:49.000000 opstool-0.8.1/src/opstool/__about__.py
+-rw-rw-rw-   0        0        0      560 2023-04-29 15:03:24.000000 opstool-0.8.1/src/opstool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.265888 opstool-0.8.1/src/opstool/analysis/
+-rw-rw-rw-   0        0        0      147 2023-03-10 09:13:36.000000 opstool-0.8.1/src/opstool/analysis/__init__.py
+-rw-rw-rw-   0        0        0    13408 2023-05-02 13:56:05.000000 opstool-0.8.1/src/opstool/analysis/_sec_analysis.py
+-rw-rw-rw-   0        0        0    35206 2023-05-02 13:57:14.000000 opstool-0.8.1/src/opstool/analysis/_smart_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.273903 opstool-0.8.1/src/opstool/examples/
+-rw-rw-rw-   0        0        0   365987 2022-12-25 13:36:57.000000 opstool-0.8.1/src/opstool/examples/ArchBridge.py
+-rw-rw-rw-   0        0        0    96069 2023-01-06 03:19:00.000000 opstool-0.8.1/src/opstool/examples/ArchBridge2.py
+-rw-rw-rw-   0        0        0   697240 2022-12-25 13:38:38.000000 opstool-0.8.1/src/opstool/examples/CableStayedBridge.py
+-rw-rw-rw-   0        0        0   289022 2022-12-25 13:39:18.000000 opstool-0.8.1/src/opstool/examples/Dam.py
+-rw-rw-rw-   0        0        0     1699 2022-12-25 13:39:55.000000 opstool-0.8.1/src/opstool/examples/DamBreak.py
+-rw-rw-rw-   0        0        0   241484 2022-12-25 13:40:30.000000 opstool-0.8.1/src/opstool/examples/Frame3D.py
+-rw-rw-rw-   0        0        0    15435 2023-05-06 11:58:20.000000 opstool-0.8.1/src/opstool/examples/Frame3D2.py
+-rw-rw-rw-   0        0        0    54201 2023-05-06 11:47:25.000000 opstool-0.8.1/src/opstool/examples/GridFrame.py
+-rw-rw-rw-   0        0        0   901646 2022-12-25 13:41:16.000000 opstool-0.8.1/src/opstool/examples/Igloo.py
+-rw-rw-rw-   0        0        0     2102 2022-12-25 13:41:50.000000 opstool-0.8.1/src/opstool/examples/Pier.py
+-rw-rw-rw-   0        0        0     1813 2022-12-25 13:42:23.000000 opstool-0.8.1/src/opstool/examples/SDOF.py
+-rw-rw-rw-   0        0        0   110248 2022-12-25 13:43:18.000000 opstool-0.8.1/src/opstool/examples/SuspensionBridge.py
+-rw-rw-rw-   0        0        0        2 2022-12-02 13:20:45.000000 opstool-0.8.1/src/opstool/examples/__init__.py
+-rw-rw-rw-   0        0        0    16275 2023-05-06 19:15:36.000000 opstool-0.8.1/src/opstool/examples/shell3D.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.273903 opstool-0.8.1/src/opstool/preprocessing/
+-rw-rw-rw-   0        0        0      838 2023-04-02 12:08:20.000000 opstool-0.8.1/src/opstool/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2876 2023-05-09 04:18:48.000000 opstool-0.8.1/src/opstool/preprocessing/geom_transf.py
+-rw-rw-rw-   0        0        0     2266 2023-05-02 14:30:35.000000 opstool-0.8.1/src/opstool/preprocessing/load.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.289529 opstool-0.8.1/src/opstool/preprocessing/section/
+-rw-rw-rw-   0        0        0      554 2023-04-02 12:05:56.000000 opstool-0.8.1/src/opstool/preprocessing/section/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-05-02 13:57:22.000000 opstool-0.8.1/src/opstool/preprocessing/section/lib_sec_mesh.py
+-rw-rw-rw-   0        0        0    60526 2023-05-13 09:31:14.000000 opstool-0.8.1/src/opstool/preprocessing/section/sec_mesh.py
+-rw-rw-rw-   0        0        0    26107 2023-05-02 13:57:35.000000 opstool-0.8.1/src/opstool/preprocessing/section/var_sec_mesh.py
+-rw-rw-rw-   0        0        0    53330 2023-03-30 08:56:24.000000 opstool-0.8.1/src/opstool/preprocessing/tcl2py.py
+-rw-rw-rw-   0        0        0     5490 2023-03-30 08:58:00.000000 opstool-0.8.1/src/opstool/preprocessing/unit_system.py
+-rw-rw-rw-   0        0        0     6848 2023-05-06 15:12:02.000000 opstool-0.8.1/src/opstool/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.289529 opstool-0.8.1/src/opstool/vis/
+-rw-rw-rw-   0        0        0      494 2023-05-04 17:23:00.000000 opstool-0.8.1/src/opstool/vis/__init__.py
+-rw-rw-rw-   0        0        0    31751 2023-05-13 10:15:56.000000 opstool-0.8.1/src/opstool/vis/_get_model_base.py
+-rw-rw-rw-   0        0        0   106637 2023-05-14 11:32:12.000000 opstool-0.8.1/src/opstool/vis/_plotly_base.py
+-rw-rw-rw-   0        0        0    61888 2023-05-14 11:24:31.000000 opstool-0.8.1/src/opstool/vis/_pyvista_base.py
+-rw-rw-rw-   0        0        0    23046 2023-05-04 17:23:18.000000 opstool-0.8.1/src/opstool/vis/fiber_sec_vis.py
+-rw-rw-rw-   0        0        0    32818 2023-05-06 16:41:25.000000 opstool-0.8.1/src/opstool/vis/get_model_data.py
+-rw-rw-rw-   0        0        0    28069 2023-05-06 14:31:33.000000 opstool-0.8.1/src/opstool/vis/ops_vis_2d.py
+-rw-rw-rw-   0        0        0    25267 2023-05-09 06:37:32.000000 opstool-0.8.1/src/opstool/vis/ops_vis_plotly.py
+-rw-rw-rw-   0        0        0    21638 2023-05-03 06:58:59.000000 opstool-0.8.1/src/opstool/vis/ops_vis_pyvista.py
+-rw-rw-rw-   0        0        0    10257 2023-05-06 12:44:36.000000 opstool-0.8.1/src/opstool/vis/quick_plot.py
+-rw-rw-rw-   0        0        0    14099 2023-05-09 07:53:13.000000 opstool-0.8.1/src/opstool/vis/save_tikz.py
+drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.265888 opstool-0.8.1/src/opstool.egg-info/
+-rw-rw-rw-   0        0        0     6424 2023-05-14 11:41:34.000000 opstool-0.8.1/src/opstool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1730 2023-05-14 11:41:34.000000 opstool-0.8.1/src/opstool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 11:41:34.000000 opstool-0.8.1/src/opstool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-05-14 11:41:34.000000 opstool-0.8.1/src/opstool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-14 11:41:34.000000 opstool-0.8.1/src/opstool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 11:41:34.289529 opstool-0.8.1/tests/
+-rw-rw-rw-   0        0        0     2002 2023-01-18 14:49:51.000000 opstool-0.8.1/tests/test_dambreak.py
+-rw-rw-rw-   0        0        0     1705 2023-03-27 03:00:39.000000 opstool-0.8.1/tests/test_fiber_sec_vis.py
+-rw-rw-rw-   0        0        0     2982 2023-05-09 11:18:04.000000 opstool-0.8.1/tests/test_model_vis.py
+-rw-rw-rw-   0        0        0     2261 2023-03-29 06:45:30.000000 opstool-0.8.1/tests/test_sec_analysis.py
+-rw-rw-rw-   0        0        0    10302 2023-04-03 08:29:31.000000 opstool-0.8.1/tests/test_sec_mesh.py
+-rw-rw-rw-   0        0        0      954 2023-05-09 13:39:18.000000 opstool-0.8.1/tests/test_temp.py
```

### Comparing `opstool-0.8.0/LICENCE.txt` & `opstool-0.8.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/PKG-INFO` & `opstool-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opstool
-Version: 0.8.0
+Version: 0.8.1
 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
 Keywords: OpenSees Visualization Seismic Simulation
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opstool Version: 0.8.0 Summary: openseespy toolbox
+Metadata-Version: 2.1 Name: opstool Version: 0.8.1 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992 Author: Yexiang Yan Author-email:
 yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees Visualization
 Seismic Simulation Platform: any Classifier: Programming Language :: Python ::
 3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENCE.txt
                                     opstool
            modelling, visualization, post-processing for OpenSeesPy.
```

### Comparing `opstool-0.8.0/README.md` & `opstool-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/setup.py` & `opstool-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/__init__.py` & `opstool-0.8.1/src/opstool/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/analysis/_sec_analysis.py` & `opstool-0.8.1/src/opstool/analysis/_sec_analysis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/analysis/_smart_analyze.py` & `opstool-0.8.1/src/opstool/analysis/_smart_analyze.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/ArchBridge.py` & `opstool-0.8.1/src/opstool/examples/ArchBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/ArchBridge2.py` & `opstool-0.8.1/src/opstool/examples/ArchBridge2.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/CableStayedBridge.py` & `opstool-0.8.1/src/opstool/examples/CableStayedBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/Dam.py` & `opstool-0.8.1/src/opstool/examples/Dam.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/DamBreak.py` & `opstool-0.8.1/src/opstool/examples/DamBreak.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/Frame3D.py` & `opstool-0.8.1/src/opstool/examples/Frame3D.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/Frame3D2.py` & `opstool-0.8.1/src/opstool/examples/Frame3D2.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/GridFrame.py` & `opstool-0.8.1/src/opstool/examples/GridFrame.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/Igloo.py` & `opstool-0.8.1/src/opstool/examples/Igloo.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/Pier.py` & `opstool-0.8.1/src/opstool/examples/Pier.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/SDOF.py` & `opstool-0.8.1/src/opstool/examples/SDOF.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/SuspensionBridge.py` & `opstool-0.8.1/src/opstool/examples/SuspensionBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/examples/shell3D.py` & `opstool-0.8.1/src/opstool/examples/shell3D.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/preprocessing/__init__.py` & `opstool-0.8.1/src/opstool/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/preprocessing/geom_transf.py` & `opstool-0.8.1/src/opstool/preprocessing/geom_transf.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/preprocessing/load.py` & `opstool-0.8.1/src/opstool/preprocessing/load.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/preprocessing/section/__init__.py` & `opstool-0.8.1/src/opstool/preprocessing/section/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/preprocessing/section/lib_sec_mesh.py` & `opstool-0.8.1/src/opstool/preprocessing/section/lib_sec_mesh.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/preprocessing/section/sec_mesh.py` & `opstool-0.8.1/src/opstool/preprocessing/section/sec_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,18 @@
         self.mesh_obj = None
         self.section = None
         self.points = None
         self.cells_map = dict()
         self.centers_map = dict()
         self.areas_map = dict()
         self.center = None
+        self.area = 0.0
+        self.Iy = 0.0
+        self.Iz = 0.0
+        self.J = 0.0
 
         # * data group
         self.group_map = dict()
         self.mat_ops_map = dict()
         self.mesh_size_map = dict()
 
         # *rebar data
@@ -75,14 +79,16 @@
     def assign_mesh_size(self, mesh_size: dict):
         """Assign the mesh size dict for each mesh.
 
         Parameters
         ------------
         mesh_size : dict[str, float]
             A dict of name as key, mesh size as value.
+            The mesh sizes describe the maximum mesh element area to be
+            used in the finite-element mesh for each Geometry object.
 
         Returns
         ------------
         instance
         """
         if not self.group_map:
             raise ValueError("The assign_group method should be run first!")
@@ -179,14 +185,15 @@
         triangles = self.mesh_obj["triangles"][:, :3]
         triangle_attributes = self.mesh_obj["triangle_attributes"]
         attributes = np.unique(triangle_attributes)
         for name, attri in zip(self.group_map.keys(), attributes):
             idx = triangle_attributes == attri
             self.cells_map[name] = triangles[idx[:, 0]]
         # * fiber data
+        iys, izs = [], []
         for name, faces in self.cells_map.items():
             areas = []
             centers = []
             for face in faces:
                 idx1, idx2, idx3 = face
                 coord1, coord2, coord3 = vertices[idx1], vertices[idx2], vertices[idx3]
                 xyo = (coord1 + coord2 + coord3) / 3
@@ -194,25 +201,29 @@
                 x1, y1 = coord1[:2]
                 x2, y2 = coord2[:2]
                 x3, y3 = coord3[:2]
                 area_ = 0.5 * np.abs(
                     x2 * y3 + x1 * y2 + x3 * y1 - x3 * y2 - x2 * y1 - x1 * y3
                 )
                 areas.append(area_)
+                iys.append(area_ * xyo[1] ** 2)
+                izs.append(area_ * xyo[0] ** 2)
             self.areas_map[name] = np.array(areas)
             self.centers_map[name] = np.array(centers)
         centers = []
         areas = []
         for name in self.cells_map.keys():
             centers.append(self.centers_map[name])
             areas.append(self.areas_map[name])
         centers = np.vstack(centers)
         areas = np.hstack(areas)
-        center = areas @ centers / np.sum(areas)
-        self.center = center
+        self.area = np.sum(areas)
+        self.center = areas @ centers / self.area
+        self.Iy = np.sum(iys)
+        self.Iz = np.sum(izs)
 
     def add_rebars(self, rebars_obj):
         """Add rebars.
 
         Parameters
         ----------
         rebars_obj : mesh obj
@@ -230,14 +241,80 @@
         Returns
         -------
         Tuple(dict, dict)
             fiber center dict, fiber area dict
         """
         return self.centers_map, self.areas_map
 
+    def get_area(self):
+        """Return section area.
+
+        Returns
+        -------
+        Float
+        """
+        area = 0
+        if self.frame_sec_props:
+            area = self.frame_sec_props["A"]
+        elif self.sec_props:
+            area = self.sec_props["A"]
+        else:
+            area = self.area
+        return area
+
+    def get_iy(self):
+        """Return Moment of inertia of the section around the y-axis.
+
+        Returns
+        -------
+        Float
+        """
+        iy = 0
+        if self.frame_sec_props:
+            iy = self.frame_sec_props["Iy"]
+        elif self.sec_props:
+            iy = self.sec_props["Iy"]
+        else:
+            iy = self.Iy
+        return iy
+
+    def get_iz(self):
+        """Return Moment of inertia of the section around the z-axis.
+
+        Returns
+        -------
+        Float
+        """
+        iz = 0
+        if self.frame_sec_props:
+            iz = self.frame_sec_props["Iz"]
+        elif self.sec_props:
+            iz = self.sec_props["Iz"]
+        else:
+            iz = self.Iz
+        return iz
+
+    def get_j(self):
+        """Return section torsion constant.
+
+        Returns
+        -------
+        Float
+        """
+        j = 0
+        if self.frame_sec_props:
+            j = self.frame_sec_props["J"]
+        elif self.sec_props:
+            j = self.sec_props["J"]
+        else:
+            raise ValueError(
+                "The Section Properties method <get_frame_props> or <get_sec_props> has not been run!"
+            )
+        return j
+
     def _run_sec_props(self, Eref, Gref, section):
         # Second moments of area centroidal axis
         ixx_c, iyy_c, ixy_c = section.get_ic()
         # Elastic centroid
         cx, cy = section.get_c()
         # Elastic section moduli about the centroidal axis with respect to the top and bottom fibres
         zxx_plus, zxx_minus, zyy_plus, zyy_minus = section.get_z()
@@ -256,15 +333,18 @@
             # St. Venant torsion constant
             j = section.get_j()
         else:
             area = section.get_ea() / Eref
             # St. Venant torsion constant
             j_ = section.get_j()
             j = G_eff / E_eff * j_ / Gref
-
+        self.area = area
+        self.Iy = ixx_c / Eref
+        self.Iz = iyy_c / Eref
+        self.J = j
         if self.rebar_data:
             all_rebar_area = 0
             for data in self.rebar_data:
                 rebar_xy = data["rebar_xy"]
                 dia = data["dia"]
                 rebar_coords = []
                 rebar_areas = []
@@ -481,14 +561,18 @@
         zxx_plus, zxx_minus, zyy_plus, zyy_minus = self.section.get_z()
         E_eff = self.section.section_props.ea / self.section.section_props.area
         G_eff = ga / self.section.section_props.area
         area = ea / Eref
         if Eref != 1.0:  # composite section
             # St. Venant torsion constant
             j = G_eff / E_eff * j / Gref
+        self.area = area
+        self.Iy = ixx_c / Eref
+        self.Iz = iyy_c / Eref
+        self.J = j
         if self.rebar_data:
             all_rebar_area = 0
             for data in self.rebar_data:
                 rebar_xy = data["rebar_xy"]
                 dia = data["dia"]
                 rebar_coords = []
                 rebar_areas = []
```

### Comparing `opstool-0.8.0/src/opstool/preprocessing/section/var_sec_mesh.py` & `opstool-0.8.1/src/opstool/preprocessing/section/var_sec_mesh.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/preprocessing/tcl2py.py` & `opstool-0.8.1/src/opstool/preprocessing/tcl2py.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/preprocessing/unit_system.py` & `opstool-0.8.1/src/opstool/preprocessing/unit_system.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/utils.py` & `opstool-0.8.1/src/opstool/utils.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/vis/_get_model_base.py` & `opstool-0.8.1/src/opstool/vis/_get_model_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,23 +101,23 @@
 
 def get_mp_constraint(node_coords, node_index):
     retained_nodes = ops.getRetainedNodes()
     points = []
     midpoints = []
     cells = []
     dofs = []
-    for i, tag in enumerate(retained_nodes):
+    for tag in retained_nodes:
         constrained_nodes = ops.getConstrainedNodes(tag)
         for tag2 in constrained_nodes:
+            cells.extend([2, len(points), len(points) + 1])
             points.append(node_coords[node_index[tag]])
             points.append(node_coords[node_index[tag2]])
             midpoints.append(
                 (node_coords[node_index[tag]] + node_coords[node_index[tag2]]) / 2
             )
-            cells.extend([2, 2 * i, 2 * i + 1])
             dof = ops.getRetainedDOFs(tag, tag2)
             dofs.append(dof)
     if dofs:
         max_dof_dim = np.max([len(dof) for dof in dofs])
         new_dofs = []
         for dof in dofs:
             if len(dof) < max_dof_dim:
@@ -339,15 +339,15 @@
             sec_cells.append(cells)
     return (
         np.array(ext_points),
         np.array(ext_cells),
         np.array(int_points),
         np.array(int_cells),
         np.array(sec_points),
-        np.vstack(sec_cells),
+        np.ravel(np.vstack(sec_cells)),
     )
 
 
 def get_other_line_info(ele_tags, node_index):
     other_line_cells = []
     other_line_cells_tags = []
     for i, ele in enumerate(ele_tags):
```

### Comparing `opstool-0.8.0/src/opstool/vis/_plotly_base.py` & `opstool-0.8.1/src/opstool/vis/_plotly_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,16 @@
     show_local_crd: bool = False,
     local_crd_alpha: float = 1.0,
     show_fix_node: bool = True,
     fix_node_alpha: float = 1.0,
     show_load: bool = False,
     load_alpha: float = 1.0,
     show_constrain_dof: bool = False,
+    show_beam_sec: bool = False,
+    beam_sec_paras: dict = None,
     label_size: float = 8,
     show_outline: bool = True,
     opacity: float = 1.0,
 ):
     fig = go.Figure()
     plotter = []
     points_no_deform = model_info["coord_no_deform"]
@@ -267,14 +269,16 @@
                     ),
                     mode="markers",
                     name=names[i],
                     hovertemplate="<b>%{text}</b>",
                     text=labels_,
                 )
             )
+    if len(cells["link"]) > 0:
+        _show_link(obj, plotter, model_info["coord_no_deform"], cells["link"])
     # point plot
     node_labels = [str(i) for i in model_info["NodeTags"]]
     x, y, z = [points_no_deform[:, j] for j in range(3)]
     plotter.append(
         go.Scatter3d(
             x=x,
             y=y,
@@ -282,14 +286,20 @@
             marker=dict(size=obj.point_size, color=obj.color_point),
             mode="markers",
             name="Node",
             customdata=node_labels,
             hovertemplate="<b>x: %{x}</b><br>y: %{y}<br>z: %{z} <br>tag: %{customdata}",
         )
     )
+    # beam section render
+    if show_beam_sec:
+        beam_sec_paras_ = dict(color="#5170d7", opacity=0.25, texture=False)
+        if beam_sec_paras is not None:
+            beam_sec_paras_.update(beam_sec_paras)
+        _show_beam_sec(plotter, model_info, cells, beam_sec_paras_)
 
     if show_node_label:
         txt_plot = go.Scatter3d(
             x=x,
             y=y,
             z=z,
             text=node_labels,
@@ -369,14 +379,80 @@
                 yaxis={"showgrid": False, "zeroline": False, "visible": False},
                 zaxis={"showgrid": False, "zeroline": False, "visible": False},
             ),
         )
     return fig
 
 
+def _show_link(obj, plotter, points, cells):
+    cells = np.reshape(cells, (-1, 3))
+    points_zero = []
+    points_nonzero = []
+    cells_nonzero = []
+    for cell in cells:
+        idx1, idx2 = cell[1:]
+        coord1, coord2 = points[idx1], points[idx2]
+        length = np.sqrt(np.sum((coord2 - coord1) ** 2))
+        if np.abs(length) < 1e-8:
+            points_zero.append(coord1)
+        else:
+            xaxis = np.array(coord2 - coord1)
+            global_z = [0.0, 0.0, 1.0]
+            cos_angle = xaxis.dot(global_z) / (
+                np.linalg.norm(xaxis) * np.linalg.norm(global_z)
+            )
+            if np.abs(1 - cos_angle**2) < 1e-10:
+                yaxis = np.cross([-1.0, 0.0, 0.0], xaxis)
+            else:
+                yaxis = np.cross(global_z, xaxis)
+            xaxis = xaxis / np.linalg.norm(xaxis)
+            yaxis = yaxis / np.linalg.norm(yaxis)
+            idx = len(points_nonzero)
+            for i in range(5):
+                cells_nonzero.extend([2, idx + i, idx + i + 1])
+            points_nonzero.extend(
+                [
+                    coord1 + 0.25 * length * xaxis,
+                    coord1 + 0.25 * length * xaxis + 0.25 * length * yaxis,
+                    coord1 + 0.5 * length * xaxis - 0.25 * length * yaxis,
+                    coord1 + 0.5 * length * xaxis + 0.25 * length * yaxis,
+                    coord1 + 0.75 * length * xaxis - 0.25 * length * yaxis,
+                    coord1 + 0.75 * length * xaxis,
+                ]
+            )
+    # plot
+    if len(points_zero) > 0:
+        plotter.append(
+            go.Scatter3d(
+                x=points_zero[:, 0],
+                y=points_zero[:, 1],
+                z=points_zero[:, 2],
+                marker=dict(size=obj.point_size * 2, color=obj.color_link),
+                mode="markers",
+                hoverinfo="skip",
+            )
+        )
+    if len(points_nonzero) > 0:
+        cells_nonzero = np.reshape(cells_nonzero, (-1, 3))
+        points_nonzero = np.array(points_nonzero)
+        line_points, _ = _make_lines(points_nonzero, cells_nonzero)
+        x, y, z = line_points[:, 0], line_points[:, 1], line_points[:, 2]
+        plotter.append(
+            go.Scatter3d(
+                x=x,
+                y=y,
+                z=z,
+                line=dict(color=obj.color_link, width=obj.line_width / 2),
+                mode="lines",
+                connectgaps=False,
+                hoverinfo="skip",
+            )
+        )
+
+
 def _make_fix_node(model_info, alpha=1.0):
     fixed_dofs = model_info["FixNodeDofs"]
     fixed_coords = model_info["FixNodeCoords"]
     beam_lengths = model_info["beam_lengths"]
     D2 = True if np.max(model_info["model_dims"]) <= 2 else False
     if len(beam_lengths) > 0:
         s = np.mean(beam_lengths) / 10 * alpha
@@ -421,14 +497,94 @@
                     [np.NAN, np.NAN, np.NAN],
                 ]
             )
     points = np.array(points)
     return points
 
 
+def _show_beam_sec(plotter, model_info, cells, paras):
+    ext_points = model_info["line_sec_ext_points"]
+    int_points = model_info["line_sec_int_points"]
+    sec_points = model_info["line_sec_points"]
+    ext_cells = cells["line_sec_ext"]
+    int_cells = cells["line_sec_int"]
+    sec_cells = cells["line_sec"]
+    if paras["texture"]:
+        warnings.warn("The backend plotly does not currently support texture!")
+    if len(ext_cells) > 0:
+        (
+            face_points,
+            _,
+            _,
+            veci,
+            vecj,
+            veck,
+        ) = _make_faces(ext_points, ext_cells)
+        x, y, z = face_points[:, 0], face_points[:, 1], face_points[:, 2]
+        plotter.append(
+            go.Mesh3d(
+                x=x,
+                y=y,
+                z=z,
+                i=veci,
+                j=vecj,
+                k=veck,
+                color=paras["color"],
+                opacity=paras["opacity"],
+                hoverinfo="skip",
+            )
+        )
+    if len(int_cells) > 0:
+        (
+            face_points,
+            _,
+            _,
+            veci,
+            vecj,
+            veck,
+        ) = _make_faces(int_points, int_cells)
+        x, y, z = face_points[:, 0], face_points[:, 1], face_points[:, 2]
+        plotter.append(
+            go.Mesh3d(
+                x=x,
+                y=y,
+                z=z,
+                i=veci,
+                j=vecj,
+                k=veck,
+                color=paras["color"],
+                opacity=paras["opacity"],
+                hoverinfo="skip",
+            )
+        )
+    if len(sec_cells) > 0:
+        (
+            face_points,
+            _,
+            _,
+            veci,
+            vecj,
+            veck,
+        ) = _make_faces(sec_points, sec_cells)
+        x, y, z = face_points[:, 0], face_points[:, 1], face_points[:, 2]
+        plotter.append(
+            go.Mesh3d(
+                x=x,
+                y=y,
+                z=z,
+                i=veci,
+                j=vecj,
+                k=veck,
+                color=paras["color"],
+                opacity=paras["opacity"],
+                hoverinfo="skip",
+            )
+        )
+
+
 def _show_local_axes(obj, plotter, model_info, alpha: float = 1.0):
     beam_midpoints = model_info["beam_midpoints"]
     beam_lengths = model_info["beam_lengths"]
     if len(beam_lengths) > 0:
         xaxis = model_info["beam_xlocal"]
         yaxis = model_info["beam_ylocal"]
         zaxis = model_info["beam_zlocal"]
@@ -892,15 +1048,15 @@
             column_widths=[1] * shape[1],
             row_heights=[1] * shape[0],
         )
         for i, idx in enumerate(range(modei, modej + 1)):
             eigen_vec = eigenvector[idx - 1]
             value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
             alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
-            alpha_ *= alpha if alpha else alpha_
+            alpha_ = alpha_ * alpha if alpha else alpha_
             eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
             scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
 
             idxi = int(np.ceil((i + 1) / shape[1]) - 1)
             idxj = int(i - idxi * shape[1])
             # ---------------------------------------------------------
             if show_origin:
@@ -977,15 +1133,15 @@
         cmins = []
         cmaxs = []
         for i, idx in enumerate(range(modei, modej + 1)):
             step = idx - 1
             eigen_vec = eigenvector[step]
             value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
             alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
-            alpha_ *= alpha if alpha else alpha_
+            alpha_ = alpha_ * alpha if alpha else alpha_
             eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
             scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
             cmins.append(np.min(scalars))
             cmaxs.append(np.max(scalars))
 
             # -------------------------------------------------------------
             # start plot
@@ -1103,15 +1259,15 @@
     num_mode_tag = len(f)
     if mode_tag > num_mode_tag:
         raise ValueError("Insufficient number of modes in open file")
     eigen_vec = eigenvector[mode_tag - 1]
     f_ = f[mode_tag - 1]
     value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
     alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
-    alpha_ *= alpha if alpha else alpha_
+    alpha_ = alpha_ * alpha if alpha else alpha_
     eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
     anti_eigen_points = eigen_data["coord_no_deform"] - eigen_vec * alpha_
     scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
     plt_points = [anti_eigen_points, eigen_data["coord_no_deform"], eigen_points]
     index = [1] + [2, 0] * n_cycle
     nb_frames = len(index)
     times = int(nb_frames / framerate)
@@ -1539,15 +1695,15 @@
     # scale factor
     if resp_type == "disp":
         max_bound = np.max(
             [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]]
         )
         value = np.max(np.sqrt(np.sum(max_node_resp**2, axis=1)))
         alpha_ = max_bound / obj.bound_fact / value
-        alpha_ *= alpha if alpha else alpha_
+        alpha_ = alpha_ * alpha if alpha else alpha_
     else:
         alpha_ = 0
     # ------------------------------------------------------------------------
     fig = go.Figure()
     # -------------------------------------------------------------------------
     if slider:
         n_data = None
@@ -1793,15 +1949,15 @@
     # scale factor
     if resp_type == "disp":
         max_bound = np.max(
             [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]]
         )
         value = np.max(np.sqrt(np.sum(max_node_resp**2, axis=1)))
         alpha_ = max_bound / obj.bound_fact / value
-        alpha_ *= alpha if alpha else alpha_
+        alpha_ = alpha_ * alpha if alpha else alpha_
     else:
         alpha_ = 0
 
     # -----------------------------------------------------------------------------
     # start plot
     def create_mesh(stepi):
         if model_update:
@@ -2028,15 +2184,15 @@
     local_forces_max = local_forces_step[maxstep]
     cmin, cmax = np.min(local_forces_max), np.max(local_forces_max)
     max_coord = np.max(beam_node_coords, axis=0)
     min_coord = np.min(beam_node_coords, axis=0)
     max_bound = np.max(max_coord - min_coord)
     maxv = np.amax(np.abs(local_forces_max))
     alpha_ = max_bound / maxv / obj.bound_fact
-    alpha_ *= alpha if alpha else alpha_
+    alpha_ = alpha_ * alpha if alpha else alpha_
 
     # ------------------------------------------------------------------------
     fig = go.Figure()
     # -------------------------------------------------------------------------
     if slider:
         n_data = None
         for step in range(num_steps):
```

### Comparing `opstool-0.8.0/src/opstool/vis/_pyvista_base.py` & `opstool-0.8.1/src/opstool/vis/_pyvista_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,16 @@
     dofs = model_info["ConstrainedDofs"]
     dofs = ["".join([str(k) for k in dof if k != -1]) for dof in dofs]
     if len(cells) > 0:
         mesh = _generate_mesh(points, cells, kind="line")
         plotter.add_mesh(
             mesh,
             color=obj.color_constraint,
-            render_lines_as_tubes=False,
-            line_width=obj.line_width / 3,
+            render_lines_as_tubes=True,
+            line_width=obj.line_width / 2,
         )
         if show_dofs:
             plotter.add_point_labels(
                 midcoords,
                 dofs,
                 text_color=obj.color_constraint,
                 font_size=12,
@@ -523,14 +523,68 @@
         plotter.add_mesh(
             fix_plot, color="#01ff07", render_lines_as_tubes=False, line_width=2
         )
     else:
         warnings.warn("Model has no fix nodes!")
 
 
+def _show_link(obj, plotter, points, cells):
+    cells = np.reshape(cells, (-1, 3))
+    points_zero = []
+    points_nonzero = []
+    cells_nonzero = []
+    for cell in cells:
+        idx1, idx2 = cell[1:]
+        coord1, coord2 = points[idx1], points[idx2]
+        length = np.sqrt(np.sum((coord2 - coord1) ** 2))
+        if np.abs(length) < 1e-8:
+            points_zero.append(coord1)
+        else:
+            xaxis = np.array(coord2 - coord1)
+            global_z = [0.0, 0.0, 1.0]
+            cos_angle = xaxis.dot(global_z) / (
+                np.linalg.norm(xaxis) * np.linalg.norm(global_z)
+            )
+            if np.abs(1 - cos_angle**2) < 1e-10:
+                yaxis = np.cross([-1.0, 0.0, 0.0], xaxis)
+            else:
+                yaxis = np.cross(global_z, xaxis)
+            xaxis = xaxis / np.linalg.norm(xaxis)
+            yaxis = yaxis / np.linalg.norm(yaxis)
+            idx = len(points_nonzero)
+            for i in range(5):
+                cells_nonzero.extend([2, idx + i, idx + i + 1])
+            points_nonzero.extend(
+                [
+                    coord1 + 0.25 * length * xaxis,
+                    coord1 + 0.25 * length * xaxis - 0.25 * length * yaxis,
+                    coord1 + 0.5 * length * xaxis + 0.25 * length * yaxis,
+                    coord1 + 0.5 * length * xaxis - 0.25 * length * yaxis,
+                    coord1 + 0.75 * length * xaxis + 0.25 * length * yaxis,
+                    coord1 + 0.75 * length * xaxis,
+                ]
+            )
+    # plot
+    if len(points_zero) > 0:
+        plotter.add_mesh(
+            pv.PolyData(points_zero),
+            color=obj.color_link,
+            point_size=obj.point_size * 2,
+            render_points_as_spheres=True,
+        )
+    if len(points_nonzero) > 0:
+        link_plot = _generate_mesh(points_nonzero, cells_nonzero, kind="line")
+        plotter.add_mesh(
+            link_plot,
+            color=obj.color_link,
+            render_lines_as_tubes=False,
+            line_width=obj.line_width / 2,
+        )
+
+
 def _plot_model(obj, plotter, model_info, cells, opacity):
     point_plot = pv.PolyData(model_info["coord_no_deform"])
     plotter.add_mesh(
         point_plot,
         color=obj.color_point,
         point_size=obj.point_size,
         render_points_as_spheres=True,
@@ -553,14 +607,15 @@
         )
         plotter.add_mesh(
             link_plot,
             color=obj.color_link,
             render_lines_as_tubes=False,
             line_width=obj.line_width / 2,
         )
+        _show_link(obj, plotter, model_info["coord_no_deform"], cells["link"])
 
     if len(cells["beam"]) > 0:
         beam_plot = _generate_mesh(
             model_info["coord_no_deform"], cells["beam"], kind="line"
         )
         plotter.add_mesh(
             beam_plot,
@@ -641,15 +696,15 @@
             plotter.subplot(idxi, idxj)
         else:
             plotter.clear_actors()
         step = int(round(idx)) - 1
         eigen_vec = eigenvector[step]
         value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
         alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
-        alpha_ = alpha * alpha if alpha else alpha_
+        alpha_ = alpha_ * alpha if alpha else alpha_
         eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
         scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
         _ = _generate_all_mesh(
             plotter,
             eigen_points,
             scalars,
             opacity,
```

### Comparing `opstool-0.8.0/src/opstool/vis/fiber_sec_vis.py` & `opstool-0.8.1/src/opstool/vis/fiber_sec_vis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/vis/get_model_data.py` & `opstool-0.8.1/src/opstool/vis/get_model_data.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/vis/ops_vis_2d.py` & `opstool-0.8.1/src/opstool/vis/ops_vis_2d.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/vis/ops_vis_plotly.py` & `opstool-0.8.1/src/opstool/vis/ops_vis_plotly.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,16 @@
         show_local_crd: bool = False,
         local_crd_alpha: float = 1.0,
         show_fix_node: bool = True,
         fix_node_alpha: float = 1.0,
         show_load: bool = False,
         load_alpha: float = 1.0,
         show_constrain_dof: bool = False,
+        show_beam_sec: bool = False,
+        beam_sec_paras: dict = None,
         label_size: float = 8,
         show_outline: bool = True,
         opacity: float = 1.0,
         save_html: str = None,
     ):
         """
         Visualize the model in the current domain.
@@ -191,14 +193,21 @@
                 when adding the ``load`` or ``eleLoad`` command,
                 even if the value is 0.
 
         load_alpha: float, default = 1.0
             On existing displays, the scaling factor for the load arrow sizes.
         show_constrain_dof: bool, default=False
             Whether to display labels for constrained degrees of freedom.
+        show_beam_sec: bool default = False
+            Whether to render the 3d section of beam or truss elements.
+            If True, the Arg `beam_sec` in :py:meth:`opstool.vis.GetFEMdata.get_model_data`
+            must be assigned in advance.
+        beam_sec_paras: dict defalut = None,
+            A dict to control beam section render, optional key: color, opacity.
+            Note that the backend plotly does not currently support texture.
         label_size: float, default=8
             The foontsize of node and ele label.
         show_outline: bool, default=True
             Whether to show the axis frame.
         opacity: float, default=1.0
             Plane and solid element transparency.
         save_html: str, default=None
@@ -222,14 +231,16 @@
             show_local_crd=show_local_crd,
             local_crd_alpha=local_crd_alpha,
             show_fix_node=show_fix_node,
             fix_node_alpha=fix_node_alpha,
             show_load=show_load,
             load_alpha=load_alpha,
             show_constrain_dof=show_constrain_dof,
+            show_beam_sec=show_beam_sec,
+            beam_sec_paras=beam_sec_paras,
             label_size=label_size,
             show_outline=show_outline,
             opacity=opacity,
             save_html=save_html,
         )
 
     def eigen_vis(
```

### Comparing `opstool-0.8.0/src/opstool/vis/ops_vis_pyvista.py` & `opstool-0.8.1/src/opstool/vis/ops_vis_pyvista.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool/vis/quick_plot.py` & `opstool-0.8.1/src/opstool/vis/quick_plot.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/src/opstool.egg-info/PKG-INFO` & `opstool-0.8.1/src/opstool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opstool
-Version: 0.8.0
+Version: 0.8.1
 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
 Keywords: OpenSees Visualization Seismic Simulation
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opstool Version: 0.8.0 Summary: openseespy toolbox
+Metadata-Version: 2.1 Name: opstool Version: 0.8.1 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992 Author: Yexiang Yan Author-email:
 yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees Visualization
 Seismic Simulation Platform: any Classifier: Programming Language :: Python ::
 3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENCE.txt
                                     opstool
            modelling, visualization, post-processing for OpenSeesPy.
```

### Comparing `opstool-0.8.0/src/opstool.egg-info/SOURCES.txt` & `opstool-0.8.1/src/opstool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/tests/test_dambreak.py` & `opstool-0.8.1/tests/test_dambreak.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/tests/test_fiber_sec_vis.py` & `opstool-0.8.1/tests/test_fiber_sec_vis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/tests/test_model_vis.py` & `opstool-0.8.1/tests/test_model_vis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # %%
 import openseespy.opensees as ops
 import opstool as opst
 
 #
 opst.load_ops_examples("ArchBridge")
-opst.load_ops_examples("CableStayedBridge")
+# opst.load_ops_examples("CableStayedBridge")
 # opst.load_ops_examples("Dam")
 # opst.load_ops_examples("Frame3D")
 # opst.load_ops_examples("Igloo")
 # opst.load_ops_examples("Pier")
 # opst.load_ops_examples("SuspensionBridge")
 # opst.plot_model(backend="pyvista")    # or backend="plotly"
 # opst.plot_eigen(mode_tags=[1, 12], backend="pyvista", subplots=True)   # or backend="plotly"
-opst.gen_grav_load(ts_tag=1, pattern_tag=1, factor=-9.81, direction="Z")
+# opst.gen_grav_load(ts_tag=1, pattern_tag=1, factor=-9.81, direction="Z")
 ModelData = opst.GetFEMdata()
 ModelData.get_model_data()
 ModelData.get_eigen_data(mode_tag=15)
-opsv = opst.OpsVisPlotly(
+opsv = opst.OpsVisPyvista(
     point_size=4,
     line_width=4,
     colors_dict=None,
-    theme="plotly",
     color_map="jet",
     on_notebook=False,
     results_dir="opstool_output",
 )
 fig = opsv.model_vis(
     show_node_label=False,
     show_ele_label=False,
-    show_local_crd=True,
+    show_local_crd=False,
     show_fix_node=True,
     # show_load=True,
     # load_alpha=0.5,
     label_size=8,
     show_outline=True,
     opacity=1.0,
 )
```

### Comparing `opstool-0.8.0/tests/test_sec_analysis.py` & `opstool-0.8.1/tests/test_sec_analysis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.8.0/tests/test_sec_mesh.py` & `opstool-0.8.1/tests/test_sec_mesh.py`

 * *Files identical despite different names*

