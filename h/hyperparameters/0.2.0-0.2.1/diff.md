# Comparing `tmp/hyperparameters-0.2.0.tar.gz` & `tmp/hyperparameters-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperparameters-0.2.0.tar", max compression
+gzip compressed data, was "hyperparameters-0.2.1.tar", max compression
```

## Comparing `hyperparameters-0.2.0.tar` & `hyperparameters-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1081 2023-05-14 10:27:43.299402 hyperparameters-0.2.0/LICENSE
--rw-r--r--   0        0        0     7491 2023-05-14 10:27:43.299402 hyperparameters-0.2.0/README.md
--rw-r--r--   0        0        0      768 2023-05-14 10:27:43.299402 hyperparameters-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       74 2023-05-14 10:27:43.299402 hyperparameters-0.2.0/src/hyperparameters/__init__.py
--rw-r--r--   0        0        0     9343 2023-05-14 10:27:43.299402 hyperparameters-0.2.0/src/hyperparameters/hyperparams.py
--rw-r--r--   0        0        0      849 2023-05-13 17:20:06.420558 hyperparameters-0.2.0/src/hyperparameters/ray_tune_hyperparams.py
--rw-r--r--   0        0        0     8235 1970-01-01 00:00:00.000000 hyperparameters-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-14 10:27:43.299402 hyperparameters-0.2.1/LICENSE
+-rw-r--r--   0        0        0     7491 2023-05-14 10:27:43.299402 hyperparameters-0.2.1/README.md
+-rw-r--r--   0        0        0      768 2023-05-14 16:10:38.643028 hyperparameters-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-05-14 10:27:43.299402 hyperparameters-0.2.1/src/hyperparameters/__init__.py
+-rw-r--r--   0        0        0     9436 2023-05-14 12:39:18.806313 hyperparameters-0.2.1/src/hyperparameters/hyperparams.py
+-rw-r--r--   0        0        0      849 2023-05-13 17:20:06.420558 hyperparameters-0.2.1/src/hyperparameters/ray_tune_hyperparams.py
+-rw-r--r--   0        0        0     8235 1970-01-01 00:00:00.000000 hyperparameters-0.2.1/PKG-INFO
```

### Comparing `hyperparameters-0.2.0/LICENSE` & `hyperparameters-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperparameters-0.2.0/README.md` & `hyperparameters-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameters-0.2.0/pyproject.toml` & `hyperparameters-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Hyperparameters"
-version = "0.2.0"
+version = "0.2.1"
 description = "Define your Hyperparameters once and use in argparse, hypertunning libraries, and as strongly-typed attributes in code!"
 authors = ["Oleh Lokshyn <olokshyn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.urls]
 "Repository" = "https://github.com/olokshyn/Hyperparameters"
```

### Comparing `hyperparameters-0.2.0/src/hyperparameters/hyperparams.py` & `hyperparameters-0.2.1/src/hyperparameters/hyperparams.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     choices: list[Any] | None = None
 
     annotation: Any = None
     type_: Any = None
     required: bool = False
 
     def can_be_none(self) -> bool:
+        if self.annotation is Any:
+            return True
         return getattr(self.annotation, "_name", None) == "Optional"
 
 
 def HP(
     description: str,
     *,
     default: Any = Undefined,
@@ -85,15 +87,15 @@
                 ):
                     raise ValueError(
                         f"Field {field_name} is of type {info.annotation} but has "
                         f"default value '{info.default}' of type {type(info.default)}"
                     )
 
             if info.type_ is bool:
-                if info.choices is not None:
+                if info.choices is not None and info.choices != [False, True]:
                     raise ValueError(
                         f"Field {field_name} is bool and cannot have choices set. "
                         "False and True are the only possible choices."
                     )
                 info.choices = [False, True]
             if info.choices is not None:
                 for choice in info.choices:
```

### Comparing `hyperparameters-0.2.0/src/hyperparameters/ray_tune_hyperparams.py` & `hyperparameters-0.2.1/src/hyperparameters/ray_tune_hyperparams.py`

 * *Files identical despite different names*

### Comparing `hyperparameters-0.2.0/PKG-INFO` & `hyperparameters-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparameters
-Version: 0.2.0
+Version: 0.2.1
 Summary: Define your Hyperparameters once and use in argparse, hypertunning libraries, and as strongly-typed attributes in code!
 License: MIT
 Author: Oleh Lokshyn
 Author-email: olokshyn@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

