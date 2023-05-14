# Comparing `tmp/hhcm_forest-1.1.8.tar.gz` & `tmp/hhcm_forest-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhcm_forest-1.1.8.tar", last modified: Sat Apr 29 18:30:09 2023, max compression
+gzip compressed data, was "hhcm_forest-1.1.9.tar", last modified: Sun May 14 09:49:08 2023, max compression
```

## Comparing `hhcm_forest-1.1.8.tar` & `hhcm_forest-1.1.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/
--rw-rw-r--   0 root         (0) root         (0)     1073 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      134 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4760 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4238 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/README.md
--rw-rw-r--   0 root         (0) root         (0)      111 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)      787 2023-04-29 18:30:09.081354 hhcm_forest-1.1.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      237 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.073353 hhcm_forest-1.1.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/src/forest/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       54 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/src/forest/cmake_tools/
--rw-rw-r--   0 root         (0) root         (0)     1649 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/cmake_tools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1959 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/cmake_tools/_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/src/forest/cmake_tools/template/
--rw-rw-r--   0 root         (0) root         (0)      101 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/cmake_tools/template/find_package.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/src/forest/common/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8418 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/build_handler.py
--rw-rw-r--   0 root         (0) root         (0)      419 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/config_handler.py
--rw-rw-r--   0 root         (0) root         (0)     4994 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/eval_handler.py
--rw-rw-r--   0 root         (0) root         (0)     7930 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/fetch_handler.py
--rw-rw-r--   0 root         (0) root         (0)      206 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/forest_dirs.py
--rw-rw-r--   0 root         (0) root         (0)     8048 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/install.py
--rw-rw-r--   0 root         (0) root         (0)     3124 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/package.py
--rw-rw-r--   0 root         (0) root         (0)     3921 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/parser.py
--rw-rw-r--   0 root         (0) root         (0)      923 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/print_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4102 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/proc_utils.py
--rw-rw-r--   0 root         (0) root         (0)     5000 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/recipe.py
--rw-rw-r--   0 root         (0) root         (0)      683 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/setup.bash
--rw-rw-r--   0 root         (0) root         (0)     1842 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/common/sudo_refresh.py
--rw-rw-r--   0 root         (0) root         (0)       45 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/forest.bash
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/src/forest/git_tools/
--rw-rw-r--   0 root         (0) root         (0)     2328 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/git_tools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/git_tools/_impl.py
--rwxrwxr-x   0 root         (0) root         (0)     9831 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/src/forest/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4760 2023-04-29 18:30:08.000000 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-04-29 18:30:09.000000 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 18:30:08.000000 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-29 18:30:08.000000 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-29 18:30:08.000000 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-29 18:30:09.000000 hhcm_forest-1.1.8/src/hhcm_forest.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 18:30:09.077353 hhcm_forest-1.1.8/test/
--rw-rw-r--   0 root         (0) root         (0)      703 2023-04-29 18:29:03.000000 hhcm_forest-1.1.8/test/test_run_bash_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:49:08.500666 hhcm_forest-1.1.9/
+-rw-rw-r--   0 root         (0) root         (0)     1073 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      134 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4760 2023-05-14 09:49:08.500666 hhcm_forest-1.1.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4238 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/README.md
+-rw-rw-r--   0 root         (0) root         (0)      111 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)      787 2023-05-14 09:49:08.500666 hhcm_forest-1.1.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      237 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:49:08.496666 hhcm_forest-1.1.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:49:08.500666 hhcm_forest-1.1.9/src/forest/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       54 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:49:08.500666 hhcm_forest-1.1.9/src/forest/cmake_tools/
+-rw-rw-r--   0 root         (0) root         (0)     1649 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/cmake_tools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1959 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/cmake_tools/_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:49:08.500666 hhcm_forest-1.1.9/src/forest/cmake_tools/template/
+-rw-rw-r--   0 root         (0) root         (0)      101 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/cmake_tools/template/find_package.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:49:08.500666 hhcm_forest-1.1.9/src/forest/common/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9344 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/build_handler.py
+-rw-rw-r--   0 root         (0) root         (0)      419 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/config_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     4994 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/eval_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     7930 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/fetch_handler.py
+-rw-rw-r--   0 root         (0) root         (0)      206 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/forest_dirs.py
+-rw-rw-r--   0 root         (0) root         (0)     8415 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/install.py
+-rw-rw-r--   0 root         (0) root         (0)     3124 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/package.py
+-rw-rw-r--   0 root         (0) root         (0)     3921 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/parser.py
+-rw-rw-r--   0 root         (0) root         (0)      923 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/print_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4102 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/proc_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5000 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/recipe.py
+-rw-rw-r--   0 root         (0) root         (0)      679 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/setup.bash
+-rw-rw-r--   0 root         (0) root         (0)     1842 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/common/sudo_refresh.py
+-rw-rw-r--   0 root         (0) root         (0)       45 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/forest.bash
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:49:08.500666 hhcm_forest-1.1.9/src/forest/git_tools/
+-rw-rw-r--   0 root         (0) root         (0)     2352 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/git_tools/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/git_tools/_impl.py
+-rwxrwxr-x   0 root         (0) root         (0)     9831 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/src/forest/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:49:08.500666 hhcm_forest-1.1.9/src/hhcm_forest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4760 2023-05-14 09:49:08.000000 hhcm_forest-1.1.9/src/hhcm_forest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-05-14 09:49:08.000000 hhcm_forest-1.1.9/src/hhcm_forest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:49:08.000000 hhcm_forest-1.1.9/src/hhcm_forest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-14 09:49:08.000000 hhcm_forest-1.1.9/src/hhcm_forest.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-14 09:49:08.000000 hhcm_forest-1.1.9/src/hhcm_forest.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 09:49:08.000000 hhcm_forest-1.1.9/src/hhcm_forest.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:49:08.500666 hhcm_forest-1.1.9/test/
+-rw-rw-r--   0 root         (0) root         (0)      703 2023-05-14 09:48:09.000000 hhcm_forest-1.1.9/test/test_run_bash_tests.py
```

### Comparing `hhcm_forest-1.1.8/LICENSE` & `hhcm_forest-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/PKG-INFO` & `hhcm_forest-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhcm_forest
-Version: 1.1.8
+Version: 1.1.9
 Summary: A minimalistic tool to automate source code cloning and building
 Home-page: https://none
 Author: Arturo Laurenzi
 Author-email: arturo.laurenzi@iit.it
 License: UNKNOWN
 Project-URL: Bug Tracker, https://none
 Platform: UNKNOWN
```

### Comparing `hhcm_forest-1.1.8/README.md` & `hhcm_forest-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/setup.cfg` & `hhcm_forest-1.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hhcm_forest
-version = 1.1.8
+version = 1.1.9
 author = Arturo Laurenzi
 author_email = arturo.laurenzi@iit.it
 description = A minimalistic tool to automate source code cloning and building
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://none
 project_urls =
```

### Comparing `hhcm_forest-1.1.8/src/forest/cmake_tools/__init__.py` & `hhcm_forest-1.1.9/src/forest/cmake_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/src/forest/cmake_tools/_impl.py` & `hhcm_forest-1.1.9/src/forest/cmake_tools/_impl.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/src/forest/common/build_handler.py` & `hhcm_forest-1.1.9/src/forest/common/build_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,40 @@
         self.pre_build_cmd = list()
         self.post_build_cmd = list()
 
         # env hook to install
         self.env_hook_content = None
 
     
-    def pre_build(self, builddir):
-        for cmd in self.pre_build_cmd:
+    def pre_build(self, builddir, srcdir, installdir):
+        eh = eval_handler.EvalHandler.instance()
+        process_string = lambda cmd: eh.process_string(cmd, {'builddir':builddir, 
+                                                             'srcdir': srcdir, 
+                                                             'installdir': installdir})
+        
+        _pre_build_cmd = map(process_string, self.pre_build_cmd)
+        
+        # apply locals to all cmds before executing the first one
+        pre_build_cmd = list(_pre_build_cmd)
+
+        for cmd in pre_build_cmd:
             proc_utils.call_process(args=[cmd], cwd=builddir, shell=True)
 
-    def post_build(self, builddir):
-        for cmd in self.post_build_cmd:
+    def post_build(self, builddir, srcdir, installdir):
+        eh = eval_handler.EvalHandler.instance()
+        process_string = lambda cmd: eh.process_string(cmd, {'builddir':builddir, 
+                                                             'srcdir': srcdir, 
+                                                             'installdir': installdir})
+        
+        _post_build_cmd = map(process_string, self.post_build_cmd)
+        
+        # apply locals to all cmds before executing the first one
+        post_build_cmd = list(_post_build_cmd)
+
+        for cmd in post_build_cmd:
             proc_utils.call_process(args=[cmd], cwd=builddir, shell=True)
     
     def install_env_hook(self, installdir):
         if self.env_hook_content is None:
             return 
 
         os.makedirs(f'{installdir}/share/forest_env_hook', exist_ok=True)
@@ -92,23 +112,20 @@
         post_build = recipe.get('post_build', list())
 
         # conditional
         eh = eval_handler.EvalHandler.instance()
 
         pre_build_if = recipe.get('pre_build_if', dict())
         pre_build.extend(eh.parse_conditional_dict(pre_build_if))
-        pre_build = map(eh.process_string, pre_build)
 
         post_build_if = recipe.get('post_build_if', dict())
         post_build.extend(eh.parse_conditional_dict(post_build_if))
-        post_build = map(eh.process_string, post_build)
 
-        # apply
-        builder.pre_build_cmd = list(pre_build)
-        builder.post_build_cmd = list(post_build)
+        builder.pre_build_cmd = pre_build
+        builder.post_build_cmd = post_build
 
         # env hooks
         env_hooks = data.get('env_hooks', list())
         env_hook_content = str()
         for hline in env_hooks:
             env_hook_content += eh.process_string(hline, shell=False)
             env_hook_content += '\n'
@@ -230,24 +247,24 @@
 
             self.pprint('running cmake...')
             if not cmake.configure(args=cmake_args):
                 self.pprint('configuring failed')
                 return False
 
         # pre-build
-        self.pre_build(builddir)
+        self.pre_build(builddir, srcdir, installdir)
 
         # build
         self.pprint('building...')
         if not cmake.build(target=self.target, jobs=jobs):
             self.pprint('build failed')
             return False 
 
         # post-build
-        self.post_build(builddir)
+        self.post_build(builddir, srcdir, installdir)
 
         # install hooks 
         self.install_env_hook(installdir)
         
         # save to cache and exit
         BuildHandler.build_cache.add(self.pkgname)
```

### Comparing `hhcm_forest-1.1.8/src/forest/common/eval_handler.py` & `hhcm_forest-1.1.9/src/forest/common/eval_handler.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/src/forest/common/fetch_handler.py` & `hhcm_forest-1.1.9/src/forest/common/fetch_handler.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/src/forest/common/install.py` & `hhcm_forest-1.1.9/src/forest/common/install.py`

 * *Files 8% similar despite different names*

```diff
@@ -220,21 +220,30 @@
 
 def write_setup_file():
     
     """
     Write a setup file to the root directory.
     """
 
+    # compute relative site-package path 
+    # without using distutils, which is deprecated
+    import sys 
+    import sysconfig
+    platlib_path = sysconfig.get_path(name='platlib')    
+    platlib_relpath = os.path.relpath(path=platlib_path, start=sys.prefix)
+
+    # replace placeholders
     this_dir = os.path.dirname(os.path.abspath(__file__))
     setup_template = os.path.join(this_dir, 'setup.bash')
     with open(setup_template, 'r') as f:
         content = f.read()
         content = content.replace('£PREFIX£', os.path.realpath(installdir))
         content = content.replace('£SRCDIR£', os.path.realpath(srcroot))
         content = content.replace('£ROOTDIR£', os.path.realpath(rootdir))
+        content = content.replace('£REL_SITE_PKG_PATH£', platlib_relpath)
     
     setup_file = os.path.join(installdir, '..', 'setup.bash')
     if not os.path.exists(setup_file):
         with open(setup_file, 'w') as f:
             f.write(content)
```

### Comparing `hhcm_forest-1.1.8/src/forest/common/package.py` & `hhcm_forest-1.1.9/src/forest/common/package.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/src/forest/common/parser.py` & `hhcm_forest-1.1.9/src/forest/common/parser.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/src/forest/common/print_utils.py` & `hhcm_forest-1.1.9/src/forest/common/print_utils.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/src/forest/common/proc_utils.py` & `hhcm_forest-1.1.9/src/forest/common/proc_utils.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/src/forest/common/recipe.py` & `hhcm_forest-1.1.9/src/forest/common/recipe.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/src/forest/common/setup.bash` & `hhcm_forest-1.1.9/src/forest/common/setup.bash`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup environment
 export LD_LIBRARY_PATH=£PREFIX£/lib:$LD_LIBRARY_PATH
 export CMAKE_PREFIX_PATH=£PREFIX£:$CMAKE_PREFIX_PATH
 export PATH=£PREFIX£/bin:$PATH
 export GAZEBO_PLUGIN_PATH=£PREFIX£/lib:$GAZEBO_PLUGIN_PATH
-export PYTHONPATH=£PREFIX£/lib/python2.7/dist-packages:£PREFIX£/lib/python3/dist-packages:$PYTHONPATH
+export PYTHONPATH=£PREFIX£/lib/python2.7/dist-packages:£PREFIX£/£REL_SITE_PKG_PATH£:$PYTHONPATH
 export ROS_PACKAGE_PATH=£ROOTDIR£/ros_src:£PREFIX£/share:£PREFIX£/lib:$ROS_PACKAGE_PATH
 export PKG_CONFIG_PATH=£PREFIX£/lib/pkgconfig:$PKG_CONFIG_PATH
 export HHCM_FOREST_PATH=£ROOTDIR£:$HHCM_FOREST_PATH
 
 # source env hooks
 if [ -d £PREFIX£/share/forest_env_hook ]; then
     for f in £PREFIX£/share/forest_env_hook/*; do source $f; done
```

### Comparing `hhcm_forest-1.1.8/src/forest/common/sudo_refresh.py` & `hhcm_forest-1.1.9/src/forest/common/sudo_refresh.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/src/forest/git_tools/__init__.py` & `hhcm_forest-1.1.9/src/forest/git_tools/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,11 +67,11 @@
             # remove src and re-raise exception
             self.rm()
             raise e
 
         return clone_ok
 
     def checkout(self, tag):
-        return proc_utils.call_process(['git', 'checkout', tag], cwd=self.srcdir)
+        return proc_utils.call_process(['git', 'checkout', '--recurse-submodules', tag], cwd=self.srcdir)
 
     def rm(self):
         shutil.rmtree(self.srcdir,  ignore_errors=True)
```

### Comparing `hhcm_forest-1.1.8/src/forest/main.py` & `hhcm_forest-1.1.9/src/forest/main.py`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/src/hhcm_forest.egg-info/PKG-INFO` & `hhcm_forest-1.1.9/src/hhcm_forest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhcm-forest
-Version: 1.1.8
+Version: 1.1.9
 Summary: A minimalistic tool to automate source code cloning and building
 Home-page: https://none
 Author: Arturo Laurenzi
 Author-email: arturo.laurenzi@iit.it
 License: UNKNOWN
 Project-URL: Bug Tracker, https://none
 Platform: UNKNOWN
```

### Comparing `hhcm_forest-1.1.8/src/hhcm_forest.egg-info/SOURCES.txt` & `hhcm_forest-1.1.9/src/hhcm_forest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hhcm_forest-1.1.8/test/test_run_bash_tests.py` & `hhcm_forest-1.1.9/test/test_run_bash_tests.py`

 * *Files identical despite different names*

