# Comparing `tmp/kintyre-splunk-conf-0.9.2.tar.gz` & `tmp/kintyre-splunk-conf-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kintyre-splunk-conf-0.9.2.tar", last modified: Fri Mar  4 14:50:39 2022, max compression
+gzip compressed data, was "kintyre-splunk-conf-0.9.3.tar", last modified: Sat Mar 26 05:09:50 2022, max compression
```

## Comparing `kintyre-splunk-conf-0.9.2.tar` & `kintyre-splunk-conf-0.9.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-04 14:50:39.674139 kintyre-splunk-conf-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (116)    10752 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2404 2022-03-04 14:50:39.674139 kintyre-splunk-conf-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3970 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-04 14:50:39.670139 kintyre-splunk-conf-0.9.2/kintyre_splunk_conf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2404 2022-03-04 14:50:39.000000 kintyre-splunk-conf-0.9.2/kintyre_splunk_conf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1356 2022-03-04 14:50:39.000000 kintyre-splunk-conf-0.9.2/kintyre_splunk_conf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-03-04 14:50:39.000000 kintyre-splunk-conf-0.9.2/kintyre_splunk_conf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      701 2022-03-04 14:50:39.000000 kintyre-splunk-conf-0.9.2/kintyre_splunk_conf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      166 2022-03-04 14:50:39.000000 kintyre-splunk-conf-0.9.2/kintyre_splunk_conf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-03-04 14:50:39.000000 kintyre-splunk-conf-0.9.2/kintyre_splunk_conf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-03-04 14:50:27.000000 kintyre-splunk-conf-0.9.2/kintyre_splunk_conf.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-04 14:50:39.670139 kintyre-splunk-conf-0.9.2/ksconf/
--rw-r--r--   0 runner    (1001) docker     (116)     4419 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11705 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      282 2022-03-04 14:50:39.000000 kintyre-splunk-conf-0.9.2/ksconf/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     3145 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-04 14:50:39.670139 kintyre-splunk-conf-0.9.2/ksconf/builder/
--rw-r--r--   0 runner    (1001) docker     (116)     5446 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8010 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/builder/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)    11439 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/builder/core.py
--rw-r--r--   0 runner    (1001) docker     (116)     7253 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/builder/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-04 14:50:39.670139 kintyre-splunk-conf-0.9.2/ksconf/commands/
--rw-r--r--   0 runner    (1001) docker     (116)    22733 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3727 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (116)    17969 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/combine.py
--rw-r--r--   0 runner    (1001) docker     (116)     3567 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (116)    12038 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     2935 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (116)     8691 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/minimize.py
--rw-r--r--   0 runner    (1001) docker     (116)    11054 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/package.py
--rw-r--r--   0 runner    (1001) docker     (116)    23142 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/promote.py
--rw-r--r--   0 runner    (1001) docker     (116)    11417 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/restexport.py
--rw-r--r--   0 runner    (1001) docker     (116)    15919 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/restpublish.py
--rw-r--r--   0 runner    (1001) docker     (116)     6649 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (116)     5538 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/sort.py
--rw-r--r--   0 runner    (1001) docker     (116)    22691 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/unarchive.py
--rw-r--r--   0 runner    (1001) docker     (116)     4327 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/commands/xmlformat.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-04 14:50:39.674139 kintyre-splunk-conf-0.9.2/ksconf/conf/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16266 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/conf/delta.py
--rw-r--r--   0 runner    (1001) docker     (116)     6440 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/conf/merge.py
--rw-r--r--   0 runner    (1001) docker     (116)     5398 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/conf/meta.py
--rw-r--r--   0 runner    (1001) docker     (116)    16894 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/conf/parser.py
--rw-r--r--   0 runner    (1001) docker     (116)     1762 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-04 14:50:39.674139 kintyre-splunk-conf-0.9.2/ksconf/ext/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    32452 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/ext/six.py
--rw-r--r--   0 runner    (1001) docker     (116)     6529 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/filter.py
--rw-r--r--   0 runner    (1001) docker     (116)    15302 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/layer.py
--rw-r--r--   0 runner    (1001) docker     (116)    13251 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/package.py
--rw-r--r--   0 runner    (1001) docker     (116)     3185 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/setup_entrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-04 14:50:39.674139 kintyre-splunk-conf-0.9.2/ksconf/util/
--rw-r--r--   0 runner    (1001) docker     (116)     3189 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      799 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (116)      598 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/util/completers.py
--rw-r--r--   0 runner    (1001) docker     (116)     6753 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/util/file.py
--rw-r--r--   0 runner    (1001) docker     (116)      527 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/util/rest.py
--rw-r--r--   0 runner    (1001) docker     (116)     1129 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/util/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-04 14:50:39.674139 kintyre-splunk-conf-0.9.2/ksconf/vc/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/vc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4194 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/vc/git.py
--rw-r--r--   0 runner    (1001) docker     (116)     5170 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/ksconf/xmlformat.py
--rw-r--r--   0 runner    (1001) docker     (116)      443 2022-03-04 14:50:39.674139 kintyre-splunk-conf-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     5142 2022-03-04 14:50:16.000000 kintyre-splunk-conf-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-26 05:09:50.880952 kintyre-splunk-conf-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (116)    10752 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     2404 2022-03-26 05:09:50.880952 kintyre-splunk-conf-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3970 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-26 05:09:50.872952 kintyre-splunk-conf-0.9.3/kintyre_splunk_conf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2404 2022-03-26 05:09:50.000000 kintyre-splunk-conf-0.9.3/kintyre_splunk_conf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1356 2022-03-26 05:09:50.000000 kintyre-splunk-conf-0.9.3/kintyre_splunk_conf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-03-26 05:09:50.000000 kintyre-splunk-conf-0.9.3/kintyre_splunk_conf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      701 2022-03-26 05:09:50.000000 kintyre-splunk-conf-0.9.3/kintyre_splunk_conf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      166 2022-03-26 05:09:50.000000 kintyre-splunk-conf-0.9.3/kintyre_splunk_conf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2022-03-26 05:09:50.000000 kintyre-splunk-conf-0.9.3/kintyre_splunk_conf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-03-26 05:09:36.000000 kintyre-splunk-conf-0.9.3/kintyre_splunk_conf.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-26 05:09:50.876952 kintyre-splunk-conf-0.9.3/ksconf/
+-rw-r--r--   0 runner    (1001) docker     (116)     4419 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11705 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      282 2022-03-26 05:09:50.000000 kintyre-splunk-conf-0.9.3/ksconf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3145 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-26 05:09:50.876952 kintyre-splunk-conf-0.9.3/ksconf/builder/
+-rw-r--r--   0 runner    (1001) docker     (116)     5446 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8010 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/builder/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11439 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/builder/core.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7253 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/builder/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-26 05:09:50.876952 kintyre-splunk-conf-0.9.3/ksconf/commands/
+-rw-r--r--   0 runner    (1001) docker     (116)    22733 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3727 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17969 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/combine.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3567 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12038 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2935 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8691 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11054 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/package.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23142 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/promote.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11417 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/restexport.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15919 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/restpublish.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6649 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5538 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/sort.py
+-rw-r--r--   0 runner    (1001) docker     (116)    22691 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/unarchive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4327 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/commands/xmlformat.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-26 05:09:50.876952 kintyre-splunk-conf-0.9.3/ksconf/conf/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16266 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/conf/delta.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6440 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/conf/merge.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5398 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/conf/meta.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16894 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/conf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1762 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-26 05:09:50.876952 kintyre-splunk-conf-0.9.3/ksconf/ext/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    32452 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/ext/six.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6529 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15302 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/layer.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13421 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/package.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3185 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/setup_entrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-26 05:09:50.880952 kintyre-splunk-conf-0.9.3/ksconf/util/
+-rw-r--r--   0 runner    (1001) docker     (116)     3189 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      799 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (116)      598 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/util/completers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6753 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/util/file.py
+-rw-r--r--   0 runner    (1001) docker     (116)      527 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/util/rest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1129 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/util/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-26 05:09:50.880952 kintyre-splunk-conf-0.9.3/ksconf/vc/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/vc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4194 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/vc/git.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5170 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/ksconf/xmlformat.py
+-rw-r--r--   0 runner    (1001) docker     (116)      443 2022-03-26 05:09:50.880952 kintyre-splunk-conf-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     5142 2022-03-26 05:09:27.000000 kintyre-splunk-conf-0.9.3/setup.py
```

### Comparing `kintyre-splunk-conf-0.9.2/LICENSE` & `kintyre-splunk-conf-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/PKG-INFO` & `kintyre-splunk-conf-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kintyre-splunk-conf
-Version: 0.9.2
+Version: 0.9.3
 Summary: KSCONF: Kintyre's Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
```

### Comparing `kintyre-splunk-conf-0.9.2/README.md` & `kintyre-splunk-conf-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/kintyre_splunk_conf.egg-info/PKG-INFO` & `kintyre-splunk-conf-0.9.3/kintyre_splunk_conf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kintyre-splunk-conf
-Version: 0.9.2
+Version: 0.9.3
 Summary: KSCONF: Kintyre's Splunk Configuration Tool
 Home-page: https://github.com/Kintyre/ksconf
 Author: Lowell Alleman
 Author-email: lowell@kintyre.co
 License: Apache Software License
 Project-URL: Documentation, https://ksconf.readthedocs.io/
 Project-URL: Splunk app, https://splunkbase.splunk.com/app/4383/
```

### Comparing `kintyre-splunk-conf-0.9.2/kintyre_splunk_conf.egg-info/SOURCES.txt` & `kintyre-splunk-conf-0.9.3/kintyre_splunk_conf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/kintyre_splunk_conf.egg-info/entry_points.txt` & `kintyre-splunk-conf-0.9.3/kintyre_splunk_conf.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/__init__.py` & `kintyre-splunk-conf-0.9.3/ksconf/__init__.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/__main__.py` & `kintyre-splunk-conf-0.9.3/ksconf/__main__.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/archive.py` & `kintyre-splunk-conf-0.9.3/ksconf/archive.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/builder/__init__.py` & `kintyre-splunk-conf-0.9.3/ksconf/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/builder/cache.py` & `kintyre-splunk-conf-0.9.3/ksconf/builder/cache.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/builder/core.py` & `kintyre-splunk-conf-0.9.3/ksconf/builder/core.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/builder/steps.py` & `kintyre-splunk-conf-0.9.3/ksconf/builder/steps.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/__init__.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/check.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/check.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/combine.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/combine.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/diff.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/diff.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/filter.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/filter.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/merge.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/merge.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/minimize.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/minimize.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/package.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/package.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/promote.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/promote.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/restexport.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/restexport.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/restpublish.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/restpublish.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/snapshot.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/sort.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/sort.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/unarchive.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/unarchive.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/commands/xmlformat.py` & `kintyre-splunk-conf-0.9.3/ksconf/commands/xmlformat.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/conf/delta.py` & `kintyre-splunk-conf-0.9.3/ksconf/conf/delta.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/conf/merge.py` & `kintyre-splunk-conf-0.9.3/ksconf/conf/merge.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/conf/meta.py` & `kintyre-splunk-conf-0.9.3/ksconf/conf/meta.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/conf/parser.py` & `kintyre-splunk-conf-0.9.3/ksconf/conf/parser.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/consts.py` & `kintyre-splunk-conf-0.9.3/ksconf/consts.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/ext/six.py` & `kintyre-splunk-conf-0.9.3/ksconf/ext/six.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/filter.py` & `kintyre-splunk-conf-0.9.3/ksconf/filter.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/layer.py` & `kintyre-splunk-conf-0.9.3/ksconf/layer.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/package.py` & `kintyre-splunk-conf-0.9.3/ksconf/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,14 +321,19 @@
         for name in dir(self):
             if name.startswith("get_"):
                 var = name[4:]
                 doc = getattr(self, name).__doc__.strip()
                 yield (var, doc)
 
     def __getitem__(self, item):
+        if item not in self._cache:
+            self._cache[item] = self._get_expanded_var(item)
+        return self._cache[item]
+
+    def _get_expanded_var(self, item):
         get_funct_name = "get_" + item
         if hasattr(self, get_funct_name):
             try:
                 funct = getattr(self, get_funct_name)
                 return funct()
             except AppVarMagicException as e:
                 if KSCONF_DEBUG in os.environ:
```

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/setup_entrypoints.py` & `kintyre-splunk-conf-0.9.3/ksconf/setup_entrypoints.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/util/__init__.py` & `kintyre-splunk-conf-0.9.3/ksconf/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/util/compare.py` & `kintyre-splunk-conf-0.9.3/ksconf/util/compare.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/util/completers.py` & `kintyre-splunk-conf-0.9.3/ksconf/util/completers.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/util/file.py` & `kintyre-splunk-conf-0.9.3/ksconf/util/file.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/util/rest.py` & `kintyre-splunk-conf-0.9.3/ksconf/util/rest.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/util/terminal.py` & `kintyre-splunk-conf-0.9.3/ksconf/util/terminal.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/vc/git.py` & `kintyre-splunk-conf-0.9.3/ksconf/vc/git.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/ksconf/xmlformat.py` & `kintyre-splunk-conf-0.9.3/ksconf/xmlformat.py`

 * *Files identical despite different names*

### Comparing `kintyre-splunk-conf-0.9.2/setup.py` & `kintyre-splunk-conf-0.9.3/setup.py`

 * *Files identical despite different names*

