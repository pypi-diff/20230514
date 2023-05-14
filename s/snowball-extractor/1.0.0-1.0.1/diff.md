# Comparing `tmp/snowball-extractor-1.0.0.tar.gz` & `tmp/snowball-extractor-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowball-extractor-1.0.0.tar", last modified: Sun May 14 21:00:38 2023, max compression
+gzip compressed data, was "snowball-extractor-1.0.1.tar", last modified: Sun May 14 21:03:08 2023, max compression
```

## Comparing `snowball-extractor-1.0.0.tar` & `snowball-extractor-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:00:38.262312 snowball-extractor-1.0.0/
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:00:38.256172 snowball-extractor-1.0.0/.github/
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:00:38.258989 snowball-extractor-1.0.0/.github/workflows/
--rw-r--r--   0 dsbatista   (501) staff       (20)     1157 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/.github/workflows/code_checks.yml
--rw-r--r--   0 dsbatista   (501) staff       (20)    35141 2023-05-06 23:42:50.000000 snowball-extractor-1.0.0/LICENSE
--rw-r--r--   0 dsbatista   (501) staff       (20)      735 2023-05-14 18:54:28.000000 snowball-extractor-1.0.0/Makefile
--rw-r--r--   0 dsbatista   (501) staff       (20)    10555 2023-05-14 21:00:38.262426 snowball-extractor-1.0.0/PKG-INFO
--rw-r--r--   0 dsbatista   (501) staff       (20)     9846 2023-05-14 20:43:34.000000 snowball-extractor-1.0.0/README.md
--rw-r--r--   0 dsbatista   (501) staff       (20)      115 2023-05-06 23:42:50.000000 snowball-extractor-1.0.0/__init__.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      238 2023-05-07 10:09:46.000000 snowball-extractor-1.0.0/mypy.ini
--rw-r--r--   0 dsbatista   (501) staff       (20)      984 2023-05-14 20:54:14.000000 snowball-extractor-1.0.0/parameters.cfg
--rw-r--r--   0 dsbatista   (501) staff       (20)      413 2023-05-07 10:09:46.000000 snowball-extractor-1.0.0/pylint.cfg
--rw-r--r--   0 dsbatista   (501) staff       (20)      950 2023-05-14 18:48:33.000000 snowball-extractor-1.0.0/pyproject.toml
--rw-r--r--   0 dsbatista   (501) staff       (20)       38 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/requirements.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)      137 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/requirements_dev.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)      569 2023-05-14 21:00:38.262743 snowball-extractor-1.0.0/setup.cfg
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:00:38.260846 snowball-extractor-1.0.0/snowball/
--rwxr-xr-x   0 dsbatista   (501) staff       (20)    14303 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/snowball/bootstrapping.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     2339 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/snowball/cli.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      453 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/snowball/commons.py
--rwxr-xr-x   0 dsbatista   (501) staff       (20)     5919 2023-05-14 20:54:35.000000 snowball-extractor-1.0.0/snowball/config.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     6565 2023-05-14 20:52:58.000000 snowball-extractor-1.0.0/snowball/pattern.py
--rw-r--r--   0 dsbatista   (501) staff       (20)    12002 2023-05-07 10:09:46.000000 snowball-extractor-1.0.0/snowball/reverb_breds.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      526 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/snowball/seed.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     6633 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/snowball/sentence.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     5336 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/snowball/snowball_tuple.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     1271 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/snowball/vector_space_model.py
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:00:38.261490 snowball-extractor-1.0.0/snowball_extractor.egg-info/
--rw-r--r--   0 dsbatista   (501) staff       (20)    10555 2023-05-14 21:00:38.000000 snowball-extractor-1.0.0/snowball_extractor.egg-info/PKG-INFO
--rw-r--r--   0 dsbatista   (501) staff       (20)      732 2023-05-14 21:00:38.000000 snowball-extractor-1.0.0/snowball_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)        1 2023-05-14 21:00:38.000000 snowball-extractor-1.0.0/snowball_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)       47 2023-05-14 21:00:38.000000 snowball-extractor-1.0.0/snowball_extractor.egg-info/entry_points.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)       40 2023-05-14 21:00:38.000000 snowball-extractor-1.0.0/snowball_extractor.egg-info/requires.txt
--rw-r--r--   0 dsbatista   (501) staff       (20)        9 2023-05-14 21:00:38.000000 snowball-extractor-1.0.0/snowball_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:00:38.262154 snowball-extractor-1.0.0/tests/
--rw-r--r--   0 dsbatista   (501) staff       (20)      540 2023-05-07 20:48:01.000000 snowball-extractor-1.0.0/tests/test_commons.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     2496 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/tests/test_pattern.py
--rw-r--r--   0 dsbatista   (501) staff       (20)      458 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/tests/test_seed.py
--rw-r--r--   0 dsbatista   (501) staff       (20)     2088 2023-05-14 16:00:11.000000 snowball-extractor-1.0.0/tests/test_sentence.py
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:03:08.080465 snowball-extractor-1.0.1/
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:03:08.073901 snowball-extractor-1.0.1/.github/
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:03:08.077056 snowball-extractor-1.0.1/.github/workflows/
+-rw-r--r--   0 dsbatista   (501) staff       (20)     1157 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/.github/workflows/code_checks.yml
+-rw-r--r--   0 dsbatista   (501) staff       (20)    35141 2023-05-06 23:42:50.000000 snowball-extractor-1.0.1/LICENSE
+-rw-r--r--   0 dsbatista   (501) staff       (20)      735 2023-05-14 18:54:28.000000 snowball-extractor-1.0.1/Makefile
+-rw-r--r--   0 dsbatista   (501) staff       (20)    10555 2023-05-14 21:03:08.080634 snowball-extractor-1.0.1/PKG-INFO
+-rw-r--r--   0 dsbatista   (501) staff       (20)     9846 2023-05-14 20:43:34.000000 snowball-extractor-1.0.1/README.md
+-rw-r--r--   0 dsbatista   (501) staff       (20)      115 2023-05-06 23:42:50.000000 snowball-extractor-1.0.1/__init__.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      238 2023-05-07 10:09:46.000000 snowball-extractor-1.0.1/mypy.ini
+-rw-r--r--   0 dsbatista   (501) staff       (20)      984 2023-05-14 20:54:14.000000 snowball-extractor-1.0.1/parameters.cfg
+-rw-r--r--   0 dsbatista   (501) staff       (20)      413 2023-05-07 10:09:46.000000 snowball-extractor-1.0.1/pylint.cfg
+-rw-r--r--   0 dsbatista   (501) staff       (20)      950 2023-05-14 21:02:27.000000 snowball-extractor-1.0.1/pyproject.toml
+-rw-r--r--   0 dsbatista   (501) staff       (20)       38 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/requirements.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)      137 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/requirements_dev.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)      569 2023-05-14 21:03:08.081015 snowball-extractor-1.0.1/setup.cfg
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:03:08.078840 snowball-extractor-1.0.1/snowball/
+-rwxr-xr-x   0 dsbatista   (501) staff       (20)    14303 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/bootstrapping.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     2339 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/cli.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      453 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/commons.py
+-rwxr-xr-x   0 dsbatista   (501) staff       (20)     5919 2023-05-14 20:54:35.000000 snowball-extractor-1.0.1/snowball/config.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     6565 2023-05-14 20:52:58.000000 snowball-extractor-1.0.1/snowball/pattern.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)    12002 2023-05-07 10:09:46.000000 snowball-extractor-1.0.1/snowball/reverb_breds.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      526 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/seed.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     6633 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/sentence.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     5336 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/snowball_tuple.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     1271 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/snowball/vector_space_model.py
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:03:08.079493 snowball-extractor-1.0.1/snowball_extractor.egg-info/
+-rw-r--r--   0 dsbatista   (501) staff       (20)    10555 2023-05-14 21:03:08.000000 snowball-extractor-1.0.1/snowball_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 dsbatista   (501) staff       (20)      732 2023-05-14 21:03:08.000000 snowball-extractor-1.0.1/snowball_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)        1 2023-05-14 21:03:08.000000 snowball-extractor-1.0.1/snowball_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)       47 2023-05-14 21:03:08.000000 snowball-extractor-1.0.1/snowball_extractor.egg-info/entry_points.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)       40 2023-05-14 21:03:08.000000 snowball-extractor-1.0.1/snowball_extractor.egg-info/requires.txt
+-rw-r--r--   0 dsbatista   (501) staff       (20)        9 2023-05-14 21:03:08.000000 snowball-extractor-1.0.1/snowball_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 dsbatista   (501) staff       (20)        0 2023-05-14 21:03:08.080109 snowball-extractor-1.0.1/tests/
+-rw-r--r--   0 dsbatista   (501) staff       (20)      540 2023-05-07 20:48:01.000000 snowball-extractor-1.0.1/tests/test_commons.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     2496 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/tests/test_pattern.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)      458 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/tests/test_seed.py
+-rw-r--r--   0 dsbatista   (501) staff       (20)     2088 2023-05-14 16:00:11.000000 snowball-extractor-1.0.1/tests/test_sentence.py
```

### Comparing `snowball-extractor-1.0.0/.github/workflows/code_checks.yml` & `snowball-extractor-1.0.1/.github/workflows/code_checks.yml`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/LICENSE` & `snowball-extractor-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/Makefile` & `snowball-extractor-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/PKG-INFO` & `snowball-extractor-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowball-extractor
-Version: 1.0.0
+Version: 1.0.1
 Summary: Snowball: Extracting Relations from Large Plain-Text Collections
 Author-email: "David S. Batista" <dsbatista@gmail.com>
 License: GNU GPLv3
 Project-URL: homepage, https://github.com/davidsbatista/Snowball
 Project-URL: documentation, https://www.davidsbatista.net/assets/documents/publications/breds-emnlp_15.pdf
 Project-URL: repository, https://github.com/davidsbatista/Snowball
 Keywords: nlp,semantic relationship extraction,bootstrapping,emnlp,tf-idf
```

### Comparing `snowball-extractor-1.0.0/README.md` & `snowball-extractor-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/parameters.cfg` & `snowball-extractor-1.0.1/parameters.cfg`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/pyproject.toml` & `snowball-extractor-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snowball-extractor"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{name = "David S. Batista", email = "dsbatista@gmail.com"}]
 description = "Snowball: Extracting Relations from Large Plain-Text Collections"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["nlp", "semantic relationship extraction", "bootstrapping", "emnlp",
     "tf-idf", ]
 license = {text = "GNU GPLv3"}
```

### Comparing `snowball-extractor-1.0.0/setup.cfg` & `snowball-extractor-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/snowball/bootstrapping.py` & `snowball-extractor-1.0.1/snowball/bootstrapping.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/snowball/cli.py` & `snowball-extractor-1.0.1/snowball/cli.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/snowball/config.py` & `snowball-extractor-1.0.1/snowball/config.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/snowball/pattern.py` & `snowball-extractor-1.0.1/snowball/pattern.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/snowball/reverb_breds.py` & `snowball-extractor-1.0.1/snowball/reverb_breds.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/snowball/seed.py` & `snowball-extractor-1.0.1/snowball/seed.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/snowball/sentence.py` & `snowball-extractor-1.0.1/snowball/sentence.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/snowball/snowball_tuple.py` & `snowball-extractor-1.0.1/snowball/snowball_tuple.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/snowball/vector_space_model.py` & `snowball-extractor-1.0.1/snowball/vector_space_model.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/snowball_extractor.egg-info/PKG-INFO` & `snowball-extractor-1.0.1/snowball_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowball-extractor
-Version: 1.0.0
+Version: 1.0.1
 Summary: Snowball: Extracting Relations from Large Plain-Text Collections
 Author-email: "David S. Batista" <dsbatista@gmail.com>
 License: GNU GPLv3
 Project-URL: homepage, https://github.com/davidsbatista/Snowball
 Project-URL: documentation, https://www.davidsbatista.net/assets/documents/publications/breds-emnlp_15.pdf
 Project-URL: repository, https://github.com/davidsbatista/Snowball
 Keywords: nlp,semantic relationship extraction,bootstrapping,emnlp,tf-idf
```

### Comparing `snowball-extractor-1.0.0/snowball_extractor.egg-info/SOURCES.txt` & `snowball-extractor-1.0.1/snowball_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/tests/test_commons.py` & `snowball-extractor-1.0.1/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/tests/test_pattern.py` & `snowball-extractor-1.0.1/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `snowball-extractor-1.0.0/tests/test_sentence.py` & `snowball-extractor-1.0.1/tests/test_sentence.py`

 * *Files identical despite different names*

