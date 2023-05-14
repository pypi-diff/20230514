# Comparing `tmp/wwpdb.apps.chem_ref_data-0.20.tar.gz` & `tmp/wwpdb.apps.chem_ref_data-0.20.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.chem_ref_data-0.20.tar", last modified: Sun May 14 14:49:10 2023, max compression
+gzip compressed data, was "wwpdb.apps.chem_ref_data-0.20.dev1.tar", last modified: Sun Apr 23 20:18:27 2023, max compression
```

## Comparing `wwpdb.apps.chem_ref_data-0.20.tar` & `wwpdb.apps.chem_ref_data-0.20.dev1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 14:49:10.043344 wwpdb.apps.chem_ref_data-0.20/
--rw-r--r--   0 vsts      (1001) docker     (123)      749 2023-05-14 14:49:10.043344 wwpdb.apps.chem_ref_data-0.20/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       92 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-05-14 14:49:10.043344 wwpdb.apps.chem_ref_data-0.20/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2528 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 14:49:10.035344 wwpdb.apps.chem_ref_data-0.20/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 14:49:10.035344 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 14:49:10.035344 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/
--rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 14:49:10.035344 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/depict/
--rw-r--r--   0 vsts      (1001) docker     (123)     8619 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4349 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 14:49:10.035344 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/io/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 14:49:10.039344 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/report/
--rw-r--r--   0 vsts      (1001) docker     (123)     8147 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/report/BirdReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5517 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/report/ChemCompReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26727 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3626 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/report/ReportUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/report/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 14:49:10.039344 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/
--rw-r--r--   0 vsts      (1001) docker     (123)    19650 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)      672 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26652 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27353 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19563 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7816 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2485 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/MiscUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 14:49:10.039344 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)    18237 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11314 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16203 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    28016 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3671 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1111 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/OSVersion.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 14:49:10.043344 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)    48574 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 14:47:40.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 14:49:10.035344 wwpdb.apps.chem_ref_data-0.20/wwpdb.apps.chem_ref_data.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      749 2023-05-14 14:49:09.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1749 2023-05-14 14:49:09.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 14:49:09.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb.apps.chem_ref_data.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 14:48:56.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb.apps.chem_ref_data.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      336 2023-05-14 14:49:09.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb.apps.chem_ref_data.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-05-14 14:49:09.000000 wwpdb.apps.chem_ref_data-0.20/wwpdb.apps.chem_ref_data.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.749084 wwpdb.apps.chem_ref_data-0.20.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      754 2023-04-23 20:18:27.749084 wwpdb.apps.chem_ref_data-0.20.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       92 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-23 20:18:27.749084 wwpdb.apps.chem_ref_data-0.20.dev1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2528 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/
+-rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8619 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4349 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.745084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8147 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/BirdReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5517 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ChemCompReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26735 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3626 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ReportUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.745084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/
+-rw-r--r--   0 vsts      (1001) docker     (123)    19650 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      672 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26652 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27353 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19563 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7816 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2485 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/MiscUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.745084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18237 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11314 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16203 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    28016 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3671 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1111 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/OSVersion.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.749084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)    48578 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-23 20:16:36.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-23 20:18:27.741084 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      754 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1749 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-23 20:18:09.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      336 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-23 20:18:27.000000 wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.chem_ref_data-0.20/PKG-INFO` & `wwpdb.apps.chem_ref_data-0.20.dev1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.chem_ref_data
-Version: 0.20
+Version: 0.20.dev1
 Summary: wwPDB chemical reference admin application
 Home-page: https://github.com/rcsb/py-wwpdb_apps_chem_ref_data
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.chem_ref_data-0.20/setup.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/depict/ChemRefDataDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/report/BirdReport.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/BirdReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/report/ChemCompReport.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ChemCompReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ChemRefReportDepictBootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,28 +309,30 @@
         oL.append("<br/>")
 
         #
         cD = eD["dataDict"]
 
         for catName in ["chem_comp"]:
             if catName in cD and (len(cD[catName]) > 0):
+
                 oL.append('<div class="sectionbar1">')
                 oL.append('  <a class="sectionbar1" href="" id="toggle_section_%s">Show</a> Category: %s' % (catName, catName))
                 oL.append("</div>")
 
                 oL.append('<div style="display: block;" id="d_%s" class="displaynone">' % catName)
                 oL.append('<table id="%s">' % catName)
                 self.__renderTableColumnWise(catName, cD[catName][0], oL)
                 oL.append("</table>")
                 oL.append("</div>")
         #
         # <div class="sb0"><a class="sb0" href="" id="toggle_section_XXXX">Show</a></div> <div class="sb1">Category:  Entity Reference</div>
         #
         for catName in tableList:
             if catName in cD and (len(cD[catName]) > 0):
+
                 oL.append('<div class="sb0">')
                 oL.append('  <a class="sb0" href="" id="toggle_section_%s">Show</a>' % catName)
                 oL.append("</div>")
                 oL.append('<div class="sb1">Category: %s </div>' % catName)
                 oL.append("<br />")
 
                 oL.append('<div style="display: block;" id="d_%s" class="displaynone">' % catName)
@@ -353,15 +355,16 @@
         to the left of column values.
         """
 
         #
         iCol = 0
         self.__markupRow(catName, rD)
         #
-        for itemName, itemDefault in self.__st.getItemNameAndDefaultList(catName):
+        for (itemName, itemDefault) in self.__st.getItemNameAndDefaultList(catName):
+
             if itemName in rD:
                 itemValue = rD[itemName]
             else:
                 itemValue = itemDefault
 
             oL.append("<tr>")
             oL.append("<td>%s</td>" % self.__attributePart(itemName))
@@ -388,15 +391,15 @@
         #
         #
 
     def __renderRow(self, catName, row, iRow, oL, insertDefault=False):  # pylint: disable=unused-argument
         """Render a row in a multirow table."""
         oL.append("<tr>")
         #
-        for itemName, itemDefault in self.__st.getItemNameAndDefaultList(catName):
+        for (itemName, itemDefault) in self.__st.getItemNameAndDefaultList(catName):
             if insertDefault:
                 itemValue = itemDefault
             elif itemName in row:
                 itemValue = row[itemName]
             else:
                 itemValue = itemDefault
 
@@ -523,14 +526,15 @@
                 itemValue = rD[itemName]
                 if len(itemValue) >= 3:
                     rD[itemName] = self.__markupLinks("cc", itemValue)
 
     # ------
 
     def __jQueryReportScript1(self, tableList, eD, oL):
+
         # Context that will get encoded for call back --
         filePath = eD["filePath"]
         localPath = eD["localPath"]
         localRelativePath = eD["localRelativePath"]
         sessionId = eD["sessionId"]
         editOpNumber = eD["editOpNumber"]
         blockId = eD["blockId"]
```

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/report/ReportUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/report/ReportUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemCompSearchIndexUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearch.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDef.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/ChemRefSearchDuplicates.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/search/MiscUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/search/MiscUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataCvsUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataDbUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/ChemRefDataMiscUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/DownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/utils/OSVersion.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/utils/OSVersion.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb/apps/chem_ref_data/webapp/ChemRefDataWebApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,14 +294,15 @@
                 rC.setStatus(statusMsg="Reports completed")
                 rC.set("webPathList", webPathList)
                 rC.set("idCodeList", myIdList)
             else:
                 rC.setError(errMsg="Report preparation failed")
 
         elif operation in ["check", "cvsupdate", "cvsadd"]:
+
             logPath = os.path.join(self.__sessionPath, rootName + "-cif-check.log")
             self.__removeFile(logPath)
             hasDiags = self.__makeCifCheckReport(filePath, logPath)
             if hasDiags:
                 du = DownloadUtils(self.__reqObj, verbose=self.__verbose, log=self.__lfh)
                 du.fetchFile(logPath)
                 aTagList.append(du.getAnchorTag())
@@ -848,14 +849,15 @@
             return self.__chemRefSupportFileUpdateOp()
         elif operation == "updateindexfiles":
             return self.__chemRefIndexFileUpdateOp()
         else:
             return self.__chemRefSyncCvsOp(repositoryType=None)
 
     def __chemRefSupportFileUpdateOp(self):
+
         self.__getSession()
         logger.info("+ChemRefDataWebAppWorker._chemRefSupportFileUpdateOp() starting with session %s", self.__sessionPath)
 
         self.__reqObj.setReturnFormat(return_format="json")
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
 
         ok = self.__chemRefSupportFiles()
@@ -880,14 +882,15 @@
             ok = ok1 and ok2 and ok3
         except:  # noqa: E722 pylint: disable=bare-except
             logger.exception("Failure in __chemRefSupportFiles")
             ok = False
         return ok
 
     def __chemRefIndexFileUpdateOp(self):
+
         self.__getSession()
         logger.info("+ChemRefDataWebAppWorker._chemRefIndexFileUpdateOp() starting with session %s", self.__sessionPath)
 
         self.__reqObj.setReturnFormat(return_format="json")
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
 
         ok = self.__chemRefIndexFiles()
@@ -941,14 +944,15 @@
                 hL.append("<br />".join(tL))
 
             rC.setError(errMsg="Repository SYNC completed with diagnostics  <br />" + "<br />".join(hL))
 
         return rC
 
     def __chemRefDatabaseUpdateOp(self, referenceDatabase="CC"):
+
         self.__getSession()
         logger.info("+ChemRefDataWebAppWorker._chemRefDatabaseUpdateOp() starting with session %s", self.__sessionPath)
 
         self.__reqObj.setReturnFormat(return_format="json")
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
 
         crdbu = ChemRefDataDbUtils(self.__reqObj, verbose=self.__debug, log=self.__lfh)
```

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.chem-ref-data
-Version: 0.20
+Version: 0.20.dev1
 Summary: wwPDB chemical reference admin application
 Home-page: https://github.com/rcsb/py-wwpdb_apps_chem_ref_data
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.chem_ref_data-0.20/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt` & `wwpdb.apps.chem_ref_data-0.20.dev1/wwpdb.apps.chem_ref_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

