# Comparing `tmp/accurating-0.4.7.tar.gz` & `tmp/accurating-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurating-0.4.7.tar", max compression
+gzip compressed data, was "accurating-0.4.8.tar", max compression
```

## Comparing `accurating-0.4.7.tar` & `accurating-0.4.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.7/LICENSE
--rw-r--r--   0        0        0     6245 2023-04-23 19:14:57.625128 accurating-0.4.7/README.md
--rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.7/accurating/__init__.py
--rw-r--r--   0        0        0     8441 2023-04-26 06:45:07.226315 accurating-0.4.7/accurating/model.py
--rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.7/accurating/tests/__init__.py
--rw-r--r--   0        0        0     3135 2023-04-26 06:46:15.146580 accurating-0.4.7/accurating/tests/model_test.py
--rw-r--r--   0        0        0      632 2023-04-26 06:47:02.358765 accurating-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     6853 1970-01-01 00:00:00.000000 accurating-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.8/LICENSE
+-rw-r--r--   0        0        0     6369 2023-05-14 19:51:52.513579 accurating-0.4.8/README.md
+-rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.8/accurating/__init__.py
+-rw-r--r--   0        0        0     8420 2023-05-14 19:49:50.236990 accurating-0.4.8/accurating/model.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.8/accurating/tests/__init__.py
+-rw-r--r--   0        0        0     3135 2023-05-14 19:49:25.928871 accurating-0.4.8/accurating/tests/model_test.py
+-rw-r--r--   0        0        0      648 2023-05-14 19:52:44.021823 accurating-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     6977 1970-01-01 00:00:00.000000 accurating-0.4.8/PKG-INFO
```

### Comparing `accurating-0.4.7/LICENSE` & `accurating-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `accurating-0.4.7/README.md` & `accurating-0.4.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -124,11 +124,14 @@
 
 ## Development
 
 ```shell
 git clone https://github.com/lukaszlew/accurating
 poetry install
 poetry run pytest
+# TODO(lew): Should automate it somehow.
+poetry run mypy accurating/model.py
+poetry run mypy accurating/tests/model_test.py
 # edit stuff; increase version
 poetry build
 poetry publish
 ```
```

### Comparing `accurating-0.4.7/accurating/model.py` & `accurating-0.4.8/accurating/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     """It is automatically adjusted, but sometimes it is too large and blows up."""
 
 
 @dataclasses.dataclass
 class Model:
     """Trained model."""
 
-    rating: dict[tuple[str, int], float]
+    rating: dict[str, dict[int, float]]
     """Player rating, indexed by name and season"""
 
 
 def fit(
     data: MatchResultArrays,
     config: Config,
 ) -> Model:
@@ -146,15 +146,15 @@
         # winner_win_prob_log += p1_win_probs * log_win_prob_diff(diff/jnp.exp(p1_cons)) + p2_win_probs * log_win_prob_diff(-diff/jnp.exp(p1_cons))
         # winner_win_prob_log += p1_win_probs * log_win_prob_diff(diff/jnp.exp(p2_cons)) + p2_win_probs * log_win_prob_diff(-diff/jnp.exp(p2_cons))
         # winner_win_prob_log /= 2
         # return jnp.mean(winner_win_prob_log) - 0.005*jnp.mean(cons ** 2)
 
     # Optimize for these params:
     rating = jnp.zeros([player_count, season_count], dtype=jnp.float64)
-    params = dataclasses.asdict(Model(rating=rating))
+    params = { 'rating': rating }
     # 'consistency': jnp.zeros([player_count, season_count]),
 
     # Momentum gradient descent with restarts
     m_lr = 1.0
     lr = float(config.initial_lr)
     momentum = tree_map(jnp.zeros_like, params)
     last_params = params
```

### Comparing `accurating-0.4.7/accurating/tests/model_test.py` & `accurating-0.4.8/accurating/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `accurating-0.4.7/pyproject.toml` & `accurating-0.4.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "AccuRating"
-version = "0.4.7"
+version = "0.4.8"
 description = "AccuRating is a library for accurate player ranking based on match results."
 authors = ["Lukasz Lew <lukasz.lew@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/lukaszlew/accurating"
 documentation = "https://lukaszlew.github.io/accurating/"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 jax = "^0.4.8"
 jaxlib = "^0.4.7"
 
 [tool.poetry.group.dev.dependencies]
 pdoc = "^13.1.0"
 pytest = "^6.2.5"
+mypy = "^1.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = [
```

### Comparing `accurating-0.4.7/PKG-INFO` & `accurating-0.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accurating
-Version: 0.4.7
+Version: 0.4.8
 Summary: AccuRating is a library for accurate player ranking based on match results.
 Home-page: https://github.com/lukaszlew/accurating
 Author: Lukasz Lew
 Author-email: lukasz.lew@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -140,12 +140,15 @@
 
 ## Development
 
 ```shell
 git clone https://github.com/lukaszlew/accurating
 poetry install
 poetry run pytest
+# TODO(lew): Should automate it somehow.
+poetry run mypy accurating/model.py
+poetry run mypy accurating/tests/model_test.py
 # edit stuff; increase version
 poetry build
 poetry publish
 ```
```

