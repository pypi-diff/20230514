# Comparing `tmp/ctfpipshell-0.0.3.tar.gz` & `tmp/ctfpipshell-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctfpipshell-0.0.3.tar", last modified: Sun May 14 13:35:06 2023, max compression
+gzip compressed data, was "ctfpipshell-0.0.4.tar", last modified: Sun May 14 14:04:49 2023, max compression
```

## Comparing `ctfpipshell-0.0.3.tar` & `ctfpipshell-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 13:35:06.433378 ctfpipshell-0.0.3/
--rw-rw-rw-   0        0        0     1084 2023-05-14 05:21:25.000000 ctfpipshell-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      388 2023-05-14 13:35:06.432378 ctfpipshell-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-05-14 05:21:25.000000 ctfpipshell-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 13:35:06.410372 ctfpipshell-0.0.3/ctfpipshell/
--rw-rw-rw-   0        0        0        0 2023-05-14 05:22:06.000000 ctfpipshell-0.0.3/ctfpipshell/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-14 05:22:17.000000 ctfpipshell-0.0.3/ctfpipshell/ctfpipshell.py
-drwxrwxrwx   0        0        0        0 2023-05-14 13:35:06.429377 ctfpipshell-0.0.3/ctfpipshell.egg-info/
--rw-rw-rw-   0        0        0      388 2023-05-14 13:35:06.000000 ctfpipshell-0.0.3/ctfpipshell.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-05-14 13:35:06.000000 ctfpipshell-0.0.3/ctfpipshell.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 13:35:06.000000 ctfpipshell-0.0.3/ctfpipshell.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-14 13:35:06.000000 ctfpipshell-0.0.3/ctfpipshell.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-14 13:35:06.000000 ctfpipshell-0.0.3/ctfpipshell.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 13:35:06.433378 ctfpipshell-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      781 2023-05-14 13:35:01.000000 ctfpipshell-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:04:49.764313 ctfpipshell-0.0.4/
+-rw-rw-rw-   0        0        0     1084 2023-05-14 05:21:25.000000 ctfpipshell-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      388 2023-05-14 14:04:49.763312 ctfpipshell-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-05-14 05:21:25.000000 ctfpipshell-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 14:04:49.739308 ctfpipshell-0.0.4/ctfpipshell/
+-rw-rw-rw-   0        0        0        0 2023-05-14 05:22:06.000000 ctfpipshell-0.0.4/ctfpipshell/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-14 05:22:17.000000 ctfpipshell-0.0.4/ctfpipshell/ctfpipshell.py
+drwxrwxrwx   0        0        0        0 2023-05-14 14:04:49.760313 ctfpipshell-0.0.4/ctfpipshell.egg-info/
+-rw-rw-rw-   0        0        0      388 2023-05-14 14:04:49.000000 ctfpipshell-0.0.4/ctfpipshell.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-05-14 14:04:49.000000 ctfpipshell-0.0.4/ctfpipshell.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 14:04:49.000000 ctfpipshell-0.0.4/ctfpipshell.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-14 14:04:49.000000 ctfpipshell-0.0.4/ctfpipshell.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-14 14:04:49.000000 ctfpipshell-0.0.4/ctfpipshell.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 14:04:49.764313 ctfpipshell-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-05-14 14:04:29.000000 ctfpipshell-0.0.4/setup.py
```

### Comparing `ctfpipshell-0.0.3/LICENSE` & `ctfpipshell-0.0.4/LICENSE`

 * *Files identical despite different names*

