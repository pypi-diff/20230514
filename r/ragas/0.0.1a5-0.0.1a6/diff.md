# Comparing `tmp/ragas-0.0.1a5.tar.gz` & `tmp/ragas-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragas-0.0.1a5.tar", last modified: Sun May 14 18:32:55 2023, max compression
+gzip compressed data, was "ragas-0.0.1a6.tar", last modified: Sun May 14 19:24:19 2023, max compression
```

## Comparing `ragas-0.0.1a5.tar` & `ragas-0.0.1a6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.189321 ragas-0.0.1a5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.185320 ragas-0.0.1a5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.189321 ragas-0.0.1a5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-14 18:32:41.000000 ragas-0.0.1a5/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-14 18:32:41.000000 ragas-0.0.1a5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-14 18:32:41.000000 ragas-0.0.1a5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 18:32:41.000000 ragas-0.0.1a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-14 18:32:41.000000 ragas-0.0.1a5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-14 18:32:55.189321 ragas-0.0.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-14 18:32:41.000000 ragas-0.0.1a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.185320 ragas-0.0.1a5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.189321 ragas-0.0.1a5/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-05-14 18:32:41.000000 ragas-0.0.1a5/docs/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.189321 ragas-0.0.1a5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 18:32:41.000000 ragas-0.0.1a5/examples/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)    25111 2023-05-14 18:32:41.000000 ragas-0.0.1a5/examples/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-14 18:32:41.000000 ragas-0.0.1a5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.189321 ragas-0.0.1a5/ragas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:41.000000 ragas-0.0.1a5/ragas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-14 18:32:55.000000 ragas-0.0.1a5/ragas/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.189321 ragas-0.0.1a5/ragas/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-14 18:32:41.000000 ragas-0.0.1a5/ragas/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-14 18:32:41.000000 ragas-0.0.1a5/ragas/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-05-14 18:32:41.000000 ragas-0.0.1a5/ragas/metrics/factual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-14 18:32:41.000000 ragas-0.0.1a5/ragas/metrics/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-14 18:32:41.000000 ragas-0.0.1a5/ragas/metrics/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-14 18:32:41.000000 ragas-0.0.1a5/ragas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.189321 ragas-0.0.1a5/ragas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-14 18:32:55.000000 ragas-0.0.1a5/ragas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-14 18:32:55.000000 ragas-0.0.1a5/ragas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:32:55.000000 ragas-0.0.1a5/ragas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-14 18:32:55.000000 ragas-0.0.1a5/ragas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 18:32:55.000000 ragas-0.0.1a5/ragas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.189321 ragas-0.0.1a5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-14 18:32:41.000000 ragas-0.0.1a5/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 18:32:41.000000 ragas-0.0.1a5/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 18:32:55.189321 ragas-0.0.1a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.189321 ragas-0.0.1a5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.189321 ragas-0.0.1a5/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-14 18:32:41.000000 ragas-0.0.1a5/tests/benchmarks/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-14 18:32:41.000000 ragas-0.0.1a5/tests/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:32:55.189321 ragas-0.0.1a5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-14 18:32:41.000000 ragas-0.0.1a5/tests/unit/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.857377 ragas-0.0.1a6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.849377 ragas-0.0.1a6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.853377 ragas-0.0.1a6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-14 19:24:02.000000 ragas-0.0.1a6/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-14 19:24:02.000000 ragas-0.0.1a6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-14 19:24:02.000000 ragas-0.0.1a6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 19:24:02.000000 ragas-0.0.1a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-14 19:24:02.000000 ragas-0.0.1a6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-14 19:24:19.857377 ragas-0.0.1a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-14 19:24:02.000000 ragas-0.0.1a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.853377 ragas-0.0.1a6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.853377 ragas-0.0.1a6/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-05-14 19:24:02.000000 ragas-0.0.1a6/docs/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.853377 ragas-0.0.1a6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 19:24:02.000000 ragas-0.0.1a6/examples/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25111 2023-05-14 19:24:02.000000 ragas-0.0.1a6/examples/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-14 19:24:02.000000 ragas-0.0.1a6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.853377 ragas-0.0.1a6/ragas/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-14 19:24:19.000000 ragas-0.0.1a6/ragas/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.857377 ragas-0.0.1a6/ragas/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/metrics/factual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/metrics/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/metrics/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.857377 ragas-0.0.1a6/ragas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-14 19:24:19.000000 ragas-0.0.1a6/ragas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-14 19:24:19.000000 ragas-0.0.1a6/ragas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 19:24:19.000000 ragas-0.0.1a6/ragas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-14 19:24:19.000000 ragas-0.0.1a6/ragas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 19:24:19.000000 ragas-0.0.1a6/ragas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.857377 ragas-0.0.1a6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-14 19:24:02.000000 ragas-0.0.1a6/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 19:24:02.000000 ragas-0.0.1a6/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 19:24:19.857377 ragas-0.0.1a6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.853377 ragas-0.0.1a6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.857377 ragas-0.0.1a6/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-14 19:24:02.000000 ragas-0.0.1a6/tests/benchmarks/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-14 19:24:02.000000 ragas-0.0.1a6/tests/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.857377 ragas-0.0.1a6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-14 19:24:02.000000 ragas-0.0.1a6/tests/unit/test_simple.py
```

### Comparing `ragas-0.0.1a5/.github/workflows/ci.yaml` & `ragas-0.0.1a6/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a5/.github/workflows/python-publish.yml` & `ragas-0.0.1a6/.github/workflows/python-publish.yml`

 * *Files 17% similar despite different names*

```diff
@@ -17,22 +17,25 @@
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     environment: pypi-release
     steps:
     - uses: actions/checkout@v3
+      with:
+        fetch-depth: 0
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install build
+        pip install --upgrade setuptools
+        pip install --upgrade build
     - name: Build package
       run: python -m build
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `ragas-0.0.1a5/.gitignore` & `ragas-0.0.1a6/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -154,10 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
-belar/_version.py
-**/tmp.ipynb
 ragas/_version.py
```

### Comparing `ragas-0.0.1a5/LICENSE` & `ragas-0.0.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a5/Makefile` & `ragas-0.0.1a6/Makefile`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a5/PKG-INFO` & `ragas-0.0.1a6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.0.1a5
+Version: 0.0.1a6
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.1a5 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.0.1a6 Description-Content-Type:
 text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
        SOTA metrics for evaluating Retrieval Augmented Generation (RAG)
         [GitHub_release] [Build] [License] [Open_In_Colab] [Downloads]
               *** Installation | Quick_Example | Hugging_Face ***
 ## What
```

### Comparing `ragas-0.0.1a5/README.md` & `ragas-0.0.1a6/README.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a5/docs/assets/logo.png` & `ragas-0.0.1a6/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a5/examples/data_prep.py` & `ragas-0.0.1a6/examples/data_prep.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a5/examples/quickstart.ipynb` & `ragas-0.0.1a6/examples/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a5/ragas/metrics/base.py` & `ragas-0.0.1a6/ragas/metrics/base.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a5/ragas/metrics/factual.py` & `ragas-0.0.1a6/ragas/metrics/factual.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     ):
         self.nlp = spacy.load(SPACY_MODEL)
         self.qa = QAGQ.from_pretrained(self.qa_model_name)
         self.qg = QAGQ.from_pretrained(self.qg_model_name)
 
     @property
     def name(self):
-        return "Q^2"
+        return "Qsquare"
 
     @property
     def is_batchable(self):
         return True
 
     def generate_candidates(self, text: str):
         text = text.strip()
@@ -336,9 +336,9 @@
                 json.dump(gnd_qans, file, indent=4)
 
         scores = [[dic["score"] for dic in item] for item in gnd_qans.values()]
         scores = [sum(sublist) / (len(sublist) + EPS) for sublist in scores]
         return scores
 
 
-ENTScore = EntailmentScore()
-Q2Score = Qsquare()
+entailment_score = EntailmentScore()
+q_square = Qsquare()
```

### Comparing `ragas-0.0.1a5/ragas/metrics/similarity.py` & `ragas-0.0.1a6/ragas/metrics/similarity.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 from sentence_transformers import SentenceTransformer
 
 from ragas.metrics.base import Metric
 
 if t.TYPE_CHECKING:
     from torch import Tensor
 
-SBERT_METRIC = t.Literal["cosine", "euclidean"]
+BERT_METRIC = t.Literal["cosine", "euclidean"]
 
 
 @dataclass
-class SBERTScore(Metric):
-    similarity_metric: t.Literal[SBERT_METRIC] = "cosine"
+class BERTScore(Metric):
+    similarity_metric: t.Literal[BERT_METRIC] = "cosine"
     model_path: str = "all-MiniLM-L6-v2"
     batch_size: int = 1000
 
     def __post_init__(self):
         self.model = SentenceTransformer(self.model_path)
 
     @property
     def name(
         self,
     ):
-        return f"SBERT_{self.similarity_metric}"
+        return f"BERTScore_{self.similarity_metric}"
 
     @property
     def is_batchable(self):
         return True
 
     def score(
         self,
@@ -60,8 +60,8 @@
 
         else:
             raise ValueError(f"Unkown metrics {self.similarity_metric}")
 
         return score
 
 
-__all__ = ["SBERTScore"]
+bert_score = BERTScore()
```

### Comparing `ragas-0.0.1a5/ragas/metrics/simple.py` & `ragas-0.0.1a6/ragas/metrics/simple.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,13 +87,13 @@
             score = [ratio(s1, s2) for s1, s2 in zip(ground_truth, generated_text)]
         else:
             raise ValueError(f"Unkown measure {self.measure}")
 
         return score
 
 
-Rouge1 = ROUGE("rouge1")
-Rouge2 = ROUGE("rouge2")
-RougeL = ROUGE("rougeL")
-BLUE = BLEUScore()
-EditDistance = EditScore("distance")
-EditRatio = EditScore("ratio")
+rouge1 = ROUGE("rouge1")
+rouge2 = ROUGE("rouge2")
+rougeL = ROUGE("rougeL")
+bleu_score = BLEUScore()
+edit_distance = EditScore("distance")
+edit_ratio = EditScore("ratio")
```

### Comparing `ragas-0.0.1a5/ragas/utils.py` & `ragas-0.0.1a6/ragas/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a5/ragas.egg-info/PKG-INFO` & `ragas-0.0.1a6/ragas.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.0.1a5
+Version: 0.0.1a6
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.1a5 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.0.1a6 Description-Content-Type:
 text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
        SOTA metrics for evaluating Retrieval Augmented Generation (RAG)
         [GitHub_release] [Build] [License] [Open_In_Colab] [Downloads]
               *** Installation | Quick_Example | Hugging_Face ***
 ## What
```

### Comparing `ragas-0.0.1a5/ragas.egg-info/SOURCES.txt` & `ragas-0.0.1a6/ragas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a5/tests/benchmarks/benchmark.py` & `ragas-0.0.1a6/tests/benchmarks/benchmark.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 import typing as t
 
-from datasets import Dataset, load_dataset
+from datasets import Dataset, arrow_dataset, load_dataset
 from torch.cuda import is_available
 from tqdm import tqdm
 from utils import print_table, timeit
 
-from ragas.metrics import (
-    EditDistance,
-    EditRatio,
-    EntailmentScore,
-    Evaluation,
-    Rouge1,
-    Rouge2,
-    RougeL,
-    SBERTScore,
-)
+from ragas.metrics import Evaluation, edit_distance, edit_ratio, rouge1, rouge2, rougeL
 
 DEVICE = "cuda" if is_available() else "cpu"
 BATCHES = [0, 1]
-# init metrics
-sbert_score = SBERTScore(similarity_metric="cosine")
-entail = EntailmentScore(max_length=512, device=DEVICE)
+
 METRICS = {
-    "Rouge1": Rouge1,
-    "Rouge2": Rouge2,
-    "RougeL": RougeL,
-    "EditRatio": EditRatio,
-    "EditDistance": EditDistance,
+    "Rouge1": rouge1,
+    "Rouge2": rouge2,
+    "RougeL": rougeL,
+    "EditRatio": edit_ratio,
+    "EditDistance": edit_distance,
     # "SBERTScore": sbert_score,
     # "EntailmentScore": entail,
 }
 DS = load_dataset("explodinggradients/eli5-test", split="test_eli5")
+assert isinstance(DS, arrow_dataset.Dataset), "Not an arrow_dataset"
+DS = DS.select(range(100))
 
 
 def setup() -> t.Iterator[tuple[str, Evaluation, Dataset]]:
     metrics = [m for m in METRICS.values()]
     for b in BATCHES:
         setup_name = f"batch-{b}"
         assert isinstance(DS, Dataset), f"{type(DS)} found in the place of Dataset!"
```

### Comparing `ragas-0.0.1a5/tests/benchmarks/utils.py` & `ragas-0.0.1a6/tests/benchmarks/utils.py`

 * *Files identical despite different names*

