# Comparing `tmp/redbuild-2.1.0.tar.gz` & `tmp/redbuild-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbuild-2.1.0.tar", max compression
+gzip compressed data, was "redbuild-2.1.1.tar", max compression
```

## Comparing `redbuild-2.1.0.tar` & `redbuild-2.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.1.0/LICENSE
--rw-r--r--   0        0        0     2475 2023-04-17 07:13:34.753986 redbuild-2.1.0/README.md
--rw-r--r--   0        0        0      604 2023-05-14 19:14:01.131832 redbuild-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.1.0/redbuild/__init__.py
--rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.1.0/redbuild/__main__.py
--rw-r--r--   0        0        0    11357 2023-05-14 19:21:28.039901 redbuild-2.1.0/redbuild/cli.py
--rw-r--r--   0        0        0     1445 2023-04-17 01:41:29.902707 redbuild-2.1.0/redbuild/composer.py
--rw-r--r--   0        0        0      856 2023-05-05 00:02:51.112733 redbuild-2.1.0/redbuild/engine.py
--rw-r--r--   0        0        0      366 2023-04-17 01:15:37.329254 redbuild-2.1.0/redbuild/res.py
--rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.1.0/redbuild/util.py
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 redbuild-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2475 2023-04-17 07:13:34.753986 redbuild-2.1.1/README.md
+-rw-r--r--   0        0        0      604 2023-05-14 19:29:53.086874 redbuild-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.1.1/redbuild/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.1.1/redbuild/__main__.py
+-rw-r--r--   0        0        0    11456 2023-05-14 19:30:28.813537 redbuild-2.1.1/redbuild/cli.py
+-rw-r--r--   0        0        0     1445 2023-04-17 01:41:29.902707 redbuild-2.1.1/redbuild/composer.py
+-rw-r--r--   0        0        0      856 2023-05-05 00:02:51.112733 redbuild-2.1.1/redbuild/engine.py
+-rw-r--r--   0        0        0      366 2023-04-17 01:15:37.329254 redbuild-2.1.1/redbuild/res.py
+-rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.1.1/redbuild/util.py
+-rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 redbuild-2.1.1/PKG-INFO
```

### Comparing `redbuild-2.1.0/LICENSE` & `redbuild-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redbuild-2.1.0/README.md` & `redbuild-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `redbuild-2.1.0/pyproject.toml` & `redbuild-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redbuild"
-version = "2.1.0"
+version = "2.1.1"
 description = "magic containerized builds"
 authors = ["redthing1 <redthing1@alt.icu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 typer = {extras = ["rich"], version = "^0.7.0"}
```

### Comparing `redbuild-2.1.0/redbuild/cli.py` & `redbuild-2.1.1/redbuild/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,21 @@
     ContainerEngine,
     detect_container_engine,
     get_container_engine_command,
 )
 from .util import get_builder_image_name, parse_secondary_args
 from .composer import BuildEnv, compose_dockerfile, DEFAULT_BUILDENV
 
+CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 APP_NAME = "redbuild"
 app = typer.Typer(
     name=APP_NAME,
     help=f"{APP_NAME}: a tool for easy magic containerized builds",
     no_args_is_help=True,
+    context_settings=CONTEXT_SETTINGS,
 )
 
 DEFAULT_DOCKERFILE = (
     "build.docker"  # filename of default dockerfile for build environment
 )
 VOLUME_OPTS = ":z"  # bind mount volume options
```

### Comparing `redbuild-2.1.0/redbuild/composer.py` & `redbuild-2.1.1/redbuild/composer.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.1.0/redbuild/engine.py` & `redbuild-2.1.1/redbuild/engine.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.1.0/redbuild/util.py` & `redbuild-2.1.1/redbuild/util.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.1.0/PKG-INFO` & `redbuild-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbuild
-Version: 2.1.0
+Version: 2.1.1
 Summary: magic containerized builds
 Author: redthing1
 Author-email: redthing1@alt.icu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

