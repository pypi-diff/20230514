# Comparing `tmp/usr_agent_rnd_rs-0.0.5.tar.gz` & `tmp/usr_agent_rnd_rs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usr_agent_rnd_rs-0.0.5.tar", last modified: Fri Mar 17 09:03:46 2023, max compression
+gzip compressed data, was "usr_agent_rnd_rs-0.0.6.tar", last modified: Sun May 14 17:29:45 2023, max compression
```

## Comparing `usr_agent_rnd_rs-0.0.5.tar` & `usr_agent_rnd_rs-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 09:03:46.884663 usr_agent_rnd_rs-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-03-17 08:14:10.000000 usr_agent_rnd_rs-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      807 2023-03-17 09:03:46.869678 usr_agent_rnd_rs-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-03-17 09:02:58.000000 usr_agent_rnd_rs-0.0.5/README.md
--rw-rw-rw-   0        0        0      609 2023-03-17 09:03:06.000000 usr_agent_rnd_rs-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-17 09:03:46.885664 usr_agent_rnd_rs-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-17 09:03:46.770597 usr_agent_rnd_rs-0.0.5/usr_agent_rnd_rs/
--rw-rw-rw-   0        0        0        0 2023-03-17 08:10:53.000000 usr_agent_rnd_rs-0.0.5/usr_agent_rnd_rs/__init__.py
--rw-rw-rw-   0        0        0     6261 2023-03-17 09:00:30.000000 usr_agent_rnd_rs-0.0.5/usr_agent_rnd_rs/useragent.py
-drwxrwxrwx   0        0        0        0 2023-03-17 09:03:46.841690 usr_agent_rnd_rs-0.0.5/usr_agent_rnd_rs.egg-info/
--rw-rw-rw-   0        0        0      807 2023-03-17 09:03:46.000000 usr_agent_rnd_rs-0.0.5/usr_agent_rnd_rs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-03-17 09:03:46.000000 usr_agent_rnd_rs-0.0.5/usr_agent_rnd_rs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 09:03:46.000000 usr_agent_rnd_rs-0.0.5/usr_agent_rnd_rs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-17 09:03:46.000000 usr_agent_rnd_rs-0.0.5/usr_agent_rnd_rs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-14 17:29:45.924412 usr_agent_rnd_rs-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-03-17 08:14:10.000000 usr_agent_rnd_rs-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      677 2023-05-14 17:29:45.922411 usr_agent_rnd_rs-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-03-17 11:08:30.000000 usr_agent_rnd_rs-0.0.6/README.md
+-rw-rw-rw-   0        0        0      609 2023-03-17 11:08:08.000000 usr_agent_rnd_rs-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-14 17:29:45.924412 usr_agent_rnd_rs-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 17:29:45.921411 usr_agent_rnd_rs-0.0.6/usr_agent_rnd_rs.egg-info/
+-rw-rw-rw-   0        0        0      677 2023-05-14 17:29:45.000000 usr_agent_rnd_rs-0.0.6/usr_agent_rnd_rs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-05-14 17:29:45.000000 usr_agent_rnd_rs-0.0.6/usr_agent_rnd_rs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 17:29:45.000000 usr_agent_rnd_rs-0.0.6/usr_agent_rnd_rs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-14 17:29:45.000000 usr_agent_rnd_rs-0.0.6/usr_agent_rnd_rs.egg-info/top_level.txt
```

### Comparing `usr_agent_rnd_rs-0.0.5/LICENSE` & `usr_agent_rnd_rs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `usr_agent_rnd_rs-0.0.5/pyproject.toml` & `usr_agent_rnd_rs-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "usr_agent_rnd_rs"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Rosario Sensale", email="pcassistenzatecnica@gmail.com" },
 ]
 description = "A simple user agent random"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

