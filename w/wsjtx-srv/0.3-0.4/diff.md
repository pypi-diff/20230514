# Comparing `tmp/wsjtx_srv-0.3.tar.gz` & `tmp/wsjtx_srv-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsjtx_srv-0.3.tar", last modified: Sun Apr 23 07:22:06 2023, max compression
+gzip compressed data, was "wsjtx_srv-0.4.tar", last modified: Sun May 14 17:55:13 2023, max compression
```

## Comparing `wsjtx_srv-0.3.tar` & `wsjtx_srv-0.4.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-23 07:22:06.562580 wsjtx_srv-0.3/
--rw-r--r--   0 ralf      (1000) priv      (1011)     2519 2023-04-23 07:22:06.566580 wsjtx_srv-0.3/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)     8175 2023-04-23 07:21:47.154585 wsjtx_srv-0.3/README.html
--rw-r--r--   0 ralf      (1000) priv      (1011)     1507 2023-04-23 07:21:15.394593 wsjtx_srv-0.3/README.rst
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-23 07:22:06.558580 wsjtx_srv-0.3/bin/
--rwxr-xr-x   0 ralf      (1000) priv      (1011)      979 2021-10-26 11:43:05.045461 wsjtx_srv-0.3/bin/wbf
--rwxr-xr-x   0 ralf      (1000) priv      (1011)       56 2021-09-13 11:37:43.842778 wsjtx_srv-0.3/bin/wsjtx-srv
--rw-r--r--   0 ralf      (1000) priv      (1011)     3089 2022-05-14 10:25:48.328549 wsjtx_srv-0.3/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-04-23 07:22:06.562580 wsjtx_srv-0.3/wsjtx_srv/
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-04-23 07:21:47.154585 wsjtx_srv-0.3/wsjtx_srv/Version.py
--rw-r--r--   0 ralf      (1000) priv      (1011)       21 2021-09-13 11:36:52.530794 wsjtx_srv-0.3/wsjtx_srv/__init__.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    45636 2023-04-23 07:17:49.078639 wsjtx_srv-0.3/wsjtx_srv/wsjtx.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-14 17:55:13.011271 wsjtx_srv-0.4/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       39 2021-09-13 11:36:52.000000 wsjtx_srv-0.4/MANIFEST.in
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2579 2023-05-14 17:55:13.007271 wsjtx_srv-0.4/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)     8175 2023-05-14 17:54:25.000000 wsjtx_srv-0.4/README.html
+-rw-r--r--   0 ralf      (1000) priv      (1011)     1507 2023-04-23 07:21:15.000000 wsjtx_srv-0.4/README.rst
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-14 17:55:12.967271 wsjtx_srv-0.4/bin/
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)      979 2021-10-26 11:43:05.000000 wsjtx_srv-0.4/bin/wbf
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)       56 2021-09-13 11:37:43.000000 wsjtx_srv-0.4/bin/wsjtx-srv
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-14 17:55:13.011271 wsjtx_srv-0.4/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2991 2023-05-14 17:53:55.000000 wsjtx_srv-0.4/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-14 17:55:12.979271 wsjtx_srv-0.4/wsjtx_srv/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-05-14 17:54:25.000000 wsjtx_srv-0.4/wsjtx_srv/Version.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)       21 2021-09-13 11:36:52.000000 wsjtx_srv-0.4/wsjtx_srv/__init__.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    45636 2023-04-23 07:17:49.000000 wsjtx_srv-0.4/wsjtx_srv/wsjtx.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-14 17:55:13.003271 wsjtx_srv-0.4/wsjtx_srv.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2579 2023-05-14 17:55:12.000000 wsjtx_srv-0.4/wsjtx_srv.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)      291 2023-05-14 17:55:12.000000 wsjtx_srv-0.4/wsjtx_srv.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-14 17:55:12.000000 wsjtx_srv-0.4/wsjtx_srv.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       16 2023-05-14 17:55:12.000000 wsjtx_srv-0.4/wsjtx_srv.egg-info/requires.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       10 2023-05-14 17:55:12.000000 wsjtx_srv-0.4/wsjtx_srv.egg-info/top_level.txt
```

### Comparing `wsjtx_srv-0.3/PKG-INFO` & `wsjtx_srv-0.4/wsjtx_srv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
-Name: wsjtx_srv
-Version: 0.3
+Metadata-Version: 2.1
+Name: wsjtx-srv
+Version: 0.4
 Summary: Library implementation of WSJTX companion program
 Home-page: https://github.com/schlatterbeck/wsjtx-srv
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: BSD License
 Description: wsjtx-srv: Library for WSJT-X server implementation
         ===================================================
@@ -56,7 +56,9 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
```

### Comparing `wsjtx_srv-0.3/README.html` & `wsjtx_srv-0.4/README.html`

 * *Files identical despite different names*

### Comparing `wsjtx_srv-0.3/README.rst` & `wsjtx_srv-0.4/README.rst`

 * *Files identical despite different names*

### Comparing `wsjtx_srv-0.3/bin/wbf` & `wsjtx_srv-0.4/bin/wbf`

 * *Files identical despite different names*

### Comparing `wsjtx_srv-0.3/setup.py` & `wsjtx_srv-0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright (C) 2021 Dr. Ralf Schlatterbeck Open Source Consulting.
+# Copyright (C) 2021-23 Dr. Ralf Schlatterbeck Open Source Consulting.
 # Reichergasse 131, A-3411 Weidling.
 # Web: http://www.runtux.com Email: office@runtux.com
 # All rights reserved
 # ****************************************************************************
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are
 # met:
@@ -24,38 +24,33 @@
 # TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
 # PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 # ****************************************************************************
 
+from setuptools import setup
 try :
     from wsjtx_srv.Version import VERSION
 except :
     VERSION = None
-from warnings       import filterwarnings
-from distutils.core import setup, Extension
-
-filterwarnings \
-    ( "ignore"
-    , "Unknown distribution option: 'install_requires'"
-    )
 
 description = []
 with open ('README.rst') as f :
     for line in f :
         description.append (line)
 
 license     = 'BSD License'
 rq          = '>=3.7'
 setup \
     ( name             = "wsjtx_srv"
     , version          = VERSION
     , description      = "Library implementation of WSJTX companion program"
     , long_description = ''.join (description)
+    , long_description_content_type = 'text/x-rst'
     , license          = license
     , author           = "Ralf Schlatterbeck"
     , author_email     = "rsc@runtux.com"
     , install_requires = ['rsclib', 'hamradio']
     , packages         = ['wsjtx_srv']
     , platforms        = 'Any'
     , url              = "https://github.com/schlatterbeck/wsjtx-srv"
```

### Comparing `wsjtx_srv-0.3/wsjtx_srv/wsjtx.py` & `wsjtx_srv-0.4/wsjtx_srv/wsjtx.py`

 * *Files identical despite different names*

