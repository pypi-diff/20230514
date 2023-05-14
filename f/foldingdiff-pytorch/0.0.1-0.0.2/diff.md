# Comparing `tmp/foldingdiff-pytorch-0.0.1.tar.gz` & `tmp/foldingdiff-pytorch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foldingdiff-pytorch-0.0.1.tar", last modified: Sun May 14 15:34:38 2023, max compression
+gzip compressed data, was "foldingdiff-pytorch-0.0.2.tar", last modified: Sun May 14 15:41:25 2023, max compression
```

## Comparing `foldingdiff-pytorch-0.0.1.tar` & `foldingdiff-pytorch-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:34:38.418987 foldingdiff-pytorch-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-14 15:34:38.418987 foldingdiff-pytorch-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-14 15:34:21.000000 foldingdiff-pytorch-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:34:38.418987 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 15:34:21.000000 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-14 15:34:21.000000 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-14 15:34:21.000000 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch/foldingdiff_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-14 15:34:21.000000 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-14 15:34:21.000000 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-14 15:34:21.000000 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:34:38.418987 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-14 15:34:38.000000 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-14 15:34:38.000000 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:34:38.000000 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 15:34:38.000000 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 15:34:38.000000 foldingdiff-pytorch-0.0.1/foldingdiff_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:34:38.418987 foldingdiff-pytorch-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-14 15:34:21.000000 foldingdiff-pytorch-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:41:25.153982 foldingdiff-pytorch-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-14 15:41:25.153982 foldingdiff-pytorch-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:41:25.153982 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/foldingdiff_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 15:41:25.153982 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-14 15:41:25.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-14 15:41:25.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 15:41:25.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 15:41:25.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 15:41:25.000000 foldingdiff-pytorch-0.0.2/foldingdiff_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 15:41:25.153982 foldingdiff-pytorch-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-14 15:41:14.000000 foldingdiff-pytorch-0.0.2/setup.py
```

### Comparing `foldingdiff-pytorch-0.0.1/README.md` & `foldingdiff-pytorch-0.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -3,19 +3,42 @@
 [![Lightning](https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white)](https://github.com/Lightning-AI/lightning)
 
 ![banner](img/banner.png)
 
 An unofficial re-implementation of FoldingDiff, a diffusion-based generative model for protein backbone structure generation.
 The image below shows the forward (noising) process of the protein backbone structure.
 
+## Noising
+
 <img src="img/noising.gif" width="325">
 
+## Denoising
+
+<img src="img/denoising_64res.gif" width="325">
+
 ## Installation
 
-WIP
+Install through pip.
+```bash
+$ pip install foldingdiff-pytorch
+```
+
+## Quickstart
+
+### Training
+```bash
+$ python -m foldingdiff_pytorch.train --meta data/meta.csv \
+  --data-dir data/npy --batch-size 64
+```
+
+### Sampling
+```bash
+$ python -m foldingdiff_pytorch.sample --ckpt [CHECKPOINT_PATH] \
+  --timepoints 1000 --out [OUTPUT_PATH]
+```
 
 ## Downloading and preprocessing training data
 Download non-redundant protein backbone structure data (40% similary cutoff) from CATH.
 ```bash 
 $ wget ftp://orengoftp.biochem.ucl.ac.uk/cath/releases/latest-release/non-redundant-data-sets/cath-dataset-nonredundant-S40.pdb.tgz
 ```
```

### Comparing `foldingdiff-pytorch-0.0.1/foldingdiff_pytorch/data.py` & `foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from torch.utils.data import Dataset, DataLoader
 from pathlib import Path
 
 import foldingdiff_pytorch.util as util
 
 
 class FoldingDiffDataset(Dataset):
-    def __init__(self, meta, data_dir, T, mu=None, std=None, s=8e-3, max_len=128, train=True):
+    def __init__(self, meta, data_dir, T, mu=None, s=8e-3, max_len=128):
         self.meta = meta
         self.records = meta.to_records()
 
         self.data_dir = Path(data_dir)
         self.T = T
         self.max_len = max_len
 
@@ -25,25 +25,39 @@
         self.alpha_bar = f_t / f_t[0]
         self.beta = torch.clip(1 - self.alpha_bar[1:] / self.alpha_bar[:-1], min=0.001, max=0.999)
         self.alpha = 1 - self.beta
 
         self.alpha_bar_sqrt = torch.sqrt(self.alpha_bar)
         self.one_minus_alpha_bar_sqrt = torch.sqrt(1 - self.alpha_bar)
 
+        if mu is None:
+            feats = []
+            for r in self.records:
+                angles = np.load(self.data_dir / f'{r.id}.npy')
+                angles = np.nan_to_num(angles)
+                feats.append(angles)
+
+            feats = np.concatenate(feats, axis=0)
+            self.mu = torch.tensor( feats.mean(axis=0) ).float()
+        else:
+            self.mu = torch.tensor(mu).float()
+    
+    def get_mu(self):
+        return self.mu
 
     def __len__(self):
         return len(self.meta)
 
     def __getitem__(self, idx):
         r = self.records[idx]
         x0 = torch.tensor(np.load(self.data_dir / f"{r.id}.npy")).float()
         x0.nan_to_num_(0.0)
+        x0 = util.wrap(x0 - self.mu)
 
         n_residues = len(x0)
-
         if n_residues < self.max_len:
             x0 = torch.cat([x0, torch.zeros([self.max_len - n_residues, 6])], axis=0)
         elif n_residues > self.max_len:
             start_idx = random.randint(0, n_residues - self.max_len)
             x0 = x0[start_idx : start_idx + self.max_len]
 
         t = torch.randint(0, self.T, (1,)).long()
```

### Comparing `foldingdiff-pytorch-0.0.1/foldingdiff_pytorch/foldingdiff_pytorch.py` & `foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/foldingdiff_pytorch.py`

 * *Files identical despite different names*

### Comparing `foldingdiff-pytorch-0.0.1/foldingdiff_pytorch/train.py` & `foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,19 +28,21 @@
 
     meta = pd.read_csv(args.meta).sample(frac=1.0, random_state=42)
     N = len(meta)
 
     train_meta, val_meta = meta.iloc[: int(0.8 * N)], meta.iloc[int(0.8 * N) :]
 
     train_set = FoldingDiffDataset(
-        meta=train_meta, data_dir=args.data_dir, T=args.timesteps, train=True
+        meta=train_meta, data_dir=args.data_dir, T=args.timesteps
     )
+    mu = train_set.get_mu()
+    wandb_logger.log_hyperparams({"mu": mu})
 
     val_set = FoldingDiffDataset(
-        meta=val_meta, data_dir=args.data_dir, T=args.timesteps, train=False,
+        meta=val_meta, data_dir=args.data_dir, T=args.timesteps, mu=mu
     )
 
     model = FoldingDiff()
 
     train_dataloader = DataLoader(
         train_set,
         batch_size=args.batch_size,
```

### Comparing `foldingdiff-pytorch-0.0.1/foldingdiff_pytorch/util.py` & `foldingdiff-pytorch-0.0.2/foldingdiff_pytorch/util.py`

 * *Files identical despite different names*

### Comparing `foldingdiff-pytorch-0.0.1/setup.py` & `foldingdiff-pytorch-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'foldingdiff-pytorch',
   packages = find_packages(exclude=[]),
   include_package_data = True,
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'Unofficial implementation of foldingdiff in PyTorch.',
   author = 'Dohoon Lee',
   author_email = 'dohlee.bioinfo@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/dohlee/foldingdiff-pytorch',
   keywords = [
```

