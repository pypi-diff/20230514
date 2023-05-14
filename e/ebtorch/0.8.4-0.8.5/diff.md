# Comparing `tmp/ebtorch-0.8.4.tar.gz` & `tmp/ebtorch-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebtorch-0.8.4.tar", last modified: Fri Mar 17 16:01:24 2023, max compression
+gzip compressed data, was "ebtorch-0.8.5.tar", last modified: Sun May 14 01:11:26 2023, max compression
```

## Comparing `ebtorch-0.8.4.tar` & `ebtorch-0.8.5.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:01:24.758418 ebtorch-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-03-17 16:01:10.000000 ebtorch-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-17 16:01:24.758418 ebtorch-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-17 16:01:10.000000 ebtorch-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:01:24.754418 ebtorch-0.8.4/ebtorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:01:24.754418 ebtorch-0.8.4/ebtorch/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/logging/avgmeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/logging/logcsv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:01:24.758418 ebtorch-0.8.4/ebtorch/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/conv2drp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/convolutional_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/coordconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/debuglayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/fieldtransform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:01:24.758418 ebtorch-0.8.4/ebtorch/nn/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/functional/inner_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/kwta.py
--rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/laplacenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/lmu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/mish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/nnsemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/reshapelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/serlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/sinlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/smelu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:01:24.758418 ebtorch-0.8.4/ebtorch/nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/utils/adverutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/utils/autoclip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/utils/onlyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/nn/utils/reprutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:01:24.758418 ebtorch-0.8.4/ebtorch/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/optim/adahessian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/optim/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/optim/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/optim/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/optim/radam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-03-17 16:01:10.000000 ebtorch-0.8.4/ebtorch/optim/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:01:24.754418 ebtorch-0.8.4/ebtorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-17 16:01:24.000000 ebtorch-0.8.4/ebtorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-17 16:01:24.000000 ebtorch-0.8.4/ebtorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 16:01:24.000000 ebtorch-0.8.4/ebtorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 16:01:24.000000 ebtorch-0.8.4/ebtorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-17 16:01:24.000000 ebtorch-0.8.4/ebtorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 16:01:24.758418 ebtorch-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-17 16:01:10.000000 ebtorch-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.580222 ebtorch-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-05-14 01:11:15.000000 ebtorch-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-14 01:11:26.580222 ebtorch-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-14 01:11:15.000000 ebtorch-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.576222 ebtorch-0.8.5/ebtorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.576222 ebtorch-0.8.5/ebtorch/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/logging/avgmeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/logging/logcsv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.576222 ebtorch-0.8.5/ebtorch/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/conv2drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/convolutional_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/coordconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/debuglayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/fieldtransform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.576222 ebtorch-0.8.5/ebtorch/nn/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/functional/inner_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/kwta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/laplacenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/lmu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/mish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/nnsemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/reshapelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/serf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/serlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/sinlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/smelu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.580222 ebtorch-0.8.5/ebtorch/nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/utils/adverutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/utils/autoclip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/utils/onlyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/nn/utils/reprutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.580222 ebtorch-0.8.5/ebtorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/adahessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/radam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-14 01:11:15.000000 ebtorch-0.8.5/ebtorch/optim/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 01:11:26.576222 ebtorch-0.8.5/ebtorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-14 01:11:26.000000 ebtorch-0.8.5/ebtorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 01:11:26.000000 ebtorch-0.8.5/ebtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:11:26.000000 ebtorch-0.8.5/ebtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 01:11:26.000000 ebtorch-0.8.5/ebtorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 01:11:26.000000 ebtorch-0.8.5/ebtorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 01:11:26.580222 ebtorch-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-14 01:11:15.000000 ebtorch-0.8.5/setup.py
```

### Comparing `ebtorch-0.8.4/LICENSE` & `ebtorch-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/PKG-INFO` & `ebtorch-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.8.4
+Version: 0.8.5
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.8.4 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.8.5 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.8.4/ebtorch/__init__.py` & `ebtorch-0.8.5/ebtorch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 del MishPulse
 del MishPulseSymmY
 del MultiSolvePoissonTensor
 del NNEnsemble
 del PoissonNetCifar
 del ProbePrintLayer
 del ReshapeLayer
+del ScaledERF
 del SERLU
 del SGRUHCell
 del SinLU
 del SmeLU
 del SolvePoisson
 del SolvePoissonTensor
 del beta_reco_bce
```

### Comparing `ebtorch-0.8.4/ebtorch/logging/__init__.py` & `ebtorch-0.8.5/ebtorch/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/logging/avgmeter.py` & `ebtorch-0.8.5/ebtorch/logging/avgmeter.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/logging/logcsv.py` & `ebtorch-0.8.5/ebtorch/logging/logcsv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/__init__.py` & `ebtorch-0.8.5/ebtorch/nn/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 from .mish import Mish
 from .mish import mishlayer_init
 from .mish import MishPulse
 from .mish import MishPulseSymmY
 from .nnsemble import NNEnsemble
 from .reshapelayers import FlatChannelize2DLayer
 from .reshapelayers import ReshapeLayer
+from .serf import ScaledERF
 from .serlu import SERLU
 from .sinlu import SinLU
 from .smelu import SmeLU
 from .utils import *
 
 # Deletions (from .)
 del architectures
@@ -77,17 +78,19 @@
 del lmu
 del mish
 del nnsemble
 del reshapelayers
 del serlu
 del sinlu
 del smelu
+del serf
 
 # Deletions (from .functional)
 # del mish  # (already done by chance!)
+# del serf  # (already done by chance!)
 
 # Deletions (from .utils)
 del AdverApply
 del AutoClipper
 del TA2ATAdapter
 del argser_f
 del argsink
```

### Comparing `ebtorch-0.8.4/ebtorch/nn/architectures.py` & `ebtorch-0.8.5/ebtorch/nn/architectures.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/conv2drp.py` & `ebtorch-0.8.5/ebtorch/nn/conv2drp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+from collections.abc import Generator
 from typing import Any
-from typing import Generator
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import torch
-from fastprogress import master_bar
-from fastprogress import progress_bar
 from torch.nn.common_types import _size_2_t
 from torch.nn.modules.batchnorm import BatchNorm2d
 from torch.nn.modules.conv import Conv2d
 from torch.nn.modules.dropout import Dropout2d
 from torch.nn.parameter import Parameter
+from tqdm.auto import tqdm
 
 
 class BatchNorm2dRP(BatchNorm2d):
     """2D batch normalization layer compatible with random patch learning. Identical to BatchNorm2d."""
 
 
 class Dropout2dRP(Dropout2d):
@@ -26,28 +25,30 @@
 
 
 class Conv2dRP(Conv2d):
     """2D convolutional layer compatible with random patch learning."""
 
     # Parent __init__
     def __init__(
-        self,
+        self,  # NOSONAR
         in_channels: int,
         out_channels: int,
         kernel_size: _size_2_t,
         stride: _size_2_t = 1,
         padding: Union[str, _size_2_t] = 0,
         dilation: _size_2_t = 1,
         groups: int = 1,
         bias: bool = True,
         padding_mode: str = "zeros",
         device: Optional[Any] = None,
         dtype: Optional[Any] = None,
         # Additional arguments
         patches_stride: Optional[_size_2_t] = None,
+        patches_online_sampling_ratio: float = 1.0,
+        patches_online_trimming_target: int = 1,
         track_inputs: bool = False,
     ) -> None:
         # Default argument substitution
         if patches_stride is None:
             patches_stride = stride
 
         # Parent class constructor
@@ -63,16 +64,18 @@
             padding_mode,
             device,
             dtype,
         )
 
         # Additional member variables
         self.patches_stride: _size_2_t = patches_stride
+        self.patches_online_sampling_ratio: float = patches_online_sampling_ratio
+        self.patches_online_trimming_target: int = patches_online_trimming_target
         self.is_tracking_inputs: bool = track_inputs
-        self.inputs: List[torch.Tensor] = []
+        # self.inputs: List[torch.Tensor] = []
 
     # Additional private methods
 
     def _produce_patches(self) -> torch.Tensor:
         with torch.no_grad():
             if isinstance(self.kernel_size, int):
                 _kernel_size: Tuple[int, int] = (self.kernel_size, self.kernel_size)
@@ -154,22 +157,23 @@
     return_net: bool = False,
 ) -> Optional[torch.nn.Module]:
     _train_toggle_status: bool = net.training  # Save training value
 
     net.eval()  # Do not track statistics
     with torch.no_grad():  # Do not track gradients
         # Iterate over all layers in the network
-        layers_master_bar = master_bar(
+        for layer in tqdm(
             [
                 _lay
                 for _lay in net.modules()
                 if isinstance(_lay, (BatchNorm2dRP, Conv2dRP, Dropout2dRP))
-            ]
-        )
-        for layer in layers_master_bar:
+            ],
+            leave=False,
+            desc="RP-training network",
+        ):
             # PREPARATION | Case 1: BatchNorm2d layer
             if isinstance(layer, BatchNorm2dRP):
                 layer.running_mean = torch.zeros_like(layer.running_mean)
                 layer.running_var = torch.ones_like(layer.running_var)
                 layer.train()
 
             # PREPARATION | Case 2: Dropout2dRP layer
@@ -180,18 +184,18 @@
             elif isinstance(layer, Conv2dRP):
                 layer.clear_tracked_inputs()
                 layer.eval()
                 layer.set_tracking(True)
 
             # DATA PASS | All cases
             if isinstance(layer, (BatchNorm2dRP, Conv2dRP, Dropout2dRP)):
-                for batched_datapoint in progress_bar(data, parent=layers_master_bar):
+                for batched_datapoint in tqdm(
+                    data, leave=True, desc=f"RP-training layer {layer}"
+                ):
                     _ = net(batched_datapoint[0])
-                    layers_master_bar.child.comment = "RP-training layer..."
-                layers_master_bar.write(f"RP-trained layer {layer}.")
 
             # POST | Case 1; Case 2
             if isinstance(layer, (BatchNorm2dRP, Dropout2dRP)):
                 layer.eval()
 
             # POST | Case 3: Conv2dRP layer
             elif isinstance(layer, Conv2dRP):
```

### Comparing `ebtorch-0.8.4/ebtorch/nn/convolutional_flatten.py` & `ebtorch-0.8.5/ebtorch/nn/convolutional_flatten.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/coordconv.py` & `ebtorch-0.8.5/ebtorch/nn/coordconv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/debuglayers.py` & `ebtorch-0.8.5/ebtorch/nn/debuglayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/fieldtransform.py` & `ebtorch-0.8.5/ebtorch/nn/fieldtransform.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/functional/__init__.py` & `ebtorch-0.8.5/ebtorch/nn/functional/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,12 +21,13 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 # Imports (specific)
 from .inner_functional import field_transform
 from .inner_functional import mish
 from .inner_functional import mishpulse
 from .inner_functional import mishpulse_symmy
+from .inner_functional import serf
 from .inner_functional import serlu
 from .inner_functional import smelu
 
 # Deletions (from .)
 del inner_functional
```

### Comparing `ebtorch-0.8.4/ebtorch/nn/functional/inner_functional.py` & `ebtorch-0.8.5/ebtorch/nn/functional/inner_functional.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 #                       orig. code: https://github.com/digantamisra98/Mish ;
 #                       license text: https://github.com/digantamisra98/Mish/blob/master/LICENSE]
 #
 # ==============================================================================
 # SPDX-License-Identifier: MIT
 # SPDX-License-Identifier: Apache-2.0
 # IMPORTS
+import math
+
 import torch
 import torch.nn.functional as F
 from torch import Tensor
 from torch.overrides import handle_torch_function
 from torch.overrides import has_torch_function_unary
 
 
@@ -118,7 +120,13 @@
     """
     assert beta >= 0
     return torch.where(
         torch.abs(x_input) <= beta,
         torch.div(torch.pow(torch.add(x_input, beta), 2), 4.0 * beta),
         F.relu(x_input),
     )
+
+
+@torch.jit.script
+def serf(x: Tensor) -> Tensor:
+    """Applies the Scaled ERror Function, element-wise."""
+    return torch.erf(x / math.sqrt(2.0))  # type: ignore
```

### Comparing `ebtorch-0.8.4/ebtorch/nn/kwta.py` & `ebtorch-0.8.5/ebtorch/nn/kwta.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 #
 # Copyright (c) 2020-* Emanuele Ballarin <emanuele@ballarin.cc>
 #                      All Rights Reserved.
 #                      [maintainance, adaptation, extension]
 #
 # ==============================================================================
 # For type-annotation
+from collections.abc import Callable
 from typing import Any
-from typing import Callable
 from typing import List
 from typing import Optional
 from typing import Union
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor
```

### Comparing `ebtorch-0.8.4/ebtorch/nn/laplacenet.py` & `ebtorch-0.8.5/ebtorch/nn/laplacenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 #                      [orig. code: https://github.com/a-rahimi/laplace-net ]
 #
 # Copyright (c) 2023-* Emanuele Ballarin <emanuele@ballarin.cc> (minor edits)
 #                      All Rights Reserved.
 #                      Licensed according to the MIT License.
 #
 # ==============================================================================
+from collections.abc import Callable
+from collections.abc import Iterable
 from copy import deepcopy
-from typing import Callable
-from typing import Iterable
 from typing import Tuple
 
 import numpy as np
 import torch
 import torch.nn.functional as F
 from torch import nn
```

### Comparing `ebtorch-0.8.4/ebtorch/nn/lmu.py` & `ebtorch-0.8.5/ebtorch/nn/lmu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/mish.py` & `ebtorch-0.8.5/ebtorch/nn/mish.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/nnsemble.py` & `ebtorch-0.8.5/ebtorch/nn/nnsemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 #
 # ==============================================================================
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Imports
 import warnings
+from collections.abc import Callable
+from collections.abc import Iterable
+from collections.abc import Sequence
 from typing import Any
-from typing import Callable
-from typing import Iterable
 from typing import Optional
-from typing import Sequence
 from typing import TypeVar
 from typing import Union
 
 import torch as th
 from functorch import combine_state_for_ensemble
 from functorch import vmap
 from torch import nn as thnn
```

### Comparing `ebtorch-0.8.4/ebtorch/nn/reshapelayers.py` & `ebtorch-0.8.5/ebtorch/nn/reshapelayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/serlu.py` & `ebtorch-0.8.5/ebtorch/nn/serlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/sinlu.py` & `ebtorch-0.8.5/ebtorch/nn/sinlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/smelu.py` & `ebtorch-0.8.5/ebtorch/nn/smelu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/utils/__init__.py` & `ebtorch-0.8.5/ebtorch/nn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/utils/adverutils.py` & `ebtorch-0.8.5/ebtorch/nn/utils/adverutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # ==============================================================================
 #
 # SPDX-License-Identifier: Apache-2.0
 #
-from typing import Callable
+from collections.abc import Callable
 from typing import List
 from typing import Tuple
 from typing import Union
 
 import torch as th
 from advertorch.attacks import Attack as ATAttack
 from torchattacks.attack import Attack as TAAttack
```

### Comparing `ebtorch-0.8.4/ebtorch/nn/utils/autoclip.py` & `ebtorch-0.8.5/ebtorch/nn/utils/autoclip.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/utils/onlyutils.py` & `ebtorch-0.8.5/ebtorch/nn/utils/onlyutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/utils/patches.py` & `ebtorch-0.8.5/ebtorch/nn/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/nn/utils/reprutils.py` & `ebtorch-0.8.5/ebtorch/nn/utils/reprutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/optim/__init__.py` & `ebtorch-0.8.5/ebtorch/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/optim/adahessian.py` & `ebtorch-0.8.5/ebtorch/optim/adahessian.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/optim/adan.py` & `ebtorch-0.8.5/ebtorch/optim/adan.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/optim/custom.py` & `ebtorch-0.8.5/ebtorch/optim/custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # ==============================================================================
 #
 # SPDX-License-Identifier: Apache-2.0
 #
-from typing import Iterable
+from collections.abc import Iterable
 from typing import Tuple
 from typing import Union
 
 from torch import Tensor
 
 from .lookahead import Lookahead
 from .radam import RAdam
```

### Comparing `ebtorch-0.8.4/ebtorch/optim/lion.py` & `ebtorch-0.8.5/ebtorch/optim/lion.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Implementation of the Lion optimizer."""
-from typing import Callable
+from collections.abc import Callable
 from typing import Optional
 from typing import Tuple
 
 import torch
 from torch.optim.optimizer import Optimizer
```

### Comparing `ebtorch-0.8.4/ebtorch/optim/lookahead.py` & `ebtorch-0.8.5/ebtorch/optim/lookahead.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/optim/radam.py` & `ebtorch-0.8.5/ebtorch/optim/radam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch/optim/sam.py` & `ebtorch-0.8.5/ebtorch/optim/sam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.8.4/ebtorch.egg-info/PKG-INFO` & `ebtorch-0.8.5/ebtorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.8.4
+Version: 0.8.5
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.8.4 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.8.5 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.8.4/ebtorch.egg-info/SOURCES.txt` & `ebtorch-0.8.5/ebtorch.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 ebtorch/nn/fieldtransform.py
 ebtorch/nn/kwta.py
 ebtorch/nn/laplacenet.py
 ebtorch/nn/lmu.py
 ebtorch/nn/mish.py
 ebtorch/nn/nnsemble.py
 ebtorch/nn/reshapelayers.py
+ebtorch/nn/serf.py
 ebtorch/nn/serlu.py
 ebtorch/nn/sinlu.py
 ebtorch/nn/smelu.py
 ebtorch/nn/functional/__init__.py
 ebtorch/nn/functional/inner_functional.py
 ebtorch/nn/utils/__init__.py
 ebtorch/nn/utils/adverutils.py
```

### Comparing `ebtorch-0.8.4/setup.py` & `ebtorch-0.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,28 +48,28 @@
 
     if missing_dependencies:
         warnings.warn(f"Missing dependencies: {missing_dependencies}")
 
 
 DEPENDENCY_PACKAGE_NAMES = [
     "advertorch",
-    "fastprogress",
     "nengolib",
     "numpy",
     "requests",
     "torch",
     "torchattacks",
+    "tqdm",
 ]
 
 check_dependencies()
 
 
 setup(
     name="ebtorch",
-    version="0.8.4",
+    version="0.8.5",
     author="Emanuele Ballarin",
     author_email="emanuele@ballarin.cc",
     url="https://github.com/emaballarin/ebtorch",
     description="Collection of PyTorch additions, extensions, utilities, uses and abuses",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     keywords=["Deep Learning", "Machine Learning"],
```

