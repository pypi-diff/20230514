# Comparing `tmp/juliacall-0.9.8.tar.gz` & `tmp/juliacall-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juliacall-0.9.8.tar", last modified: Tue Oct 18 12:33:09 2022, max compression
+gzip compressed data, was "juliacall-0.9.9.tar", last modified: Thu Oct 20 18:59:33 2022, max compression
```

## Comparing `juliacall-0.9.8.tar` & `juliacall-0.9.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:33:09.696148 juliacall-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-18 12:33:00.000000 juliacall-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-10-18 12:33:09.696148 juliacall-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4505 2022-10-18 12:33:00.000000 juliacall-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-10-18 12:33:00.000000 juliacall-0.9.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:33:09.692148 juliacall-0.9.8/pysrc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:33:09.696148 juliacall-0.9.8/pysrc/juliacall/
--rw-r--r--   0 runner    (1001) docker     (121)     7526 2022-10-18 12:33:00.000000 juliacall-0.9.8/pysrc/juliacall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3280 2022-10-18 12:33:00.000000 juliacall-0.9.8/pysrc/juliacall/importer.py
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-18 12:33:00.000000 juliacall-0.9.8/pysrc/juliacall/init.jl
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-10-18 12:33:00.000000 juliacall-0.9.8/pysrc/juliacall/ipython.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-10-18 12:33:00.000000 juliacall-0.9.8/pysrc/juliacall/juliapkg-dev.json
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-18 12:33:00.000000 juliacall-0.9.8/pysrc/juliacall/juliapkg.json
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-10-18 12:33:00.000000 juliacall-0.9.8/pysrc/juliacall/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:33:09.696148 juliacall-0.9.8/pysrc/juliacall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-10-18 12:33:09.000000 juliacall-0.9.8/pysrc/juliacall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-10-18 12:33:09.000000 juliacall-0.9.8/pysrc/juliacall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 12:33:09.000000 juliacall-0.9.8/pysrc/juliacall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 12:33:09.000000 juliacall-0.9.8/pysrc/juliacall.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-18 12:33:09.000000 juliacall-0.9.8/pysrc/juliacall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-18 12:33:09.000000 juliacall-0.9.8/pysrc/juliacall.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-10-18 12:33:09.696148 juliacall-0.9.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 18:59:33.094355 juliacall-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-20 18:59:23.000000 juliacall-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-10-20 18:59:33.094355 juliacall-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4505 2022-10-20 18:59:23.000000 juliacall-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-10-20 18:59:23.000000 juliacall-0.9.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 18:59:33.090355 juliacall-0.9.9/pysrc/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 18:59:33.094355 juliacall-0.9.9/pysrc/juliacall/
+-rw-r--r--   0 runner    (1001) docker     (121)     7653 2022-10-20 18:59:23.000000 juliacall-0.9.9/pysrc/juliacall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3280 2022-10-20 18:59:23.000000 juliacall-0.9.9/pysrc/juliacall/importer.py
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-20 18:59:23.000000 juliacall-0.9.9/pysrc/juliacall/init.jl
+-rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-10-20 18:59:23.000000 juliacall-0.9.9/pysrc/juliacall/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-10-20 18:59:23.000000 juliacall-0.9.9/pysrc/juliacall/juliapkg-dev.json
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-20 18:59:23.000000 juliacall-0.9.9/pysrc/juliacall/juliapkg.json
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2022-10-20 18:59:23.000000 juliacall-0.9.9/pysrc/juliacall/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 18:59:33.094355 juliacall-0.9.9/pysrc/juliacall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-10-20 18:59:33.000000 juliacall-0.9.9/pysrc/juliacall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2022-10-20 18:59:33.000000 juliacall-0.9.9/pysrc/juliacall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 18:59:33.000000 juliacall-0.9.9/pysrc/juliacall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 18:59:32.000000 juliacall-0.9.9/pysrc/juliacall.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-20 18:59:33.000000 juliacall-0.9.9/pysrc/juliacall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-20 18:59:33.000000 juliacall-0.9.9/pysrc/juliacall.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      574 2022-10-20 18:59:33.094355 juliacall-0.9.9/setup.cfg
```

### Comparing `juliacall-0.9.8/LICENSE` & `juliacall-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `juliacall-0.9.8/PKG-INFO` & `juliacall-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juliacall
-Version: 0.9.8
+Version: 0.9.9
 Summary: Julia and Python in seamless harmony
 Home-page: http://github.com/cjdoris/PythonCall.jl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

### Comparing `juliacall-0.9.8/README.md` & `juliacall-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `juliacall-0.9.8/pysrc/juliacall/__init__.py` & `juliacall-0.9.9/pysrc/juliacall/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This module gets modified by PythonCall when it is loaded, e.g. to include Core, Base
 # and Main modules.
 
-__version__ = '0.9.8'
+__version__ = '0.9.9'
 
 _newmodule = None
 
 def newmodule(name):
     "A new module with the given name."
     global _newmodule
     if _newmodule is None:
@@ -147,68 +147,72 @@
     cmd = [exepath, '--project='+project, '--startup-file=no', '-O0', '--compile=min',
            '-e', 'import Libdl; print(abspath(Libdl.dlpath("libjulia")), "\\0", Sys.BINDIR)']
     libpath, default_bindir = subprocess.run(cmd, check=True, capture_output=True, encoding='utf8').stdout.split('\0')
     assert os.path.exists(libpath)
     assert os.path.exists(default_bindir)
     CONFIG['libpath'] = libpath
 
-    # Initialise Julia
-    d = os.getcwd()
-    try:
-        # Open the library
-        os.chdir(os.path.dirname(libpath))
-        CONFIG['lib'] = lib = c.CDLL(libpath, mode=c.RTLD_GLOBAL)
-
-        # parse options
-        argc, argv = args_from_config()
-        jl_parse_opts = lib.jl_parse_opts
-        jl_parse_opts.argtypes = [c.c_void_p, c.c_void_p]
-        jl_parse_opts.restype = None
-        jl_parse_opts(c.pointer(argc), c.pointer(argv))
-        assert argc.value == 0
+    # Add the Julia library directory to the PATH on Windows so Julia's system libraries can
+    # be found. They are normally found because they are in the same directory as julia.exe,
+    # but python.exe is somewhere else!
+    if os.name == 'nt':
+        libdir = os.path.dirname(libpath)
+        if 'PATH' in os.environ:
+            os.environ['PATH'] = libdir + ';' + os.environ['PATH']
+        else:
+            os.environ['PATH'] = libdir
 
-        # initialise julia
-        try:
-            jl_init = lib.jl_init_with_image__threading
-        except AttributeError:
-            jl_init = lib.jl_init_with_image
-        jl_init.argtypes = [c.c_char_p, c.c_char_p]
-        jl_init.restype = None
-        jl_init(
-            (default_bindir if bindir is None else bindir).encode('utf8'),
-            None if sysimg is None else sysimg.encode('utf8'),
-        )
-
-        # initialise PythonCall
-        jl_eval = lib.jl_eval_string
-        jl_eval.argtypes = [c.c_char_p]
-        jl_eval.restype = c.c_void_p
-        def jlstr(x):
-            return 'raw"' + x.replace('"', '\\"').replace('\\', '\\\\') + '"'
-        script = '''
-        try
-            Base.require(Main, :CompilerSupportLibraries_jll)
-            import Pkg
-            ENV["JULIA_PYTHONCALL_LIBPTR"] = {}
-            ENV["JULIA_PYTHONCALL_EXE"] = {}
-            Pkg.activate({}, io=devnull)
-            import PythonCall
-        catch err
-            print(stderr, "ERROR: ")
-            showerror(stderr, err, catch_backtrace())
-            flush(stderr)
-            rethrow()
-        end
-        '''.format(
-            jlstr(str(c.pythonapi._handle)),
-            jlstr(sys.executable or ''),
-            jlstr(project),
-        )
-        res = jl_eval(script.encode('utf8'))
-        if res is None:
-            raise Exception('PythonCall.jl did not start properly')
-    finally:
-        os.chdir(d)
+    # Open the library
+    CONFIG['lib'] = lib = c.CDLL(libpath, mode=c.RTLD_GLOBAL)
+
+    # parse options
+    argc, argv = args_from_config()
+    jl_parse_opts = lib.jl_parse_opts
+    jl_parse_opts.argtypes = [c.c_void_p, c.c_void_p]
+    jl_parse_opts.restype = None
+    jl_parse_opts(c.pointer(argc), c.pointer(argv))
+    assert argc.value == 0
+
+    # initialise julia
+    try:
+        jl_init = lib.jl_init_with_image__threading
+    except AttributeError:
+        jl_init = lib.jl_init_with_image
+    jl_init.argtypes = [c.c_char_p, c.c_char_p]
+    jl_init.restype = None
+    jl_init(
+        (default_bindir if bindir is None else bindir).encode('utf8'),
+        None if sysimg is None else sysimg.encode('utf8'),
+    )
+
+    # initialise PythonCall
+    jl_eval = lib.jl_eval_string
+    jl_eval.argtypes = [c.c_char_p]
+    jl_eval.restype = c.c_void_p
+    def jlstr(x):
+        return 'raw"' + x.replace('"', '\\"').replace('\\', '\\\\') + '"'
+    script = '''
+    try
+        Base.require(Main, :CompilerSupportLibraries_jll)
+        import Pkg
+        ENV["JULIA_PYTHONCALL_LIBPTR"] = {}
+        ENV["JULIA_PYTHONCALL_EXE"] = {}
+        Pkg.activate({}, io=devnull)
+        import PythonCall
+    catch err
+        print(stderr, "ERROR: ")
+        showerror(stderr, err, catch_backtrace())
+        flush(stderr)
+        rethrow()
+    end
+    '''.format(
+        jlstr(str(c.pythonapi._handle)),
+        jlstr(sys.executable or ''),
+        jlstr(project),
+    )
+    res = jl_eval(script.encode('utf8'))
+    if res is None:
+        raise Exception('PythonCall.jl did not start properly')
 
     CONFIG['inited'] = True
 
 init()
```

### Comparing `juliacall-0.9.8/pysrc/juliacall/importer.py` & `juliacall-0.9.9/pysrc/juliacall/importer.py`

 * *Files identical despite different names*

### Comparing `juliacall-0.9.8/pysrc/juliacall/ipython.py` & `juliacall-0.9.9/pysrc/juliacall/ipython.py`

 * *Files identical despite different names*

### Comparing `juliacall-0.9.8/pysrc/juliacall/matplotlib.py` & `juliacall-0.9.9/pysrc/juliacall/matplotlib.py`

 * *Files identical despite different names*

### Comparing `juliacall-0.9.8/pysrc/juliacall.egg-info/PKG-INFO` & `juliacall-0.9.9/pysrc/juliacall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juliacall
-Version: 0.9.8
+Version: 0.9.9
 Summary: Julia and Python in seamless harmony
 Home-page: http://github.com/cjdoris/PythonCall.jl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

### Comparing `juliacall-0.9.8/setup.cfg` & `juliacall-0.9.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = juliacall
-version = 0.9.8
+version = 0.9.9
 description = Julia and Python in seamless harmony
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://github.com/cjdoris/PythonCall.jl
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

