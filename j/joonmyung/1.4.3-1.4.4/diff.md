# Comparing `tmp/joonmyung-1.4.3.tar.gz` & `tmp/joonmyung-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/joonmyung-1.4.3.tar", last modified: Sun Apr 16 11:49:36 2023, max compression
+gzip compressed data, was "dist/joonmyung-1.4.4.tar", last modified: Fri May 12 04:54:10 2023, max compression
```

## Comparing `joonmyung-1.4.3.tar` & `joonmyung-1.4.4.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-04-16 11:49:36.000000 joonmyung-1.4.3/
--rw-r--r--   0 joonmyung   (501) staff       (20)      241 2023-04-16 11:49:36.000000 joonmyung-1.4.3/PKG-INFO
--rw-r--r--   0 joonmyung   (501) staff       (20)     1138 2023-04-06 18:15:10.000000 joonmyung-1.4.3/README.md
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-04-16 11:49:36.000000 joonmyung-1.4.3/joonmyung/
--rw-r--r--   0 joonmyung   (501) staff       (20)       15 2023-02-22 17:22:56.000000 joonmyung-1.4.3/joonmyung/__init__.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     6700 2023-04-03 12:26:27.000000 joonmyung-1.4.3/joonmyung/app.py
--rw-r--r--   0 joonmyung   (501) staff       (20)      695 2023-02-24 17:07:52.000000 joonmyung-1.4.3/joonmyung/data.py
--rw-r--r--   0 joonmyung   (501) staff       (20)    13369 2023-04-15 08:30:38.000000 joonmyung-1.4.3/joonmyung/draw.py
--rw-r--r--   0 joonmyung   (501) staff       (20)       29 2023-04-03 12:26:27.000000 joonmyung-1.4.3/joonmyung/dummy.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     2755 2023-02-22 17:22:56.000000 joonmyung-1.4.3/joonmyung/file.py
--rw-r--r--   0 joonmyung   (501) staff       (20)      920 2023-02-22 17:22:56.000000 joonmyung-1.4.3/joonmyung/gradcam.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     5375 2023-04-06 18:13:55.000000 joonmyung-1.4.3/joonmyung/log.py
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-04-16 11:49:36.000000 joonmyung-1.4.3/joonmyung/meta_data/
--rw-r--r--   0 joonmyung   (501) staff       (20)       41 2023-03-01 06:51:46.000000 joonmyung-1.4.3/joonmyung/meta_data/__init__.py
--rw-r--r--   0 joonmyung   (501) staff       (20)    45491 2023-02-22 17:22:56.000000 joonmyung-1.4.3/joonmyung/meta_data/label.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     2277 2023-03-01 06:32:47.000000 joonmyung-1.4.3/joonmyung/meta_data/utils.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     6030 2023-03-04 10:44:55.000000 joonmyung-1.4.3/joonmyung/metric.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     3214 2023-03-30 15:51:49.000000 joonmyung-1.4.3/joonmyung/script.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     1487 2023-03-01 13:25:20.000000 joonmyung-1.4.3/joonmyung/status.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     3949 2023-04-06 17:51:01.000000 joonmyung-1.4.3/joonmyung/utils.py
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-04-16 11:49:36.000000 joonmyung-1.4.3/joonmyung.egg-info/
--rw-r--r--   0 joonmyung   (501) staff       (20)      241 2023-04-16 11:49:36.000000 joonmyung-1.4.3/joonmyung.egg-info/PKG-INFO
--rw-r--r--   0 joonmyung   (501) staff       (20)      501 2023-04-16 11:49:36.000000 joonmyung-1.4.3/joonmyung.egg-info/SOURCES.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-04-16 11:49:36.000000 joonmyung-1.4.3/joonmyung.egg-info/dependency_links.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-03-08 20:12:53.000000 joonmyung-1.4.3/joonmyung.egg-info/not-zip-safe
--rw-r--r--   0 joonmyung   (501) staff       (20)       10 2023-04-16 11:49:36.000000 joonmyung-1.4.3/joonmyung.egg-info/top_level.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)       38 2023-04-16 11:49:36.000000 joonmyung-1.4.3/setup.cfg
--rw-r--r--   0 joonmyung   (501) staff       (20)      781 2023-04-16 11:49:33.000000 joonmyung-1.4.3/setup.py
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-12 04:54:10.000000 joonmyung-1.4.4/
+-rw-r--r--   0 joonmyung   (501) staff       (20)      241 2023-05-12 04:54:10.000000 joonmyung-1.4.4/PKG-INFO
+-rw-r--r--   0 joonmyung   (501) staff       (20)     1138 2023-04-06 18:15:10.000000 joonmyung-1.4.4/README.md
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung/
+-rw-r--r--   0 joonmyung   (501) staff       (20)       15 2023-02-22 17:22:56.000000 joonmyung-1.4.4/joonmyung/__init__.py
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung/analysis/
+-rw-r--r--   0 joonmyung   (501) staff       (20)      110 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/analysis/__init__.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     6956 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/analysis/analysis.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     4346 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/analysis/dataset.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)        0 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/analysis/hook.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     1192 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/analysis/metric.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     1825 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/analysis/model.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     6700 2023-04-03 12:26:27.000000 joonmyung-1.4.4/joonmyung/app.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)      695 2023-02-24 17:07:52.000000 joonmyung-1.4.4/joonmyung/data.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)    13576 2023-04-26 06:40:35.000000 joonmyung-1.4.4/joonmyung/draw.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)       29 2023-04-03 12:26:27.000000 joonmyung-1.4.4/joonmyung/dummy.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     2755 2023-02-22 17:22:56.000000 joonmyung-1.4.4/joonmyung/file.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)      920 2023-02-22 17:22:56.000000 joonmyung-1.4.4/joonmyung/gradcam.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     5375 2023-04-06 18:13:55.000000 joonmyung-1.4.4/joonmyung/log.py
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung/meta_data/
+-rw-r--r--   0 joonmyung   (501) staff       (20)       41 2023-03-01 06:51:46.000000 joonmyung-1.4.4/joonmyung/meta_data/__init__.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)    45491 2023-02-22 17:22:56.000000 joonmyung-1.4.4/joonmyung/meta_data/label.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     2252 2023-05-12 04:53:27.000000 joonmyung-1.4.4/joonmyung/meta_data/utils.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     6030 2023-03-04 10:44:55.000000 joonmyung-1.4.4/joonmyung/metric.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     3214 2023-03-30 15:51:49.000000 joonmyung-1.4.4/joonmyung/script.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     1487 2023-03-01 13:25:20.000000 joonmyung-1.4.4/joonmyung/status.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     3949 2023-04-06 17:51:01.000000 joonmyung-1.4.4/joonmyung/utils.py
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung.egg-info/
+-rw-r--r--   0 joonmyung   (501) staff       (20)      241 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung.egg-info/PKG-INFO
+-rw-r--r--   0 joonmyung   (501) staff       (20)      677 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung.egg-info/SOURCES.txt
+-rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung.egg-info/dependency_links.txt
+-rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung.egg-info/not-zip-safe
+-rw-r--r--   0 joonmyung   (501) staff       (20)       10 2023-05-12 04:54:10.000000 joonmyung-1.4.4/joonmyung.egg-info/top_level.txt
+-rw-r--r--   0 joonmyung   (501) staff       (20)       38 2023-05-12 04:54:10.000000 joonmyung-1.4.4/setup.cfg
+-rw-r--r--   0 joonmyung   (501) staff       (20)      781 2023-05-12 04:53:27.000000 joonmyung-1.4.4/setup.py
```

### Comparing `joonmyung-1.4.3/README.md` & `joonmyung-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.3/joonmyung/app.py` & `joonmyung-1.4.4/joonmyung/app.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.3/joonmyung/data.py` & `joonmyung-1.4.4/joonmyung/data.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.3/joonmyung/draw.py` & `joonmyung-1.4.4/joonmyung/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import PIL
 import os
 
 def drawHeatmap(matrixes, col=1, title=[], fmt=1, p=False,
                 vmin=None, vmax=None, xticklabels=False, yticklabels=False,
                 linecolor=None, linewidths=0.1, fontsize=30, r=[1,1],
                 cmap="Greys", cbar=True, l=0, border=False,
-                output_dir=None, file_name=None, show=True):
+                output_dir='./result', file_name=None, show=True):
     row = (len(matrixes) - 1) // col + 1
     annot = True if fmt > 0 else False
 
     if p:
         print("|- Parameter Information")
         print("  |- Data Info (G, H, W)")
         print("    |- G : Graph Num")
@@ -222,15 +222,15 @@
          or type(datas) == PIL.Image.Image:
         pils = datas
     else:
         raise ValueError
     return pils
 
 def drawImgPlot(datas:list, col=1, title:str=None, columns=None, showRows:list=None,
-    output_dir=None, file_name=None, show=True, p=False):
+    output_dir=None, file_name=None, show=True, fmt=1, p=False):
     if type(datas) != list or 'shape' not in dir(datas[0]) : datas = [datas]
 
     if showRows is not None:
         for d in range(len(datas)):
             datas[d] = datas[d][showRows]
     data_num = len(datas[0]) * len(datas)
     row = (data_num - 1) // col + 1
@@ -239,20 +239,22 @@
     fig.set_size_inches(col * 8, row * 8)
     if title: fig.suptitle(title, fontsize=16)
     for i in range(data_num):
         r_num, c_num   = i // col, i % col
         dr_num, dc_num = i // len(datas), i % len(datas)
         data = data2PIL(datas[dc_num][dr_num])
         ax = axes[r_num][c_num]
-        if "shape" not in dir(data):
+        if "shape" not in dir(data): # IMAGE
             ax.imshow(data)
-        elif data.shape[-1] == 3:
+        elif data.shape[-1] == 3: #
             ax.imshow(data)
-        elif data.shape[-1] == 1:
-            ax.imshow(data, cmap="gray")
+        elif data.shape[-1] == 1: #
+            # ax.imshow(data, cmap="gray")
+            sns.heatmap(data[:,:,0], annot=True, fmt=f".{fmt}f", cmap="Greys"
+                        , yticklabels=False, xticklabels=False, ax=ax, vmax=1.0, vmin=0.0)
         if columns:
             ax.set_title(columns[c_num] + str(r_num)) if len(columns) == col else ax.set_title(columns[i])
 
     plt.legend(bbox_to_anchor=(1.05, 1.0), loc='upper left')
     plt.tight_layout()
 
 
@@ -289,15 +291,15 @@
         for img, attn in zip(imgs, attns):
             result = overlay_mask(to_pil_image(img), to_pil_image(normalization(attn, type=0), mode='F')) # (3, 224, 224), (1, 14, 14)
             # plt.imshow(overlay_mask(to_pil_image(dataset.unNormalize(samples)[0]), to_pil_image(normalization(a[:, 0]), mode='F'), alpha=0.5))
             results.append(result)
     return results
 
 import copy
-def unNormalize(image, dataset):
+def unNormalize(image, dataset="imagenet"):
     # images : (B, C, H, W)
     if dataset == "imagenet":
         mean, std = [0.485, 0.456, 0.406], [0.229, 0.224, 0.225]
     elif dataset == "cifar":
         mean, std = [0.4914, 0.4822, 0.4465], [0.2023, 0.1994, 0.2010]
     else:
         return image
```

### Comparing `joonmyung-1.4.3/joonmyung/file.py` & `joonmyung-1.4.4/joonmyung/file.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.3/joonmyung/gradcam.py` & `joonmyung-1.4.4/joonmyung/gradcam.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.3/joonmyung/log.py` & `joonmyung-1.4.4/joonmyung/log.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.3/joonmyung/meta_data/label.py` & `joonmyung-1.4.4/joonmyung/meta_data/label.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.3/joonmyung/meta_data/utils.py` & `joonmyung-1.4.4/joonmyung/meta_data/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 def data2path(server, dataset,
               conference="", wandb_version="", wandb_name=""):
     if "kakao" in server:
         data_path = "/data/opensets/imagenet-pytorch"
         output_dir = "/data/project/rw/joonmyung/conference"
     elif server in ["148", "137", "151", "152", "113", "68", "67", "64"]:
-        data_path = "/hub_data/joonmyung/data"
-        output_dir = "/hub_data/joonmyung/conference"
+        data_path = "/hub_data1/joonmyung/data"
+        output_dir = "/hub_data1/joonmyung/conference"
     elif server in ["154"]:
         data_path = "/data1/joonmyung/data"
         output_dir = "/data1/joonmyung/conference"
     elif server in ["65"]:
         data_path = "/hub_data2/joonmyung/data"
         output_dir = "/hub_data2/joonmyung/conference"
     elif server in ["kisti"]:
@@ -30,15 +30,15 @@
     if dataset in ["imagenet", "IMNET"]:
         if "kakao" in server:
             data_path = os.path.join(data_path, "imagenet-pytorch")
         else:
             data_path = os.path.join(data_path, "imagenet")
 
 
-    output_dir = os.path.join(output_dir, conference, wandb_version, wandb_name) if conference else os.path.join(output_dir, "ETC")
+    output_dir = os.path.join(output_dir, conference, wandb_version, wandb_name) if conference else None
 
 
     return data_path, output_dir
 
 def get_label(key, d_name ="imagenet"):
     d_name = d_name.lower()
     if d_name in ["imagenet", "IMNET"] :
```

### Comparing `joonmyung-1.4.3/joonmyung/metric.py` & `joonmyung-1.4.4/joonmyung/metric.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.3/joonmyung/script.py` & `joonmyung-1.4.4/joonmyung/script.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.3/joonmyung/status.py` & `joonmyung-1.4.4/joonmyung/status.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.3/joonmyung/utils.py` & `joonmyung-1.4.4/joonmyung/utils.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.3/setup.py` & `joonmyung-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import find_packages
 setuptools.setup(
     name="joonmyung",
-    version="1.4.3",
+    version="1.4.4",
     author="JoonMyung Choi",
     author_email="pizard@korea.ac.kr",
     description="JoonMyung's Library",
     url="https://github.com/pizard/JoonMyung.git",
     license="MIT",
     packages=find_packages(exclude=["playground",
                                     "playground.*",
```

