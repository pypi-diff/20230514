# Comparing `tmp/jupyter_glances_proxy-0.0.1.tar.gz` & `tmp/jupyter_glances_proxy-0.0.2.tar.gz`

## Comparing `jupyter_glances_proxy-0.0.1.tar` & `jupyter_glances_proxy-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.1/.editorconfig
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.1/jupyter_glances_proxy/__init__.py
--rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.1/jupyter_glances_proxy/glances.svg
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.1/jupyter_glances_proxy/jupyter_config.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.1/LICENSE.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.1/README.md
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.2/.editorconfig
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.2/jupyter_glances_proxy/__init__.py
+-rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.2/jupyter_glances_proxy/glances.svg
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.2/jupyter_glances_proxy/jupyter_config.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.2/README.md
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 jupyter_glances_proxy-0.0.2/PKG-INFO
```

### Comparing `jupyter_glances_proxy-0.0.1/jupyter_glances_proxy/__init__.py` & `jupyter_glances_proxy-0.0.2/jupyter_glances_proxy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,11 +75,11 @@
             "--enable-plugin=cpu,core,mem,memswap,load,now,processcount,processlist,system,uptime,cloud,fs,folders,ip,network",
         ],
         "timeout": 100,
         "environment": _get_env,
         "absolute_url": False,
         # "rewrite_response": rewrite_netloc,
         "launcher_entry": {
-            "title": "glances",
+            "title": "Glances",
             "icon_path": icon_path
         },
     }
```

### Comparing `jupyter_glances_proxy-0.0.1/jupyter_glances_proxy/glances.svg` & `jupyter_glances_proxy-0.0.2/jupyter_glances_proxy/glances.svg`

 * *Files identical despite different names*

### Comparing `jupyter_glances_proxy-0.0.1/.gitignore` & `jupyter_glances_proxy-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_glances_proxy-0.0.1/LICENSE.md` & `jupyter_glances_proxy-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jupyter_glances_proxy-0.0.1/pyproject.toml` & `jupyter_glances_proxy-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter-glances-proxy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Matus Kosut", email="matus.kosut@ntnu.no" },
   { name="Diepiriye Okujagu", email="diepirio@ntnu.no" },
 ]
 description = "Jupyter server proxy for glances"
 readme = "README.md"
 license = { file = "LICENSE.md" }
```

### Comparing `jupyter_glances_proxy-0.0.1/PKG-INFO` & `jupyter_glances_proxy-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-glances-proxy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Jupyter server proxy for glances
 Project-URL: Homepage, https://github.com/huntdatacenter/jupyter-glances-proxy
 Author-email: Matus Kosut <matus.kosut@ntnu.no>, Diepiriye Okujagu <diepirio@ntnu.no>
 License: MIT License
         
         Copyright (c) 2023 HUNT Cloud
         
@@ -44,14 +44,16 @@
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: ruamel-yaml; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # jupyter-glances-proxy
 
+**[Glances](https://glances.readthedocs.io/): An eye on your system** 
+
 ## Build
 
 ```
 python3 -m pip install hatch
 
 hatch build
```

