# Comparing `tmp/ksconf-0.10.2a1.tar.gz` & `tmp/ksconf-0.10.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksconf-0.10.2a1.tar", last modified: Sat May 13 00:47:32 2023, max compression
+gzip compressed data, was "ksconf-0.10.2a2.tar", last modified: Sat May 13 16:38:53 2023, max compression
```

## Comparing `ksconf-0.10.2a1.tar` & `ksconf-0.10.2a2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:32.916813 ksconf-0.10.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-13 00:47:32.916813 ksconf-0.10.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:32.912813 ksconf-0.10.2a1/ksconf/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-13 00:47:32.000000 ksconf-0.10.2a1/ksconf/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:32.912813 ksconf-0.10.2a1/ksconf/app/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/app/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/app/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/app/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:32.912813 ksconf-0.10.2a1/ksconf/builder/
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/builder/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/builder/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/builder/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:32.912813 ksconf-0.10.2a1/ksconf/commands/
--rw-r--r--   0 runner    (1001) docker     (123)    22120 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    22959 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/promote.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/restexport.py
--rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/restpublish.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/unarchive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/commands/xmlformat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:32.916813 ksconf-0.10.2a1/ksconf/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/conf/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/conf/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/conf/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/conf/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:32.916813 ksconf-0.10.2a1/ksconf/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/setup_entrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:32.916813 ksconf-0.10.2a1/ksconf/util/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/util/completers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/util/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/util/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/util/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:32.916813 ksconf-0.10.2a1/ksconf/vc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/vc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/vc/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/ksconf/xmlformat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 00:47:32.912813 ksconf-0.10.2a1/ksconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-13 00:47:32.000000 ksconf-0.10.2a1/ksconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-13 00:47:32.000000 ksconf-0.10.2a1/ksconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 00:47:32.000000 ksconf-0.10.2a1/ksconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-13 00:47:32.000000 ksconf-0.10.2a1/ksconf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-13 00:47:32.000000 ksconf-0.10.2a1/ksconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 00:47:32.000000 ksconf-0.10.2a1/ksconf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 00:47:17.000000 ksconf-0.10.2a1/ksconf.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-13 00:47:32.916813 ksconf-0.10.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-13 00:47:02.000000 ksconf-0.10.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.219379 ksconf-0.10.2a2/ksconf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.219379 ksconf-0.10.2a2/ksconf/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/app/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/app/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12491 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/app/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.219379 ksconf-0.10.2a2/ksconf/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/builder/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/builder/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/builder/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/ksconf/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)    22120 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22959 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/promote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/restexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/restpublish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/unarchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/commands/xmlformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/ksconf/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/conf/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/conf/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/conf/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/conf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/ksconf/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/setup_entrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/ksconf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/util/completers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/util/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/util/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/util/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/ksconf/vc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/vc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/vc/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/ksconf/xmlformat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:38:53.219379 ksconf-0.10.2a2/ksconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 16:38:53.000000 ksconf-0.10.2a2/ksconf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 16:38:38.000000 ksconf-0.10.2a2/ksconf.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-13 16:38:53.223379 ksconf-0.10.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-13 16:38:27.000000 ksconf-0.10.2a2/setup.py
```

### Comparing `ksconf-0.10.2a1/LICENSE` & `ksconf-0.10.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/PKG-INFO` & `ksconf-0.10.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksconf
-Version: 0.10.2a1
+Version: 0.10.2a2
 Summary: KSCONF: Ksconf Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
```

### Comparing `ksconf-0.10.2a1/README.md` & `ksconf-0.10.2a2/README.md`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/__init__.py` & `ksconf-0.10.2a2/ksconf/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/__main__.py` & `ksconf-0.10.2a2/ksconf/__main__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/app/__init__.py` & `ksconf-0.10.2a2/ksconf/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/app/deploy.py` & `ksconf-0.10.2a2/ksconf/app/deploy.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/app/facts.py` & `ksconf-0.10.2a2/ksconf/app/facts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 from __future__ import absolute_import, annotations, unicode_literals
 
 from collections import defaultdict
-from dataclasses import asdict, dataclass, field
+from dataclasses import asdict, dataclass, field, fields
 from io import StringIO
 from os import fspath
 from pathlib import Path
 from typing import ClassVar
 
 from ksconf.app.manifest import AppArchiveContentError
 from ksconf.archive import extract_archive, gaf_filter_name_like
@@ -27,25 +27,25 @@
     id: str = None
     version: str = None
     author: str = None
     description: str = None
     state: str = None
     build: int = None
 
-    is_configured: bool = field(init=False)
-    allows_disable: bool = field(init=False)
-    state_change_requires_restart: bool = field(init=False)
-
-    install_source_checksum: str = field(init=False)
-    install_source_local_checksum: str = field(init=False)
-    check_for_updates: bool = field(init=False)
-    is_visible: bool = field(init=False)
+    is_configured: bool = field(init=False, default=None)
+    allows_disable: bool = field(init=False, default=None)
+    state_change_requires_restart: bool = field(init=False, default=None)
+
+    install_source_checksum: str = field(init=False, default=None)
+    install_source_local_checksum: str = field(init=False, default=None)
+    check_for_updates: bool = field(init=False, default=None)
+    is_visible: bool = field(init=False, default=None)
 
-    deployer_lookups_push_mode: str = field(init=False)
-    deployer_push_mode: str = field(init=False)
+    deployer_lookups_push_mode: str = field(init=False, default=None)
+    deployer_push_mode: str = field(init=False, default=None)
 
     _conf_translate_pairs: ClassVar[List[Tuple[str, List[str]]]] = [
         ("launcher", [
             "version",
             "author",
             "description"]),
         ("install", [
@@ -68,24 +68,30 @@
             "deployer_push_mode"]
          ),
     ]
 
     def to_dict(self) -> dict:
         return asdict(self)
 
+    def to_tiny_dict(self, *keep_attrs) -> dict:
+        """ Return dict representation, discarding the Nones """
+        return {k: v for k, v in asdict(self).items() if v is not None or k in keep_attrs}
+
     @classmethod
     def from_conf(cls, name, conf: ConfType) -> "AppFacts":
         """
         Create AppFacts from an app.conf configuration content.
         """
         new = cls(name)
 
+        type_mapping = {f.name: f.type for f in fields(cls) if f.type in ("bool", "int")}
+
         def convert_attr(attr_name, value):
             # XXX: Is there a better approach for dataclasses?  fields() returns a list
-            data_type = cls.__annotations__.get(attr_name, None)
+            data_type = type_mapping.get(attr_name, None)
             convert_function = None
             if data_type == "bool":
                 convert_function = conf_attr_boolean
             elif data_type == "int":
                 convert_function = int
             else:
                 return value
```

### Comparing `ksconf-0.10.2a1/ksconf/app/manifest.py` & `ksconf-0.10.2a2/ksconf/app/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,15 @@
     been changed since the ``manifest_file`` was written.
 
     If no ``manifest_file`` is provided, the default manifest naming convention
     will be applied where the ``manifest_file`` is stored in the same directory
     as ``archive``.
     """
     # XXX: Add optimization to check if archive is newer than manifest_file, assume old
+    archive = Path(archive)
     manifest = None
 
     if manifest_file is None and read_manifest or write_manifest:
         manifest_file = get_stored_manifest_name(archive)
 
     if read_manifest and manifest_file.exists():
         try:
@@ -339,11 +340,15 @@
         except AppManifestStorageError as e:
             print(f"WARN:   loading stored manifest failed:  {e}")
 
     if manifest is None:
         print(f"Calculating manifest for {archive}")
         manifest = AppManifest.from_archive(archive)
 
+        # We assume that a previously stored manifest has already undergone the
+        # path check.  Checks should be redone from within the extraction process.
+        manifest.check_paths()
+
         if write_manifest:
             create_manifest_from_archive(archive, manifest_file, manifest)
 
     return manifest
```

### Comparing `ksconf-0.10.2a1/ksconf/archive.py` & `ksconf-0.10.2a2/ksconf/archive.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/builder/__init__.py` & `ksconf-0.10.2a2/ksconf/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/builder/cache.py` & `ksconf-0.10.2a2/ksconf/builder/cache.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/builder/core.py` & `ksconf-0.10.2a2/ksconf/builder/core.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/builder/steps.py` & `ksconf-0.10.2a2/ksconf/builder/steps.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/cli.py` & `ksconf-0.10.2a2/ksconf/cli.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/combine.py` & `ksconf-0.10.2a2/ksconf/combine.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/__init__.py` & `ksconf-0.10.2a2/ksconf/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/check.py` & `ksconf-0.10.2a2/ksconf/commands/check.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/combine.py` & `ksconf-0.10.2a2/ksconf/commands/combine.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/diff.py` & `ksconf-0.10.2a2/ksconf/commands/diff.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/filter.py` & `ksconf-0.10.2a2/ksconf/commands/filter.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/merge.py` & `ksconf-0.10.2a2/ksconf/commands/merge.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/minimize.py` & `ksconf-0.10.2a2/ksconf/commands/minimize.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/package.py` & `ksconf-0.10.2a2/ksconf/commands/package.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/promote.py` & `ksconf-0.10.2a2/ksconf/commands/promote.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/restexport.py` & `ksconf-0.10.2a2/ksconf/commands/restexport.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/restpublish.py` & `ksconf-0.10.2a2/ksconf/commands/restpublish.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/snapshot.py` & `ksconf-0.10.2a2/ksconf/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/sort.py` & `ksconf-0.10.2a2/ksconf/commands/sort.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/unarchive.py` & `ksconf-0.10.2a2/ksconf/commands/unarchive.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/commands/xmlformat.py` & `ksconf-0.10.2a2/ksconf/commands/xmlformat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/compat.py` & `ksconf-0.10.2a2/ksconf/compat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/conf/delta.py` & `ksconf-0.10.2a2/ksconf/conf/delta.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/conf/merge.py` & `ksconf-0.10.2a2/ksconf/conf/merge.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/conf/meta.py` & `ksconf-0.10.2a2/ksconf/conf/meta.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/conf/parser.py` & `ksconf-0.10.2a2/ksconf/conf/parser.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/consts.py` & `ksconf-0.10.2a2/ksconf/consts.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/filter.py` & `ksconf-0.10.2a2/ksconf/filter.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/layer.py` & `ksconf-0.10.2a2/ksconf/layer.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/package.py` & `ksconf-0.10.2a2/ksconf/package.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/setup_entrypoints.py` & `ksconf-0.10.2a2/ksconf/setup_entrypoints.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/util/__init__.py` & `ksconf-0.10.2a2/ksconf/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/util/compare.py` & `ksconf-0.10.2a2/ksconf/util/compare.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/util/completers.py` & `ksconf-0.10.2a2/ksconf/util/completers.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/util/file.py` & `ksconf-0.10.2a2/ksconf/util/file.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/util/rest.py` & `ksconf-0.10.2a2/ksconf/util/rest.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/util/terminal.py` & `ksconf-0.10.2a2/ksconf/util/terminal.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/vc/git.py` & `ksconf-0.10.2a2/ksconf/vc/git.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf/xmlformat.py` & `ksconf-0.10.2a2/ksconf/xmlformat.py`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf.egg-info/PKG-INFO` & `ksconf-0.10.2a2/ksconf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksconf
-Version: 0.10.2a1
+Version: 0.10.2a2
 Summary: KSCONF: Ksconf Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
```

### Comparing `ksconf-0.10.2a1/ksconf.egg-info/SOURCES.txt` & `ksconf-0.10.2a2/ksconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/ksconf.egg-info/entry_points.txt` & `ksconf-0.10.2a2/ksconf.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ksconf-0.10.2a1/setup.py` & `ksconf-0.10.2a2/setup.py`

 * *Files identical despite different names*

