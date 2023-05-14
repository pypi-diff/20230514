# Comparing `tmp/snowball-extractor-1.0.3.tar.gz` & `tmp/snowball-extractor-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowball-extractor-1.0.3.tar", last modified: Sun May 14 21:28:28 2023, max compression
+gzip compressed data, was "snowball-extractor-1.0.5.tar", last modified: Sun May 14 21:48:57 2023, max compression
```

## Comparing `snowball-extractor-1.0.3.tar` & `snowball-extractor-1.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:28:28.226702 snowball-extractor-1.0.3/
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:28:28.220561 snowball-extractor-1.0.3/.github/
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:28:28.223384 snowball-extractor-1.0.3/.github/workflows/
--rw-r--r--   0 dsbatista   (501) staff       (20)     1157 2023-05-14 16:00:11.000000 snowball-extractor-1.0.3/.github/workflows/code_checks.yml
--rw-r--r--   0 dsbatista   (501) staff       (20)    35141 2023-05-06 23:42:50.000000 snowball-extractor-1.0.3/LICENSE
--rw-r--r--   0 dsbatista   (501) staff       (20)      747 2023-05-14 21:22:11.000000 snowball-extractor-1.0.3/Makefile
--rw-r--r--   0 dsbatista   (501) staff       (20)    10555 2023-05-14 21:28:28.226839 snowball-extractor-1.0.3/PKG-INFO
--rw-r--r--   0 dsbatista   (501) staff       (20)     9846 2023-05-14 20:43:34.000000 snowball-extractor-1.0.3/README.md
--rw-r--r--   0 dsbatista   (501) staff       (20)      115 2023-05-06 23:42:50.000000 snowball-extractor-1.0.3/__init__.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      238 2023-05-07 10:09:46.000000 snowball-extractor-1.0.3/mypy.ini
--rw-r--r--   0 dsbatista   (501) staff       (20)      984 2023-05-14 20:54:14.000000 snowball-extractor-1.0.3/parameters.cfg
--rw-r--r--   0 dsbatista   (501) staff       (20)      413 2023-05-07 10:09:46.000000 snowball-extractor-1.0.3/pylint.cfg
--rw-r--r--   0 dsbatista   (501) staff       (20)      950 2023-05-14 21:25:39.000000 snowball-extractor-1.0.3/pyproject.toml
--rw-r--r--   0 dsbatista   (501) staff       (20)       38 2023-05-14 16:00:11.000000 snowball-extractor-1.0.3/requirements.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)      137 2023-05-14 16:00:11.000000 snowball-extractor-1.0.3/requirements_dev.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)      569 2023-05-14 21:28:28.227166 snowball-extractor-1.0.3/setup.cfg
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:28:28.225372 snowball-extractor-1.0.3/snowball/
--rwxr-xr-x   0 dsbatista   (501) staff       (20)    14303 2023-05-14 21:25:13.000000 snowball-extractor-1.0.3/snowball/bootstrapping.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     2339 2023-05-14 21:24:22.000000 snowball-extractor-1.0.3/snowball/cli.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      453 2023-05-14 16:00:11.000000 snowball-extractor-1.0.3/snowball/commons.py
--rwxr-xr-x   0 dsbatista   (501) staff       (20)     5930 2023-05-14 21:24:27.000000 snowball-extractor-1.0.3/snowball/config.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     6565 2023-05-14 20:52:58.000000 snowball-extractor-1.0.3/snowball/pattern.py
--rw-r--r--   0 dsbatista   (501) staff       (20)    12002 2023-05-07 10:09:46.000000 snowball-extractor-1.0.3/snowball/reverb_breds.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      526 2023-05-14 16:00:11.000000 snowball-extractor-1.0.3/snowball/seed.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     6633 2023-05-14 16:00:11.000000 snowball-extractor-1.0.3/snowball/sentence.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     5336 2023-05-14 16:00:11.000000 snowball-extractor-1.0.3/snowball/snowball_tuple.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     1271 2023-05-14 16:00:11.000000 snowball-extractor-1.0.3/snowball/vector_space_model.py
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:28:28.226015 snowball-extractor-1.0.3/snowball_extractor.egg-info/
--rw-r--r--   0 dsbatista   (501) staff       (20)    10555 2023-05-14 21:28:28.000000 snowball-extractor-1.0.3/snowball_extractor.egg-info/PKG-INFO
--rw-r--r--   0 dsbatista   (501) staff       (20)      732 2023-05-14 21:28:28.000000 snowball-extractor-1.0.3/snowball_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)        1 2023-05-14 21:28:28.000000 snowball-extractor-1.0.3/snowball_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)       47 2023-05-14 21:28:28.000000 snowball-extractor-1.0.3/snowball_extractor.egg-info/entry_points.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)       40 2023-05-14 21:28:28.000000 snowball-extractor-1.0.3/snowball_extractor.egg-info/requires.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)        9 2023-05-14 21:28:28.000000 snowball-extractor-1.0.3/snowball_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:28:28.226597 snowball-extractor-1.0.3/tests/
--rw-r--r--   0 dsbatista   (501) staff       (20)      540 2023-05-07 20:48:01.000000 snowball-extractor-1.0.3/tests/test_commons.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     2496 2023-05-14 16:00:11.000000 snowball-extractor-1.0.3/tests/test_pattern.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      458 2023-05-14 16:00:11.000000 snowball-extractor-1.0.3/tests/test_seed.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     2088 2023-05-14 16:00:11.000000 snowball-extractor-1.0.3/tests/test_sentence.py
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:48:57.786650 snowball-extractor-1.0.5/
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:48:57.780141 snowball-extractor-1.0.5/.github/
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:48:57.783047 snowball-extractor-1.0.5/.github/workflows/
+-rw-r--r--   0 dsbatista   (501) staff       (20)     1157 2023-05-14 16:00:11.000000 snowball-extractor-1.0.5/.github/workflows/code_checks.yml
+-rw-r--r--   0 dsbatista   (501) staff       (20)    35141 2023-05-06 23:42:50.000000 snowball-extractor-1.0.5/LICENSE
+-rw-r--r--   0 dsbatista   (501) staff       (20)      747 2023-05-14 21:22:11.000000 snowball-extractor-1.0.5/Makefile
+-rw-r--r--   0 dsbatista   (501) staff       (20)    10539 2023-05-14 21:48:57.786775 snowball-extractor-1.0.5/PKG-INFO
+-rw-r--r--   0 dsbatista   (501) staff       (20)     9830 2023-05-14 21:44:04.000000 snowball-extractor-1.0.5/README.md
+-rw-r--r--   0 dsbatista   (501) staff       (20)      115 2023-05-06 23:42:50.000000 snowball-extractor-1.0.5/__init__.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      238 2023-05-07 10:09:46.000000 snowball-extractor-1.0.5/mypy.ini
+-rw-r--r--   0 dsbatista   (501) staff       (20)      984 2023-05-14 20:54:14.000000 snowball-extractor-1.0.5/parameters.cfg
+-rw-r--r--   0 dsbatista   (501) staff       (20)      413 2023-05-07 10:09:46.000000 snowball-extractor-1.0.5/pylint.cfg
+-rw-r--r--   0 dsbatista   (501) staff       (20)      950 2023-05-14 21:47:54.000000 snowball-extractor-1.0.5/pyproject.toml
+-rw-r--r--   0 dsbatista   (501) staff       (20)       38 2023-05-14 16:00:11.000000 snowball-extractor-1.0.5/requirements.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)      137 2023-05-14 16:00:11.000000 snowball-extractor-1.0.5/requirements_dev.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)      569 2023-05-14 21:48:57.787137 snowball-extractor-1.0.5/setup.cfg
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:48:57.785275 snowball-extractor-1.0.5/snowball/
+-rwxr-xr-x   0 dsbatista   (501) staff       (20)    13792 2023-05-14 21:47:43.000000 snowball-extractor-1.0.5/snowball/bootstrapping.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     2339 2023-05-14 21:24:22.000000 snowball-extractor-1.0.5/snowball/cli.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      453 2023-05-14 16:00:11.000000 snowball-extractor-1.0.5/snowball/commons.py
+-rwxr-xr-x   0 dsbatista   (501) staff       (20)     5924 2023-05-14 21:39:16.000000 snowball-extractor-1.0.5/snowball/config.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     6565 2023-05-14 20:52:58.000000 snowball-extractor-1.0.5/snowball/pattern.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)    12002 2023-05-07 10:09:46.000000 snowball-extractor-1.0.5/snowball/reverb_breds.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      526 2023-05-14 16:00:11.000000 snowball-extractor-1.0.5/snowball/seed.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     6633 2023-05-14 16:00:11.000000 snowball-extractor-1.0.5/snowball/sentence.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     5810 2023-05-14 21:48:11.000000 snowball-extractor-1.0.5/snowball/snowball_tuple.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     1271 2023-05-14 16:00:11.000000 snowball-extractor-1.0.5/snowball/vector_space_model.py
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:48:57.785922 snowball-extractor-1.0.5/snowball_extractor.egg-info/
+-rw-r--r--   0 dsbatista   (501) staff       (20)    10539 2023-05-14 21:48:57.000000 snowball-extractor-1.0.5/snowball_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 dsbatista   (501) staff       (20)      732 2023-05-14 21:48:57.000000 snowball-extractor-1.0.5/snowball_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)        1 2023-05-14 21:48:57.000000 snowball-extractor-1.0.5/snowball_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)       47 2023-05-14 21:48:57.000000 snowball-extractor-1.0.5/snowball_extractor.egg-info/entry_points.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)       40 2023-05-14 21:48:57.000000 snowball-extractor-1.0.5/snowball_extractor.egg-info/requires.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)        9 2023-05-14 21:48:57.000000 snowball-extractor-1.0.5/snowball_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:48:57.786542 snowball-extractor-1.0.5/tests/
+-rw-r--r--   0 dsbatista   (501) staff       (20)      540 2023-05-07 20:48:01.000000 snowball-extractor-1.0.5/tests/test_commons.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     2496 2023-05-14 16:00:11.000000 snowball-extractor-1.0.5/tests/test_pattern.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      458 2023-05-14 16:00:11.000000 snowball-extractor-1.0.5/tests/test_seed.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     2088 2023-05-14 16:00:11.000000 snowball-extractor-1.0.5/tests/test_sentence.py
```

### Comparing `snowball-extractor-1.0.3/.github/workflows/code_checks.yml` & `snowball-extractor-1.0.5/.github/workflows/code_checks.yml`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/LICENSE` & `snowball-extractor-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/Makefile` & `snowball-extractor-1.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/PKG-INFO` & `snowball-extractor-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowball-extractor
-Version: 1.0.3
+Version: 1.0.5
 Summary: Snowball: Extracting Relations from Large Plain-Text Collections
 Author-email: "David S. Batista" <dsbatista@gmail.com>
 License: GNU GPLv3
 Project-URL: homepage, https://github.com/davidsbatista/Snowball
 Project-URL: documentation, https://www.davidsbatista.net/assets/documents/publications/breds-emnlp_15.pdf
 Project-URL: repository, https://github.com/davidsbatista/Snowball
 Keywords: nlp,semantic relationship extraction,bootstrapping,emnlp,tf-idf
@@ -35,28 +35,28 @@
 An implementation of Snowball, a relationship extraction system that uses a bootstrapping/semi-supervised approach, it 
 relies on an initial set of seeds, i.e. paris of named-entities representing relationship type to be extracted. 
 
 ## Extracting companies headquarters:
 
 The input text needs to have the named-entities tagged, like show in the example bellow:
  
-```
+```yaml
 The tech company <ORG>Soundcloud</ORG> is based in <LOC>Berlin</LOC>, capital of Germany.
 <ORG>Pfizer</ORG> says it has hired <ORG>Morgan Stanley</ORG> to conduct the review.
 <ORG>Allianz</ORG>, based in <LOC>Munich</LOC>, said net income rose to EUR 1.32 billion.
 <LOC>Switzerland</LOC> and <LOC>South Africa</LOC> are co-chairing the meeting.
 <LOC>Ireland</LOC> beat <LOC>Italy</LOC> , then lost 43-31 to <LOC>France</LOC>.
 <ORG>Pfizer</ORG>, based in <LOC>New York City</LOC> , employs about 90,000 workers.
 <PER>Burton</PER> 's engine passed <ORG>NASCAR</ORG> inspection following the qualifying session.
 ```
 
 We need to give seeds to boostrap the extraction process, specifying the type of each named-entity and relationships 
 examples that should also be present in the input text:
 
-```   
+```yaml
 e1:ORG
 e2:LOC
 
 Lufthansa;Cologne
 Nokia;Espoo
 Google;Mountain View
 DoubleClick;New York
@@ -69,29 +69,29 @@
 ```
 - sentences_short.txt.bz2
 - seeds_positive.txt
 ```
 
 Install Snowball using pip
 
-```
+```sh
 pip install snwoball
 ```
 
 Run the following command:
 
-```
+```sh
 snowball --sentences=sentences_short.txt --positive_seeds=seeds_positive.txt --similarity=0.6 --confidence=0.6
 ```
 
 After the  process is terminated an output file `relationships.jsonl` is generated containing the extracted  relationships. 
 
 You can pretty print it's content to the terminal with: `jq '.' < relationships.jsonl`: 
 
-```
+```json
 {
   "entity_1": "Medtronic",
   "entity_2": "Minneapolis",
   "confidence": 0.9982486865148862,
   "sentence": "<ORG>Medtronic</ORG> , based in <LOC>Minneapolis</LOC> , is the nation 's largest independent medical device maker . ",
   "bef_words": "",
   "bet_words": ", based in",
@@ -122,34 +122,35 @@
 }
 ```
 <br>
 
 Snowball has several parameters to tune the extraction process, in the example above it uses the default values, but 
 these can be set in the configuration file: `parameters.cfg`
 
-    max_tokens_away=6           # maximum number of tokens between the two entities
-    min_tokens_away=1           # minimum number of tokens between the two entities
-    context_window_size=2       # number of tokens to the left and right of each entity
-
-    alpha=0.2                   # weight of the BEF context in the similarity function
-    beta=0.6                    # weight of the BET context in the similarity function
-    gamma=0.2                   # weight of the AFT context in the similarity function
-
-    wUpdt=0.5                   # < 0.5 trusts new examples less on each iteration
-    number_iterations=4         # number of bootstrap iterations
-    wUnk=0.1                    # weight given to unknown extracted relationship instances
-    wNeg=2                      # weight given to extracted relationship instances
-    min_pattern_support=2       # minimum number of instances in a cluster to be considered a pattern
-
+```yaml
+max_tokens_away=6           # maximum number of tokens between the two entities
+min_tokens_away=1           # minimum number of tokens between the two entities
+context_window_size=2       # number of tokens to the left and right of each entity
+
+alpha=0.2                   # weight of the BEF context in the similarity function
+beta=0.6                    # weight of the BET context in the similarity function
+gamma=0.2                   # weight of the AFT context in the similarity function
+
+wUpdt=0.5                   # < 0.5 trusts new examples less on each iteration
+number_iterations=3         # number of bootstrap iterations
+wUnk=0.1                    # weight given to unknown extracted relationship instances
+wNeg=2                      # weight given to extracted relationship instances
+min_pattern_support=2       # minimum number of instances in a cluster to be considered a pattern
+```
 
 and passed with the argument `--config=parameters.cfg`.
 
 The full command line parameters are:
 
-```
+```sh
   -h, --help            show this help message and exit
   --config CONFIG       file with bootstrapping configuration parameters
   --sentences SENTENCES
                         a text file with a sentence per line, and with at least two entities per sentence
   --positive_seeds POSITIVE_SEEDS
                         a text file with a seed per line, in the format, e.g.: 'Nokia;Espoo'
   --negative_seeds NEGATIVE_SEEDS
@@ -199,15 +200,15 @@
 
 
 ## Preparing the development environment
 
 Make sure you have Python3.9 installed on your system
 
 macOs
-```
+```sh
 brew install python@3.9
 python3.9 -m pip install --user --upgrade pip
 python3.9 -m pip install virtualenv
 ```
 
 Clone the repository and prepare the development environment:
```

### Comparing `snowball-extractor-1.0.3/README.md` & `snowball-extractor-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 An implementation of Snowball, a relationship extraction system that uses a bootstrapping/semi-supervised approach, it 
 relies on an initial set of seeds, i.e. paris of named-entities representing relationship type to be extracted. 
 
 ## Extracting companies headquarters:
 
 The input text needs to have the named-entities tagged, like show in the example bellow:
  
-```
+```yaml
 The tech company <ORG>Soundcloud</ORG> is based in <LOC>Berlin</LOC>, capital of Germany.
 <ORG>Pfizer</ORG> says it has hired <ORG>Morgan Stanley</ORG> to conduct the review.
 <ORG>Allianz</ORG>, based in <LOC>Munich</LOC>, said net income rose to EUR 1.32 billion.
 <LOC>Switzerland</LOC> and <LOC>South Africa</LOC> are co-chairing the meeting.
 <LOC>Ireland</LOC> beat <LOC>Italy</LOC> , then lost 43-31 to <LOC>France</LOC>.
 <ORG>Pfizer</ORG>, based in <LOC>New York City</LOC> , employs about 90,000 workers.
 <PER>Burton</PER> 's engine passed <ORG>NASCAR</ORG> inspection following the qualifying session.
 ```
 
 We need to give seeds to boostrap the extraction process, specifying the type of each named-entity and relationships 
 examples that should also be present in the input text:
 
-```   
+```yaml
 e1:ORG
 e2:LOC
 
 Lufthansa;Cologne
 Nokia;Espoo
 Google;Mountain View
 DoubleClick;New York
@@ -53,29 +53,29 @@
 ```
 - sentences_short.txt.bz2
 - seeds_positive.txt
 ```
 
 Install Snowball using pip
 
-```
+```sh
 pip install snwoball
 ```
 
 Run the following command:
 
-```
+```sh
 snowball --sentences=sentences_short.txt --positive_seeds=seeds_positive.txt --similarity=0.6 --confidence=0.6
 ```
 
 After the  process is terminated an output file `relationships.jsonl` is generated containing the extracted  relationships. 
 
 You can pretty print it's content to the terminal with: `jq '.' < relationships.jsonl`: 
 
-```
+```json
 {
   "entity_1": "Medtronic",
   "entity_2": "Minneapolis",
   "confidence": 0.9982486865148862,
   "sentence": "<ORG>Medtronic</ORG> , based in <LOC>Minneapolis</LOC> , is the nation 's largest independent medical device maker . ",
   "bef_words": "",
   "bet_words": ", based in",
@@ -106,34 +106,35 @@
 }
 ```
 <br>
 
 Snowball has several parameters to tune the extraction process, in the example above it uses the default values, but 
 these can be set in the configuration file: `parameters.cfg`
 
-    max_tokens_away=6           # maximum number of tokens between the two entities
-    min_tokens_away=1           # minimum number of tokens between the two entities
-    context_window_size=2       # number of tokens to the left and right of each entity
-
-    alpha=0.2                   # weight of the BEF context in the similarity function
-    beta=0.6                    # weight of the BET context in the similarity function
-    gamma=0.2                   # weight of the AFT context in the similarity function
-
-    wUpdt=0.5                   # < 0.5 trusts new examples less on each iteration
-    number_iterations=4         # number of bootstrap iterations
-    wUnk=0.1                    # weight given to unknown extracted relationship instances
-    wNeg=2                      # weight given to extracted relationship instances
-    min_pattern_support=2       # minimum number of instances in a cluster to be considered a pattern
-
+```yaml
+max_tokens_away=6           # maximum number of tokens between the two entities
+min_tokens_away=1           # minimum number of tokens between the two entities
+context_window_size=2       # number of tokens to the left and right of each entity
+
+alpha=0.2                   # weight of the BEF context in the similarity function
+beta=0.6                    # weight of the BET context in the similarity function
+gamma=0.2                   # weight of the AFT context in the similarity function
+
+wUpdt=0.5                   # < 0.5 trusts new examples less on each iteration
+number_iterations=3         # number of bootstrap iterations
+wUnk=0.1                    # weight given to unknown extracted relationship instances
+wNeg=2                      # weight given to extracted relationship instances
+min_pattern_support=2       # minimum number of instances in a cluster to be considered a pattern
+```
 
 and passed with the argument `--config=parameters.cfg`.
 
 The full command line parameters are:
 
-```
+```sh
   -h, --help            show this help message and exit
   --config CONFIG       file with bootstrapping configuration parameters
   --sentences SENTENCES
                         a text file with a sentence per line, and with at least two entities per sentence
   --positive_seeds POSITIVE_SEEDS
                         a text file with a seed per line, in the format, e.g.: 'Nokia;Espoo'
   --negative_seeds NEGATIVE_SEEDS
@@ -183,15 +184,15 @@
 
 
 ## Preparing the development environment
 
 Make sure you have Python3.9 installed on your system
 
 macOs
-```
+```sh
 brew install python@3.9
 python3.9 -m pip install --user --upgrade pip
 python3.9 -m pip install virtualenv
 ```
 
 Clone the repository and prepare the development environment:
```

### Comparing `snowball-extractor-1.0.3/parameters.cfg` & `snowball-extractor-1.0.5/parameters.cfg`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/pyproject.toml` & `snowball-extractor-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snowball-extractor"
-version = "1.0.3"
+version = "1.0.5"
 authors = [{name = "David S. Batista", email = "dsbatista@gmail.com"}]
 description = "Snowball: Extracting Relations from Large Plain-Text Collections"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["nlp", "semantic relationship extraction", "bootstrapping", "emnlp",
     "tf-idf", ]
 license = {text = "GNU GPLv3"}
```

### Comparing `snowball-extractor-1.0.3/setup.cfg` & `snowball-extractor-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/snowball/bootstrapping.py` & `snowball-extractor-1.0.5/snowball/bootstrapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 __author__ = "David S. Batista"
 __email__ = "dsbatista@gmail.com"
 
+import json
 import operator
 import os
 import pickle
 import sys
 from collections import defaultdict
 from typing import Dict, List, Optional, Tuple
 
@@ -40,26 +41,18 @@
         self.candidate_tuples: Dict[SnowballTuple, List[Tuple[Pattern, float]]] = defaultdict(list)
         self.config = Config(
             config_file, seeds_file, negative_seeds, sentences_file, similarity, confidence, n_iterations
         )
 
     def write_relationships_to_disk(self) -> None:
         """Write extracted relationships to disk"""
-        # ToDo: write this in JSON format
         print("\nWriting extracted relationships to disk")
-        with open("relationships.txt", "wt", encoding="utf8") as f_output:
-            tmp = sorted(self.candidate_tuples, key=lambda out_tpl: out_tpl.confidence, reverse=True)
-            for tpl in tmp:
-                f_output.write("instance: " + tpl.ent1 + "\t" + tpl.ent2 + "\tscore:" + str(tpl.confidence) + "\n")
-                f_output.write("sentence: " + tpl.sentence + "\n")
-                if tpl.passive_voice is False or tpl.passive_voice is None:
-                    f_output.write("passive voice: False\n")
-                elif tpl.passive_voice is True:
-                    f_output.write("passive voice: True\n")
-                f_output.write("\n")
+        with open("relationships.jsonl", "wt", encoding="utf8") as f_out:
+            for tpl in self.candidate_tuples.keys():
+                f_out.write(json.dumps(tpl.to_json()) + "\n")
 
     def debug_patterns(self) -> None:
         """
         Print patterns to stdout
         """
         if PRINT_PATTERNS is True:
             print("\nPatterns:")
```

### Comparing `snowball-extractor-1.0.3/snowball/cli.py` & `snowball-extractor-1.0.5/snowball/cli.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/snowball/config.py` & `snowball-extractor-1.0.5/snowball/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self.stopwords: Set[str] = set(stopwords.words("english"))
         self.threshold_similarity: float = similarity
         self.instance_confidence: float = confidence
         self.reverb: "Reverb" = Reverb()
         self.number_iterations = n_iterations
         self.read_seeds(positive_seeds, self.positive_seeds)
         if negative_seeds:
-            self.read_seeds(negative_seeds, self.negative_seed_tuples)
+            self.read_seeds(negative_seeds, self.negative_seeds)
 
         print("\nConfiguration parameters")
         print("========================")
         print("e1 type              :", self.e1_type)
         print("e2 type              :", self.e2_type)
         print("context window       :", self.context_window_size)
         print("max tokens away      :", self.max_tokens_away)
```

### Comparing `snowball-extractor-1.0.3/snowball/pattern.py` & `snowball-extractor-1.0.5/snowball/pattern.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/snowball/reverb_breds.py` & `snowball-extractor-1.0.5/snowball/reverb_breds.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/snowball/seed.py` & `snowball-extractor-1.0.5/snowball/seed.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/snowball/sentence.py` & `snowball-extractor-1.0.5/snowball/sentence.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/snowball/snowball_tuple.py` & `snowball-extractor-1.0.5/snowball/snowball_tuple.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "David S. Batista"
 __email__ = "dsbatista@gmail.com"
 
-from typing import Any, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 from snowball.reverb_breds import Reverb
 
 
 class SnowballTuple:
     # pylint: disable=too-many-instance-attributes, too-many-arguments
     """
@@ -134,7 +134,22 @@
 
         # extract two words before the first entity, and two words after the second entity
         if len(self.bef_words) > 0:
             self.bef_vector = self.construct_words_vectors(self.bef_words)
 
         if len(self.aft_words) > 0:
             self.aft_vector = self.construct_words_vectors(self.aft_words)
+
+    def to_json(self) -> Dict[str, Any]:
+        """
+        Return a JSON representation of the tuple.
+        """
+        return {
+            "entity_1": self.ent1,
+            "entity_2": self.ent2,
+            "confidence": self.confidence,
+            "sentence": self.sentence,
+            "bef_words": self.bef_words,
+            "bet_words": self.bet_words,
+            "aft_words": self.aft_words,
+            "passive_voice": self.passive_voice,
+        }
```

### Comparing `snowball-extractor-1.0.3/snowball/vector_space_model.py` & `snowball-extractor-1.0.5/snowball/vector_space_model.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/snowball_extractor.egg-info/PKG-INFO` & `snowball-extractor-1.0.5/snowball_extractor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowball-extractor
-Version: 1.0.3
+Version: 1.0.5
 Summary: Snowball: Extracting Relations from Large Plain-Text Collections
 Author-email: "David S. Batista" <dsbatista@gmail.com>
 License: GNU GPLv3
 Project-URL: homepage, https://github.com/davidsbatista/Snowball
 Project-URL: documentation, https://www.davidsbatista.net/assets/documents/publications/breds-emnlp_15.pdf
 Project-URL: repository, https://github.com/davidsbatista/Snowball
 Keywords: nlp,semantic relationship extraction,bootstrapping,emnlp,tf-idf
@@ -35,28 +35,28 @@
 An implementation of Snowball, a relationship extraction system that uses a bootstrapping/semi-supervised approach, it 
 relies on an initial set of seeds, i.e. paris of named-entities representing relationship type to be extracted. 
 
 ## Extracting companies headquarters:
 
 The input text needs to have the named-entities tagged, like show in the example bellow:
  
-```
+```yaml
 The tech company <ORG>Soundcloud</ORG> is based in <LOC>Berlin</LOC>, capital of Germany.
 <ORG>Pfizer</ORG> says it has hired <ORG>Morgan Stanley</ORG> to conduct the review.
 <ORG>Allianz</ORG>, based in <LOC>Munich</LOC>, said net income rose to EUR 1.32 billion.
 <LOC>Switzerland</LOC> and <LOC>South Africa</LOC> are co-chairing the meeting.
 <LOC>Ireland</LOC> beat <LOC>Italy</LOC> , then lost 43-31 to <LOC>France</LOC>.
 <ORG>Pfizer</ORG>, based in <LOC>New York City</LOC> , employs about 90,000 workers.
 <PER>Burton</PER> 's engine passed <ORG>NASCAR</ORG> inspection following the qualifying session.
 ```
 
 We need to give seeds to boostrap the extraction process, specifying the type of each named-entity and relationships 
 examples that should also be present in the input text:
 
-```   
+```yaml
 e1:ORG
 e2:LOC
 
 Lufthansa;Cologne
 Nokia;Espoo
 Google;Mountain View
 DoubleClick;New York
@@ -69,29 +69,29 @@
 ```
 - sentences_short.txt.bz2
 - seeds_positive.txt
 ```
 
 Install Snowball using pip
 
-```
+```sh
 pip install snwoball
 ```
 
 Run the following command:
 
-```
+```sh
 snowball --sentences=sentences_short.txt --positive_seeds=seeds_positive.txt --similarity=0.6 --confidence=0.6
 ```
 
 After the  process is terminated an output file `relationships.jsonl` is generated containing the extracted  relationships. 
 
 You can pretty print it's content to the terminal with: `jq '.' < relationships.jsonl`: 
 
-```
+```json
 {
   "entity_1": "Medtronic",
   "entity_2": "Minneapolis",
   "confidence": 0.9982486865148862,
   "sentence": "<ORG>Medtronic</ORG> , based in <LOC>Minneapolis</LOC> , is the nation 's largest independent medical device maker . ",
   "bef_words": "",
   "bet_words": ", based in",
@@ -122,34 +122,35 @@
 }
 ```
 <br>
 
 Snowball has several parameters to tune the extraction process, in the example above it uses the default values, but 
 these can be set in the configuration file: `parameters.cfg`
 
-    max_tokens_away=6           # maximum number of tokens between the two entities
-    min_tokens_away=1           # minimum number of tokens between the two entities
-    context_window_size=2       # number of tokens to the left and right of each entity
-
-    alpha=0.2                   # weight of the BEF context in the similarity function
-    beta=0.6                    # weight of the BET context in the similarity function
-    gamma=0.2                   # weight of the AFT context in the similarity function
-
-    wUpdt=0.5                   # < 0.5 trusts new examples less on each iteration
-    number_iterations=4         # number of bootstrap iterations
-    wUnk=0.1                    # weight given to unknown extracted relationship instances
-    wNeg=2                      # weight given to extracted relationship instances
-    min_pattern_support=2       # minimum number of instances in a cluster to be considered a pattern
-
+```yaml
+max_tokens_away=6           # maximum number of tokens between the two entities
+min_tokens_away=1           # minimum number of tokens between the two entities
+context_window_size=2       # number of tokens to the left and right of each entity
+
+alpha=0.2                   # weight of the BEF context in the similarity function
+beta=0.6                    # weight of the BET context in the similarity function
+gamma=0.2                   # weight of the AFT context in the similarity function
+
+wUpdt=0.5                   # < 0.5 trusts new examples less on each iteration
+number_iterations=3         # number of bootstrap iterations
+wUnk=0.1                    # weight given to unknown extracted relationship instances
+wNeg=2                      # weight given to extracted relationship instances
+min_pattern_support=2       # minimum number of instances in a cluster to be considered a pattern
+```
 
 and passed with the argument `--config=parameters.cfg`.
 
 The full command line parameters are:
 
-```
+```sh
   -h, --help            show this help message and exit
   --config CONFIG       file with bootstrapping configuration parameters
   --sentences SENTENCES
                         a text file with a sentence per line, and with at least two entities per sentence
   --positive_seeds POSITIVE_SEEDS
                         a text file with a seed per line, in the format, e.g.: 'Nokia;Espoo'
   --negative_seeds NEGATIVE_SEEDS
@@ -199,15 +200,15 @@
 
 
 ## Preparing the development environment
 
 Make sure you have Python3.9 installed on your system
 
 macOs
-```
+```sh
 brew install python@3.9
 python3.9 -m pip install --user --upgrade pip
 python3.9 -m pip install virtualenv
 ```
 
 Clone the repository and prepare the development environment:
```

### Comparing `snowball-extractor-1.0.3/snowball_extractor.egg-info/SOURCES.txt` & `snowball-extractor-1.0.5/snowball_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/tests/test_commons.py` & `snowball-extractor-1.0.5/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/tests/test_pattern.py` & `snowball-extractor-1.0.5/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.3/tests/test_sentence.py` & `snowball-extractor-1.0.5/tests/test_sentence.py`

 * *Files identical despite different names*

