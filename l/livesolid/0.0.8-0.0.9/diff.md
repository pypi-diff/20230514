# Comparing `tmp/livesolid-0.0.8.tar.gz` & `tmp/livesolid-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livesolid-0.0.8.tar", last modified: Fri May 12 13:38:17 2023, max compression
+gzip compressed data, was "livesolid-0.0.9.tar", last modified: Fri May 12 21:18:12 2023, max compression
```

## Comparing `livesolid-0.0.8.tar` & `livesolid-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.198697 livesolid-0.0.8/
--rw-r--r--   0 mtm        (501) staff       (20)      592 2023-04-28 13:28:55.000000 livesolid-0.0.8/.coveragerc
--rw-r--r--   0 mtm        (501) staff       (20)      566 2023-04-28 13:28:55.000000 livesolid-0.0.8/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       57 2023-04-28 13:28:55.000000 livesolid-0.0.8/.isort.cfg
--rw-r--r--   0 mtm        (501) staff       (20)     1670 2023-04-28 14:23:15.000000 livesolid-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 mtm        (501) staff       (20)      530 2023-04-28 13:28:55.000000 livesolid-0.0.8/.readthedocs.yml
--rw-r--r--   0 mtm        (501) staff       (20)       87 2023-04-28 13:28:55.000000 livesolid-0.0.8/AUTHORS.rst
--rw-r--r--   0 mtm        (501) staff       (20)      128 2023-04-28 13:28:55.000000 livesolid-0.0.8/CHANGELOG.rst
--rw-r--r--   0 mtm        (501) staff       (20)    13840 2023-04-28 13:28:55.000000 livesolid-0.0.8/CONTRIBUTING.rst
--rw-r--r--   0 mtm        (501) staff       (20)     1083 2023-04-28 13:28:55.000000 livesolid-0.0.8/LICENSE.txt
--rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-05-12 13:38:17.198942 livesolid-0.0.8/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)     2084 2023-04-28 13:28:55.000000 livesolid-0.0.8/README.rst
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.185542 livesolid-0.0.8/docs/
--rw-r--r--   0 mtm        (501) staff       (20)     1154 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/Makefile
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.186579 livesolid-0.0.8/docs/_static/
--rw-r--r--   0 mtm        (501) staff       (20)       18 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/_static/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       41 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/authors.rst
--rw-r--r--   0 mtm        (501) staff       (20)       43 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/changelog.rst
--rw-r--r--   0 mtm        (501) staff       (20)     9742 2023-04-28 13:36:58.000000 livesolid-0.0.8/docs/conf.py
--rw-r--r--   0 mtm        (501) staff       (20)       33 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/contributing.rst
--rw-r--r--   0 mtm        (501) staff       (20)     2321 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/index.rst
--rw-r--r--   0 mtm        (501) staff       (20)       67 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/license.rst
--rw-r--r--   0 mtm        (501) staff       (20)       39 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/readme.rst
--rw-r--r--   0 mtm        (501) staff       (20)      233 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/requirements.txt
--rw-r--r--   0 mtm        (501) staff       (20)      346 2023-04-28 13:28:55.000000 livesolid-0.0.8/pyproject.toml
--rw-r--r--   0 mtm        (501) staff       (20)     1253 2023-05-12 13:38:17.200198 livesolid-0.0.8/setup.cfg
--rw-r--r--   0 mtm        (501) staff       (20)      704 2023-04-28 13:28:55.000000 livesolid-0.0.8/setup.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.168704 livesolid-0.0.8/src/
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.191314 livesolid-0.0.8/src/livesolid/
--rw-r--r--   0 mtm        (501) staff       (20)      577 2023-04-28 13:28:55.000000 livesolid-0.0.8/src/livesolid/__init__.py
--rw-r--r--   0 mtm        (501) staff       (20)      779 2023-04-28 14:23:22.000000 livesolid-0.0.8/src/livesolid/lib.py
--rw-r--r--   0 mtm        (501) staff       (20)     2881 2023-04-28 14:28:31.000000 livesolid-0.0.8/src/livesolid/main.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.197016 livesolid-0.0.8/src/livesolid/templates/
--rw-r--r--   0 mtm        (501) staff       (20)      735 2023-05-12 13:36:34.000000 livesolid-0.0.8/src/livesolid/templates/Makefile.j2
--rw-r--r--   0 mtm        (501) staff       (20)     1184 2023-04-28 14:17:25.000000 livesolid-0.0.8/src/livesolid/templates/goreleaser.yaml.j2
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.195719 livesolid-0.0.8/src/livesolid.egg-info/
--rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-05-12 13:38:17.000000 livesolid-0.0.8/src/livesolid.egg-info/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)      810 2023-05-12 13:38:17.000000 livesolid-0.0.8/src/livesolid.egg-info/SOURCES.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-12 13:38:17.000000 livesolid-0.0.8/src/livesolid.egg-info/dependency_links.txt
--rw-r--r--   0 mtm        (501) staff       (20)       49 2023-05-12 13:38:17.000000 livesolid-0.0.8/src/livesolid.egg-info/entry_points.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-12 13:38:16.000000 livesolid-0.0.8/src/livesolid.egg-info/not-zip-safe
--rw-r--r--   0 mtm        (501) staff       (20)       93 2023-05-12 13:38:17.000000 livesolid-0.0.8/src/livesolid.egg-info/requires.txt
--rw-r--r--   0 mtm        (501) staff       (20)       10 2023-05-12 13:38:17.000000 livesolid-0.0.8/src/livesolid.egg-info/top_level.txt
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.198091 livesolid-0.0.8/tests/
--rw-r--r--   0 mtm        (501) staff       (20)      277 2023-04-28 13:28:55.000000 livesolid-0.0.8/tests/conftest.py
--rw-r--r--   0 mtm        (501) staff       (20)      594 2023-04-28 13:28:55.000000 livesolid-0.0.8/tests/test_skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)     2851 2023-04-28 13:28:55.000000 livesolid-0.0.8/tox.ini
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 21:18:12.606520 livesolid-0.0.9/
+-rw-r--r--   0 mtm        (501) staff       (20)      592 2023-04-28 13:28:55.000000 livesolid-0.0.9/.coveragerc
+-rw-r--r--   0 mtm        (501) staff       (20)      566 2023-04-28 13:28:55.000000 livesolid-0.0.9/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       57 2023-04-28 13:28:55.000000 livesolid-0.0.9/.isort.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)     1670 2023-04-28 14:23:15.000000 livesolid-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 mtm        (501) staff       (20)      530 2023-04-28 13:28:55.000000 livesolid-0.0.9/.readthedocs.yml
+-rw-r--r--   0 mtm        (501) staff       (20)       87 2023-04-28 13:28:55.000000 livesolid-0.0.9/AUTHORS.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      128 2023-04-28 13:28:55.000000 livesolid-0.0.9/CHANGELOG.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    13840 2023-04-28 13:28:55.000000 livesolid-0.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     1083 2023-04-28 13:28:55.000000 livesolid-0.0.9/LICENSE.txt
+-rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-05-12 21:18:12.606747 livesolid-0.0.9/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)     2084 2023-04-28 13:28:55.000000 livesolid-0.0.9/README.rst
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 21:18:12.597585 livesolid-0.0.9/docs/
+-rw-r--r--   0 mtm        (501) staff       (20)     1154 2023-04-28 13:28:55.000000 livesolid-0.0.9/docs/Makefile
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 21:18:12.598065 livesolid-0.0.9/docs/_static/
+-rw-r--r--   0 mtm        (501) staff       (20)       18 2023-04-28 13:28:55.000000 livesolid-0.0.9/docs/_static/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       41 2023-04-28 13:28:55.000000 livesolid-0.0.9/docs/authors.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       43 2023-04-28 13:28:55.000000 livesolid-0.0.9/docs/changelog.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     9742 2023-04-28 13:36:58.000000 livesolid-0.0.9/docs/conf.py
+-rw-r--r--   0 mtm        (501) staff       (20)       33 2023-04-28 13:28:55.000000 livesolid-0.0.9/docs/contributing.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     2321 2023-04-28 13:28:55.000000 livesolid-0.0.9/docs/index.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       67 2023-04-28 13:28:55.000000 livesolid-0.0.9/docs/license.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       39 2023-04-28 13:28:55.000000 livesolid-0.0.9/docs/readme.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      233 2023-04-28 13:28:55.000000 livesolid-0.0.9/docs/requirements.txt
+-rw-r--r--   0 mtm        (501) staff       (20)      346 2023-04-28 13:28:55.000000 livesolid-0.0.9/pyproject.toml
+-rw-r--r--   0 mtm        (501) staff       (20)     1253 2023-05-12 21:18:12.608255 livesolid-0.0.9/setup.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)      704 2023-04-28 13:28:55.000000 livesolid-0.0.9/setup.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 21:18:12.583503 livesolid-0.0.9/src/
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 21:18:12.599624 livesolid-0.0.9/src/livesolid/
+-rw-r--r--   0 mtm        (501) staff       (20)      577 2023-04-28 13:28:55.000000 livesolid-0.0.9/src/livesolid/__init__.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1691 2023-05-12 21:16:29.000000 livesolid-0.0.9/src/livesolid/lib.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2893 2023-05-12 21:04:18.000000 livesolid-0.0.9/src/livesolid/main.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 21:18:12.604601 livesolid-0.0.9/src/livesolid/templates/
+-rw-r--r--   0 mtm        (501) staff       (20)      420 2023-05-12 14:09:29.000000 livesolid-0.0.9/src/livesolid/templates/Makefile.j2
+-rw-r--r--   0 mtm        (501) staff       (20)      820 2023-05-12 21:11:15.000000 livesolid-0.0.9/src/livesolid/templates/github_ci.yml
+-rw-r--r--   0 mtm        (501) staff       (20)      567 2023-05-12 21:10:54.000000 livesolid-0.0.9/src/livesolid/templates/github_release.yml
+-rw-r--r--   0 mtm        (501) staff       (20)     1184 2023-04-28 14:17:25.000000 livesolid-0.0.9/src/livesolid/templates/goreleaser.yaml.j2
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 21:18:12.602803 livesolid-0.0.9/src/livesolid.egg-info/
+-rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-05-12 21:18:12.000000 livesolid-0.0.9/src/livesolid.egg-info/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)      891 2023-05-12 21:18:12.000000 livesolid-0.0.9/src/livesolid.egg-info/SOURCES.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-12 21:18:12.000000 livesolid-0.0.9/src/livesolid.egg-info/dependency_links.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       49 2023-05-12 21:18:12.000000 livesolid-0.0.9/src/livesolid.egg-info/entry_points.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-12 21:18:12.000000 livesolid-0.0.9/src/livesolid.egg-info/not-zip-safe
+-rw-r--r--   0 mtm        (501) staff       (20)       93 2023-05-12 21:18:12.000000 livesolid-0.0.9/src/livesolid.egg-info/requires.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       10 2023-05-12 21:18:12.000000 livesolid-0.0.9/src/livesolid.egg-info/top_level.txt
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 21:18:12.606040 livesolid-0.0.9/tests/
+-rw-r--r--   0 mtm        (501) staff       (20)      277 2023-04-28 13:28:55.000000 livesolid-0.0.9/tests/conftest.py
+-rw-r--r--   0 mtm        (501) staff       (20)      594 2023-04-28 13:28:55.000000 livesolid-0.0.9/tests/test_skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2851 2023-04-28 13:28:55.000000 livesolid-0.0.9/tox.ini
```

### Comparing `livesolid-0.0.8/.coveragerc` & `livesolid-0.0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/.gitignore` & `livesolid-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/.pre-commit-config.yaml` & `livesolid-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/.readthedocs.yml` & `livesolid-0.0.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/CONTRIBUTING.rst` & `livesolid-0.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/LICENSE.txt` & `livesolid-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/PKG-INFO` & `livesolid-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livesolid
-Version: 0.0.8
+Version: 0.0.9
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `livesolid-0.0.8/README.rst` & `livesolid-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/docs/Makefile` & `livesolid-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/docs/conf.py` & `livesolid-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/docs/index.rst` & `livesolid-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/setup.cfg` & `livesolid-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/setup.py` & `livesolid-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/src/livesolid/__init__.py` & `livesolid-0.0.9/src/livesolid/__init__.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/src/livesolid/main.py` & `livesolid-0.0.9/src/livesolid/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
       args (List[str]): command line parameters as list of strings
           (for example  ``["--verbose", "42"]``).
     """
     args = parse_args(args)
     setup_logging(args.loglevel)
     _logger.debug("Starting crazy calculations...")
     # print(f"The {args.n}-th Fibonacci number is {fib(args.n)}")
-    lib.doit(path=args.path)
+    lib.render_templates(path=args.path)
     _logger.info("Script ends here")
 
 
 def run():
     """Calls :func:`main` passing the CLI arguments extracted from :obj:`sys.argv`
 
     This function can be used as entry point to create console scripts with setuptools.
```

### Comparing `livesolid-0.0.8/src/livesolid/templates/goreleaser.yaml.j2` & `livesolid-0.0.9/src/livesolid/templates/goreleaser.yaml.j2`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/src/livesolid.egg-info/PKG-INFO` & `livesolid-0.0.9/src/livesolid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livesolid
-Version: 0.0.8
+Version: 0.0.9
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `livesolid-0.0.8/src/livesolid.egg-info/SOURCES.txt` & `livesolid-0.0.9/src/livesolid.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,10 +29,12 @@
 src/livesolid.egg-info/SOURCES.txt
 src/livesolid.egg-info/dependency_links.txt
 src/livesolid.egg-info/entry_points.txt
 src/livesolid.egg-info/not-zip-safe
 src/livesolid.egg-info/requires.txt
 src/livesolid.egg-info/top_level.txt
 src/livesolid/templates/Makefile.j2
+src/livesolid/templates/github_ci.yml
+src/livesolid/templates/github_release.yml
 src/livesolid/templates/goreleaser.yaml.j2
 tests/conftest.py
 tests/test_skeleton.py
```

### Comparing `livesolid-0.0.8/tests/test_skeleton.py` & `livesolid-0.0.9/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.8/tox.ini` & `livesolid-0.0.9/tox.ini`

 * *Files identical despite different names*

