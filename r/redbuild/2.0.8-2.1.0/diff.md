# Comparing `tmp/redbuild-2.0.8.tar.gz` & `tmp/redbuild-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbuild-2.0.8.tar", max compression
+gzip compressed data, was "redbuild-2.1.0.tar", max compression
```

## Comparing `redbuild-2.0.8.tar` & `redbuild-2.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.0.8/LICENSE
--rw-r--r--   0        0        0     2475 2023-04-17 07:13:34.753986 redbuild-2.0.8/README.md
--rw-r--r--   0        0        0      604 2023-05-05 00:03:01.111520 redbuild-2.0.8/pyproject.toml
--rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.0.8/redbuild/__init__.py
--rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.0.8/redbuild/__main__.py
--rw-r--r--   0        0        0    10678 2023-04-17 01:56:34.767608 redbuild-2.0.8/redbuild/cli.py
--rw-r--r--   0        0        0     1445 2023-04-17 01:41:29.902707 redbuild-2.0.8/redbuild/composer.py
--rw-r--r--   0        0        0      856 2023-05-05 00:02:51.112733 redbuild-2.0.8/redbuild/engine.py
--rw-r--r--   0        0        0      366 2023-04-17 01:15:37.329254 redbuild-2.0.8/redbuild/res.py
--rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.0.8/redbuild/util.py
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 redbuild-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2475 2023-04-17 07:13:34.753986 redbuild-2.1.0/README.md
+-rw-r--r--   0        0        0      604 2023-05-14 19:14:01.131832 redbuild-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.1.0/redbuild/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.1.0/redbuild/__main__.py
+-rw-r--r--   0        0        0    11357 2023-05-14 19:21:28.039901 redbuild-2.1.0/redbuild/cli.py
+-rw-r--r--   0        0        0     1445 2023-04-17 01:41:29.902707 redbuild-2.1.0/redbuild/composer.py
+-rw-r--r--   0        0        0      856 2023-05-05 00:02:51.112733 redbuild-2.1.0/redbuild/engine.py
+-rw-r--r--   0        0        0      366 2023-04-17 01:15:37.329254 redbuild-2.1.0/redbuild/res.py
+-rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.1.0/redbuild/util.py
+-rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 redbuild-2.1.0/PKG-INFO
```

### Comparing `redbuild-2.0.8/LICENSE` & `redbuild-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.8/README.md` & `redbuild-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.8/pyproject.toml` & `redbuild-2.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redbuild"
-version = "2.0.8"
+version = "2.1.0"
 description = "magic containerized builds"
 authors = ["redthing1 <redthing1@alt.icu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 typer = {extras = ["rich"], version = "^0.7.0"}
```

### Comparing `redbuild-2.0.8/redbuild/cli.py` & `redbuild-2.1.0/redbuild/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,14 +132,20 @@
     ),
     build_args=typer.Option(
         "",
         "--build-args",
         "-B",
         help="Additional arguments to pass to build script",
     ),
+    cache_mounts: List[str] = typer.Option(
+        [],
+        "--cache-mounts",
+        "-k",
+        help="Volume mount directories to use for caching",
+    ),
 ):
     # 0. get container engine
     ctr_engine = get_container_engine_command(detect_container_engine())
 
     # 1. get name for builder image
     builder_image_name = get_builder_image_name(cwd)
 
@@ -154,21 +160,34 @@
             f"Build script [{buildscript_path}] not found. Create it or pass a specific path with -s."
         )
         raise typer.Exit(1)
     # $CONTAINER_ENGINE run --rm -it -v $(pwd):/prj $CRUN_ARGS $BUILDER_TAG /bin/bash -l -c "cd /prj && $BUILDSCRIPT $ARGS" | sed 's/^/  /'
     print(
         f"Running build in [{builder_image_name}] with buildscript [{buildscript}] in context [{cwd}]:"
     )
+
+    cache_volume_mount_args = []
+    for cache_mount in cache_mounts:
+        cache_mount_source, cache_mount_target = cache_mount.split(":")
+        # cache_volume_mount_args.extend(["-v", f"{cache_mount}"])
+        # create source directory if it doesn't exist
+        os.makedirs(cache_mount_source, exist_ok=True)
+        cache_volume_mount_args.extend(
+            ["-v", f"{cache_mount_source}:{cache_mount_target}{VOLUME_OPTS}"]
+        )
+
     run_cmd_args = [
         "run",
         # podman run args
         "--rm",
         # "-it",
+        # mount project directory
         "-v",
         f"{cwd}:/prj{VOLUME_OPTS}",
+        *cache_volume_mount_args,
         *parse_secondary_args(crun_args),
     ]
     run_cmd = ctr_engine.bake(
         *run_cmd_args,
         # _fg=True,
         # output formatting
         _out=lambda line: print(f"  {line}", end=""),
```

### Comparing `redbuild-2.0.8/redbuild/composer.py` & `redbuild-2.1.0/redbuild/composer.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.8/redbuild/engine.py` & `redbuild-2.1.0/redbuild/engine.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.8/redbuild/util.py` & `redbuild-2.1.0/redbuild/util.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.8/PKG-INFO` & `redbuild-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbuild
-Version: 2.0.8
+Version: 2.1.0
 Summary: magic containerized builds
 Author: redthing1
 Author-email: redthing1@alt.icu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

