# Comparing `tmp/adamr-0.0.1.tar.gz` & `tmp/adamr-0.0.2.tar.gz`

## Comparing `adamr-0.0.1.tar` & `adamr-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0   318511 2020-02-02 00:00:00.000000 adamr-0.0.1/images/adamwr_algorithm.png
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 adamr-0.0.1/src/adamr/__init__.py
--rw-r--r--   0        0        0    19837 2020-02-02 00:00:00.000000 adamr-0.0.1/src/adamr/adamr.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 adamr-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 adamr-0.0.1/LICENSE
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 adamr-0.0.1/README.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 adamr-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 adamr-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0   318511 2020-02-02 00:00:00.000000 adamr-0.0.2/images/adamwr_algorithm.png
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 adamr-0.0.2/src/adamr/__init__.py
+-rw-r--r--   0        0        0    21217 2020-02-02 00:00:00.000000 adamr-0.0.2/src/adamr/adamr.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 adamr-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 adamr-0.0.2/LICENSE
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 adamr-0.0.2/README.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 adamr-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 adamr-0.0.2/PKG-INFO
```

### Comparing `adamr-0.0.1/images/adamwr_algorithm.png` & `adamr-0.0.2/images/adamwr_algorithm.png`

 * *Files identical despite different names*

### Comparing `adamr-0.0.1/src/adamr/adamr.py` & `adamr-0.0.2/src/adamr/adamr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import math
 import torch
 from torch import Tensor
 from torch.optim.optimizer import Optimizer
 from typing import List, Optional
 
-# TODO: add a method to bind specific recovery parmeters.
-
 class AdamR(Optimizer):
     r"""Implements AdamW algorithm. TODO: Modify the documentation for adamr
 
     .. math::
        \begin{aligned}
             &\rule{110mm}{0.4pt}                                                                 \\
             &\textbf{input}      : \gamma \text{(lr)}, \: \beta_1, \beta_2
@@ -69,16 +67,16 @@
     .. _Decoupled Weight Decay Regularization:
         https://arxiv.org/abs/1711.05101
     .. _On the Convergence of Adam and Beyond:
         https://openreview.net/forum?id=ryQu7f-RZ
     """
 
     def __init__(self, params, lr=1e-3, betas=(0.9, 0.999), eps=1e-8,
-                 weight_recovery=1e-2, amsgrad=False, *, maximize: bool = False,
-                 foreach: Optional[bool] = None,
+                 weight_recovery=1e-2, recov_params=None, amsgrad=False, *, 
+                 maximize: bool = False, foreach: Optional[bool] = None,
                  capturable: bool = False):
         if not 0.0 <= lr:
             raise ValueError("Invalid learning rate: {}".format(lr))
         if not 0.0 <= eps:
             raise ValueError("Invalid epsilon value: {}".format(eps))
         if not 0.0 <= betas[0] < 1.0:
             raise ValueError("Invalid beta parameter at index 0: {}".format(betas[0]))
@@ -86,27 +84,49 @@
             raise ValueError("Invalid beta parameter at index 1: {}".format(betas[1]))
         if not 0.0 <= weight_recovery:
             raise ValueError("Invalid weight_recovery value: {}".format(weight_recovery))
         defaults = dict(lr=lr, betas=betas, eps=eps,
                         weight_recovery=weight_recovery, amsgrad=amsgrad,
                         foreach=foreach, maximize=maximize, capturable=capturable)
         super(AdamR, self).__init__(params, defaults)
+        self.__init_recov_groups(recov_params)
 
     def __setstate__(self, state):
         super().__setstate__(state)
         for group in self.param_groups:
             group.setdefault('amsgrad', False)
             group.setdefault('maximize', False)
             group.setdefault('foreach', None)
             group.setdefault('capturable', False)
         state_values = list(self.state.values())
         step_is_tensor = (len(state_values) != 0) and torch.is_tensor(state_values[0]['step'])
         if not step_is_tensor:
             for s in state_values:
                 s['step'] = torch.tensor(float(s['step']))
+                
+    def __init_recov_groups(self, recov_params):
+        if recov_params is None:
+            self.recov_groups = None
+            return
+        recov_groups = list(recov_params)
+        if len(recov_groups) == 0:
+            raise ValueError("optimizer got an empty parameter list")
+        if not isinstance(recov_groups[0], dict):
+            recov_groups = [{'recov_params': recov_groups}]
+
+        for recov_group in recov_groups:
+            recov_params = recov_group['recov_params']
+            if isinstance(recov_params, torch.Tensor):
+                recov_group['recov_params'] = [recov_params]
+            elif isinstance(recov_params, set):
+                raise TypeError('optimizer parameters need to be organized in ordered collections, but '
+                                'the ordering of tensors in sets will change between runs. Please use a list instead.')
+            else:
+                recov_group['recov_params'] = list(recov_params)
+        self.recov_groups = recov_groups
 
     @torch.no_grad()
     def step(self, closure=None):
         """Performs a single optimization step.
 
         Args:
             closure (Callable, optional): A closure that reevaluates the model
@@ -115,26 +135,30 @@
         self._cuda_graph_capture_health_check()
 
         loss = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
-        for group in self.param_groups:
+        for group_idx, group in enumerate(self.param_groups):
             params_with_grad = []
             grads = []
             exp_avgs = []
             exp_avg_sqs = []
             max_exp_avg_sqs = []
             recov_params = []
             state_steps = []
             amsgrad = group['amsgrad']
             beta1, beta2 = group['betas']
+            if self.recov_groups is None:
+                recov_group = None
+            else:
+                recov_group = self.recov_groups[group_idx]
 
-            for p in group['params']:
+            for p_idx, p in enumerate(group['params']):
                 if p.grad is None:
                     continue
                 params_with_grad.append(p)
                 if p.grad.is_sparse:
                     raise RuntimeError('AdamR does not support sparse gradients')
                 grads.append(p.grad)
 
@@ -148,15 +172,18 @@
                     state['exp_avg'] = torch.zeros_like(p, memory_format=torch.preserve_format)
                     # Exponential moving average of squared gradient values
                     state['exp_avg_sq'] = torch.zeros_like(p, memory_format=torch.preserve_format)
                     if amsgrad:
                         # Maintains max of all exp. moving avg. of sq. grad. values
                         state['max_exp_avg_sq'] = torch.zeros_like(p, memory_format=torch.preserve_format)
                     # The recovery parameter values
-                    state['recov_param'] = torch.clone(p, memory_format=torch.preserve_format).detach()
+                    if recov_group is None:
+                        state['recov_param'] = torch.clone(p, memory_format=torch.preserve_format).detach()
+                    else:
+                        state['recov_param'] = recov_group['recov_params'][p_idx]
 
                 exp_avgs.append(state['exp_avg'])
                 exp_avg_sqs.append(state['exp_avg_sq'])
 
                 if amsgrad:
                     max_exp_avg_sqs.append(state['max_exp_avg_sq'])
```

### Comparing `adamr-0.0.1/.gitignore` & `adamr-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adamr-0.0.1/LICENSE` & `adamr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adamr-0.0.1/README.md` & `adamr-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `adamr-0.0.1/pyproject.toml` & `adamr-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "hatchling",
     "torch>=1.13.1",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "adamr"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Yintao Tai", email="tai.yintao@gmail.com" },
 ]
 description = "Adam with weight recovery optimizer for pytorch"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `adamr-0.0.1/PKG-INFO` & `adamr-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adamr
-Version: 0.0.1
+Version: 0.0.2
 Summary: Adam with weight recovery optimizer for pytorch
 Project-URL: Homepage, https://github.com/TYTTYTTYT/AdamR
 Project-URL: Bug Tracker, https://github.com/TYTTYTTYT/AdamR/issues
 Project-URL: repository, https://github.com/TYTTYTTYT/AdamR.git
 Author-email: Yintao Tai <tai.yintao@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

