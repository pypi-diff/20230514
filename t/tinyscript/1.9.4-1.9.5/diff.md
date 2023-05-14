# Comparing `tmp/tinyscript-1.9.4.tar.gz` & `tmp/tinyscript-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tinyscript-1.9.4.tar", last modified: Sat May  4 16:13:14 2019, max compression
+gzip compressed data, was "dist/tinyscript-1.9.5.tar", last modified: Sat May  4 17:06:45 2019, max compression
```

## Comparing `tinyscript-1.9.4.tar` & `tinyscript-1.9.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-04 16:13:14.000000 tinyscript-1.9.4/
--rwxr-xr-x   0 root         (0) root         (0)      919 2019-03-08 11:38:21.000000 tinyscript-1.9.4/tinyscript-new
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-04 16:13:14.000000 tinyscript-1.9.4/tinyscript/
--rw-r--r--   0 root         (0) root         (0)     3810 2019-04-07 13:29:12.000000 tinyscript-1.9.4/tinyscript/loglib.py
--rw-r--r--   0 root         (0) root         (0)    25200 2019-04-13 21:51:25.000000 tinyscript-1.9.4/tinyscript/argreparse.py
--rw-r--r--   0 root         (0) root         (0)     4157 2019-04-11 11:14:20.000000 tinyscript-1.9.4/tinyscript/interact.py
--rw-r--r--   0 root         (0) root         (0)     1539 2019-04-11 17:29:46.000000 tinyscript-1.9.4/tinyscript/handlers.py
--rw-r--r--   0 root         (0) root         (0)     3102 2019-04-11 10:30:47.000000 tinyscript-1.9.4/tinyscript/template.py
--rw-r--r--   0 root         (0) root         (0)      580 2019-03-06 06:31:14.000000 tinyscript-1.9.4/tinyscript/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-04 16:13:14.000000 tinyscript-1.9.4/tinyscript/report/
--rw-r--r--   0 root         (0) root         (0)     8769 2019-04-12 16:20:24.000000 tinyscript-1.9.4/tinyscript/report/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2284 2019-02-28 16:33:06.000000 tinyscript-1.9.4/tinyscript/report/default.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-04 16:13:14.000000 tinyscript-1.9.4/tinyscript/helpers/
--rw-rw-r--   0 root         (0) root         (0)     2196 2019-04-12 05:52:27.000000 tinyscript-1.9.4/tinyscript/helpers/licenses.py
--rw-r--r--   0 root         (0) root         (0)      432 2019-04-10 07:03:26.000000 tinyscript-1.9.4/tinyscript/helpers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3692 2019-04-26 13:01:48.000000 tinyscript-1.9.4/tinyscript/helpers/types.py
--rw-r--r--   0 root         (0) root         (0)     1568 2019-04-15 10:22:19.000000 tinyscript-1.9.4/tinyscript/helpers/lambdas.py
--rw-r--r--   0 root         (0) root         (0)     4254 2019-05-04 16:03:37.000000 tinyscript-1.9.4/tinyscript/helpers/utils.py
--rw-r--r--   0 root         (0) root         (0)      250 2019-05-04 16:13:13.000000 tinyscript-1.9.4/tinyscript/__info__.py
--rw-r--r--   0 root         (0) root         (0)     1740 2019-04-12 07:53:45.000000 tinyscript-1.9.4/tinyscript/step.py
--rw-r--r--   0 root         (0) root         (0)     3302 2019-04-12 09:40:41.000000 tinyscript-1.9.4/tinyscript/timing.py
--rw-r--r--   0 root         (0) root         (0)    17152 2019-04-13 09:39:19.000000 tinyscript-1.9.4/tinyscript/parser.py
--rw-r--r--   0 root         (0) root         (0)      870 2019-04-12 10:43:59.000000 tinyscript-1.9.4/tinyscript/preimports.py
--rw-r--r--   0 root         (0) root         (0)       91 2019-03-06 08:59:58.000000 tinyscript-1.9.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      103 2019-04-12 14:07:04.000000 tinyscript-1.9.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2019-05-04 16:13:14.000000 tinyscript-1.9.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1996 2019-05-04 16:13:13.000000 tinyscript-1.9.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-04 16:13:14.000000 tinyscript-1.9.4/tinyscript.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2019-05-04 16:13:13.000000 tinyscript-1.9.4/tinyscript.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2019-05-04 16:13:13.000000 tinyscript-1.9.4/tinyscript.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2019-05-04 16:13:13.000000 tinyscript-1.9.4/tinyscript.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2684 2019-05-04 16:13:13.000000 tinyscript-1.9.4/tinyscript.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      704 2019-05-04 16:13:13.000000 tinyscript-1.9.4/tinyscript.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     2684 2019-05-04 16:13:14.000000 tinyscript-1.9.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    34524 2019-02-28 16:33:06.000000 tinyscript-1.9.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1362 2019-04-12 21:36:55.000000 tinyscript-1.9.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-04 17:06:45.000000 tinyscript-1.9.5/
+-rwxr-xr-x   0 root         (0) root         (0)      919 2019-03-08 11:38:21.000000 tinyscript-1.9.5/tinyscript-new
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-04 17:06:45.000000 tinyscript-1.9.5/tinyscript/
+-rw-r--r--   0 root         (0) root         (0)     3810 2019-04-07 13:29:12.000000 tinyscript-1.9.5/tinyscript/loglib.py
+-rw-r--r--   0 root         (0) root         (0)    25200 2019-04-13 21:51:25.000000 tinyscript-1.9.5/tinyscript/argreparse.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2019-04-11 11:14:20.000000 tinyscript-1.9.5/tinyscript/interact.py
+-rw-r--r--   0 root         (0) root         (0)     1539 2019-04-11 17:29:46.000000 tinyscript-1.9.5/tinyscript/handlers.py
+-rw-r--r--   0 root         (0) root         (0)     3102 2019-04-11 10:30:47.000000 tinyscript-1.9.5/tinyscript/template.py
+-rw-r--r--   0 root         (0) root         (0)      580 2019-03-06 06:31:14.000000 tinyscript-1.9.5/tinyscript/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-04 17:06:45.000000 tinyscript-1.9.5/tinyscript/report/
+-rw-r--r--   0 root         (0) root         (0)     8769 2019-04-12 16:20:24.000000 tinyscript-1.9.5/tinyscript/report/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2019-02-28 16:33:06.000000 tinyscript-1.9.5/tinyscript/report/default.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-04 17:06:45.000000 tinyscript-1.9.5/tinyscript/helpers/
+-rw-rw-r--   0 root         (0) root         (0)     2196 2019-04-12 05:52:27.000000 tinyscript-1.9.5/tinyscript/helpers/licenses.py
+-rw-r--r--   0 root         (0) root         (0)      432 2019-04-10 07:03:26.000000 tinyscript-1.9.5/tinyscript/helpers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3692 2019-04-26 13:01:48.000000 tinyscript-1.9.5/tinyscript/helpers/types.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2019-04-15 10:22:19.000000 tinyscript-1.9.5/tinyscript/helpers/lambdas.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2019-05-04 17:03:38.000000 tinyscript-1.9.5/tinyscript/helpers/utils.py
+-rw-r--r--   0 root         (0) root         (0)      250 2019-05-04 17:06:44.000000 tinyscript-1.9.5/tinyscript/__info__.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2019-04-12 07:53:45.000000 tinyscript-1.9.5/tinyscript/step.py
+-rw-r--r--   0 root         (0) root         (0)     3302 2019-04-12 09:40:41.000000 tinyscript-1.9.5/tinyscript/timing.py
+-rw-r--r--   0 root         (0) root         (0)    17152 2019-04-13 09:39:19.000000 tinyscript-1.9.5/tinyscript/parser.py
+-rw-r--r--   0 root         (0) root         (0)      870 2019-04-12 10:43:59.000000 tinyscript-1.9.5/tinyscript/preimports.py
+-rw-r--r--   0 root         (0) root         (0)       91 2019-03-06 08:59:58.000000 tinyscript-1.9.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      103 2019-04-12 14:07:04.000000 tinyscript-1.9.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2019-05-04 17:06:45.000000 tinyscript-1.9.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1996 2019-05-04 17:06:44.000000 tinyscript-1.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-05-04 17:06:45.000000 tinyscript-1.9.5/tinyscript.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2019-05-04 17:06:45.000000 tinyscript-1.9.5/tinyscript.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2019-05-04 17:06:45.000000 tinyscript-1.9.5/tinyscript.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2019-05-04 17:06:45.000000 tinyscript-1.9.5/tinyscript.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2684 2019-05-04 17:06:45.000000 tinyscript-1.9.5/tinyscript.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      704 2019-05-04 17:06:45.000000 tinyscript-1.9.5/tinyscript.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     2684 2019-05-04 17:06:45.000000 tinyscript-1.9.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    34524 2019-02-28 16:33:06.000000 tinyscript-1.9.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1362 2019-04-12 21:36:55.000000 tinyscript-1.9.5/README.md
```

### Comparing `tinyscript-1.9.4/tinyscript-new` & `tinyscript-1.9.5/tinyscript-new`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/loglib.py` & `tinyscript-1.9.5/tinyscript/loglib.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/argreparse.py` & `tinyscript-1.9.5/tinyscript/argreparse.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/interact.py` & `tinyscript-1.9.5/tinyscript/interact.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/handlers.py` & `tinyscript-1.9.5/tinyscript/handlers.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/template.py` & `tinyscript-1.9.5/tinyscript/template.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/__init__.py` & `tinyscript-1.9.5/tinyscript/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/report/__init__.py` & `tinyscript-1.9.5/tinyscript/report/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/report/default.css` & `tinyscript-1.9.5/tinyscript/report/default.css`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/helpers/licenses.py` & `tinyscript-1.9.5/tinyscript/helpers/licenses.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/helpers/types.py` & `tinyscript-1.9.5/tinyscript/helpers/types.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/helpers/lambdas.py` & `tinyscript-1.9.5/tinyscript/helpers/lambdas.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/helpers/utils.py` & `tinyscript-1.9.5/tinyscript/helpers/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Common utility functions.
 
 """
 import re
 import sys
 from humanfriendly.terminal import ansi_wrap
 from platform import uname
-from six import b as six_b, u, StringIO as SIO
+from six import b as six_b, u, StringIO
 from sys import version_info
 
 from .lambdas import is_lambda
 from ..__info__ import __author__, __copyright__, __version__
 
 
 __all__ = __features__ = ["LINUX", "PYTHON3", "WINDOWS", "b", "byteindex",
@@ -38,36 +38,51 @@
     """
     try:
         return six_b(text)
     except:
         return text
 
 
-class StringIO(SIO):
+class _Text(object):
     """
-    Tuned StringIO class.
+    Dummy Text class for storing StringIO's content before closing it.
     """
-    def __str__(self):
-        return self.getvalue().strip()
-    
-    @property
-    def text(self):
+    def __repr__(self):
         return str(self)
 
+    def __str__(self):
+        return self.text
+
 
 class Capture(object):
     """
     Context manager for capturing stdout and stderr.
     """
+    def __init__(self, out=sys.stdout, err=sys.stderr):
+        # backup original output file handles
+        self._stdout = sys.stdout
+        self._stderr = sys.stderr
+        
     def __enter__(self):
+        # create new file handles
         sys.stdout, sys.stderr = StringIO(), StringIO()
-        return sys.stdout, sys.stderr
+        self.stdout, self.stderr = _Text(), _Text()
+        # return references of the dummy objects
+        return self.stdout, self.stderr
     
     def __exit__(self, *args):
-        sys.stdout, sys.stderr = sys.__stdout__, sys.__stderr__
+        # freeze stdout and stderr contents before closing the file handles,
+        #  using the references previously returned by __enter__
+        self.stdout.text = sys.stdout.getvalue().strip() 
+        self.stderr.text = sys.stderr.getvalue().strip()
+        # close current file handles
+        sys.stdout.close()
+        sys.stderr.close()
+        # restore original output file handles
+        sys.stdout, sys.stderr = self._stdout, self._stderr
 
 
 def capture(f):
     """
     Decorator for capturing stdout and stderr.
     """
     def _wrapper(*a, **kw):
```

### Comparing `tinyscript-1.9.4/tinyscript/step.py` & `tinyscript-1.9.5/tinyscript/step.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/timing.py` & `tinyscript-1.9.5/tinyscript/timing.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/parser.py` & `tinyscript-1.9.5/tinyscript/parser.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/tinyscript/preimports.py` & `tinyscript-1.9.5/tinyscript/preimports.py`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/setup.py` & `tinyscript-1.9.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 requirements = parse_requirements("requirements.txt", session=False)
 setup(
   name = "tinyscript",
   packages = find_packages(exclude=("tests*", )),
   include_package_data = True,
   author = "Alexandre D\'Hondt",
   author_email = "alexandre.dhondt@gmail.com",
-  version = "1.9.4",
+  version = "1.9.5",
   license = "AGPLv3",
   url = "https://github.com/dhondta/tinyscript",
-  download_url = "https://github.com/dhondta/tinyscript/archive/1.9.4.tar.gz",
+  download_url = "https://github.com/dhondta/tinyscript/archive/1.9.5.tar.gz",
   description = "A library for quickly building CLI Python-based tools with "
                 "basic features in a shortened way",
   long_description=long_descr,
   long_description_content_type='text/markdown',
   scripts = ["tinyscript-new"],
   keywords = ["CLI", "tool"],
   classifiers = [
```

### Comparing `tinyscript-1.9.4/tinyscript.egg-info/PKG-INFO` & `tinyscript-1.9.5/tinyscript.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tinyscript
-Version: 1.9.4
+Version: 1.9.5
 Summary: A library for quickly building CLI Python-based tools with basic features in a shortened way
 Home-page: https://github.com/dhondta/tinyscript
 Author: Alexandre D'Hondt
 Author-email: alexandre.dhondt@gmail.com
 License: AGPLv3
-Download-URL: https://github.com/dhondta/tinyscript/archive/1.9.4.tar.gz
+Download-URL: https://github.com/dhondta/tinyscript/archive/1.9.5.tar.gz
 Description: [![PyPi](https://img.shields.io/pypi/v/tinyscript.svg)](https://pypi.python.org/pypi/tinyscript/)
         [![Read The Docs](https://readthedocs.org/projects/tinyscript/badge/?version=latest)](https://tinyscript.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.org/dhondta/tinyscript.svg?branch=master)](https://travis-ci.org/dhondta/tinyscript)
         [![Coverage Status](https://coveralls.io/repos/github/dhondta/tinyscript/badge.svg?branch=master)](https://coveralls.io/github/dhondta/tinyscript?branch=master)
         [![Python Versions](https://img.shields.io/pypi/pyversions/tinyscript.svg)](https://pypi.python.org/pypi/tinyscript/)
         [![Requirements Status](https://requires.io/github/dhondta/tinyscript/requirements.svg?branch=master)](https://requires.io/github/dhondta/tinyscript/requirements/?branch=master)
         [![Known Vulnerabilities](https://snyk.io/test/github/dhondta/tinyscript/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/dhondta/tinyscript?targetFile=requirements.txt)
```

### Comparing `tinyscript-1.9.4/tinyscript.egg-info/SOURCES.txt` & `tinyscript-1.9.5/tinyscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/PKG-INFO` & `tinyscript-1.9.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tinyscript
-Version: 1.9.4
+Version: 1.9.5
 Summary: A library for quickly building CLI Python-based tools with basic features in a shortened way
 Home-page: https://github.com/dhondta/tinyscript
 Author: Alexandre D'Hondt
 Author-email: alexandre.dhondt@gmail.com
 License: AGPLv3
-Download-URL: https://github.com/dhondta/tinyscript/archive/1.9.4.tar.gz
+Download-URL: https://github.com/dhondta/tinyscript/archive/1.9.5.tar.gz
 Description: [![PyPi](https://img.shields.io/pypi/v/tinyscript.svg)](https://pypi.python.org/pypi/tinyscript/)
         [![Read The Docs](https://readthedocs.org/projects/tinyscript/badge/?version=latest)](https://tinyscript.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.org/dhondta/tinyscript.svg?branch=master)](https://travis-ci.org/dhondta/tinyscript)
         [![Coverage Status](https://coveralls.io/repos/github/dhondta/tinyscript/badge.svg?branch=master)](https://coveralls.io/github/dhondta/tinyscript?branch=master)
         [![Python Versions](https://img.shields.io/pypi/pyversions/tinyscript.svg)](https://pypi.python.org/pypi/tinyscript/)
         [![Requirements Status](https://requires.io/github/dhondta/tinyscript/requirements.svg?branch=master)](https://requires.io/github/dhondta/tinyscript/requirements/?branch=master)
         [![Known Vulnerabilities](https://snyk.io/test/github/dhondta/tinyscript/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/dhondta/tinyscript?targetFile=requirements.txt)
```

### Comparing `tinyscript-1.9.4/LICENSE` & `tinyscript-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyscript-1.9.4/README.md` & `tinyscript-1.9.5/README.md`

 * *Files identical despite different names*

