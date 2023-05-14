# Comparing `tmp/concurrent-log-handler-0.9.8.tar.gz` & `tmp/concurrent-log-handler-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\concurrent-log-handler-0.9.8.tar", last modified: Fri Mar  2 17:45:09 2018, max compression
+gzip compressed data, was "dist\concurrent-log-handler-0.9.9.tar", last modified: Sat Mar 10 15:37:14 2018, max compression
```

## Comparing `concurrent-log-handler-0.9.8.tar` & `concurrent-log-handler-0.9.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2018-03-02 17:45:09.000000 concurrent-log-handler-0.9.8/
--rw-rw-rw-   0        0        0    13817 2018-03-02 17:45:09.000000 concurrent-log-handler-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     5258 2018-03-02 17:33:05.000000 concurrent-log-handler-0.9.8/README.md
--rw-rw-rw-   0        0        0       96 2018-03-02 17:45:09.000000 concurrent-log-handler-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0    13027 2018-03-02 17:33:05.000000 concurrent-log-handler-0.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2018-03-02 17:45:09.000000 concurrent-log-handler-0.9.8/src/
-drwxrwxrwx   0        0        0        0 2018-03-02 17:45:09.000000 concurrent-log-handler-0.9.8/src/concurrent_log_handler/
--rw-rw-rw-   0        0        0    11547 2018-02-25 21:24:42.000000 concurrent-log-handler-0.9.8/src/concurrent_log_handler/portalocker.py
--rw-rw-rw-   0        0        0     4383 2017-07-29 17:48:44.000000 concurrent-log-handler-0.9.8/src/concurrent_log_handler/queue.py
--rw-rw-rw-   0        0        0    18473 2018-03-02 17:33:05.000000 concurrent-log-handler-0.9.8/src/concurrent_log_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2018-03-02 17:45:09.000000 concurrent-log-handler-0.9.8/src/concurrent_log_handler.egg-info/
--rw-rw-rw-   0        0        0        1 2018-03-02 17:45:09.000000 concurrent-log-handler-0.9.8/src/concurrent_log_handler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    13817 2018-03-02 17:45:09.000000 concurrent-log-handler-0.9.8/src/concurrent_log_handler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2018-03-02 17:45:09.000000 concurrent-log-handler-0.9.8/src/concurrent_log_handler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       23 2018-03-02 17:45:09.000000 concurrent-log-handler-0.9.8/src/concurrent_log_handler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2017-09-04 14:37:53.000000 concurrent-log-handler-0.9.8/src/concurrent_log_handler.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2018-03-10 15:37:14.000000 concurrent-log-handler-0.9.9/
+-rw-rw-rw-   0        0        0    13895 2018-03-10 15:37:14.000000 concurrent-log-handler-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5321 2018-03-10 15:32:32.000000 concurrent-log-handler-0.9.9/README.md
+-rw-rw-rw-   0        0        0       96 2018-03-10 15:37:14.000000 concurrent-log-handler-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0    13089 2018-03-10 15:32:43.000000 concurrent-log-handler-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2018-03-10 15:37:14.000000 concurrent-log-handler-0.9.9/src/
+drwxrwxrwx   0        0        0        0 2018-03-10 15:37:14.000000 concurrent-log-handler-0.9.9/src/concurrent_log_handler/
+-rw-rw-rw-   0        0        0    11547 2018-02-25 21:24:42.000000 concurrent-log-handler-0.9.9/src/concurrent_log_handler/portalocker.py
+-rw-rw-rw-   0        0        0     4383 2017-07-29 17:48:44.000000 concurrent-log-handler-0.9.9/src/concurrent_log_handler/queue.py
+-rw-rw-rw-   0        0        0    18556 2018-03-10 15:31:42.000000 concurrent-log-handler-0.9.9/src/concurrent_log_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2018-03-10 15:37:14.000000 concurrent-log-handler-0.9.9/src/concurrent_log_handler.egg-info/
+-rw-rw-rw-   0        0        0        1 2018-03-10 15:37:14.000000 concurrent-log-handler-0.9.9/src/concurrent_log_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    13895 2018-03-10 15:37:14.000000 concurrent-log-handler-0.9.9/src/concurrent_log_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2018-03-10 15:37:14.000000 concurrent-log-handler-0.9.9/src/concurrent_log_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       23 2018-03-10 15:37:14.000000 concurrent-log-handler-0.9.9/src/concurrent_log_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2017-09-04 14:37:53.000000 concurrent-log-handler-0.9.9/src/concurrent_log_handler.egg-info/zip-safe
```

### Comparing `concurrent-log-handler-0.9.8/PKG-INFO` & `concurrent-log-handler-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: concurrent-log-handler
-Version: 0.9.8
+Version: 0.9.9
 Summary: RotatingFileHandler replacement with concurrency, gzip and Windows support
 Home-page: https://github.com/Preston-Landers/concurrent-log-handler
 Author: Preston Landers
 Author-email: planders@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description-Content-Type: UNKNOWN
 Description: 
@@ -140,14 +140,16 @@
             logging.config.fileConfig("logging.ini")
             log = logging.getLogger()
             log.info("Here is a very exciting log message, just for you")
         
         
         Change Log
         ==========
+        - 0.9.9: Fix Python 2 compatibility broken in last release
+        
         - 0.9.8: Bug fixes and permission features
            * Fix for issue #4 - AttributeError: 'NoneType' object has no attribute 'write'
               This error could be caused if a rollover occurred inside a logging statement
               that was generated from within another logging statement's format() call.
            * Fix for PyWin32 dependency specification (explicitly require PyWin32)
            * Ability to specify owner and permissions (mode) of rollover files [Unix only]
```

### Comparing `concurrent-log-handler-0.9.8/README.md` & `concurrent-log-handler-0.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,16 @@
 
 This may mean that if you change the logging settings at any point you may need to 
 restart your app service so that all processes are using the same settings at the same time.
 
 
 ## Change Log ##
 
+- 0.9.9: Fix Python 2 compatibility broken in last release 
+
 - 0.9.8: Bug fixes and permission features
    * Fix for issue #4 - AttributeError: 'NoneType' object has no attribute 'write'
       This error could be caused if a rollover occurred inside a logging statement
       that was generated from within another logging statement's format() call.
    * Fix for PyWin32 dependency specification (explicitly require PyWin32)
    * Ability to specify owner and permissions (mode) of rollover files [Unix only]
```

### Comparing `concurrent-log-handler-0.9.8/setup.py` & `concurrent-log-handler-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,16 @@
     logging.config.fileConfig("logging.ini")
     log = logging.getLogger()
     log.info("Here is a very exciting log message, just for you")
 
 
 Change Log
 ==========
+- 0.9.9: Fix Python 2 compatibility broken in last release
+
 - 0.9.8: Bug fixes and permission features
    * Fix for issue #4 - AttributeError: 'NoneType' object has no attribute 'write'
       This error could be caused if a rollover occurred inside a logging statement
       that was generated from within another logging statement's format() call.
    * Fix for PyWin32 dependency specification (explicitly require PyWin32)
    * Ability to specify owner and permissions (mode) of rollover files [Unix only]
 
@@ -266,15 +268,15 @@
 
 from ez_setup import use_setuptools
 
 use_setuptools()
 
 from setuptools import setup
 
-VERSION = "0.9.8"
+VERSION = "0.9.9"
 classifiers = """\
 Development Status :: 4 - Beta
 Topic :: System :: Logging
 Operating System :: POSIX
 Operating System :: Microsoft :: Windows
 Programming Language :: Python
 Programming Language :: Python :: 2.6
```

### Comparing `concurrent-log-handler-0.9.8/src/concurrent_log_handler/portalocker.py` & `concurrent-log-handler-0.9.9/src/concurrent_log_handler/portalocker.py`

 * *Files identical despite different names*

### Comparing `concurrent-log-handler-0.9.8/src/concurrent_log_handler/queue.py` & `concurrent-log-handler-0.9.9/src/concurrent_log_handler/queue.py`

 * *Files identical despite different names*

### Comparing `concurrent-log-handler-0.9.8/src/concurrent_log_handler/__init__.py` & `concurrent-log-handler-0.9.9/src/concurrent_log_handler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             return random.Random().getrandbits(nb)
 
 try:
     import gzip
 except ImportError:
     gzip = None
 
-__version__ = '0.9.8'
+__version__ = '0.9.9'
 __author__ = "Preston Landers <planders@gmail.com>"
 # __author__ = "Lowell Alleman"
 __all__ = [
     "ConcurrentRotatingFileHandler",
 ]
 
 
@@ -174,14 +174,17 @@
         self._debug = debug
         self.use_gzip = True if gzip and use_gzip else False
 
         # Absolute file name handling done by FileHandler since Python 2.5
         super(ConcurrentRotatingFileHandler, self).__init__(
             filename, mode, encoding=encoding, delay=delay)
 
+        if not hasattr(self, "terminator"):
+            self.terminator = "\n"
+
         if owner and os.chown and pwd and grp:
             self._set_uid = pwd.getpwnam(self.owner[0]).pw_uid
             self._set_gid = grp.getgrnam(self.owner[1]).gr_gid
 
         self._open_lockfile()
 
     def _open_lockfile(self):
```

### Comparing `concurrent-log-handler-0.9.8/src/concurrent_log_handler.egg-info/PKG-INFO` & `concurrent-log-handler-0.9.9/src/concurrent_log_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: concurrent-log-handler
-Version: 0.9.8
+Version: 0.9.9
 Summary: RotatingFileHandler replacement with concurrency, gzip and Windows support
 Home-page: https://github.com/Preston-Landers/concurrent-log-handler
 Author: Preston Landers
 Author-email: planders@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description-Content-Type: UNKNOWN
 Description: 
@@ -140,14 +140,16 @@
             logging.config.fileConfig("logging.ini")
             log = logging.getLogger()
             log.info("Here is a very exciting log message, just for you")
         
         
         Change Log
         ==========
+        - 0.9.9: Fix Python 2 compatibility broken in last release
+        
         - 0.9.8: Bug fixes and permission features
            * Fix for issue #4 - AttributeError: 'NoneType' object has no attribute 'write'
               This error could be caused if a rollover occurred inside a logging statement
               that was generated from within another logging statement's format() call.
            * Fix for PyWin32 dependency specification (explicitly require PyWin32)
            * Ability to specify owner and permissions (mode) of rollover files [Unix only]
```

