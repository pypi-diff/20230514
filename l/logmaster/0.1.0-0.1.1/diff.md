# Comparing `tmp/logmaster-0.1.0.tar.gz` & `tmp/logmaster-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logmaster-0.1.0.tar", last modified: Sat May 13 20:20:20 2023, max compression
+gzip compressed data, was "logmaster-0.1.1.tar", last modified: Sun May 14 14:46:58 2023, max compression
```

## Comparing `logmaster-0.1.0.tar` & `logmaster-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 20:20:20.748018 logmaster-0.1.0/
--rw-rw-rw-   0        0        0     1083 2023-05-08 22:14:25.000000 logmaster-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1336 2023-05-13 20:20:20.748018 logmaster-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1031 2023-05-11 15:57:31.000000 logmaster-0.1.0/README.md
--rw-rw-rw-   0        0        0      109 2023-05-09 16:02:47.000000 logmaster-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      432 2023-05-13 20:20:20.753019 logmaster-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-13 20:20:20.697021 logmaster-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-13 20:20:20.742023 logmaster-0.1.0/src/logmaster.egg-info/
--rw-rw-rw-   0        0        0     1336 2023-05-13 20:20:20.000000 logmaster-0.1.0/src/logmaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-05-13 20:20:20.000000 logmaster-0.1.0/src/logmaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 20:20:20.000000 logmaster-0.1.0/src/logmaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 20:20:20.000000 logmaster-0.1.0/src/logmaster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 14:46:58.257327 logmaster-0.1.1/
+-rw-rw-rw-   0        0        0     1083 2023-05-08 22:14:25.000000 logmaster-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1336 2023-05-14 14:46:58.258326 logmaster-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1031 2023-05-11 15:57:31.000000 logmaster-0.1.1/README.md
+-rw-rw-rw-   0        0        0      109 2023-05-09 16:02:47.000000 logmaster-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      432 2023-05-14 14:46:58.262321 logmaster-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 14:46:58.172322 logmaster-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-14 14:46:58.211325 logmaster-0.1.1/src/logmaster/
+-rw-rw-rw-   0        0        0      993 2023-05-14 14:45:28.000000 logmaster-0.1.1/src/logmaster/__init__.py
+-rw-rw-rw-   0        0        0     1743 2023-05-09 15:46:03.000000 logmaster-0.1.1/src/logmaster/logger.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:46:58.254321 logmaster-0.1.1/src/logmaster.egg-info/
+-rw-rw-rw-   0        0        0     1336 2023-05-14 14:46:58.000000 logmaster-0.1.1/src/logmaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-05-14 14:46:58.000000 logmaster-0.1.1/src/logmaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:46:58.000000 logmaster-0.1.1/src/logmaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-14 14:46:58.000000 logmaster-0.1.1/src/logmaster.egg-info/top_level.txt
```

### Comparing `logmaster-0.1.0/LICENSE` & `logmaster-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logmaster-0.1.0/PKG-INFO` & `logmaster-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logmaster
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple logging library for Python
 Home-page: https://github.com/W1L7dev/logmaster
 Author: W1L7dev
 Author-email: w1l7dev@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `logmaster-0.1.0/README.md` & `logmaster-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `logmaster-0.1.0/src/logmaster.egg-info/PKG-INFO` & `logmaster-0.1.1/src/logmaster.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logmaster
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple logging library for Python
 Home-page: https://github.com/W1L7dev/logmaster
 Author: W1L7dev
 Author-email: w1l7dev@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

