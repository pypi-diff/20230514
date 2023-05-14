# Comparing `tmp/tensor_parallel-1.2.2.tar.gz` & `tmp/tensor_parallel-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_parallel-1.2.2.tar", last modified: Mon Apr 17 07:49:25 2023, max compression
+gzip compressed data, was "tensor_parallel-1.2.3.tar", last modified: Sun May 14 16:53:58 2023, max compression
```

## Comparing `tensor_parallel-1.2.2.tar` & `tensor_parallel-1.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:49:25.490471 tensor_parallel-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-17 07:49:25.490471 tensor_parallel-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-17 07:49:25.490471 tensor_parallel-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:49:25.474471 tensor_parallel-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:49:25.486471 tensor_parallel-1.2.2/src/tensor_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/aux_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/communications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/cross_device_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/per_device_tensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/shard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/sharding.py
--rw-r--r--   0 runner    (1001) docker     (123)    19224 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/slicing_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/state_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/tensor_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:49:25.486471 tensor_parallel-1.2.2/src/tensor_parallel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-17 07:49:25.000000 tensor_parallel-1.2.2/src/tensor_parallel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-17 07:49:25.000000 tensor_parallel-1.2.2/src/tensor_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 07:49:25.000000 tensor_parallel-1.2.2/src/tensor_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-17 07:49:25.000000 tensor_parallel-1.2.2/src/tensor_parallel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 07:49:25.000000 tensor_parallel-1.2.2/src/tensor_parallel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:49:25.490471 tensor_parallel-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:53:58.024569 tensor_parallel-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-05-14 16:53:58.028569 tensor_parallel-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-14 16:53:58.028569 tensor_parallel-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:53:58.020569 tensor_parallel-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:53:58.024569 tensor_parallel-1.2.3/src/tensor_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/aux_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/communications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/cross_device_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/per_device_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/sharding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19224 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/slicing_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/state_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/tensor_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:53:58.024569 tensor_parallel-1.2.3/src/tensor_parallel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-05-14 16:53:58.000000 tensor_parallel-1.2.3/src/tensor_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-14 16:53:58.000000 tensor_parallel-1.2.3/src/tensor_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:53:58.000000 tensor_parallel-1.2.3/src/tensor_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-14 16:53:58.000000 tensor_parallel-1.2.3/src/tensor_parallel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 16:53:58.000000 tensor_parallel-1.2.3/src/tensor_parallel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:53:58.024569 tensor_parallel-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/tests/test_transformers.py
```

### Comparing `tensor_parallel-1.2.2/LICENCE` & `tensor_parallel-1.2.3/LICENCE`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/PKG-INFO` & `tensor_parallel-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor_parallel
-Version: 1.2.2
+Version: 1.2.3
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.2 Summary:
+Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.3 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.2.2/README.md` & `tensor_parallel-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/setup.cfg` & `tensor_parallel-1.2.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tensor_parallel
-version = 1.2.2
+version = 1.2.3
 author = Andrei Panferov and Yaroslav Lisnyak
 author_email = yalisnyak@nes.com
 description = Automatically shard your large model between multiple GPUs, works without torch.distributed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackSamorez/tensor_parallel
 project_urls = 
@@ -30,14 +30,15 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	torch>=1.11
 	transformers>=4.20.1
+	peft>=0.3.0
 
 [options.extras_require]
 dev = 
 	pytest==6.2.5
 	pytest-forked
 	pytest-asyncio==0.16.0
 	accelerate==0.15.0
```

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/__init__.py` & `tensor_parallel-1.2.3/src/tensor_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/autoconfig.py` & `tensor_parallel-1.2.3/src/tensor_parallel/autoconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         if isinstance(module, (nn.Embedding, nn.EmbeddingBag)):
             assert module.max_norm is None or module.norm_type < 2
             assert getattr(module, "bias", None) is None or module.bias.shape == module.embedding_dim
             state_rules[f"^{name}.weight$"] = Split(world_size=len(device_ids), dim=1)
             if hasattr(module, "bias"):
                 state_rules[f"^{name}.bias$"] = Split(world_size=len(device_ids), dim=0)
             output_rules[f"^{name}$"] = {0: "gather -1"}
-        elif isinstance(module, nn.Linear):
+        elif isinstance(module, nn.Linear) and "lora_A" not in name and "lora_B" not in name:
             assert module.weight.shape == (module.out_features, module.in_features)
             assert module.bias is None or module.bias.shape == (module.out_features,)
             if module.weight not in emb_weights:  # regular linear layer
                 state_rules[f"^{name}.(weight|bias)$"] = Split(world_size=len(device_ids), dim=0)
                 output_rules[f"^{name}$"] = {0: "gather -1"}
             else:
                 # linear weight tied with embeddings; this is a popular special case for language models;
```

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/aux_actions.py` & `tensor_parallel-1.2.3/src/tensor_parallel/aux_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/communications.py` & `tensor_parallel-1.2.3/src/tensor_parallel/communications.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/config.py` & `tensor_parallel-1.2.3/src/tensor_parallel/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 import logging
 import os
 import re
 from functools import partial
 from typing import Any, Callable, Dict, Sequence, Union
 
 import torch
+from peft.tuners.lora import LoraLayer
+from torch import nn
 
 import tensor_parallel.cross_device_ops as cross_device_ops
 from tensor_parallel.communications import (
     AllGather,
     AllReduce,
     DistributedAllGather,
     DistributedAllReduce,
     NCCLAllGather,
     NCCLAllReduce,
 )
-from tensor_parallel.state_actions import LegacyStateAction, StateAction
+from tensor_parallel.state_actions import LegacyStateAction, Split, StateAction
 
 logger = logging.getLogger(__file__)
 
 Arg = Union[int, str]
 Action = Callable[[Any, int], Any]  # actions describe what to do with tensors
 MappedActions = Dict[Arg, Action]
 
@@ -116,7 +118,36 @@
             transform_map[transform] = make_allgather(world_size, dim)
 
     initialized_output_rules = {}
     for pattern, output_actions in rules.items():
         output_actions = {key: transform_map.get(rule, rule) for key, rule in output_actions.items()}
         initialized_output_rules[pattern] = output_actions
     return initialized_output_rules
+
+
+def add_lora_rules(model: nn.Module, config: Config) -> Config:
+    lora_state_rules = {}
+    lora_input_rules = {}
+    lora_output_rules = {}
+    for name, module in model.named_modules():
+        if isinstance(module, LoraLayer):
+            for pattern, action in config.state_rules.items():
+                if pattern.search(name + ".weight") is not None:
+                    if isinstance(action, Split):
+                        if action.dim == 0:
+                            lora_state_rules[re.compile(rf"^{name}.lora_B")] = action
+                        elif action.dim == 1:
+                            lora_input_rules[re.compile(rf"^{name}.lora_A.*.")] = {0: "gather -1"}
+                            lora_output_rules[re.compile(rf"^{name}.lora_A.*.")] = {0: "scale"}
+                        else:
+                            raise Exception(
+                                "Expected dim in [0, 1]. Don't know what to do with LoRA linear split along dim {i}"
+                            )
+                    else:
+                        raise Exception(
+                            f"Can't apply action {action} since it uses LoRA. The only actions with LoRA support are Split and it's variations."
+                        )
+
+    config.state_rules.update(lora_state_rules)
+    config.input_rules.update(lora_input_rules)
+    config.output_rules.update(lora_output_rules)
+    return config
```

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/cross_device_ops.py` & `tensor_parallel-1.2.3/src/tensor_parallel/cross_device_ops.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/dispatch.py` & `tensor_parallel-1.2.3/src/tensor_parallel/dispatch.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/factory.py` & `tensor_parallel-1.2.3/src/tensor_parallel/factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/per_device_tensors.py` & `tensor_parallel-1.2.3/src/tensor_parallel/per_device_tensors.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/pretrained_model.py` & `tensor_parallel-1.2.3/src/tensor_parallel/pretrained_model.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/shard.py` & `tensor_parallel-1.2.3/src/tensor_parallel/shard.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/sharding.py` & `tensor_parallel-1.2.3/src/tensor_parallel/sharding.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/slicing_configs.py` & `tensor_parallel-1.2.3/src/tensor_parallel/slicing_configs.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/state_actions.py` & `tensor_parallel-1.2.3/src/tensor_parallel/state_actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,23 +59,21 @@
     def __call__(self, tensor: Tensor, rank: int) -> Tensor:
         return tensor / self.world_size
 
     def undo(self, tensors: Sequence[Tensor]) -> Tensor:
         return tensors[0] * self.world_size
 
 
-class SplitInChunks(StateAction):
+class SplitInChunks(Split):
     """AAABBBCCCDDDEEE -> (world_size = 3, chunk_size = 3) -> [AAABBB, CCCDDD, EEE]
     Split retaining whole chunks
     """
 
     def __init__(self, world_size: int, dim: int, chunk_size: int, optional: bool = False):
-        super().__init__()
-        self.world_size = world_size
-        self.dim = dim
+        super().__init__(world_size, dim)
         self.chunk_size = chunk_size
         self.optional = optional
 
     def __call__(self, tensor: Tensor, rank: int) -> Tensor:
         if tensor is None and self.optional:
             return None
         dim = self.dim
@@ -88,21 +86,19 @@
         tensor_part = tensor.reshape(shape).tensor_split(self.world_size, dim=dim)[rank].flatten(dim, dim + 1)
         return tensor_part
 
     def undo(self, tensors: Sequence[Tensor]) -> Tensor:
         return torch.cat([tensor.cpu() for tensor in tensors], dim=self.dim)
 
 
-class SplitInsideChunks(StateAction):
+class SplitInsideChunks(Split):
     """AAABBBCCCDDDEEE -> (world_size = 3, num_chunks = 5) -> [ABCDE, ABCDE, ABCDE]"""
 
     def __init__(self, world_size: int, dim: int, num_chunks: int) -> None:
-        super().__init__()
-        self.world_size = world_size
-        self.dim = dim
+        super().__init__(world_size, dim)
         self.num_chunks = num_chunks
 
     def __call__(self, tensor: Tensor, rank: int) -> Tensor:
         shape = list(tensor.shape)
         shape[self.dim] = shape[self.dim] // self.num_chunks
         shape.insert(self.dim, self.num_chunks)
         grouped_tensor = tensor.reshape(*shape)
```

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/tensor_parallel.py` & `tensor_parallel-1.2.3/src/tensor_parallel/tensor_parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import torch
 from torch import nn
 from torch._utils import ExceptionWrapper, _get_all_device_indices, _get_device_index
 from torch.cuda.amp import autocast
 from torch.nn.parallel import parallel_apply
 
 from tensor_parallel.autoconfig import get_default_config
-from tensor_parallel.config import TENSOR_PARALLEL_USE_NATIVE, Config
+from tensor_parallel.config import TENSOR_PARALLEL_USE_NATIVE, Config, add_lora_rules
 from tensor_parallel.cross_device_ops import broadcast_coalesced
 from tensor_parallel.shard import make_shard
 from tensor_parallel.utils import nested_flatten, nested_pack
 
 logger = logging.getLogger(__file__)
 
 
@@ -59,14 +59,15 @@
                 self.module_shards[0].to(device_ids[0])
             return
 
         if tensor_parallel_config is None:
             tensor_parallel_config = get_default_config(module, self.devices)
             logger.info("Using automatic config: sharding individual linear/conv/emb layers")
 
+        tensor_parallel_config = add_lora_rules(module, tensor_parallel_config)
         self.tensor_parallel_config = tensor_parallel_config
 
         config_with_ops = tensor_parallel_config.create_collective_ops(self.devices)
         # ^-- creates a copy of comfig with collective op instances, such as AllReduce and AllGather
 
         for rank, device in enumerate(self.devices):
             if delay_init:
```

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/utils.py` & `tensor_parallel-1.2.3/src/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel/wrapper.py` & `tensor_parallel-1.2.3/src/tensor_parallel/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 def process_output(output, output_actions: MappedActions, *, rank: int, world_size: int):
     if isinstance(output, torch.Tensor):
         return process_output({0: output}, output_actions, rank=rank, world_size=world_size)[0]
     if isinstance(output, Sequence):
         output_dict = process_output(dict(enumerate(output)), output_actions, rank=rank, world_size=world_size)
         return type(output)((output_dict[i] for i in range(len(output))))
     for target, action in output_actions.items():
-        output[target] = action(output.get(target), rank=rank)
+        output[target] = apply_action(output.get(target), action, rank=rank, world_size=world_size)
     return output
 
 
 class TensorParallelWrapper(nn.Module):
     """Wraps a single module, applies tensor parallelism actions to module inputs and outputs"""
 
     def __init__(
```

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel.egg-info/PKG-INFO` & `tensor_parallel-1.2.3/src/tensor_parallel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor-parallel
-Version: 1.2.2
+Version: 1.2.3
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.2 Summary:
+Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.3 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.2.2/src/tensor_parallel.egg-info/SOURCES.txt` & `tensor_parallel-1.2.3/src/tensor_parallel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/tests/test_basic.py` & `tensor_parallel-1.2.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/tests/test_factory.py` & `tensor_parallel-1.2.3/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/tests/test_integration.py` & `tensor_parallel-1.2.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/tests/test_saving.py` & `tensor_parallel-1.2.3/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.2/tests/test_transformers.py` & `tensor_parallel-1.2.3/tests/test_transformers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,49 @@
+import re
 from typing import Sequence
 
 import pytest
 import torch
 import transformers
+from peft import LoraConfig, get_peft_model
 from transformers import AutoModelForCausalLM, AutoTokenizer, BertModel, T5ForConditionalGeneration
 
 from tensor_parallel import TensorParallel, TensorParallelPreTrainedModel, tensor_parallel
 from tensor_parallel.pretrained_model import find_predefined_tensor_parallel_config
 
 
+def add_lora(model: torch.nn.Module, model_name: str) -> torch.nn.Module:
+    try:
+        lora_config = LoraConfig(base_model_name_or_path=model_name, lora_alpha=32, lora_dropout=0.05)
+        model = get_peft_model(model, lora_config)
+    except ValueError:
+
+        def get_num_layers(model):
+            numbers = set()
+            for name, _ in model.named_parameters():
+                for number in re.findall(r"\d+", name):
+                    numbers.add(int(number))
+            return max(numbers)
+
+        def get_last_layer_linears(model):
+            names = []
+
+            num_layers = get_num_layers(model)
+            for name, module in model.named_modules():
+                if str(num_layers) in name and not "encoder" in name:
+                    if isinstance(module, torch.nn.Linear):
+                        names.append(name)
+            return names
+
+        lora_config = LoraConfig(target_modules=get_last_layer_linears(model), lora_alpha=32, lora_dropout=0.05)
+        model = get_peft_model(model, lora_config)
+
+    return model
+
+
 @pytest.mark.parametrize(
     "model_classes",
     [
         [
             transformers.AutoModel,
             transformers.AutoModelForCausalLM,
             transformers.AutoModelForSequenceClassification,
@@ -37,33 +68,38 @@
         tensor_parallel_configs.append(find_predefined_tensor_parallel_config(model.config, devices))
 
     assert all_equal(
         map(lambda x: x.attr_rules.keys(), tensor_parallel_configs)
     )  # basically asserting that all of those have the same config
 
 
+@pytest.mark.parametrize("use_lora", [False, True])
 @pytest.mark.parametrize("use_config", [False, True])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize(
     "model_name",
     [
         "bigscience/bloom-560m",
         "gpt2",
         "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
         "Salesforce/codegen-350M-mono",
         "Bingsu/llama-190m-arch",
     ],
 )
-def test_forward_gpt2_like(use_config, devices, model_name):
+def test_forward_gpt2_like(use_lora, use_config, devices, model_name):
     torch.manual_seed(0)
 
     try:
         model = AutoModelForCausalLM.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
     except KeyError as err:
         pytest.skip(f"Could not create model {model_name} with error {err}")
+    if use_lora:
+        if model_name == "gpt2":
+            pytest.skip("Not testing LoRA for gpt2")
+        model = add_lora(model, model_name)
 
     inp1 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     inp2 = torch.randint(1, 1000, size=(2, 1), device=devices[0])
     inp3 = torch.randint(1, 1000, size=(2, 2), device=devices[0])
 
     out1_ref = model(inp1, use_cache=True, output_hidden_states=True)
     out2_ref = model(inp2, use_cache=True, past_key_values=out1_ref.past_key_values)
@@ -81,21 +117,24 @@
 
     torch.testing.assert_close(out1_ref.hidden_states[-1], out1.hidden_states[-1], atol=3e-3, rtol=1e-05)
     torch.testing.assert_close(out1_ref.logits, out1.logits, atol=3e-3, rtol=1e-05)
     torch.testing.assert_close(out2_ref.logits, out2.logits, atol=3e-3, rtol=1e-05)
     torch.testing.assert_close(out3_ref.logits, out3.logits, atol=3e-3, rtol=1e-05)
 
 
+@pytest.mark.parametrize("use_lora", [False, True])
 @pytest.mark.parametrize("use_config", [False, True])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["t5-small"])
-def test_forward_t5_like(use_config, devices, model_name):
+def test_forward_t5_like(use_lora, use_config, devices, model_name):
     torch.manual_seed(0)
 
     model = T5ForConditionalGeneration.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
+    if use_lora:
+        model = add_lora(model, model_name)
 
     enc = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     dec1 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     dec2 = torch.randint(1, 1000, size=(2, 1), device=devices[0])
     dec3 = torch.randint(1, 1000, size=(2, 2), device=devices[0])
 
     out1_ref = model(enc, decoder_input_ids=dec1, use_cache=True, output_hidden_states=True)
@@ -116,21 +155,24 @@
         out1_ref.decoder_hidden_states[-1], out1.decoder_hidden_states[-1], atol=3e-3, rtol=1e-05
     )
     torch.testing.assert_close(out1_ref.logits, out1.logits, atol=3e-3, rtol=1e-05)
     torch.testing.assert_close(out2_ref.logits, out2.logits, atol=3e-3, rtol=1e-05)
     torch.testing.assert_close(out3_ref.logits, out3.logits, atol=3e-3, rtol=1e-05)
 
 
+@pytest.mark.parametrize("use_lora", [False, True])
 @pytest.mark.parametrize("use_config", [False, True])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["bert-base-uncased"])
-def test_forward_bert_like(use_config, devices, model_name):
+def test_forward_bert_like(use_lora, use_config, devices, model_name):
     torch.manual_seed(0)
 
     model = BertModel.from_pretrained(model_name).to(devices[0])
+    if use_lora:
+        model = add_lora(model, model_name)
 
     inp1 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     inp2 = torch.randint(1, 1000, size=(2, 1), device=devices[0])
     inp3 = torch.randint(1, 1000, size=(2, 2), device=devices[0])
 
     out1_ref = model(inp1, output_hidden_states=True)
     out2_ref = model(inp2, output_hidden_states=True)
```

