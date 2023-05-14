# Comparing `tmp/torchinfo-1.7.2.tar.gz` & `tmp/torchinfo-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchinfo-1.7.2.tar", last modified: Sun Feb  5 20:47:30 2023, max compression
+gzip compressed data, was "torchinfo-1.8.0.tar", last modified: Sun May 14 19:23:18 2023, max compression
```

## Comparing `torchinfo-1.7.2.tar` & `torchinfo-1.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tyler.yep   (501) staff       (20)        0 2023-02-05 20:47:30.689785 torchinfo-1.7.2/
--rw-r--r--   0 tyler.yep   (501) staff       (20)     1065 2022-09-18 21:00:17.000000 torchinfo-1.7.2/LICENSE
--rw-r--r--   0 tyler.yep   (501) staff       (20)    21777 2023-02-05 20:47:30.689890 torchinfo-1.7.2/PKG-INFO
--rw-r--r--   0 tyler.yep   (501) staff       (20)    20792 2022-11-28 05:07:46.000000 torchinfo-1.7.2/README.md
--rw-r--r--   0 tyler.yep   (501) staff       (20)     1764 2023-02-05 20:47:30.690493 torchinfo-1.7.2/setup.cfg
--rw-r--r--   0 tyler.yep   (501) staff       (20)       38 2023-02-05 20:07:54.000000 torchinfo-1.7.2/setup.py
-drwxr-xr-x   0 tyler.yep   (501) staff       (20)        0 2023-02-05 20:47:30.688628 torchinfo-1.7.2/torchinfo/
--rw-r--r--   0 tyler.yep   (501) staff       (20)      306 2023-02-05 20:25:23.000000 torchinfo-1.7.2/torchinfo/__init__.py
--rw-r--r--   0 tyler.yep   (501) staff       (20)     1026 2022-11-28 05:07:46.000000 torchinfo-1.7.2/torchinfo/enums.py
--rw-r--r--   0 tyler.yep   (501) staff       (20)     5675 2022-11-28 05:07:46.000000 torchinfo-1.7.2/torchinfo/formatting.py
--rw-r--r--   0 tyler.yep   (501) staff       (20)    13172 2023-02-05 20:07:54.000000 torchinfo-1.7.2/torchinfo/layer_info.py
--rw-r--r--   0 tyler.yep   (501) staff       (20)     5055 2023-02-05 20:16:43.000000 torchinfo-1.7.2/torchinfo/model_statistics.py
--rw-r--r--   0 tyler.yep   (501) staff       (20)        0 2022-09-18 21:00:17.000000 torchinfo-1.7.2/torchinfo/py.typed
--rw-r--r--   0 tyler.yep   (501) staff       (20)    23416 2023-02-05 20:42:50.000000 torchinfo-1.7.2/torchinfo/torchinfo.py
-drwxr-xr-x   0 tyler.yep   (501) staff       (20)        0 2023-02-05 20:47:30.689623 torchinfo-1.7.2/torchinfo.egg-info/
--rw-r--r--   0 tyler.yep   (501) staff       (20)    21777 2023-02-05 20:47:30.000000 torchinfo-1.7.2/torchinfo.egg-info/PKG-INFO
--rw-r--r--   0 tyler.yep   (501) staff       (20)      329 2023-02-05 20:47:30.000000 torchinfo-1.7.2/torchinfo.egg-info/SOURCES.txt
--rw-r--r--   0 tyler.yep   (501) staff       (20)        1 2023-02-05 20:47:30.000000 torchinfo-1.7.2/torchinfo.egg-info/dependency_links.txt
--rw-r--r--   0 tyler.yep   (501) staff       (20)       10 2023-02-05 20:47:30.000000 torchinfo-1.7.2/torchinfo.egg-info/top_level.txt
+drwxr-xr-x   0 tyler.yep   (501) staff       (20)        0 2023-05-14 19:23:18.985066 torchinfo-1.8.0/
+-rw-r--r--   0 tyler.yep   (501) staff       (20)     1065 2022-09-18 21:00:17.000000 torchinfo-1.8.0/LICENSE
+-rw-r--r--   0 tyler.yep   (501) staff       (20)    21887 2023-05-14 19:23:18.985224 torchinfo-1.8.0/PKG-INFO
+-rw-r--r--   0 tyler.yep   (501) staff       (20)    20902 2023-05-14 19:07:57.000000 torchinfo-1.8.0/README.md
+-rw-r--r--   0 tyler.yep   (501) staff       (20)     1764 2023-05-14 19:23:18.985821 torchinfo-1.8.0/setup.cfg
+-rw-r--r--   0 tyler.yep   (501) staff       (20)       38 2023-02-05 20:07:54.000000 torchinfo-1.8.0/setup.py
+drwxr-xr-x   0 tyler.yep   (501) staff       (20)        0 2023-05-14 19:23:18.983278 torchinfo-1.8.0/torchinfo/
+-rw-r--r--   0 tyler.yep   (501) staff       (20)      306 2023-05-14 19:07:57.000000 torchinfo-1.8.0/torchinfo/__init__.py
+-rw-r--r--   0 tyler.yep   (501) staff       (20)     1026 2022-11-28 05:07:46.000000 torchinfo-1.8.0/torchinfo/enums.py
+-rw-r--r--   0 tyler.yep   (501) staff       (20)     5675 2022-11-28 05:07:46.000000 torchinfo-1.8.0/torchinfo/formatting.py
+-rw-r--r--   0 tyler.yep   (501) staff       (20)    13622 2023-03-10 19:14:56.000000 torchinfo-1.8.0/torchinfo/layer_info.py
+-rw-r--r--   0 tyler.yep   (501) staff       (20)     5055 2023-02-05 20:16:43.000000 torchinfo-1.8.0/torchinfo/model_statistics.py
+-rw-r--r--   0 tyler.yep   (501) staff       (20)        0 2022-09-18 21:00:17.000000 torchinfo-1.8.0/torchinfo/py.typed
+-rw-r--r--   0 tyler.yep   (501) staff       (20)    24599 2023-05-14 19:07:57.000000 torchinfo-1.8.0/torchinfo/torchinfo.py
+drwxr-xr-x   0 tyler.yep   (501) staff       (20)        0 2023-05-14 19:23:18.984830 torchinfo-1.8.0/torchinfo.egg-info/
+-rw-r--r--   0 tyler.yep   (501) staff       (20)    21887 2023-05-14 19:23:18.000000 torchinfo-1.8.0/torchinfo.egg-info/PKG-INFO
+-rw-r--r--   0 tyler.yep   (501) staff       (20)      329 2023-05-14 19:23:18.000000 torchinfo-1.8.0/torchinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler.yep   (501) staff       (20)        1 2023-05-14 19:23:18.000000 torchinfo-1.8.0/torchinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler.yep   (501) staff       (20)       10 2023-05-14 19:23:18.000000 torchinfo-1.8.0/torchinfo.egg-info/top_level.txt
```

### Comparing `torchinfo-1.7.2/LICENSE` & `torchinfo-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchinfo-1.7.2/PKG-INFO` & `torchinfo-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchinfo
-Version: 1.7.2
+Version: 1.8.0
 Summary: Model summary in PyTorch, based off of the original torchsummary.
 Home-page: https://github.com/tyleryep/torchinfo
 Author: Tyler Yep @tyleryep
 Author-email: tyep@cs.stanford.edu
 License: MIT
 Keywords: torch pytorch torchsummary torch-summary summary keras deep-learning ml torchinfo torch-info visualize model statistics layer stats
 Classifier: License :: OSI Approved :: MIT License
@@ -203,15 +203,17 @@
     depth (int):
             Depth of nested layers to display (e.g. Sequentials).
             Nested layers below this depth will not be displayed in the summary.
             Default: 3
 
     device (torch.Device):
             Uses this torch device for model and input_data.
-            If not specified, uses result of torch.cuda.is_available().
+            If not specified, uses the dtype of input_data if given, or the
+            parameters of the model. Otherwise, uses the result of
+            torch.cuda.is_available().
             Default: None
 
     dtypes (List[torch.dtype]):
             If you use input_size, torchinfo assumes your input uses FloatTensors.
             If your model use a different data type, specify that dtype.
             For multiple inputs, specify the size of both inputs, and
             also specify the types of each parameter here.
```

### Comparing `torchinfo-1.7.2/README.md` & `torchinfo-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,17 @@
     depth (int):
             Depth of nested layers to display (e.g. Sequentials).
             Nested layers below this depth will not be displayed in the summary.
             Default: 3
 
     device (torch.Device):
             Uses this torch device for model and input_data.
-            If not specified, uses result of torch.cuda.is_available().
+            If not specified, uses the dtype of input_data if given, or the
+            parameters of the model. Otherwise, uses the result of
+            torch.cuda.is_available().
             Default: None
 
     dtypes (List[torch.dtype]):
             If you use input_size, torchinfo assumes your input uses FloatTensors.
             If your model use a different data type, specify that dtype.
             For multiple inputs, specify the size of both inputs, and
             also specify the types of each parameter here.
```

### Comparing `torchinfo-1.7.2/setup.cfg` & `torchinfo-1.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `torchinfo-1.7.2/torchinfo/enums.py` & `torchinfo-1.8.0/torchinfo/enums.py`

 * *Files identical despite different names*

### Comparing `torchinfo-1.7.2/torchinfo/formatting.py` & `torchinfo-1.8.0/torchinfo/formatting.py`

 * *Files identical despite different names*

### Comparing `torchinfo-1.7.2/torchinfo/layer_info.py` & `torchinfo-1.8.0/torchinfo/layer_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import Any, Dict, Iterable, Sequence, Union
 
+import numpy as np
 import torch
 from torch import nn
 from torch.jit import ScriptModule
 
 from .enums import ColumnSettings
 
 try:
@@ -94,15 +95,18 @@
         a single element in bytes.
         """
         if inputs is None:
             size, elem_bytes = [], 0
 
         # pack_padded_seq and pad_packed_seq store feature into data attribute
         elif (
-            isinstance(inputs, (list, tuple)) and inputs and hasattr(inputs[0], "data")
+            isinstance(inputs, (list, tuple))
+            and inputs
+            and hasattr(inputs[0], "data")
+            and hasattr(inputs[0].data, "size")
         ):
             size = list(inputs[0].data.size())
             elem_bytes = inputs[0].data.element_size()
             if batch_dim is not None:
                 size = size[:batch_dim] + [1] + size[batch_dim + 1 :]
 
         elif isinstance(inputs, dict):
@@ -111,14 +115,18 @@
             if batch_dim is not None:
                 size = [size[:batch_dim] + [1] + size[batch_dim + 1 :]]
 
         elif isinstance(inputs, torch.Tensor):
             size = list(inputs.size())
             elem_bytes = inputs.element_size()
 
+        elif isinstance(inputs, np.ndarray):
+            inputs_ = torch.from_numpy(inputs)
+            size, elem_bytes = list(inputs_.size()), inputs_.element_size()
+
         elif isinstance(inputs, (list, tuple)):
             size, elem_bytes = nested_list_size(inputs)
             if batch_dim is not None and batch_dim < len(size):
                 size[batch_dim] = 1
 
         else:
             raise TypeError(
@@ -311,14 +319,17 @@
 
 def nested_list_size(inputs: Sequence[Any] | torch.Tensor) -> tuple[list[int], int]:
     """Flattens nested list size."""
     if hasattr(inputs, "tensors"):
         size, elem_bytes = nested_list_size(inputs.tensors)
     elif isinstance(inputs, torch.Tensor):
         size, elem_bytes = list(inputs.size()), inputs.element_size()
+    elif isinstance(inputs, np.ndarray):
+        inputs_torch = torch.from_numpy(inputs)  # preserves dtype
+        size, elem_bytes = list(inputs_torch.size()), inputs_torch.element_size()
     elif not hasattr(inputs, "__getitem__") or not inputs:
         size, elem_bytes = [], 0
     elif isinstance(inputs, dict):
         size, elem_bytes = nested_list_size(list(inputs.values()))
     elif (
         hasattr(inputs, "size")
         and callable(inputs.size)
```

### Comparing `torchinfo-1.7.2/torchinfo/model_statistics.py` & `torchinfo-1.8.0/torchinfo/model_statistics.py`

 * *Files identical despite different names*

### Comparing `torchinfo-1.7.2/torchinfo/torchinfo.py` & `torchinfo-1.8.0/torchinfo/torchinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Mapping,
     Optional,
     Sequence,
     Union,
     cast,
 )
 
+import numpy as np
 import torch
 from torch import nn
 from torch.jit import ScriptModule
 from torch.utils.hooks import RemovableHandle
 
 from .enums import ColumnSettings, Mode, RowSettings, Verbosity
 from .formatting import FormattingOptions
@@ -28,15 +29,15 @@
 # Some modules do the computation themselves using parameters
 # or the parameters of children. Treat these as layers.
 # TODO: figure out a test case for this
 LAYER_MODULES = (torch.nn.MultiheadAttention,)
 # These modules are not recorded during a forward pass. Handle them separately.
 WRAPPER_MODULES = (ScriptModule,)
 
-INPUT_DATA_TYPE = Union[torch.Tensor, Sequence[Any], Mapping[str, Any]]
+INPUT_DATA_TYPE = Union[torch.Tensor, np.ndarray, Sequence[Any], Mapping[str, Any]]
 CORRECTED_INPUT_DATA_TYPE = Optional[Union[Iterable[Any], Mapping[Any, Any]]]
 INPUT_SIZE_TYPE = Sequence[Union[int, Sequence[Any], torch.Size]]
 CORRECTED_INPUT_SIZE_TYPE = List[Union[Sequence[Any], torch.Size]]
 
 DEFAULT_COLUMN_NAMES = (ColumnSettings.OUTPUT_SIZE, ColumnSettings.NUM_PARAMS)
 DEFAULT_ROW_SETTINGS = {RowSettings.DEPTH}
 REQUIRES_INPUT = {
@@ -135,15 +136,17 @@
         depth (int):
                 Depth of nested layers to display (e.g. Sequentials).
                 Nested layers below this depth will not be displayed in the summary.
                 Default: 3
 
         device (torch.Device):
                 Uses this torch device for model and input_data.
-                If not specified, uses result of torch.cuda.is_available().
+                If not specified, uses the dtype of input_data if given, or the
+                parameters of the model. Otherwise, uses the result of
+                torch.cuda.is_available().
                 Default: None
 
         dtypes (List[torch.dtype]):
                 If you use input_size, torchinfo assumes your input uses FloatTensors.
                 If your model use a different data type, specify that dtype.
                 For multiple inputs, specify the size of both inputs, and
                 also specify the types of each parameter here.
@@ -202,15 +205,17 @@
         verbose = 0 if hasattr(sys, "ps1") and sys.ps1 else 1
 
     if cache_forward_pass is None:
         # In the future, this may be enabled by default in Jupyter Notebooks
         cache_forward_pass = False
 
     if device is None:
-        device = get_device(model)
+        device = get_device(model, input_data)
+    elif isinstance(device, str):
+        device = torch.device(device)
 
     validate_user_params(
         input_data, input_size, columns, col_width, device, dtypes, verbose
     )
 
     x, correct_input_size = process_input(
         input_data, input_size, batch_dim, device, dtypes
@@ -227,40 +232,41 @@
     return results
 
 
 def process_input(
     input_data: INPUT_DATA_TYPE | None,
     input_size: INPUT_SIZE_TYPE | None,
     batch_dim: int | None,
-    device: torch.device | str,
+    device: torch.device | None,
     dtypes: list[torch.dtype] | None = None,
 ) -> tuple[CORRECTED_INPUT_DATA_TYPE, Any]:
     """Reads sample input data to get the input size."""
     x = None
     correct_input_size = []
     if input_data is not None:
         correct_input_size = get_input_data_sizes(input_data)
         x = set_device(input_data, device)
-        if isinstance(x, torch.Tensor):
+        if isinstance(x, (torch.Tensor, np.ndarray)):
             x = [x]
 
     if input_size is not None:
+        assert device is not None
         if dtypes is None:
             dtypes = [torch.float] * len(input_size)
         correct_input_size = get_correct_input_sizes(input_size)
         x = get_input_tensor(correct_input_size, batch_dim, dtypes, device)
     return x, correct_input_size
 
 
 def forward_pass(
     model: nn.Module,
     x: CORRECTED_INPUT_DATA_TYPE,
     batch_dim: int | None,
     cache_forward_pass: bool,
-    device: torch.device | str,
+    device: torch.device | None,
     mode: Mode,
     **kwargs: Any,
 ) -> list[LayerInfo]:
     """Perform a forward pass on the model using forward hooks."""
     global _cached_forward_pass  # pylint: disable=global-variable-not-assigned
     model_name = model.__class__.__name__
     if cache_forward_pass and model_name in _cached_forward_pass:
@@ -280,18 +286,19 @@
             model.eval()
         else:
             raise RuntimeError(
                 f"Specified model mode ({list(Mode)}) not recognized: {mode}"
             )
 
         with torch.no_grad():
+            model = model if device is None else model.to(device)
             if isinstance(x, (list, tuple)):
-                _ = model.to(device)(*x, **kwargs)
+                _ = model(*x, **kwargs)
             elif isinstance(x, dict):
-                _ = model.to(device)(**x, **kwargs)
+                _ = model(**x, **kwargs)
             else:
                 # Should not reach this point, since process_input_data ensures
                 # x is either a list, tuple, or dict
                 raise ValueError("Unknown input type")
     except Exception as e:
         executed_layers = [layer for layer in summary_list if layer.executed]
         raise RuntimeError(
@@ -361,15 +368,15 @@
 
 
 def validate_user_params(
     input_data: INPUT_DATA_TYPE | None,
     input_size: INPUT_SIZE_TYPE | None,
     col_names: tuple[ColumnSettings, ...],
     col_width: int,
-    device: torch.device | str | None,
+    device: torch.device | None,
     dtypes: list[torch.dtype] | None,
     verbose: int,
 ) -> None:
     """Raise exceptions if the user's input is invalid."""
     if col_width <= 0:
         raise ValueError(f"Column width must be greater than 0: col_width={col_width}")
     if verbose not in (0, 1, 2):
@@ -390,78 +397,99 @@
 
     if dtypes is not None and any(
         dtype in (torch.float16, torch.bfloat16) for dtype in dtypes
     ):
         if input_size is not None:
             warnings.warn(
                 "Half precision is not supported with input_size parameter, and may "
-                "output incorrect results. Try passing input_data directly."
+                "output incorrect results. Try passing input_data directly.",
+                stacklevel=2,
             )
-
-        device_str = device.type if isinstance(device, torch.device) else device
-        if device_str == "cpu":
+        if device is not None and device.type == "cpu":
             warnings.warn(
                 "Half precision is not supported on cpu. Set the `device` field or "
-                "pass `input_data` using the correct device."
+                "pass `input_data` using the correct device.",
+                stacklevel=2,
             )
 
 
 def traverse_input_data(
     data: Any, action_fn: Callable[..., Any], aggregate_fn: Callable[..., Any]
 ) -> Any:
     """
     Traverses any type of nested input data. On a tensor, returns the action given by
     action_fn, and afterwards aggregates the results using aggregate_fn.
     """
     if isinstance(data, torch.Tensor):
-        return action_fn(data)
+        result = action_fn(data)
+    elif isinstance(data, np.ndarray):
+        result = action_fn(torch.from_numpy(data))
+        # If the result of action_fn is a torch.Tensor, then action_fn was meant for
+        #   torch.Tensors only (like calling .to(...)) -> Ignore.
+        if isinstance(result, torch.Tensor):
+            result = data
 
     # Recursively apply to collection items
-    aggregate = aggregate_fn(data)
-    if isinstance(data, Mapping):
-        return aggregate(
+    elif isinstance(data, Mapping):
+        aggregate = aggregate_fn(data)
+        result = aggregate(
             {
                 k: traverse_input_data(v, action_fn, aggregate_fn)
                 for k, v in data.items()
             }
         )
-    if isinstance(data, tuple) and hasattr(data, "_fields"):  # Named tuple
-        return aggregate(
+    elif isinstance(data, tuple) and hasattr(data, "_fields"):  # Named tuple
+        aggregate = aggregate_fn(data)
+        result = aggregate(
             *(traverse_input_data(d, action_fn, aggregate_fn) for d in data)
         )
-    if isinstance(data, Iterable) and not isinstance(data, str):
-        return aggregate(
+    elif isinstance(data, Iterable) and not isinstance(data, str):
+        aggregate = aggregate_fn(data)
+        result = aggregate(
             [traverse_input_data(d, action_fn, aggregate_fn) for d in data]
         )
-    # Data is neither a tensor nor a collection
-    return data
+    else:
+        # Data is neither a tensor nor a collection
+        result = data
+    return result
 
 
-def set_device(data: Any, device: torch.device | str) -> Any:
+def set_device(data: Any, device: torch.device | None) -> Any:
     """Sets device for all input types and collections of input types."""
-    return traverse_input_data(
-        data,
-        action_fn=lambda data: data.to(device, non_blocking=True),
-        aggregate_fn=type,
+    return (
+        data
+        if device is None
+        else traverse_input_data(
+            data,
+            action_fn=lambda data: data.to(device, non_blocking=True),
+            aggregate_fn=type,
+        )
     )
 
 
-def get_device(model: nn.Module) -> torch.device | str:
+def get_device(
+    model: nn.Module, input_data: INPUT_DATA_TYPE | None
+) -> torch.device | None:
     """
-    Gets device of first parameter of model and returns it if it is on cuda,
+    If input_data is given, the device should not be changed
+    (to allow for multi-device models, etc.)
+
+    Otherwise gets device of first parameter of model and returns it if it is on cuda,
     otherwise returns cuda if available or cpu if not.
     """
-    try:
-        model_parameter = next(model.parameters())
-    except StopIteration:
-        model_parameter = None
-
-    if model_parameter is not None and model_parameter.is_cuda:
-        return model_parameter.device
-    return torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    if input_data is None:
+        try:
+            model_parameter = next(model.parameters())
+        except StopIteration:
+            model_parameter = None
+
+        if model_parameter is not None and model_parameter.is_cuda:
+            return model_parameter.device
+        return torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    return None
 
 
 def get_input_data_sizes(data: Any) -> Any:
     """
     Converts input data to an equivalent data structure of torch.Sizes
     instead of tensors.
     """
@@ -470,30 +498,34 @@
     )
 
 
 def get_total_memory_used(data: CORRECTED_INPUT_DATA_TYPE) -> int:
     """Calculates the total memory of all tensors stored in data."""
     result = traverse_input_data(
         data,
-        action_fn=lambda data: sys.getsizeof(data.storage()),
+        action_fn=lambda data: sys.getsizeof(
+            data.untyped_storage()
+            if hasattr(data, "untyped_storage")
+            else data.storage()
+        ),
         aggregate_fn=(
             # We don't need the dictionary keys in this case
             lambda data: (lambda d: sum(d.values()))
             if isinstance(data, Mapping)
             else sum
         ),
     )
     return cast(int, result)
 
 
 def get_input_tensor(
     input_size: CORRECTED_INPUT_SIZE_TYPE,
     batch_dim: int | None,
     dtypes: list[torch.dtype],
-    device: torch.device | str,
+    device: torch.device,
 ) -> list[torch.Tensor]:
     """Get input_tensor with batch size 1 for use in model.forward()"""
     x = []
     for size, dtype in zip(input_size, dtypes):
         input_tensor = torch.rand(*size)
         if batch_dim is not None:
             input_tensor = input_tensor.unsqueeze(dim=batch_dim)
```

### Comparing `torchinfo-1.7.2/torchinfo.egg-info/PKG-INFO` & `torchinfo-1.8.0/torchinfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchinfo
-Version: 1.7.2
+Version: 1.8.0
 Summary: Model summary in PyTorch, based off of the original torchsummary.
 Home-page: https://github.com/tyleryep/torchinfo
 Author: Tyler Yep @tyleryep
 Author-email: tyep@cs.stanford.edu
 License: MIT
 Keywords: torch pytorch torchsummary torch-summary summary keras deep-learning ml torchinfo torch-info visualize model statistics layer stats
 Classifier: License :: OSI Approved :: MIT License
@@ -203,15 +203,17 @@
     depth (int):
             Depth of nested layers to display (e.g. Sequentials).
             Nested layers below this depth will not be displayed in the summary.
             Default: 3
 
     device (torch.Device):
             Uses this torch device for model and input_data.
-            If not specified, uses result of torch.cuda.is_available().
+            If not specified, uses the dtype of input_data if given, or the
+            parameters of the model. Otherwise, uses the result of
+            torch.cuda.is_available().
             Default: None
 
     dtypes (List[torch.dtype]):
             If you use input_size, torchinfo assumes your input uses FloatTensors.
             If your model use a different data type, specify that dtype.
             For multiple inputs, specify the size of both inputs, and
             also specify the types of each parameter here.
```

