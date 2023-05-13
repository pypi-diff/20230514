# Comparing `tmp/asyncio_task_logger-0.0.1.tar.gz` & `tmp/asyncio_task_logger-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio_task_logger-0.0.1.tar", last modified: Sat May 13 21:21:53 2023, max compression
+gzip compressed data, was "asyncio_task_logger-0.0.2.tar", last modified: Sat May 13 22:47:00 2023, max compression
```

## Comparing `asyncio_task_logger-0.0.1.tar` & `asyncio_task_logger-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)        0 2023-05-13 21:21:52.109675 asyncio_task_logger-0.0.1/
--rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)      645 2023-05-13 21:21:53.137616 asyncio_task_logger-0.0.1/PKG-INFO
--rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)      762 2023-05-13 21:21:47.000000 asyncio_task_logger-0.0.1/pyproject.toml
--rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)       38 2023-05-13 21:21:53.149615 asyncio_task_logger-0.0.1/setup.cfg
-drwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)        0 2023-05-13 21:21:52.111673 asyncio_task_logger-0.0.1/src/
-drwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)        0 2023-05-13 21:21:52.243077 asyncio_task_logger-0.0.1/src/asyncio_task_logger.egg-info/
--rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)      645 2023-05-13 21:21:52.000000 asyncio_task_logger-0.0.1/src/asyncio_task_logger.egg-info/PKG-INFO
--rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)      281 2023-05-13 21:21:52.000000 asyncio_task_logger-0.0.1/src/asyncio_task_logger.egg-info/SOURCES.txt
--rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)        1 2023-05-13 21:21:52.000000 asyncio_task_logger-0.0.1/src/asyncio_task_logger.egg-info/dependency_links.txt
--rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)       22 2023-05-13 21:21:52.000000 asyncio_task_logger-0.0.1/src/asyncio_task_logger.egg-info/top_level.txt
-drwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)        0 2023-05-13 21:21:52.336080 asyncio_task_logger-0.0.1/src/task_logger_pinghajen/
--rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)        0 2023-05-13 21:21:53.000000 asyncio_task_logger-0.0.1/src/task_logger_pinghajen/__init__.py
--rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)     1836 2023-05-13 18:36:30.000000 asyncio_task_logger-0.0.1/src/task_logger_pinghajen/task_logger.py
+drwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)        0 2023-05-13 22:46:59.437932 asyncio_task_logger-0.0.2/
+-rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)     1064 2023-05-13 21:49:06.000000 asyncio_task_logger-0.0.2/LICENSE
+-rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)     1323 2023-05-13 22:47:00.513825 asyncio_task_logger-0.0.2/PKG-INFO
+-rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)      655 2023-05-13 21:50:21.000000 asyncio_task_logger-0.0.2/README.md
+-rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)      762 2023-05-13 22:45:41.000000 asyncio_task_logger-0.0.2/pyproject.toml
+-rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)       38 2023-05-13 22:47:00.529825 asyncio_task_logger-0.0.2/setup.cfg
+drwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)        0 2023-05-13 22:46:59.448537 asyncio_task_logger-0.0.2/src/
+drwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)        0 2023-05-13 22:46:59.535865 asyncio_task_logger-0.0.2/src/asyncio_task_logger/
+-rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)        0 2023-05-13 18:37:09.000000 asyncio_task_logger-0.0.2/src/asyncio_task_logger/__init__.py
+-rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)     1836 2023-05-13 18:36:30.000000 asyncio_task_logger-0.0.2/src/asyncio_task_logger/task_logger.py
+drwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)        0 2023-05-13 22:46:59.628751 asyncio_task_logger-0.0.2/src/asyncio_task_logger.egg-info/
+-rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)     1323 2023-05-13 22:47:00.000000 asyncio_task_logger-0.0.2/src/asyncio_task_logger.egg-info/PKG-INFO
+-rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)      295 2023-05-13 22:47:00.000000 asyncio_task_logger-0.0.2/src/asyncio_task_logger.egg-info/SOURCES.txt
+-rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)        1 2023-05-13 22:47:00.000000 asyncio_task_logger-0.0.2/src/asyncio_task_logger.egg-info/dependency_links.txt
+-rwxr-xr-x   0 pinghajen  (1000) pinghajen  (1000)       20 2023-05-13 22:47:00.000000 asyncio_task_logger-0.0.2/src/asyncio_task_logger.egg-info/top_level.txt
```

### Comparing `asyncio_task_logger-0.0.1/pyproject.toml` & `asyncio_task_logger-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asyncio_task_logger"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Quantlane", email="code@quantlane.com" },
   { name="Jeremiah Payne", email="jeremiah@pinghajen.com" },
 ]
 description = "Allows logging on long running tasks that throw an exception but are still loaded into memory"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `asyncio_task_logger-0.0.1/src/task_logger_pinghajen/task_logger.py` & `asyncio_task_logger-0.0.2/src/asyncio_task_logger/task_logger.py`

 * *Files identical despite different names*

