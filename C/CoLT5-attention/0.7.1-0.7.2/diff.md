# Comparing `tmp/CoLT5-attention-0.7.1.tar.gz` & `tmp/CoLT5-attention-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.7.1.tar", last modified: Fri May 12 17:15:30 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.7.2.tar", last modified: Sun May 14 18:29:06 2023, max compression
```

## Comparing `CoLT5-attention-0.7.1.tar` & `CoLT5-attention-0.7.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:15:30.453575 CoLT5-attention-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:15:30.453575 CoLT5-attention-0.7.1/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-12 17:15:30.000000 CoLT5-attention-0.7.1/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-12 17:15:30.000000 CoLT5-attention-0.7.1/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:15:30.000000 CoLT5-attention-0.7.1/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 17:15:30.000000 CoLT5-attention-0.7.1/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 17:15:30.000000 CoLT5-attention-0.7.1/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-12 17:15:30.453575 CoLT5-attention-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:15:30.453575 CoLT5-attention-0.7.1/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/colt5_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)    35723 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:15:30.453575 CoLT5-attention-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-12 17:15:19.000000 CoLT5-attention-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:29:06.275940 CoLT5-attention-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:29:06.275940 CoLT5-attention-0.7.2/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-14 18:29:06.000000 CoLT5-attention-0.7.2/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-14 18:29:06.000000 CoLT5-attention-0.7.2/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:29:06.000000 CoLT5-attention-0.7.2/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-14 18:29:06.000000 CoLT5-attention-0.7.2/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 18:29:06.000000 CoLT5-attention-0.7.2/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-14 18:29:06.275940 CoLT5-attention-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:29:06.275940 CoLT5-attention-0.7.2/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/colt5_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36118 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 18:29:06.275940 CoLT5-attention-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/setup.py
```

### Comparing `CoLT5-attention-0.7.1/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.7.2/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.7.1
+Version: 0.7.2
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.7.1/LICENSE` & `CoLT5-attention-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.1/PKG-INFO` & `CoLT5-attention-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.7.1
+Version: 0.7.2
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.7.1/README.md` & `CoLT5-attention-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.1/colt5_attention/attend.py` & `CoLT5-attention-0.7.2/colt5_attention/attend.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.1/colt5_attention/coor_descent.py` & `CoLT5-attention-0.7.2/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.1/colt5_attention/transformer_block.py` & `CoLT5-attention-0.7.2/colt5_attention/transformer_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,15 @@
         self,
         dim,
         straight_through = True,
         n_iters = 50,                   # 50 iterations in the paper
         fetch_k_ratio = 9 / 8,          # in the paper, they do a bit slightly higher k (times this ratio) for better learning
         eps = 1.,                       # the epsilon for coordinate descent. in CoLT5 paper they used 1. apparently
         num_routing_tokens = 1,
+        learned_routing_tokens = False,
         use_triton = False,
         route_block_size = None,
         triton_checkpoint_segments = 4  # whether to recompute the coordinate descent in segments, with 4 and 50 iterations, backwards is sped up 3x times at the expense of forwards and some memory for saving initial a and b
     ):
         super().__init__()
         assert fetch_k_ratio >= 1.
         self.eps = eps
@@ -268,29 +269,30 @@
             self.coor_descent = partial(triton_coor_descent, checkpoint_segments = triton_checkpoint_segments)
 
         self.is_one_routing_token = num_routing_tokens == 1
         self.num_routing_tokens = num_routing_tokens
 
         self.route_block_size = route_block_size
 
-        self.routing_token = nn.Parameter(torch.randn(num_routing_tokens, dim))
+        self.routing_token = nn.Parameter(torch.randn(num_routing_tokens, dim)) if not learned_routing_tokens else None
         self.straight_through = straight_through
 
     def route_back(self, src, routed_tokens, indices):
         batch_range = create_batch_range(routed_tokens)
         src[batch_range, indices] = routed_tokens
         return src
 
     def forward(
         self,
         x,
         *,
         num_tokens,
         mask = None,
-        random_route = False
+        random_route = False,
+        routing_tokens = None
     ):
         n, device, eps, num_routes, route_block_size = x.shape[-2], x.device, self.eps, self.num_routing_tokens, self.route_block_size
 
         # whether to route even amounts from blocks of the sequence
 
         if exists(route_block_size):
             num_blocks = n // route_block_size
@@ -309,15 +311,23 @@
                 mask = rearrange(mask, 'b (n w) -> (b n) w', w = route_block_size)
 
             n = route_block_size
             num_tokens = math.ceil(num_tokens / num_blocks)
 
         # s stands for eventual normalized score
 
-        s = einsum('b n d, r d -> b r n', x, self.routing_token)
+        if exists(self.routing_token):
+            s = einsum('b n d, r d -> b r n', x, self.routing_token)
+        else:
+            assert exists(routing_tokens)
+
+            if routing_tokens.ndim == 2:
+                routing_tokens = rearrange(routing_tokens, 'b d -> b 1 d')
+
+            s = einsum('b n d, b r d -> b r n', x, routing_tokens)
 
         # merge routing dimension into batch
 
         x = repeat(x, 'b ... -> (b r) ...', r = num_routes)
         s, ps = pack_one(s, '* n')
 
         if exists(mask):
```

### Comparing `CoLT5-attention-0.7.1/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.7.2/colt5_attention/triton_coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.1/setup.py` & `CoLT5-attention-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.7.1',
+  version = '0.7.2',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

