# Comparing `tmp/snowball-extractor-1.0.1.tar.gz` & `tmp/snowball-extractor-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowball-extractor-1.0.1.tar", last modified: Sun May 14 21:03:08 2023, max compression
+gzip compressed data, was "snowball-extractor-1.0.2.tar", last modified: Sun May 14 21:22:19 2023, max compression
```

## Comparing `snowball-extractor-1.0.1.tar` & `snowball-extractor-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:03:08.080465 snowball-extractor-1.0.1/
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:03:08.073901 snowball-extractor-1.0.1/.github/
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:03:08.077056 snowball-extractor-1.0.1/.github/workflows/
--rw-r--r--   0 dsbatista   (501) staff       (20)     1157 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/.github/workflows/code_checks.yml
--rw-r--r--   0 dsbatista   (501) staff       (20)    35141 2023-05-06 23:42:50.000000 snowball-extractor-1.0.1/LICENSE
--rw-r--r--   0 dsbatista   (501) staff       (20)      735 2023-05-14 18:54:28.000000 snowball-extractor-1.0.1/Makefile
--rw-r--r--   0 dsbatista   (501) staff       (20)    10555 2023-05-14 21:03:08.080634 snowball-extractor-1.0.1/PKG-INFO
--rw-r--r--   0 dsbatista   (501) staff       (20)     9846 2023-05-14 20:43:34.000000 snowball-extractor-1.0.1/README.md
--rw-r--r--   0 dsbatista   (501) staff       (20)      115 2023-05-06 23:42:50.000000 snowball-extractor-1.0.1/__init__.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      238 2023-05-07 10:09:46.000000 snowball-extractor-1.0.1/mypy.ini
--rw-r--r--   0 dsbatista   (501) staff       (20)      984 2023-05-14 20:54:14.000000 snowball-extractor-1.0.1/parameters.cfg
--rw-r--r--   0 dsbatista   (501) staff       (20)      413 2023-05-07 10:09:46.000000 snowball-extractor-1.0.1/pylint.cfg
--rw-r--r--   0 dsbatista   (501) staff       (20)      950 2023-05-14 21:02:27.000000 snowball-extractor-1.0.1/pyproject.toml
--rw-r--r--   0 dsbatista   (501) staff       (20)       38 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/requirements.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)      137 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/requirements_dev.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)      569 2023-05-14 21:03:08.081015 snowball-extractor-1.0.1/setup.cfg
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:03:08.078840 snowball-extractor-1.0.1/snowball/
--rwxr-xr-x   0 dsbatista   (501) staff       (20)    14303 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/bootstrapping.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     2339 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/cli.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      453 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/commons.py
--rwxr-xr-x   0 dsbatista   (501) staff       (20)     5919 2023-05-14 20:54:35.000000 snowball-extractor-1.0.1/snowball/config.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     6565 2023-05-14 20:52:58.000000 snowball-extractor-1.0.1/snowball/pattern.py
--rw-r--r--   0 dsbatista   (501) staff       (20)    12002 2023-05-07 10:09:46.000000 snowball-extractor-1.0.1/snowball/reverb_breds.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      526 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/seed.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     6633 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/sentence.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     5336 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/snowball_tuple.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     1271 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/vector_space_model.py
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:03:08.079493 snowball-extractor-1.0.1/snowball_extractor.egg-info/
--rw-r--r--   0 dsbatista   (501) staff       (20)    10555 2023-05-14 21:03:08.000000 snowball-extractor-1.0.1/snowball_extractor.egg-info/PKG-INFO
--rw-r--r--   0 dsbatista   (501) staff       (20)      732 2023-05-14 21:03:08.000000 snowball-extractor-1.0.1/snowball_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)        1 2023-05-14 21:03:08.000000 snowball-extractor-1.0.1/snowball_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)       47 2023-05-14 21:03:08.000000 snowball-extractor-1.0.1/snowball_extractor.egg-info/entry_points.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)       40 2023-05-14 21:03:08.000000 snowball-extractor-1.0.1/snowball_extractor.egg-info/requires.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)        9 2023-05-14 21:03:08.000000 snowball-extractor-1.0.1/snowball_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:03:08.080109 snowball-extractor-1.0.1/tests/
--rw-r--r--   0 dsbatista   (501) staff       (20)      540 2023-05-07 20:48:01.000000 snowball-extractor-1.0.1/tests/test_commons.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     2496 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/tests/test_pattern.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      458 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/tests/test_seed.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     2088 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/tests/test_sentence.py
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:22:19.409209 snowball-extractor-1.0.2/
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:22:19.401305 snowball-extractor-1.0.2/.github/
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:22:19.404693 snowball-extractor-1.0.2/.github/workflows/
+-rw-r--r--   0 dsbatista   (501) staff       (20)     1157 2023-05-14 16:00:11.000000 snowball-extractor-1.0.2/.github/workflows/code_checks.yml
+-rw-r--r--   0 dsbatista   (501) staff       (20)    35141 2023-05-06 23:42:50.000000 snowball-extractor-1.0.2/LICENSE
+-rw-r--r--   0 dsbatista   (501) staff       (20)      747 2023-05-14 21:22:11.000000 snowball-extractor-1.0.2/Makefile
+-rw-r--r--   0 dsbatista   (501) staff       (20)    10555 2023-05-14 21:22:19.409335 snowball-extractor-1.0.2/PKG-INFO
+-rw-r--r--   0 dsbatista   (501) staff       (20)     9846 2023-05-14 20:43:34.000000 snowball-extractor-1.0.2/README.md
+-rw-r--r--   0 dsbatista   (501) staff       (20)      115 2023-05-06 23:42:50.000000 snowball-extractor-1.0.2/__init__.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      238 2023-05-07 10:09:46.000000 snowball-extractor-1.0.2/mypy.ini
+-rw-r--r--   0 dsbatista   (501) staff       (20)      984 2023-05-14 20:54:14.000000 snowball-extractor-1.0.2/parameters.cfg
+-rw-r--r--   0 dsbatista   (501) staff       (20)      413 2023-05-07 10:09:46.000000 snowball-extractor-1.0.2/pylint.cfg
+-rw-r--r--   0 dsbatista   (501) staff       (20)      950 2023-05-14 21:21:18.000000 snowball-extractor-1.0.2/pyproject.toml
+-rw-r--r--   0 dsbatista   (501) staff       (20)       38 2023-05-14 16:00:11.000000 snowball-extractor-1.0.2/requirements.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)      137 2023-05-14 16:00:11.000000 snowball-extractor-1.0.2/requirements_dev.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)      569 2023-05-14 21:22:19.409807 snowball-extractor-1.0.2/setup.cfg
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:22:19.407063 snowball-extractor-1.0.2/snowball/
+-rwxr-xr-x   0 dsbatista   (501) staff       (20)    14414 2023-05-14 21:12:18.000000 snowball-extractor-1.0.2/snowball/bootstrapping.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     2357 2023-05-14 21:11:44.000000 snowball-extractor-1.0.2/snowball/cli.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      453 2023-05-14 16:00:11.000000 snowball-extractor-1.0.2/snowball/commons.py
+-rwxr-xr-x   0 dsbatista   (501) staff       (20)     6045 2023-05-14 21:21:03.000000 snowball-extractor-1.0.2/snowball/config.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     6565 2023-05-14 20:52:58.000000 snowball-extractor-1.0.2/snowball/pattern.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)    12002 2023-05-07 10:09:46.000000 snowball-extractor-1.0.2/snowball/reverb_breds.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      526 2023-05-14 16:00:11.000000 snowball-extractor-1.0.2/snowball/seed.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     6633 2023-05-14 16:00:11.000000 snowball-extractor-1.0.2/snowball/sentence.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     5336 2023-05-14 16:00:11.000000 snowball-extractor-1.0.2/snowball/snowball_tuple.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     1271 2023-05-14 16:00:11.000000 snowball-extractor-1.0.2/snowball/vector_space_model.py
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:22:19.408184 snowball-extractor-1.0.2/snowball_extractor.egg-info/
+-rw-r--r--   0 dsbatista   (501) staff       (20)    10555 2023-05-14 21:22:19.000000 snowball-extractor-1.0.2/snowball_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 dsbatista   (501) staff       (20)      732 2023-05-14 21:22:19.000000 snowball-extractor-1.0.2/snowball_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)        1 2023-05-14 21:22:19.000000 snowball-extractor-1.0.2/snowball_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)       47 2023-05-14 21:22:19.000000 snowball-extractor-1.0.2/snowball_extractor.egg-info/entry_points.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)       40 2023-05-14 21:22:19.000000 snowball-extractor-1.0.2/snowball_extractor.egg-info/requires.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)        9 2023-05-14 21:22:19.000000 snowball-extractor-1.0.2/snowball_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:22:19.408993 snowball-extractor-1.0.2/tests/
+-rw-r--r--   0 dsbatista   (501) staff       (20)      540 2023-05-07 20:48:01.000000 snowball-extractor-1.0.2/tests/test_commons.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     2496 2023-05-14 16:00:11.000000 snowball-extractor-1.0.2/tests/test_pattern.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      458 2023-05-14 16:00:11.000000 snowball-extractor-1.0.2/tests/test_seed.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     2088 2023-05-14 16:00:11.000000 snowball-extractor-1.0.2/tests/test_sentence.py
```

### Comparing `snowball-extractor-1.0.1/.github/workflows/code_checks.yml` & `snowball-extractor-1.0.2/.github/workflows/code_checks.yml`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/LICENSE` & `snowball-extractor-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/Makefile` & `snowball-extractor-1.0.2/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 clean:
 	rm -rf build dist *.egg-info .coverage .pytest_cache .mypy_cache .pytest_cache src/*.egg-info
 
 
 publish:
+	make clean
 	python -m pip install --upgrade build
 	python -m build
 	python -m pip install --upgrade twine
 	python -m twine upload --repository testpypi dist/*
 
 
 all:
```

### Comparing `snowball-extractor-1.0.1/PKG-INFO` & `snowball-extractor-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowball-extractor
-Version: 1.0.1
+Version: 1.0.2
 Summary: Snowball: Extracting Relations from Large Plain-Text Collections
 Author-email: "David S. Batista" <dsbatista@gmail.com>
 License: GNU GPLv3
 Project-URL: homepage, https://github.com/davidsbatista/Snowball
 Project-URL: documentation, https://www.davidsbatista.net/assets/documents/publications/breds-emnlp_15.pdf
 Project-URL: repository, https://github.com/davidsbatista/Snowball
 Keywords: nlp,semantic relationship extraction,bootstrapping,emnlp,tf-idf
```

### Comparing `snowball-extractor-1.0.1/README.md` & `snowball-extractor-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/parameters.cfg` & `snowball-extractor-1.0.2/parameters.cfg`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/pyproject.toml` & `snowball-extractor-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snowball-extractor"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{name = "David S. Batista", email = "dsbatista@gmail.com"}]
 description = "Snowball: Extracting Relations from Large Plain-Text Collections"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["nlp", "semantic relationship extraction", "bootstrapping", "emnlp",
     "tf-idf", ]
 license = {text = "GNU GPLv3"}
```

### Comparing `snowball-extractor-1.0.1/setup.cfg` & `snowball-extractor-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/snowball/bootstrapping.py` & `snowball-extractor-1.0.2/snowball/bootstrapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,17 @@
         negative_seeds: str,
         sentences_file: str,
         similarity: float,
         confidence: float,
         n_iterations: int,
     ):
         # pylint: disable=too-many-arguments
+
+        print(config_file, seeds_file, negative_seeds, sentences_file, similarity, confidence, n_iterations)
+
         self.current_iteration: int = 0
         self.patterns: List[Pattern] = []
         self.processed_tuples: List[SnowballTuple] = []
         self.candidate_tuples: Dict[SnowballTuple, List[Tuple[Pattern, float]]] = defaultdict(list)
         self.config = Config(
             config_file, seeds_file, negative_seeds, sentences_file, similarity, confidence, n_iterations
         )
```

### Comparing `snowball-extractor-1.0.1/snowball/cli.py` & `snowball-extractor-1.0.2/snowball/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 
 def main() -> None:  # pylint: disable=missing-function-docstring
     parser = create_args()
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
     args = parser.parse_args()
+
+    print(args)
+
     snowball = Snowball(
         args.config,
         args.positive_seeds,
         args.negative_seeds,
         args.sentences,
         args.similarity,
         args.confidence,
```

### Comparing `snowball-extractor-1.0.1/snowball/config.py` & `snowball-extractor-1.0.2/snowball/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
         positive_seeds: str,
         negative_seeds: str,
         sentences_file: str,
         similarity: float,
         confidence: float,
         n_iterations: int,
     ) -> None:  # noqa: C901
+
+        print(config_file, positive_seeds, negative_seeds, sentences_file, similarity, confidence, n_iterations)
+
         # pylint: disable=too-many-arguments, too-many-statements
         if config_file is None:
             self.context_window_size: int = 2
             self.min_tokens_away: int = 1
             self.max_tokens_away: int = 6
             self.similarity: float = 0.6
             self.alpha: float = 0.0
@@ -51,16 +54,16 @@
         self.e2_type: str
         self.stopwords: Set[str] = set(stopwords.words("english"))
         self.threshold_similarity: float = similarity
         self.instance_confidence: float = confidence
         self.reverb: "Reverb" = Reverb()
         self.number_iterations = n_iterations
         self.read_seeds(positive_seeds, self.positive_seeds)
-        self.read_seeds(negative_seeds, self.negative_seeds)
-        fileinput.close()
+        if negative_seeds:
+            self.read_seeds(negative_seeds, self.negative_seed_tuples)
 
         print("\nConfiguration parameters")
         print("========================")
         print("e1 type              :", self.e1_type)
         print("e2 type              :", self.e2_type)
         print("context window       :", self.context_window_size)
         print("max tokens away      :", self.max_tokens_away)
```

### Comparing `snowball-extractor-1.0.1/snowball/pattern.py` & `snowball-extractor-1.0.2/snowball/pattern.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/snowball/reverb_breds.py` & `snowball-extractor-1.0.2/snowball/reverb_breds.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/snowball/seed.py` & `snowball-extractor-1.0.2/snowball/seed.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/snowball/sentence.py` & `snowball-extractor-1.0.2/snowball/sentence.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/snowball/snowball_tuple.py` & `snowball-extractor-1.0.2/snowball/snowball_tuple.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/snowball/vector_space_model.py` & `snowball-extractor-1.0.2/snowball/vector_space_model.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/snowball_extractor.egg-info/PKG-INFO` & `snowball-extractor-1.0.2/snowball_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowball-extractor
-Version: 1.0.1
+Version: 1.0.2
 Summary: Snowball: Extracting Relations from Large Plain-Text Collections
 Author-email: "David S. Batista" <dsbatista@gmail.com>
 License: GNU GPLv3
 Project-URL: homepage, https://github.com/davidsbatista/Snowball
 Project-URL: documentation, https://www.davidsbatista.net/assets/documents/publications/breds-emnlp_15.pdf
 Project-URL: repository, https://github.com/davidsbatista/Snowball
 Keywords: nlp,semantic relationship extraction,bootstrapping,emnlp,tf-idf
```

### Comparing `snowball-extractor-1.0.1/snowball_extractor.egg-info/SOURCES.txt` & `snowball-extractor-1.0.2/snowball_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/tests/test_commons.py` & `snowball-extractor-1.0.2/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/tests/test_pattern.py` & `snowball-extractor-1.0.2/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.1/tests/test_sentence.py` & `snowball-extractor-1.0.2/tests/test_sentence.py`

 * *Files identical despite different names*

