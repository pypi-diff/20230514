# Comparing `tmp/syncdsgen-0.0.8.tar.gz` & `tmp/syncdsgen-0.0.9.tar.gz`

## Comparing `syncdsgen-0.0.8.tar` & `syncdsgen-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/requirements.txt
--rwxr-xr-x   0        0        0     9221 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/syncdsgen_demo.ipynb
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/.vscode/settings.json
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/SynCDsGen/__init__.py
--rwxr-xr-x   0        0        0    16514 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/SynCDsGen/syncdsgen.py
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/.gitignore
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/LICENCE
--rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/README.md
--rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 syncdsgen-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 syncdsgen-0.0.9/requirements.txt
+-rwxr-xr-x   0        0        0    10844 2020-02-02 00:00:00.000000 syncdsgen-0.0.9/syncdsgen_demo.ipynb
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 syncdsgen-0.0.9/.vscode/settings.json
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 syncdsgen-0.0.9/SynCDsGen/__init__.py
+-rwxr-xr-x   0        0        0    20681 2020-02-02 00:00:00.000000 syncdsgen-0.0.9/SynCDsGen/syncdsgen.py
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 syncdsgen-0.0.9/.gitignore
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 syncdsgen-0.0.9/LICENCE
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 syncdsgen-0.0.9/README.md
+-rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 syncdsgen-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 syncdsgen-0.0.9/PKG-INFO
```

### Comparing `syncdsgen-0.0.8/requirements.txt` & `syncdsgen-0.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.8/syncdsgen_demo.ipynb` & `syncdsgen-0.0.9/syncdsgen_demo.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9610152714932126%*

 * *Differences: {"'cells'": "{3: {'execution_count': 9}, 7: {'source': {insert: [(0, '#define and configure the "*

 * *            'data generator\\n\'), (4, "conf.codons = [\'aa\', \'ab\', \'ac\', \'ba\', \'bb\', '*

 * *            '\'bc\', \'ca\', \'cb\']\\n"), (11, "    \'C\': [\'ba\', \'bc\', \'bb\'],\\n"), (12, '*

 * *            '"    \'D\': [\'ca\', \'cb\']\\n")], delete: [11, 10, 3]}}, 10: {\'execution_count\': '*

 * *            "4, 'source': {insert: [(1, 'synthetic_data, _, _ = generator.sample(length=100, "*

 * *            "n_samples= […]*

```diff
@@ -23,15 +23,15 @@
             "outputs": [],
             "source": [
                 "exit()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import torch\n",
                 "import SynCDsGen\n",
                 "import re"
             ]
@@ -42,51 +42,119 @@
             "metadata": {},
             "source": [
                 "## Generate data from a purely stochastic/Markov type model"
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": 10,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "#define and configure the data generator\n",
+                "conf = SynCDsGen.SyncCDsGeneratorConf(nb_codons=10, nb_AAs=4, codon_length=2)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 14,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "tensor([[0.0000, 0.0000, 0.5000, 0.5000],\n",
+                            "        [0.0000, 0.0000, 0.5000, 0.5000],\n",
+                            "        [0.0000, 0.0000, 0.5000, 0.5000],\n",
+                            "        [0.0000, 0.0000, 0.5000, 0.5000]])"
+                        ]
+                    },
+                    "execution_count": 14,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "conf.transition_prob_t"
+            ]
+        },
+        {
+            "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
+                "#define and configure the data generator\n",
                 "conf = SynCDsGen.SyncCDsGeneratorConf()\n",
                 "\n",
                 "conf.bases = ['a', 'b', 'c']\n",
-                "conf.codons = ['aa', 'ab', 'ac', 'ba', 'ca', 'bb', 'bc', 'cb']\n",
+                "conf.codons = ['aa', 'ab', 'ac', 'ba', 'bb', 'bc', 'ca', 'cb']\n",
                 "conf.start_codons = ['aa', 'ab']\n",
                 "conf.stop_codons = ['ac']\n",
                 "conf.AAs = ['A', 'B', 'C', 'D']\n",
                 "conf.translation_dict = {\n",
                 "    'A':  ['aa', 'ab'],\n",
                 "    'B': ['ac'],\n",
-                "    'C': ['ba', 'bc', 'cb'],\n",
-                "    'D': ['ca', 'bb']\n",
+                "    'C': ['ba', 'bc', 'bb'],\n",
+                "    'D': ['ca', 'cb']\n",
                 "}\n",
                 "conf.transition_prob_t = torch.Tensor([[0,  0, 1/2, 1/2],\n",
                 "                            [0, 0, 1/2, 1/2],\n",
                 "                            [0, 0, 1/2, 1/2],\n",
                 "                            [0, 0, 1/2, 1/2]])\n",
                 "\n",
                 "conf.emission_prob_t = torch.Tensor([[1/2, 1/2, 0.0],\n",
                 "                          [1, 0.0, 0.0],\n",
                 "                          [0.6, 0.2, 0.2],\n",
                 "                          [0.7, 0.3, 0.0]])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
-                "generator = SynCDsGen.StochasticSynCDsGenerator(conf)\n",
+                "import torch\n",
                 "\n",
-                "synthetic_data = generator.sample(length=5)"
+                "tensor = torch.randn(3, 3)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "tensor([[ 5.9571e-01,  1.0000e+00,  1.3763e-03],\n",
+                            "        [-7.2472e-01,  1.0000e+00, -4.3362e-01],\n",
+                            "        [-1.5265e+00,  1.0000e+00, -2.8351e-01]])"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "tensor[:, 1] = 1\n",
+                "\n",
+                "tensor"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "generator = SynCDsGen.StochasticSynCDsGenerator(conf)\n",
+                "synthetic_data, _, _ = generator.sample(length=100, n_samples=250000)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
@@ -301,14 +369,21 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "synthetic_data.head()"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "venv",
             "language": "python",
             "name": "python3"
```

### Comparing `syncdsgen-0.0.8/SynCDsGen/syncdsgen.py` & `syncdsgen-0.0.9/SynCDsGen/syncdsgen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,69 @@
 #import useful modules
 import torch
 import pyro
 import pandas as pd
 import numpy as np
 import re
 from enum import Enum
+import string
+import math
+import itertools
+import random
+
+LOWERCASE_ALPHABET = list(string.ascii_lowercase)
+UPPERCASE_ALPHABET = list(string.ascii_uppercase)
 
 def check_row_sum(tensor, tol=1e-6):
     """
         Function to check if each row of a given tensor sum up to 1
     """
     row_sums = tensor.sum(dim=1)
     return torch.all(torch.abs(row_sums - 1) < tol)
 
 
+def generate_codons_distribution(nb_AAs, nb_codons):
+    """
+        Function to generate the distribution of the codons within the differents amino acids
+    """
+    if nb_AAs == 1:
+        return [nb_codons]
+    
+    num = random.randint(1, nb_codons - (nb_AAs - 1))  # ensures there's enough "total" left for future numbers
+    return [num] + generate_codons_distribution(nb_AAs - 1, nb_codons - num)
+
+def generate_prob_dist(length):
+    """
+        Function to generate a list of length numbers summing up to 1
+    """
+    # Generate random numbers
+    numbers = [random.random() for _ in range(length)]
+
+    # Normalize the numbers so that their sum equals 1
+    total = sum(numbers)
+    normalized_numbers = [n / total for n in numbers]
+
+    return normalized_numbers
+
 class SyncCDsGeneratorConf:
-    def __init__(self, bases=None, codons=None, start_codons=None,
-                  stop_codons=None, AAs=None, translation_dict=None,
+    def __init__(self, bases=None, codons=None, nb_codons=None,
+                 start_codons=None, nb_AAs=None, nb_start_codons=2,
+                 stop_codons=None, AAs=None, translation_dict={},
+                 nb_stop_codons=1,
                   transition_prob_t=None, emission_prob_t=None, AAs_initial_prob_dist=None,
                   codon_length=None, constraints_dict=None, AAs_stop_prob_dist=None):
         """
         Initialize a new instance of SyncCDsGeneratorConf
 
         Args:
             bases (list): list of bases
             codons (list): list of codons
+            nb_codons (int): number of codons
             start_codons (list): list of start codons
+            nb_AAs (int): number of amino acids
             stop_codons (list): list of stop codons
             AAs (list): list of amino acids
 
             translation_dict (dict): dictionary containing the rules of translation of the codons into amino acids
                 key: amino aicd
                 value: codons encoding the amino acid
 
@@ -82,25 +116,92 @@
                 conf.emission_prob_t = torch.Tensor([[1/2, 1/2, 0.0],
                                         [1, 0.0, 0.0],
                                         [0.6, 0.2, 0.2],
                                         [0.7, 0.3, 0.0]])
         """
         self.bases = bases
         self.codons = codons
+        self.nb_codons = nb_codons
         self.start_codons = start_codons
+        self.nb_AAs = nb_AAs
+        self.nb_start_codons = nb_start_codons
         self.stop_codons = stop_codons
         self.AAs = AAs
         self.translation_dict = translation_dict
+        self.nb_stop_codons = nb_stop_codons
         self.transition_prob_t = transition_prob_t
         self.emission_prob_t = emission_prob_t
         self.AAs_initial_prob_dist = AAs_initial_prob_dist
         self.codon_length = codon_length
         self.constraints_dict = constraints_dict
         self.AAs_stop_prob_dist = AAs_stop_prob_dist
 
+        if all(el is not None for el in [self.nb_codons, self.nb_AAs, self.codon_length]):
+            #if we specified the number of codons and the number of amino acids, we automatically
+            #compute the parameters of the configurator
+            if self.codon_length is None:
+                self.codon_length = 2
+            
+            self.nb_bases = math.ceil(math.log(self.nb_codons, self.codon_length))
+            self.bases = LOWERCASE_ALPHABET[:self.nb_bases]
+
+            # Generate all possible arrangements of the bases
+            arrangements = list(itertools.permutations(self.bases, self.codon_length))
+            possible_codons = [''.join(arrangement) for arrangement in arrangements]
+            self.codons = possible_codons[:self.nb_codons]
+
+            self.start_codons = self.codons[:self.nb_start_codons]
+            self.stop_codons = self.codons[self.nb_start_codons:self.nb_start_codons+self.nb_stop_codons]
+
+            #define the list of amino acids
+            self.AAs = UPPERCASE_ALPHABET[:self.nb_AAs]
+
+            #generate the distribution of codons between the different amino acids
+            codons_dist = generate_codons_distribution(self.nb_AAs - 2, self.nb_codons - self.nb_start_codons - self.nb_stop_codons)
+            
+            pos = 0
+            self.translation_dict[self.AAs[0]] = self.codons[:self.nb_start_codons]
+            pos += self.nb_start_codons
+            self.translation_dict[self.AAs[1]] = self.codons[pos:pos+1]
+            pos += 1
+
+            for i, nb in enumerate(codons_dist):
+                self.translation_dict[self.AAs[i+2]] = self.codons[pos:nb]
+                pos += nb
+            
+            #construct the transition probability table
+            self.transition_prob_t = torch.zeros((self.nb_AAs, self.nb_AAs))
+            for i in range(2, self.nb_AAs):
+                self.transition_prob_t[:, i] = 1/(self.nb_AAs-2)
+
+            #build the emission matrix
+            n_cols = max(max(codons_dist), 2)
+            self.emission_prob_t = torch.zeros((self.nb_AAs, n_cols))
+            
+            #emission distribution of the start codons
+            new_row = [0] * n_cols
+            for i in range(self.nb_start_codons):
+                new_row[i] = 1/self.nb_start_codons
+            self.emission_prob_t[0, :] = torch.tensor(new_row)
+
+            #emission distribution of the stop codons
+            new_row = [0] * n_cols
+            new_row[0] = 1
+            self.emission_prob_t[1, :] = torch.tensor(new_row)
+
+            #emission distributions of the other amino acids
+            for i, nb in enumerate(codons_dist):
+                new_row = [0] * n_cols
+                emission_dist = generate_prob_dist(nb)
+
+                for k in range(nb):
+                    new_row[k] = emission_dist[k]
+
+                self.emission_prob_t[i+2] = torch.tensor(new_row)
+
     def is_AA_start_AA(self, AA):
         coding_codons = self.translation_dict[AA]
 
         for codon in coding_codons:
             if codon in self.start_codons:
                 return 1
         return 0
```

### Comparing `syncdsgen-0.0.8/LICENCE` & `syncdsgen-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `syncdsgen-0.0.8/pyproject.toml` & `syncdsgen-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "syncdsgen"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Ramses TANANKEM", email="tanankemr@gmail.com" },
 ]
 description = "A package to generate synthetic coding sequences data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `syncdsgen-0.0.8/PKG-INFO` & `syncdsgen-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncdsgen
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to generate synthetic coding sequences data
 Project-URL: Homepage, https://github.com/wl-research/syncdsgen
 Author-email: Ramses TANANKEM <tanankemr@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

