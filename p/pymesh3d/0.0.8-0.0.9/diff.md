# Comparing `tmp/pymesh3d-0.0.8-py3-none-any.whl.zip` & `tmp/pymesh3d-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 8210 bytes, number of entries: 19
+Zip file size: 8208 bytes, number of entries: 19
 -rw-r--r--  2.0 unx       87 b- defN 23-Mar-22 07:09 pymesh/__init__.py
 -rw-r--r--  2.0 unx       30 b- defN 23-Mar-22 07:09 pymesh/colormap/__init__.py
 -rw-r--r--  2.0 unx      166 b- defN 23-Mar-22 07:09 pymesh/colormap/colormap.py
 -rw-r--r--  2.0 unx       81 b- defN 23-Mar-22 07:09 pymesh/interp3d/__init__.py
 -rw-r--r--  2.0 unx      261 b- defN 23-Mar-22 07:09 pymesh/interp3d/interp_color.py
 -rw-r--r--  2.0 unx     1242 b- defN 23-Mar-22 07:09 pymesh/interp3d/rotate.py
 -rw-r--r--  2.0 unx       34 b- defN 23-Mar-22 07:09 pymesh/iso_surf/__init__.py
 -rw-r--r--  2.0 unx     1006 b- defN 23-Mar-22 07:09 pymesh/iso_surf/iso_surf.py
 -rw-r--r--  2.0 unx     1888 b- defN 23-Mar-22 07:21 pymesh/iso_surf/marching_cubes.py
 -rw-r--r--  2.0 unx       22 b- defN 23-Mar-22 08:14 pymesh/mesh/__init__.py
 -rw-r--r--  2.0 unx     1380 b- defN 23-Mar-22 08:17 pymesh/mesh/mesh.py
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-22 07:09 pymesh/show/__init__.py
 -rw-r--r--  2.0 unx      261 b- defN 23-Mar-22 07:25 pymesh/show/mlab_plot.py
 -rw-r--r--  2.0 unx     1634 b- defN 23-Mar-22 07:09 pymesh/show/plt_plot.py
--rw-r--r--  2.0 unx     1064 b- defN 23-Mar-22 12:46 pymesh3d-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2564 b- defN 23-Mar-22 12:46 pymesh3d-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-22 12:46 pymesh3d-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-22 12:46 pymesh3d-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1527 b- defN 23-Mar-22 12:46 pymesh3d-0.0.8.dist-info/RECORD
-19 files, 13422 bytes uncompressed, 5708 bytes compressed:  57.5%
+-rw-r--r--  2.0 unx     1064 b- defN 23-Mar-22 12:55 pymesh3d-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2565 b- defN 23-Mar-22 12:55 pymesh3d-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-22 12:55 pymesh3d-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Mar-22 12:55 pymesh3d-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1527 b- defN 23-Mar-22 12:55 pymesh3d-0.0.9.dist-info/RECORD
+19 files, 13423 bytes uncompressed, 5706 bytes compressed:  57.5%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: pymesh/show/mlab_plot.py
 Comment: 
 
 Filename: pymesh/show/plt_plot.py
 Comment: 
 
-Filename: pymesh3d-0.0.8.dist-info/LICENSE
+Filename: pymesh3d-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: pymesh3d-0.0.8.dist-info/METADATA
+Filename: pymesh3d-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pymesh3d-0.0.8.dist-info/WHEEL
+Filename: pymesh3d-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pymesh3d-0.0.8.dist-info/top_level.txt
+Filename: pymesh3d-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pymesh3d-0.0.8.dist-info/RECORD
+Filename: pymesh3d-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pymesh3d-0.0.8.dist-info/LICENSE` & `pymesh3d-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pymesh3d-0.0.8.dist-info/METADATA` & `pymesh3d-0.0.9.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymesh3d
-Version: 0.0.8
+Version: 0.0.9
 Summary: mesh extract and render by python
 Home-page: https://github.com/zhazhajust/pymesh.git
 Author: Cai Jie
 Author-email: jiecai@stu.pku.edu.cn
 License: UNKNOWN
 Description-Content-Type: text/markdown
 Platform: UNKNOWN
@@ -18,19 +18,19 @@
 Requires-Dist: vtk
 Requires-Dist: matplotlib
 Requires-Dist: trimesh
 
 
 # PyMesh3D
 
-This project for mesh render in data science.
-
 ## Basic Installation
 
-```shell
+This project for mesh render in data science.
+
+```python
 conda create -n pymesh3d python=3.6
 conda activate pymesh3d
 pip install pymesh3d
 ```
 
 ## Quick Start
```

## Comparing `pymesh3d-0.0.8.dist-info/RECORD` & `pymesh3d-0.0.9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 pymesh/iso_surf/iso_surf.py,sha256=SDs-ZWMnLal9OU54yFhp-Q0n7pwAUwXKB6lkJSxHGQ4,1006
 pymesh/iso_surf/marching_cubes.py,sha256=LYZgr4jrCk73kxMnXJpmY-a57Nvzy6gA7QxWHjjS8Zg,1888
 pymesh/mesh/__init__.py,sha256=sjC-ffyugXQfrocv7H8UDuR4hjVdjkBkRcCYZUsem2A,22
 pymesh/mesh/mesh.py,sha256=qD0mLkg5cojujHyF1gnLQRpAt19cGm9Rte1c7PvkFwU,1380
 pymesh/show/__init__.py,sha256=E2PJVqAQyWBMRJsabSbNATc5j8a79tTunWyZqHS2wkU,76
 pymesh/show/mlab_plot.py,sha256=vE47DuzFrzEvtZqWsx0v2jnizrBWTlSzQhTBxXQWnjE,261
 pymesh/show/plt_plot.py,sha256=Vr1uOeFc318KFTqaFusrwbthOsc5EN0o4fKSTCEwv_g,1634
-pymesh3d-0.0.8.dist-info/LICENSE,sha256=zqyn0bIMoOQs_3k4MZfyQlEfbbVsx8s7hh8E1VapdXY,1064
-pymesh3d-0.0.8.dist-info/METADATA,sha256=c_z5oP-MBJZpyowbVpXYvwRfWcCw5624h0oTzAjsXRM,2564
-pymesh3d-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pymesh3d-0.0.8.dist-info/top_level.txt,sha256=dmufgfhy9374FeEv98trixob_XFC_bIZwJCmBLGpi7I,7
-pymesh3d-0.0.8.dist-info/RECORD,,
+pymesh3d-0.0.9.dist-info/LICENSE,sha256=zqyn0bIMoOQs_3k4MZfyQlEfbbVsx8s7hh8E1VapdXY,1064
+pymesh3d-0.0.9.dist-info/METADATA,sha256=YaiR2fjyPvjDxB1hB61hD62UBH4ccKz8reLqLCSK-fk,2565
+pymesh3d-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pymesh3d-0.0.9.dist-info/top_level.txt,sha256=dmufgfhy9374FeEv98trixob_XFC_bIZwJCmBLGpi7I,7
+pymesh3d-0.0.9.dist-info/RECORD,,
```

