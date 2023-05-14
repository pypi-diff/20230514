# Comparing `tmp/onnx2kerastl-0.0.86.tar.gz` & `tmp/onnx2kerastl-0.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.86.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.87.tar", max compression
```

## Comparing `onnx2kerastl-0.0.86.tar` & `onnx2kerastl-0.0.87.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1067 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/LICENSE
--rw-r--r--   0        0        0       66 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.86/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.86/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    13572 2023-05-08 05:49:57.483750 onnx2kerastl-0.0.86/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11968 2023-05-08 05:48:07.717080 onnx2kerastl-0.0.86/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      584 2023-05-08 05:48:07.745079 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1730 2023-05-08 05:48:07.745079 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2022-09-29 08:59:30.260148 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9372 2023-04-24 14:18:00.054331 onnx2kerastl-0.0.86/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3867 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.86/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.86/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3791 2023-05-08 05:48:07.745079 onnx2kerastl-0.0.86/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5551 2023-05-08 05:48:07.717080 onnx2kerastl-0.0.86/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    15619 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.86/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.86/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.86/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    17867 2023-05-08 05:48:07.753079 onnx2kerastl-0.0.86/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     5354 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.86/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.86/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     4415 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.86/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1030 2023-05-09 06:01:41.299601 onnx2kerastl-0.0.86/pyproject.toml
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.86/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-05-24 13:45:54.506384 onnx2kerastl-0.0.87/LICENSE
+-rw-r--r--   0        0        0       66 2022-05-26 14:37:02.229998 onnx2kerastl-0.0.87/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-30 14:23:13.629683 onnx2kerastl-0.0.87/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-07-21 11:24:20.166257 onnx2kerastl-0.0.87/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2022-10-13 14:52:08.546058 onnx2kerastl-0.0.87/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    13572 2023-05-14 16:26:09.893812 onnx2kerastl-0.0.87/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11968 2023-05-14 16:26:09.894508 onnx2kerastl-0.0.87/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      584 2023-05-14 16:26:09.896883 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2022-10-19 12:00:07.113921 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-05-30 10:49:29.064709 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2022-05-24 13:45:54.510879 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1730 2023-05-14 16:26:09.897336 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2022-08-04 16:14:29.703956 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-05-30 11:45:55.347781 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9372 2023-04-30 14:23:13.630051 onnx2kerastl-0.0.87/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-07-21 11:24:20.167508 onnx2kerastl-0.0.87/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-04-30 14:23:13.630361 onnx2kerastl-0.0.87/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-04-02 11:17:38.561077 onnx2kerastl-0.0.87/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3791 2023-05-14 16:26:09.898000 onnx2kerastl-0.0.87/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-05-24 13:45:54.512524 onnx2kerastl-0.0.87/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5551 2023-05-14 16:26:09.898639 onnx2kerastl-0.0.87/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    15619 2023-04-30 14:23:13.630719 onnx2kerastl-0.0.87/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-04-30 14:23:13.631034 onnx2kerastl-0.0.87/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-04-02 11:17:38.563036 onnx2kerastl-0.0.87/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    17943 2023-05-14 16:26:09.900619 onnx2kerastl-0.0.87/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     5271 2023-05-14 16:26:20.525387 onnx2kerastl-0.0.87/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-04-02 11:17:38.563943 onnx2kerastl-0.0.87/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     4415 2023-04-02 11:17:38.564336 onnx2kerastl-0.0.87/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1030 2023-05-14 16:27:26.673934 onnx2kerastl-0.0.87/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.87/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.86/LICENSE` & `onnx2kerastl-0.0.87/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.87/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/__init__.py` & `onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxlstm.py` & `onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxlstm.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/ltsm_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/reshape_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,16 @@
             axis_index = axes_positives.index(axis)
             start = starts[axis_index]
             end = ends[axis_index] if ends[axis_index] < 2147483647 else None
             step = steps[axis_index]
             slice_spec_param.append({'start': start, 'step': step, 'stop': end})
         else:
             slice_spec_param.append({'start': None, 'step': None, 'stop': None})
-    if is_numpy(layers[node.input[0]]) and not np.array([not x is None for x in layers[node.input[0]]]).all(): # shape with None
+    if is_numpy(layers[node.input[0]]) and np.array([_shape is None for _shape in layers[node.input[0]]]).any()\
+            and len(layers[node.input[0]].shape) == 1: # slice numpy array which is a shape
         sliced = layers[node.input[0]][start:end:step]
     else:
         input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
         slicing_layer = SlicingOpLambda(tf.__operators__.getitem)
         sliced = slicing_layer(input_0, slice_spec=slice_spec_param)
         if is_numpy(layers[node.input[0]]):
             sliced = sliced.numpy()
```

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/sampling_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/sampling_layers.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,29 +27,25 @@
     params['padding_mode'] = params['padding_mode'].decode('ascii')
     img = layers[node.input[0]]
     sample_grid = layers[node.input[1]]
     torch_shape = tf.shape(img)
     max_xy = tf.expand_dims(
         tf.expand_dims(tf.expand_dims(tf.convert_to_tensor([torch_shape[3] - 1, torch_shape[2] - 1]), 0), 0), 0)
     max_xy = tf.cast(max_xy, tf.float32)
-    grid_index_coords = 0.5 * (sample_grid + 1.) * max_xy # transform from [-1,1] to [0,H-1]/[0,W-1]
+    grid_index_coords = 0.5 * (sample_grid + 1.) * max_xy  # transform from [-1,1] to [0,H-1]/[0,W-1]
     lambda_layer = keras.layers.Lambda(interpolate_wrapper, name=keras_name)
     layers[node_name] = lambda_layer([img, grid_index_coords, torch_shape])
 
 
-def interpolate_wrapper(x):
-    return _interpolate_bilinear_impl(x[0], x[1], x[2])
-
-
-def _interpolate_bilinear_impl(
-        torch_img,
-        grid_index_coords,
-        torch_shape,
-) -> tf.Tensor:
+def interpolate_wrapper(x) -> tf.Tensor:
     """tf.function implementation of interpolate_bilinear."""
+    torch_img = x[0]
+    grid_index_coords = x[1]
+    torch_shape = x[2]
+
     grid_index_coords = grid_index_coords + 1  # fix locs considering we add padding
     orig_query_shape = tf.shape(grid_index_coords)
     query_points = tf.reshape(grid_index_coords, [orig_query_shape[0], -1, 2])
     padded_img = tf.keras.layers.ZeroPadding2D(padding=(1, 1), data_format="channels_first")(torch_img)
     grid = tf.keras.layers.Permute((2, 3, 1))(padded_img)
     indexing = 'ji'
     grid_shape = tf.shape(grid)
@@ -120,8 +116,8 @@
     bottom_left = gather(ceils[0], floors[1], "bottom_left")
     bottom_right = gather(ceils[0], ceils[1], "bottom_right")
 
     interp_top = alphas[1] * (top_right - top_left) + top_left
     interp_bottom = alphas[1] * (bottom_right - bottom_left) + bottom_left
     interp = alphas[0] * (interp_bottom - interp_top) + interp_top
     tf_reshaped_results = tf.reshape(interp, tf.concat([orig_query_shape[:-1], torch_shape[1:2]], axis=0))
-    return tf.keras.layers.Permute((3,1,2))(tf_reshaped_results)
+    return tf.keras.layers.Permute((3, 1, 2))(tf_reshaped_results)
```

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.87/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.87/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.86/pyproject.toml` & `onnx2kerastl-0.0.87/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.86"
+version = "0.0.87"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.86/PKG-INFO` & `onnx2kerastl-0.0.87/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.86
+Version: 0.0.87
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

