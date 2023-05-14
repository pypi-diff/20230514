# Comparing `tmp/vctoolkit-0.1.9.8.tar.gz` & `tmp/vctoolkit-0.1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vctoolkit-0.1.9.8.tar", last modified: Tue Mar 22 14:08:21 2022, max compression
+gzip compressed data, was "dist\vctoolkit-0.1.9.9.tar", last modified: Wed Mar 23 02:19:29 2022, max compression
```

## Comparing `vctoolkit-0.1.9.8.tar` & `vctoolkit-0.1.9.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/
--rw-rw-rw-   0        0        0      346 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/PKG-INFO
--rw-rw-rw-   0        0        0       78 2020-05-16 02:53:55.000000 vctoolkit-0.1.9.8/README.md
--rw-rw-rw-   0        0        0       42 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/setup.cfg
--rw-rw-rw-   0        0        0      493 2022-03-22 14:04:53.000000 vctoolkit-0.1.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/vctoolkit/
--rw-rw-rw-   0        0        0    10248 2022-03-21 13:42:56.000000 vctoolkit-0.1.9.8/vctoolkit/io.py
--rw-rw-rw-   0        0        0     3898 2022-03-18 14:45:22.000000 vctoolkit-0.1.9.8/vctoolkit/lbs.py
--rw-rw-rw-   0        0        0     8161 2022-03-22 14:07:59.000000 vctoolkit-0.1.9.8/vctoolkit/math_np.py
--rw-rw-rw-   0        0        0    11225 2022-03-18 14:46:02.000000 vctoolkit-0.1.9.8/vctoolkit/misc.py
--rw-rw-rw-   0        0        0    10398 2022-03-22 14:04:44.000000 vctoolkit-0.1.9.8/vctoolkit/skeletons.py
-drwxrwxrwx   0        0        0        0 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/vctoolkit/tf/
--rw-rw-rw-   0        0        0     6915 2020-12-24 11:10:08.000000 vctoolkit-0.1.9.8/vctoolkit/tf/__init__.py
--rw-rw-rw-   0        0        0     6221 2022-03-20 14:20:38.000000 vctoolkit-0.1.9.8/vctoolkit/vis2d.py
--rw-rw-rw-   0        0        0     2928 2022-03-18 14:47:23.000000 vctoolkit-0.1.9.8/vctoolkit/vis3d.py
-drwxrwxrwx   0        0        0        0 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/vctoolkit/visgl/
--rw-rw-rw-   0        0        0     9164 2020-05-16 02:53:55.000000 vctoolkit-0.1.9.8/vctoolkit/visgl/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/vctoolkit/viso3d/
--rw-rw-rw-   0        0        0     3379 2022-03-21 13:49:44.000000 vctoolkit-0.1.9.8/vctoolkit/viso3d/__init__.py
--rw-rw-rw-   0        0        0      135 2021-12-21 02:24:14.000000 vctoolkit-0.1.9.8/vctoolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/vctoolkit.egg-info/
--rw-rw-rw-   0        0        0        1 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/vctoolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      346 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/vctoolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       75 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/vctoolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0      419 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/vctoolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2022-03-22 14:08:21.000000 vctoolkit-0.1.9.8/vctoolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/
+-rw-rw-rw-   0        0        0      346 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2020-05-16 02:53:55.000000 vctoolkit-0.1.9.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      493 2022-03-23 02:19:19.000000 vctoolkit-0.1.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/vctoolkit/
+-rw-rw-rw-   0        0        0    10248 2022-03-21 13:42:56.000000 vctoolkit-0.1.9.9/vctoolkit/io.py
+-rw-rw-rw-   0        0        0     3898 2022-03-18 14:45:22.000000 vctoolkit-0.1.9.9/vctoolkit/lbs.py
+-rw-rw-rw-   0        0        0     8161 2022-03-22 14:07:59.000000 vctoolkit-0.1.9.9/vctoolkit/math_np.py
+-rw-rw-rw-   0        0        0    11350 2022-03-23 02:14:19.000000 vctoolkit-0.1.9.9/vctoolkit/misc.py
+-rw-rw-rw-   0        0        0    10398 2022-03-22 14:04:44.000000 vctoolkit-0.1.9.9/vctoolkit/skeletons.py
+drwxrwxrwx   0        0        0        0 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/vctoolkit/tf/
+-rw-rw-rw-   0        0        0     6915 2020-12-24 11:10:08.000000 vctoolkit-0.1.9.9/vctoolkit/tf/__init__.py
+-rw-rw-rw-   0        0        0     6221 2022-03-20 14:20:38.000000 vctoolkit-0.1.9.9/vctoolkit/vis2d.py
+-rw-rw-rw-   0        0        0     2842 2022-03-23 02:19:06.000000 vctoolkit-0.1.9.9/vctoolkit/vis3d.py
+drwxrwxrwx   0        0        0        0 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/vctoolkit/visgl/
+-rw-rw-rw-   0        0        0     9164 2020-05-16 02:53:55.000000 vctoolkit-0.1.9.9/vctoolkit/visgl/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/vctoolkit/viso3d/
+-rw-rw-rw-   0        0        0     3379 2022-03-21 13:49:44.000000 vctoolkit-0.1.9.9/vctoolkit/viso3d/__init__.py
+-rw-rw-rw-   0        0        0      135 2021-12-21 02:24:14.000000 vctoolkit-0.1.9.9/vctoolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/vctoolkit.egg-info/
+-rw-rw-rw-   0        0        0        1 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/vctoolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      346 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/vctoolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/vctoolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      419 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/vctoolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2022-03-23 02:19:29.000000 vctoolkit-0.1.9.9/vctoolkit.egg-info/top_level.txt
```

### Comparing `vctoolkit-0.1.9.8/vctoolkit/io.py` & `vctoolkit-0.1.9.9/vctoolkit/io.py`

 * *Files identical despite different names*

### Comparing `vctoolkit-0.1.9.8/vctoolkit/lbs.py` & `vctoolkit-0.1.9.9/vctoolkit/lbs.py`

 * *Files identical despite different names*

### Comparing `vctoolkit-0.1.9.8/vctoolkit/math_np.py` & `vctoolkit-0.1.9.9/vctoolkit/math_np.py`

 * *Files identical despite different names*

### Comparing `vctoolkit-0.1.9.8/vctoolkit/misc.py` & `vctoolkit-0.1.9.9/vctoolkit/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,15 +73,15 @@
   if w is None:
     w = int(round(h / img.shape[0] * img.shape[1]))
   else:
     h = int(round(w / img.shape[1] * img.shape[0]))
   return imresize(img, (w, h))
 
 
-def render_gaussian_hmap(centers, shape, sigma=None):
+def render_gaussian_hmap(centers, shape, sigma=None, dtype=np.float32):
   """
   Render gaussian heat maps from given centers.
 
   Parameters
   ----------
   centers : np.ndarray, shape [N, 2]
     Gussian centers, (row, column).
@@ -96,23 +96,22 @@
     Rendered heat maps
   """
   if sigma is None:
     sigma = shape[0] / 40
   x = [i for i in range(shape[1])]
   y = [i for i in range(shape[0])]
   xx, yy = np.meshgrid(x, y)
-  xx = np.reshape(xx.astype(np.float32), [shape[0], shape[1], 1])
-  yy = np.reshape(yy.astype(np.float32), [shape[0], shape[1], 1])
+  xx = np.reshape(xx.astype(dtype), [shape[0], shape[1], 1])
+  yy = np.reshape(yy.astype(dtype), [shape[0], shape[1], 1])
   x = np.reshape(centers[:,1], [1, 1, -1])
   y = np.reshape(centers[:,0], [1, 1, -1])
-  distance = np.square(xx - x) + np.square(yy - y)
-  hmap = np.exp(-distance / (2 * sigma**2 )) / np.sqrt(2 * np.pi * sigma**2)
-  hmap /= (
-    np.max(hmap, axis=(0, 1), keepdims=True) + np.finfo(np.float32).eps
-  )
+  distance = np.square(xx - x, dtype=dtype) + np.square(yy - y, dtype=dtype)
+  hmap = np.exp(-distance / (2 * sigma**2 ), dtype=dtype) / \
+         np.sqrt(2 * np.pi * sigma**2, dtype=dtype)
+  hmap /= (np.max(hmap, axis=(0, 1), keepdims=True) + np.finfo(dtype).eps)
   return hmap
 
 
 def print_important(s, sep='='):
   """
   Print important message.
 
@@ -475,14 +474,16 @@
 
 
 def examine_dict(data, indent=0):
   for k, v in data.items():
     print('  ' * indent, k, type(v), end=', ')
     if hasattr(v, 'shape'):
       print(f'shape = {v.shape}')
+      if hasattr(v,'dtype'):
+        print(f' | dtype = {v.dtype}')
     elif type(v) == dict:
       print()
       examine_dict(v, indent + 1)
     elif hasattr(v, '__len__'):
       print(f'length = {len(v)}')
     else:
       print()
@@ -490,8 +491,7 @@
 
 def set_extension(file_name, ext):
   return os.path.splitext(file_name)[0] + '.' + ext
 
 
 def count_model_parameters(model):
   return sum(p.numel() for p in model.parameters() if p.requires_grad)
-
```

### Comparing `vctoolkit-0.1.9.8/vctoolkit/skeletons.py` & `vctoolkit-0.1.9.9/vctoolkit/skeletons.py`

 * *Files identical despite different names*

### Comparing `vctoolkit-0.1.9.8/vctoolkit/tf/__init__.py` & `vctoolkit-0.1.9.9/vctoolkit/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `vctoolkit-0.1.9.8/vctoolkit/vis2d.py` & `vctoolkit-0.1.9.9/vctoolkit/vis2d.py`

 * *Files identical despite different names*

### Comparing `vctoolkit-0.1.9.8/vctoolkit/vis3d.py` & `vctoolkit-0.1.9.9/vctoolkit/vis3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,14 @@
   Returns
   -------
   np.ndarray, shape [v, 3]
     Vertices of the mesh.
   np.ndarray, shape [f, 3]
     Face indices of the mesh.
   """
-  if colors is None and hasattr(skeleton, 'colors'):
-    colors = skeleton.colors
-
   n_bones = len(list(filter(lambda x: x is not None, skeleton.parents)))
   faces = np.empty([n_bones * 8, 3], dtype=np.int32)
   verts = np.empty([n_bones * 6, 3], dtype=np.float32)
   face_color = []
   bone_idx = -1
   for child, parent in enumerate(skeleton.parents):
     if parent is None:
@@ -78,14 +75,14 @@
     faces[bone_idx*8+7] = \
       np.flip(np.array([1, 2, 5], dtype=np.int32), axis=0) + bone_idx * 6
 
     if colors is not None:
       for _ in range(8):
         face_color.append(colors[child])
 
-  if colors is not None:
-    return verts, faces, face_color
-
   if save_path is not None:
     save(save_path, (verts, faces))
 
+  if colors is not None:
+    return verts, faces, face_color
+
   return verts, faces
```

### Comparing `vctoolkit-0.1.9.8/vctoolkit/visgl/__init__.py` & `vctoolkit-0.1.9.9/vctoolkit/visgl/__init__.py`

 * *Files identical despite different names*

### Comparing `vctoolkit-0.1.9.8/vctoolkit/viso3d/__init__.py` & `vctoolkit-0.1.9.9/vctoolkit/viso3d/__init__.py`

 * *Files identical despite different names*

