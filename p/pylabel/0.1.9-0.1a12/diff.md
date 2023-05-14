# Comparing `tmp/pylabel-0.1.9.tar.gz` & `tmp/pylabel-0.1a12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylabel-0.1.9.tar", last modified: Fri Nov 12 15:12:59 2021, max compression
+gzip compressed data, was "dist/pylabel-0.1a12.tar", last modified: Wed Nov 24 06:54:29 2021, max compression
```

## Comparing `pylabel-0.1.9.tar` & `pylabel-0.1a12.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-11-12 15:12:58.976914 pylabel-0.1.9/
--rw-r--r--   0 alex       (501) staff       (20)     1069 2021-10-19 01:51:34.000000 pylabel-0.1.9/LICENSE.txt
--rw-r--r--   0 alex       (501) staff       (20)      233 2021-11-12 15:12:58.976670 pylabel-0.1.9/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     2228 2021-11-08 05:51:32.000000 pylabel-0.1.9/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-11-12 15:12:58.974044 pylabel-0.1.9/pylabel/
--rw-r--r--   0 alex       (501) staff       (20)       84 2021-10-19 01:51:34.000000 pylabel-0.1.9/pylabel/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1814 2021-11-07 03:03:39.000000 pylabel-0.1.9/pylabel/analyze.py
--rw-r--r--   0 alex       (501) staff       (20)      864 2021-10-31 18:39:25.000000 pylabel-0.1.9/pylabel/constants.py
--rw-r--r--   0 alex       (501) staff       (20)      847 2021-11-07 03:14:25.000000 pylabel-0.1.9/pylabel/dataset.py
--rw-r--r--   0 alex       (501) staff       (20)    16636 2021-11-02 14:24:44.000000 pylabel-0.1.9/pylabel/exporter.py
--rw-r--r--   0 alex       (501) staff       (20)    10206 2021-11-06 16:42:36.000000 pylabel-0.1.9/pylabel/importer.py
--rw-r--r--   0 alex       (501) staff       (20)     6968 2021-11-12 14:47:08.000000 pylabel-0.1.9/pylabel/labeler.py
--rw-r--r--   0 alex       (501) staff       (20)     6287 2021-10-27 15:39:36.000000 pylabel-0.1.9/pylabel/splitter.py
--rw-r--r--   0 alex       (501) staff       (20)     1586 2021-10-30 15:43:11.000000 pylabel-0.1.9/pylabel/visualize.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-11-12 15:12:58.976365 pylabel-0.1.9/pylabel.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      233 2021-11-12 15:12:56.000000 pylabel-0.1.9/pylabel.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      363 2021-11-12 15:12:56.000000 pylabel-0.1.9/pylabel.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2021-11-12 15:12:56.000000 pylabel-0.1.9/pylabel.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       81 2021-11-12 15:12:56.000000 pylabel-0.1.9/pylabel.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)        8 2021-11-12 15:12:56.000000 pylabel-0.1.9/pylabel.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2021-11-12 15:12:58.976978 pylabel-0.1.9/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      353 2021-11-12 14:49:50.000000 pylabel-0.1.9/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-11-24 06:54:29.504881 pylabel-0.1a12/
+-rw-r--r--   0 alex       (501) staff       (20)      241 2021-11-24 06:54:29.504527 pylabel-0.1a12/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     2228 2021-11-08 05:51:32.000000 pylabel-0.1a12/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-11-24 06:54:29.439239 pylabel-0.1a12/pylabel/
+-rw-r--r--   0 alex       (501) staff       (20)       84 2021-10-19 01:51:34.000000 pylabel-0.1a12/pylabel/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2085 2021-11-24 00:08:10.000000 pylabel-0.1a12/pylabel/analyze.py
+-rw-r--r--   0 alex       (501) staff       (20)      877 2021-11-24 06:48:26.000000 pylabel-0.1a12/pylabel/constants.py
+-rw-r--r--   0 alex       (501) staff       (20)      855 2021-11-13 15:32:25.000000 pylabel-0.1a12/pylabel/dataset.py
+-rw-r--r--   0 alex       (501) staff       (20)    16885 2021-11-24 06:51:18.000000 pylabel-0.1a12/pylabel/exporter.py
+-rw-r--r--   0 alex       (501) staff       (20)    10437 2021-11-22 18:02:08.000000 pylabel-0.1a12/pylabel/importer.py
+-rw-r--r--   0 alex       (501) staff       (20)     9007 2021-11-24 04:27:23.000000 pylabel-0.1a12/pylabel/labeler.py
+-rw-r--r--   0 alex       (501) staff       (20)     6287 2021-10-27 15:39:36.000000 pylabel-0.1a12/pylabel/splitter.py
+-rw-r--r--   0 alex       (501) staff       (20)     1586 2021-10-30 15:43:11.000000 pylabel-0.1a12/pylabel/visualize.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-11-24 06:54:29.503492 pylabel-0.1a12/pylabel.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      241 2021-11-24 06:54:29.000000 pylabel-0.1a12/pylabel.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      351 2021-11-24 06:54:29.000000 pylabel-0.1a12/pylabel.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2021-11-24 06:54:29.000000 pylabel-0.1a12/pylabel.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       88 2021-11-24 06:54:29.000000 pylabel-0.1a12/pylabel.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)        8 2021-11-24 06:54:29.000000 pylabel-0.1a12/pylabel.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2021-11-24 06:54:29.505045 pylabel-0.1a12/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      364 2021-11-24 06:53:28.000000 pylabel-0.1a12/setup.py
```

### Comparing `pylabel-0.1.9/README.md` & `pylabel-0.1a12/README.md`

 * *Files identical despite different names*

### Comparing `pylabel-0.1.9/pylabel/analyze.py` & `pylabel-0.1a12/pylabel/analyze.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 import pandas as pd
 import numpy as np
 
 class Analyze:
 
     def  __init__(self, dataset=None):
-        self.dataset = dataset 
-        ds = self.dataset
-        self.class_counts = ds.df["cat_name"].value_counts(dropna=False)
-        self.num_classes = ds.df["cat_name"].nunique()
-        self.classes = list(ds.df["cat_name"].unique())
-        self.num_images = ds.df["img_filename"].nunique()
-        self.split_counts = ds.df["split"].value_counts(dropna=False)
-        self.split_pct = ds.df["split"].value_counts(normalize=True, dropna=False)
+        self.dataset = dataset
+        #self.split_counts = ds.df["split"].value_counts(dropna=False)
+        #self.split_pct = ds.df["split"].value_counts(normalize=True, dropna=False)
+    
+    @property 
+    def classes(self):
+        cat_names = list(self.dataset.df.cat_name.unique())
+        return [i for i in cat_names if i.strip() != '']
+
+    @property 
+    def class_counts(self):
+        return self.dataset.df["cat_name"].value_counts(dropna=False)
+
+    @property 
+    def num_classes(self):
+        cat_names = list(self.dataset.df.cat_name.unique())
+        return len([i for i in cat_names if i.strip() != ''])
         
+    @property 
+    def num_images(self):
+        return self.dataset.df["img_filename"].nunique()
+
     def ShowClassSplits(self, normalize=True):
         ds = self.dataset
 
         def move_column_inplace(df, col, pos):
             """
             Assists to rearrange columns to a desired order. 
             """
```

### Comparing `pylabel-0.1.9/pylabel/constants.py` & `pylabel-0.1a12/pylabel/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 #########
 # This file has variables that are used by the rest of the package 
 #########
 
 #These are the valid columns in the pylabel annotations table.              
-schema = ['img_folder','img_filename','img_path','img_id','img_width','img_height','img_depth','ann_segmented','ann_bbox_xmin','ann_bbox_ymin','ann_bbox_xmax','ann_bbox_ymax','ann_bbox_width','ann_bbox_height','ann_area','ann_segmentation','ann_iscrowd','ann_pose','ann_truncated','ann_difficult','cat_id','cat_name','cat_supercategory','split']
+schema = ['img_folder','img_filename','img_path','img_id','img_width','img_height','img_depth','ann_segmented','ann_bbox_xmin','ann_bbox_ymin','ann_bbox_xmax','ann_bbox_ymax','ann_bbox_width','ann_bbox_height','ann_area','ann_segmentation','ann_iscrowd','ann_pose','ann_truncated','ann_difficult','cat_id','cat_name','cat_supercategory','split', 'annotated']
 #schema = ['id','img_folder','img_filename','img_path','img_id','img_width','img_height','img_depth','ann_segmented','ann_bbox_xmin','ann_bbox_ymin','ann_bbox_xmax','ann_bbox_ymax','ann_bbox_width','ann_bbox_height','ann_area','ann_segmentation','ann_iscrowd','ann_pose','ann_truncated','ann_difficult','cat_id','cat_name','cat_supercategory','split']
```

### Comparing `pylabel-0.1.9/pylabel/dataset.py` & `pylabel-0.1a12/pylabel/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,12 +17,12 @@
         self.name = "dataset"
         self.path_to_annotations = ""    
         self.GroupShuffleSplit = GroupShuffleSplit
         self.test = test
         self.StratifiedGroupShuffleSplit = StratifiedGroupShuffleSplit
         self.export = Export(dataset=self)
         self.visualize = Visualize(dataset=self)
-        self.analyze = Analyze(self)
+        self.analyze = Analyze(dataset=self)
         self.labeler = Labeler(self)
 
         #self.splitter = Splitter(dataset=self)
```

### Comparing `pylabel-0.1.9/pylabel/exporter.py` & `pylabel-0.1a12/pylabel/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import xml.dom.minidom
 import os 
 from pathlib import PurePath, Path
 
 class Export():
     def  __init__(self, dataset=None):
         self.dataset = dataset
-        
+
     def ExportToVoc(self, output_path=None, segmented_=False, path_=False, database_=False, folder_=False, occluded_=False):
         ds = self.dataset
 
         if output_path == None:
             output_path = ds.path_to_annotations
         else:        
             output_path = output_path
@@ -214,14 +214,22 @@
                 If not-specified then the path will be derived from the .path_to_annotations and
                 .name properties of the dataset object. 
 
         Returns:
             A list with 1 or more paths (strings) to annotations files.
         """
         ds = self.dataset
+
+        #Drop rows that are not annotated
+        #Note, having zero annotates can still be considered annotated 
+        #in cases there are no objects in the image thats should be indentified
+        ds.df = ds.df.loc[ds.df["annotated"] == 1]
+        
+
+
         #Inspired by https://github.com/aws-samples/groundtruth-object-detection/blob/master/create_annot.py 
         unique_images = ds.df["img_filename"].unique()
         output_file_paths = []
 
         yolo_dataset = ds.df.copy(deep=True)
         yolo_dataset.cat_id = yolo_dataset.cat_id.str.strip()
         yolo_dataset.cat_id = yolo_dataset.cat_id.astype('float').astype('Int32')
```

### Comparing `pylabel-0.1.9/pylabel/importer.py` & `pylabel-0.1a12/pylabel/importer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import pandas as pd
 import xml.etree.ElementTree as ET
 import os
+from os.path import exists
 from pathlib import Path, PurePath
 import copy
 import cv2
 
 from pylabel.constants import schema
 from pylabel.dataset import Dataset
 from pylabel.exporter import Export
@@ -186,14 +187,19 @@
 
                 cat_id, x_center_norm, y_center_norm, width_norm, height_norm = line.split()
                 row["img_folder"] = path_to_images
                 row["img_filename"] = filename.name.replace("txt",img_ext)
 
                 #Get the path to the image file to extract the height, width, and depth
                 image_path = PurePath(path, path_to_images, row["img_filename"])
+
+                #Check if there is a file at this location.
+                assert exists(image_path), f"File does not exist: {image_path}. Check path_to_images and img_ext arguments."
+
+                
                 im = cv2.imread(str(image_path))
                 img_height, img_width, img_depth =  im.shape
 
                 row["img_id"] = img_id
                 row["img_width"] = img_width
                 row["img_height"] = img_height
                 row["img_depth"] = img_depth
```

### Comparing `pylabel-0.1.9/pylabel/splitter.py` & `pylabel-0.1a12/pylabel/splitter.py`

 * *Files identical despite different names*

### Comparing `pylabel-0.1.9/pylabel/visualize.py` & `pylabel-0.1a12/pylabel/visualize.py`

 * *Files identical despite different names*

