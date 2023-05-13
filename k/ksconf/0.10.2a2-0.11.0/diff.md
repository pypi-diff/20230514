# Comparing `tmp/ksconf-0.10.2a2.tar.gz` & `tmp/ksconf-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksconf-0.10.2a2.tar", last modified: Sat May 13 16:38:53 2023, max compression
+gzip compressed data, was "ksconf-0.11.0.tar", last modified: Sat May 13 23:31:04 2023, max compression
```

## Comparing `ksconf-0.10.2a2.tar` & `ksconf-0.11.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.219379 ksconf-0.10.2a2/ksconf/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.219379 ksconf-0.10.2a2/ksconf/app/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/app/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/app/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12491 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/app/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.219379 ksconf-0.10.2a2/ksconf/builder/
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/builder/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/builder/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/builder/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/ksconf/commands/
--rw-r--r--   0 runner    (1001) docker     (123)    22120 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    22959 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/promote.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/restexport.py
--rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/restpublish.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/unarchive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/xmlformat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/ksconf/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/conf/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/conf/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/conf/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/conf/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/ksconf/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/setup_entrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/ksconf/util/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/util/completers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/util/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/util/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/util/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/ksconf/vc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/vc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/vc/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/xmlformat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.219379 ksconf-0.10.2a2/ksconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 16:38:38.000000 ksconf-0.10.2a2/ksconf.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:31:04.414942 ksconf-0.11.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-13 23:30:40.000000 ksconf-0.11.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-13 23:31:04.414942 ksconf-0.11.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-13 23:30:40.000000 ksconf-0.11.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:31:04.410942 ksconf-0.11.0/ksconf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-13 23:31:04.000000 ksconf-0.11.0/ksconf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:31:04.410942 ksconf-0.11.0/ksconf/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/app/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/app/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/app/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:31:04.410942 ksconf-0.11.0/ksconf/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/builder/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/builder/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/builder/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:31:04.414942 ksconf-0.11.0/ksconf/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)    22120 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22959 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/promote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/restexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/restpublish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/unarchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/commands/xmlformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:31:04.414942 ksconf-0.11.0/ksconf/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/conf/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/conf/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/conf/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/conf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:31:04.414942 ksconf-0.11.0/ksconf/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14340 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/setup_entrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:31:04.414942 ksconf-0.11.0/ksconf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/util/completers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/util/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/util/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/util/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:31:04.414942 ksconf-0.11.0/ksconf/vc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/vc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/vc/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-13 23:30:40.000000 ksconf-0.11.0/ksconf/xmlformat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:31:04.410942 ksconf-0.11.0/ksconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-13 23:31:04.000000 ksconf-0.11.0/ksconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-13 23:31:04.000000 ksconf-0.11.0/ksconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 23:31:04.000000 ksconf-0.11.0/ksconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-13 23:31:04.000000 ksconf-0.11.0/ksconf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-13 23:31:04.000000 ksconf-0.11.0/ksconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 23:31:04.000000 ksconf-0.11.0/ksconf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 23:30:50.000000 ksconf-0.11.0/ksconf.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-13 23:31:04.414942 ksconf-0.11.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-13 23:30:40.000000 ksconf-0.11.0/setup.py
```

### Comparing `ksconf-0.10.2a2/LICENSE` & `ksconf-0.11.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/PKG-INFO` & `ksconf-0.11.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksconf
-Version: 0.10.2a2
+Version: 0.11.0
 Summary: KSCONF: Ksconf Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
```

### Comparing `ksconf-0.10.2a2/README.md` & `ksconf-0.11.0/README.md`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/__init__.py` & `ksconf-0.11.0/ksconf/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/__main__.py` & `ksconf-0.11.0/ksconf/__main__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/app/__init__.py` & `ksconf-0.11.0/ksconf/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/app/deploy.py` & `ksconf-0.11.0/ksconf/app/deploy.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/app/facts.py` & `ksconf-0.11.0/ksconf/app/facts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+""" Splunk Application facts:
 
+Easily collect Splunk app name, version, label, and other nuggets from ``app.conf``
+
+"""
 
 from __future__ import absolute_import, annotations, unicode_literals
 
 from collections import defaultdict
 from dataclasses import asdict, dataclass, field, fields
 from io import StringIO
 from os import fspath
```

### Comparing `ksconf-0.10.2a2/ksconf/app/manifest.py` & `ksconf-0.11.0/ksconf/app/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,18 +184,17 @@
                 yield f
 
     def check_paths(self):
         """ Check for dangerous paths in the archive. """
         for file in self.files:
             path = file.path
             if path.is_absolute():
-                raise AppManifestContentError(f"Found an absolute path {file.path}")
-            if ".." in path.parts or "~" in path.parts or \
-                    path.parts[0].endswith("~"):
-                raise AppManifestContentError(f"Found questionable path manipulation in '{file.path}'")
+                raise AppArchiveContentError(f"Found an absolute path {file.path}")
+            if ".." in path.parts or path.parts[0].startswith("~"):
+                raise AppArchiveContentError(f"Found questionable path manipulation in '{file.path}'")
 
 
 @dataclass
 class StoredArchiveManifest:
     """
     Stored manifest for a tarball.  Typically the manifest file lives in the
     same directory as the archive.  Details around the naming, storage, and
@@ -234,15 +233,15 @@
             "hash": self.hash,
             "manifest": self.manifest.to_dict(),
         }
 
     def write_json_manifest(self, manifest_file: Path):
         data = self.to_dict()
         with open(manifest_file, "w") as fp:
-            json.dump(data, fp)
+            json.dump(data, fp, indent=1)
 
     @classmethod
     def read_json_manifest(cls, manifest_file: Path) -> "StoredArchiveManifest":
         with open(manifest_file) as fp:
             data = json.load(fp)
         return cls.from_dict(data)
 
@@ -300,14 +299,16 @@
 def create_manifest_from_archive(
         archive_file: Path,
         manifest_file: Path,
         manifest: AppManifest) -> StoredArchiveManifest:
     """
     Create a new stored manifest file based on a given archive.
     """
+    if manifest_file is None:
+        manifest_file = get_stored_manifest_name(archive_file)
     sam = StoredArchiveManifest.from_file(archive_file, manifest)
     sam.write_json_manifest(manifest_file)
     return sam
 
 
 def load_manifest_for_archive(
         archive: Path,
```

### Comparing `ksconf-0.10.2a2/ksconf/archive.py` & `ksconf-0.11.0/ksconf/archive.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/builder/__init__.py` & `ksconf-0.11.0/ksconf/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/builder/cache.py` & `ksconf-0.11.0/ksconf/builder/cache.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/builder/core.py` & `ksconf-0.11.0/ksconf/builder/core.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/builder/steps.py` & `ksconf-0.11.0/ksconf/builder/steps.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/cli.py` & `ksconf-0.11.0/ksconf/cli.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/combine.py` & `ksconf-0.11.0/ksconf/combine.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/__init__.py` & `ksconf-0.11.0/ksconf/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/check.py` & `ksconf-0.11.0/ksconf/commands/check.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/combine.py` & `ksconf-0.11.0/ksconf/commands/combine.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/diff.py` & `ksconf-0.11.0/ksconf/commands/diff.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/filter.py` & `ksconf-0.11.0/ksconf/commands/filter.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/merge.py` & `ksconf-0.11.0/ksconf/commands/merge.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/minimize.py` & `ksconf-0.11.0/ksconf/commands/minimize.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/package.py` & `ksconf-0.11.0/ksconf/commands/package.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/promote.py` & `ksconf-0.11.0/ksconf/commands/promote.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/restexport.py` & `ksconf-0.11.0/ksconf/commands/restexport.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/restpublish.py` & `ksconf-0.11.0/ksconf/commands/restpublish.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/snapshot.py` & `ksconf-0.11.0/ksconf/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/sort.py` & `ksconf-0.11.0/ksconf/commands/sort.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/unarchive.py` & `ksconf-0.11.0/ksconf/commands/unarchive.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/commands/xmlformat.py` & `ksconf-0.11.0/ksconf/commands/xmlformat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/compat.py` & `ksconf-0.11.0/ksconf/compat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/conf/delta.py` & `ksconf-0.11.0/ksconf/conf/delta.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/conf/merge.py` & `ksconf-0.11.0/ksconf/conf/merge.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/conf/meta.py` & `ksconf-0.11.0/ksconf/conf/meta.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/conf/parser.py` & `ksconf-0.11.0/ksconf/conf/parser.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/consts.py` & `ksconf-0.11.0/ksconf/consts.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/filter.py` & `ksconf-0.11.0/ksconf/filter.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/layer.py` & `ksconf-0.11.0/ksconf/layer.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/package.py` & `ksconf-0.11.0/ksconf/package.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import hashlib
 import os
 import re
 import shutil
 import tarfile
 import tempfile
+from typing import TextIO
 
+from ksconf.app.manifest import AppManifest
 from ksconf.combine import LayerCombiner
 from ksconf.conf.merge import merge_app_local, merge_conf_dicts
 from ksconf.conf.parser import conf_attr_boolean, parse_conf, update_conf
 from ksconf.consts import KSCONF_DEBUG
 from ksconf.vc.git import git_cmd
 
 
@@ -48,15 +50,15 @@
 
 class PackagingException(Exception):
     pass
 
 
 class AppPackager:
 
-    def __init__(self, src_path, app_name, output):
+    def __init__(self, src_path, app_name: str, output: TextIO):
         self.src_path = src_path
         self.app_name = app_name
         self.build_dir = None
         self.app_dir = None
         self.output = output
         self._var_magic = None
 
@@ -224,14 +226,24 @@
             self.output.write(f"Creating archive:  {filename}\n")
 
         normalize_directory_mtime(self.app_dir)
         with tarfile.open(filename, mode="w:gz") as spl:
             spl.add(self.app_dir, arcname=self.app_name)
         return filename
 
+    def make_manifest(self, calculate_hash=True) -> AppManifest:
+        """
+        Create a manifest of the app's contents.
+        """
+        app_name = self.expand_var(self.app_name)
+        manifest = AppManifest.from_filesystem(self.app_dir, name=app_name,
+                                               calculate_hash=calculate_hash)
+        manifest.source = self.src_path
+        return manifest
+
     def __enter__(self):
         self.build_dir = tempfile.mkdtemp("-ksconf-package-build")
         if self.app_name == "." or "{{" in self.app_name:
             # Use a placeholder app name, otherwise build_dir == app_dir
             self.app_dir = os.path.join(self.build_dir, "app")
         else:
             self.app_dir = os.path.join(self.build_dir, self.app_name)
```

### Comparing `ksconf-0.10.2a2/ksconf/setup_entrypoints.py` & `ksconf-0.11.0/ksconf/setup_entrypoints.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/util/__init__.py` & `ksconf-0.11.0/ksconf/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/util/compare.py` & `ksconf-0.11.0/ksconf/util/compare.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/util/completers.py` & `ksconf-0.11.0/ksconf/util/completers.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/util/file.py` & `ksconf-0.11.0/ksconf/util/file.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/util/rest.py` & `ksconf-0.11.0/ksconf/util/rest.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/util/terminal.py` & `ksconf-0.11.0/ksconf/util/terminal.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/vc/git.py` & `ksconf-0.11.0/ksconf/vc/git.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf/xmlformat.py` & `ksconf-0.11.0/ksconf/xmlformat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf.egg-info/PKG-INFO` & `ksconf-0.11.0/ksconf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksconf
-Version: 0.10.2a2
+Version: 0.11.0
 Summary: KSCONF: Ksconf Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
```

### Comparing `ksconf-0.10.2a2/ksconf.egg-info/SOURCES.txt` & `ksconf-0.11.0/ksconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/ksconf.egg-info/entry_points.txt` & `ksconf-0.11.0/ksconf.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a2/setup.py` & `ksconf-0.11.0/setup.py`

 * *Files identical despite different names*

