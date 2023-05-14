# Comparing `tmp/wwpdb.apps.ccmodule-0.25.dev1.tar.gz` & `tmp/wwpdb.apps.ccmodule-0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.ccmodule-0.25.dev1.tar", last modified: Thu Mar  2 12:22:58 2023, max compression
+gzip compressed data, was "wwpdb.apps.ccmodule-0.26.tar", last modified: Sun May 14 15:43:08 2023, max compression
```

## Comparing `wwpdb.apps.ccmodule-0.25.dev1.tar` & `wwpdb.apps.ccmodule-0.26.tar`

### file list

```diff
@@ -1,81 +1,77 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.197444 wwpdb.apps.ccmodule-0.25.dev1/
--rw-r--r--   0 vsts      (1001) docker     (123)      784 2023-03-02 12:22:58.197444 wwpdb.apps.ccmodule-0.25.dev1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       80 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-03-02 12:22:58.201444 wwpdb.apps.ccmodule-0.25.dev1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2600 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.189443 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.189443 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.189443 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/
--rw-r--r--   0 vsts      (1001) docker     (123)      156 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.189443 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/admin/
--rw-r--r--   0 vsts      (1001) docker     (123)     4247 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/admin/ChemCompAdmin.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/admin/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.189443 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/chem/
--rw-r--r--   0 vsts      (1001) docker     (123)     5912 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py
--rw-r--r--   0 vsts      (1001) docker     (123)   121256 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/chem/ChemCompAssign.py
--rw-r--r--   0 vsts      (1001) docker     (123)   102562 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)    73501 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11689 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/chem/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.193443 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/depict/
--rw-r--r--   0 vsts      (1001) docker     (123)    11302 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/depict/ChemCompDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.193443 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/edit/
--rw-r--r--   0 vsts      (1001) docker     (123)    14647 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/edit/ChemCompTableEditor.py
--rw-r--r--   0 vsts      (1001) docker     (123)    25954 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/edit/ChemCompTableEditorDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/edit/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.193443 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/extract/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/extract/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2951 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/extract/ccOps.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.193443 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/
--rw-r--r--   0 vsts      (1001) docker     (123)    90790 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7123 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/ChemCompDataExport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7305 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/ChemCompDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12540 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/ChemCompEditStore.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13230 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/ChemCompIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12545 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/PdbxChemComp.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.193443 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/
--rw-r--r--   0 vsts      (1001) docker     (123)     5013 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     4885 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2842 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3367 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15510 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/ChemCompReports.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6341 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.197444 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/search/
--rw-r--r--   0 vsts      (1001) docker     (123)    10865 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/search/ChemCompSearch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13150 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6259 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8708 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/search/DbSession.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/search/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.197444 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/sketch/
--rw-r--r--   0 vsts      (1001) docker     (123)     9280 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6407 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/sketch/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.197444 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)     7276 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/utils/ChemCompConfig.py
--rw-r--r--   0 vsts      (1001) docker     (123)    28919 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1136 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)      586 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/utils/Exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7974 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.197444 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/view/
--rw-r--r--   0 vsts      (1001) docker     (123)     7378 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/view/ChemCompView.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5738 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/view/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.197444 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)   138505 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    96979 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/webapp/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     4642 2023-03-02 12:20:49.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/webapp/wsgi.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-02 12:22:58.189443 wwpdb.apps.ccmodule-0.25.dev1/wwpdb.apps.ccmodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      784 2023-03-02 12:22:58.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb.apps.ccmodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2629 2023-03-02 12:22:58.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb.apps.ccmodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-02 12:22:58.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb.apps.ccmodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-02 12:22:42.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb.apps.ccmodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      255 2023-03-02 12:22:58.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb.apps.ccmodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-03-02 12:22:58.000000 wwpdb.apps.ccmodule-0.25.dev1/wwpdb.apps.ccmodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/
+-rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       80 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-05-14 15:43:08.206798 wwpdb.apps.ccmodule-0.26/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2595 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.194798 wwpdb.apps.ccmodule-0.26/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.194798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.194798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/
+-rw-r--r--   0 vsts      (1001) docker     (123)      151 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.198798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5950 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   121176 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAssign.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   102562 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    73835 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11689 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.198798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11302 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/depict/ChemCompDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.198798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/edit/
+-rw-r--r--   0 vsts      (1001) docker     (123)    14647 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/edit/ChemCompTableEditor.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    25954 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/edit/ChemCompTableEditorDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/edit/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.198798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/extract/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/extract/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2951 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/extract/ccOps.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.198798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)    90790 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7123 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompDataExport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7305 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12540 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompEditStore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13230 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.198798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4801 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     4885 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2842 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3367 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15551 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompReports.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6341 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10865 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13150 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6259 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8708 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/DbSession.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/sketch/
+-rw-r--r--   0 vsts      (1001) docker     (123)     9280 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6407 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/sketch/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7373 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/ChemCompConfig.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    28706 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1136 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      586 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/Exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7974 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/view/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7378 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/view/ChemCompView.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5738 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/view/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)   138409 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    96877 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     4642 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/wsgi.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.194798 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-05-14 15:43:08.000000 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2509 2023-05-14 15:43:08.000000 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 15:43:08.000000 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 15:42:57.000000 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      250 2023-05-14 15:43:08.000000 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-05-14 15:43:08.000000 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/PKG-INFO` & `wwpdb.apps.ccmodule-0.26/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ccmodule
-Version: 0.25.dev1
+Version: 0.26
 Summary: wwPDB workflow engine utils
 Home-page: https://github.com/rcsb/py-wwpdb_apps_wf_engine_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/setup.py` & `wwpdb.apps.ccmodule-0.26/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,20 @@
         'Programming Language :: Python :: 3.7',
     ],
     entry_points={
         'console_scripts': []
     },
     #
     # Also depends on 'openeye.oechem' but cannot install by pypi
-    install_requires=['mmcif', 'mmcif.utils >= 0.13', 'wwpdb.utils.config ~= 0.24',
+    install_requires=['mmcif', 'mmcif.utils >= 0.13', 'wwpdb.utils.config ~= 0.34',
                       'wwpdb.utils.dp >= 0.11', 'rcsb.utils.multiproc',
                       'wwpdb.utils.wf',
                       'wwpdb.utils.session >= 0.2',
                       'mysqlclient',
-                      "wwpdb.io >= 0.16.dev1"
+                      "wwpdb.io ~= 0.27"
                       ],
     packages=find_packages(exclude=['wwpdb.apps.tests_ccmodule']),
     package_data={
         # If any package contains *.md or *.rst ...  files, include them:
         '': ['*.md', '*.rst', '*.txt', '*.cfg']
     },
     #
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/admin/ChemCompAdmin.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,114 @@
 ##
-# File:  ChemCompAdmin.py
+# File:  ChemCompAnnotate.py
 # Date:  14-Aug-2010
 # Updates:
 # 14-Aug-2010 jdw - Refactor -
 #
 ##
 """
-Chemical component administrative and archiving functions -
+Annotation functions -
 """
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.01"
 
 import os
 import sys
 import shutil
 
+
 from wwpdb.apps.ccmodule.utils.ChemCompConfig import ChemCompConfig
+from wwpdb.io.locator.ChemRefPathInfo import ChemRefPathInfo
 
 
-class ChemCompAdmin(object):
-    """Chemical component adiminstrative and archiving functions.
+class ChemCompAnnotate(object):
+    """Chemical component annotation operations -
 
     """
     def __init__(self, reqObj, verbose=False, log=sys.stderr):
-        """Chemical component adiminstrative and archiving functions.
+        """Chemical component annotation operations -
 
 
          :param `verbose`:  boolean flag to activate verbose logging.
          :param `log`:      stream for logging.
 
         """
         self.__verbose = verbose
         self.__lfh = log
         # self.__debug = True
         #
         self.__reqObj = reqObj
         #
         self.__sObj = self.__reqObj.getSessionObj()
         self.__sessionPath = self.__sObj.getPath()
-        # self.__sessionRelativePath = self.__sObj.getRelativePath()
+        self.__sessionRelativePath = self.__sObj.getRelativePath()
         #
         self.__ccConfig = ChemCompConfig(reqObj, verbose=self.__verbose, log=self.__lfh)
         #
         self.__definitionId = None
         self.__definitionFilePath = None
+        self.__annotatedFileName = None
+        self.__annotatedFilePath = None
+        self.__annotatedRelativeFilePath = None
 
     def setDefinitionId(self, definitionId):
         """Set an existing chemical component identifier in archive collection as
            the report target
         """
         self.__definitionId = str(definitionId).upper()
+        if self.__annotatedFileName is None:
+            self.__annotatedFileName = self.__definitionId + "-upd.cif"
         return self.__getFilePathFromId(self.__definitionId)
 
     def setFilePath(self, definitionFilePath, definitionId="TMP"):
         self.__definitionFilePath = definitionFilePath
         if (not os.access(self.__definitionFilePath, os.R_OK)):
             return False
         self.__definitionId = str(definitionId).upper()
+        if self.__annotatedFileName is None:
+            self.__annotatedFileName = self.__definitionId + "-upd.cif"
         return True
 
     def getFilePath(self):
         return self.__definitionFilePath
 
     def __getFilePathFromId(self, ccId):
         """
         """
         idUc = str(ccId).upper()
-        fileName = idUc + ".cif"
-        self.__definitionFilePath = os.path.join(self.__ccConfig.getPath('chemCompCachePath'), idUc[0:1], idUc[0:3], fileName)
+        crpi = ChemRefPathInfo(verbose=self.__verbose, log=self.__lfh)
+
+        self.__definitionFilePath = crpi.getFilePath(idUc, "CC")
         #
         if (not os.access(self.__definitionFilePath, os.R_OK)):
             return False
         return True
 
+    def setAnnotatedFileName(self, fileName):
+        self.__annotatedFileName = fileName
+
+    def getAnnotatedFilePath(self):
+        return (self.__annotatedFilePath)
+
+    def getAnnotatedRelativeFilePath(self):
+        return (self.__annotatedRelativeFilePath)
+
     ##
-    def doAdmin(self):
-        """ template admin function.
+    ##
+    def doAnnotate(self):
+        """ annotation operation -
         """
         #
+        swap = "SWAP"
         #
         dirPath = os.path.join(self.__sessionPath, self.__definitionId)
-        # dirRelativePath = os.path.join(self.__sessionRelativePath, self.__definitionId)
+        dirRelativePath = os.path.join(self.__sessionRelativePath, self.__definitionId)
         # create the report path in the session directory
         #
         if (not os.access(dirPath, os.F_OK)):
             try:
                 os.makedirs(dirPath)
             except:  # noqa: E722 pylint: disable=bare-except
                 return False
@@ -97,31 +118,52 @@
         #
         (_pth, fileName) = os.path.split(self.__definitionFilePath)
         lclPath = os.path.join(dirPath, fileName)
         if (self.__definitionFilePath != lclPath):
             shutil.copyfile(self.__definitionFilePath, lclPath)
             #
             if (self.__verbose):
-                self.__lfh.write("+ChemCompAdmin.doAnnotate() - Copied input file %s to local path %s \n" %
+                self.__lfh.write("+ChemCompAnnotate.doAnnotate() - Copied input file %s to local path %s \n" %
                                  (self.__definitionFilePath, lclPath))
                 self.__lfh.flush()
         #
         #
         logPath = os.path.join(dirPath, "annotate.log")
-        cmd = ''
-        outFile = ''
+        outFile = self.__annotatedFileName
         #
+        if str(swap).upper() == "SWAP":
+            cmd = self.__ccConfig.getPath("annotateFileScript") + " " + \
+                self.__ccConfig.getPath("binPath") + " " + dirPath + " " + fileName + \
+                " " + outFile + " SWAP > " + logPath + " 2>&1"
+        else:
+            cmd = self.__ccConfig.getPath("annotateFileScript") + " " + \
+                self.__ccConfig.getPath("binPath") + " " + dirPath + " " + fileName + \
+                " " + outFile + " > " + logPath + " 2>&1"
         if (self.__verbose):
-            self.__lfh.write("+ChemCompAdmin.doAnnotate() directory path  = %s\n" % dirPath)
-            self.__lfh.write("+ChemCompAdmin.doAnnotate() Target filename = %s\n" % fileName)
-            self.__lfh.write("+ChemCompAdmin.doAnnotate() Output filename = %s\n" % outFile)
-            self.__lfh.write("+ChemCompAdmin.doAnnotate() Log    path     = %s\n" % logPath)
-            self.__lfh.write("+ChemCompAdmin.doAnnotate() command string  = %s\n" % cmd)
+            self.__lfh.write("+ChemCompAnnotate.doAnnotate() directory path  = %s\n" % dirPath)
+            self.__lfh.write("+ChemCompAnnotate.doAnnotate() Target filename = %s\n" % fileName)
+            self.__lfh.write("+ChemCompAnnotate.doAnnotate() Output filename = %s\n" % outFile)
+            self.__lfh.write("+ChemCompAnnotate.doAnnotate() Swap option     = %s\n" % str(swap))
+            self.__lfh.write("+ChemCompAnnotate.doAnnotate() Log    path     = %s\n" % logPath)
+            self.__lfh.write("+ChemCompAnnotate.doAnnotate() command string  = %s\n" % cmd)
 
         os.system(cmd)
         #
         outPath = os.path.join(dirPath, outFile)
         if os.path.exists(outPath):
+            self.__annotatedFilePath = outPath
+            self.__annotatedRelativeFilePath = os.path.join(dirRelativePath, self.__annotatedFileName)
             return True
         else:
             return False
     ##
+
+    def getAnnotatedFileText(self):
+        #
+        textData = ""
+        try:
+            if os.path.exists(self.__annotatedFilePath):
+                textData = open(self.__annotatedFilePath).read()
+        except:  # noqa: E722 pylint: disable=bare-except
+            pass
+
+        return textData
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/chem/ChemCompAssign.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAssign.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,18 +100,18 @@
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
 from wwpdb.apps.ccmodule.chem.PdbxChemCompAssign import PdbxChemCompAssignReader
 from wwpdb.apps.ccmodule.io.ChemCompDataImport import ChemCompDataImport
 from wwpdb.apps.ccmodule.io.ChemCompDataExport import ChemCompDataExport
 from wwpdb.apps.ccmodule.io.ChemCompIo import ChemCompReader
 from wwpdb.apps.ccmodule.io.ChemCompAssignDataStore import ChemCompAssignDataStore
-from wwpdb.apps.ccmodule.utils.ChemCompConfig import ChemCompConfig
 from mmcif.io.PdbxReader import PdbxReader
 from pathlib import Path
 from wwpdb.io.locator.PathInfo import PathInfo
+from wwpdb.io.locator.ChemRefPathInfo import ChemRefPathInfo
 from mmcif.io.IoAdapterCore import IoAdapterCore
 
 
 class ChemCompAssign(object):
     """Residue-level chemical component assignment operations
 
     """
@@ -800,17 +800,17 @@
 
         """
         if (self.__verbose):
             self.__lfh.write("--------------------------------------------\n")
             self.__lfh.write("+%s.%s() starting\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name))
         #
         rtrnCode = -1
-        ccConfig = ChemCompConfig(self.__reqObj, verbose=self.__verbose, log=self.__lfh)
-        pathPrefix = ccConfig.getPath('chemCompCachePath')
-        validationPth = os.path.join(pathPrefix, ccId[:1], ccId, ccId + '.cif')
+        crpi = ChemRefPathInfo(self.__cI.get("SITE_PREFIX"), verbose=self.__verbose, log=self.__lfh)
+        validationPth = crpi.getFilePath(ccId, "CC")
+
         #
         if os.access(validationPth, os.R_OK):
             rtrnCode = 0
             if self.__verbose:
                 self.__lfh.write("+%s.%s() %s PASSES simple validation.\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, ccId))
 
         else:
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
 from logging import getLogger, StreamHandler, Formatter, DEBUG, INFO
 from wwpdb.apps.ccmodule.depict.ChemCompDepict import ChemCompDepict
 from wwpdb.apps.ccmodule.chem.ChemCompAssign import ChemCompAssign
 # from wwpdb.apps.ccmodule.chem.PdbxChemCompAssign import PdbxCategoryDefinition
 from wwpdb.apps.ccmodule.io.ChemCompAssignDataStore import ChemCompAssignDataStore
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCc
 from pathlib import Path
 from wwpdb.io.locator.PathInfo import PathInfo
 
 
 class ChemCompAssignDepictLite(ChemCompDepict):
     """ Class responsible for generating HTML depictions of
         chemical component search results for the Common Tool Deposition UI.
@@ -83,15 +84,15 @@
 
         """
         super(ChemCompAssignDepictLite, self).__init__(verbose, log)
         self.__verbose = verbose
         self.__lfh = log
         self.__debug = False
         self.__reqObj = p_reqObj
-        self.__depId = "D_0" if self.__reqObj.getValue("identifier") in [None, 'TMP_ID'] else str(self.__reqObj.getValue("identifier")).upper()
+        self.__depId = "D_0" if self.__reqObj.getValue("identifier") in [None, "", 'TMP_ID'] else str(self.__reqObj.getValue("identifier")).upper()
         #
         # self.__cDict = PdbxCategoryDefinition._cDict
         #
         # self.__noDisplayList = ['']
         #
         # self.__pathGlblVwTmplts = "templates/workflow_ui/global_view"
         # self.__pathInstncsVwTmplts = " templates/workflow_ui/instances_view"
@@ -111,20 +112,23 @@
         #
         self.__pathCCliteAllInstcs = "templates/workflow_ui/instances_view/all_instances"
         self.__pathCCliteAllInstncsCmprTmplts = self.__pathCCliteAllInstcs + "/comparison_view"
         self.__pathCCliteAllInstncsJmolTmplts = self.__pathCCliteAllInstncsCmprTmplts + "/jmol"
         #
         self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
         self.__cI = ConfigInfo(self.__siteId)
+        self.__cIAppCc = ConfigInfoAppCc(self.__siteId, verbose=self.__verbose, log=self.__lfh)
+
         # self.__deployPath = self.__cI.get('SITE_DEPLOY_PATH')
         self.__siteSrvcUrlPathPrefix = self.__cI.get('SITE_SERVICE_URL_PATH_PREFIX', '')
         self.__workingRltvAssgnSessionPath = ''
 
         self.__alternateTopHitMarkup = '''<input id="use_exact_mtch_id_%(auth_assgnd_grp)s_%(tophit_id)s" class="c_%(auth_assgnd_grp)s addrss_msmtch use_exact_mtch_id" type="radio" name="addrss_msmtch_chc" value="use_exact_mtch_id" %(use_exact_mtch_id_checked)s %(disabled)s /><label for="use_exact_mtch_id_%(auth_assgnd_grp)s_%(tophit_id)s">Use exact match ID of <span name="%(tophit_id)s" style="color: #F00;" class="strong tophit">%(tophit_id)s</span> (<a href="http://ligand-expo.rcsb.org/pyapps/ldHandler.py?formid=cc-index-search&target=%(tophit_id)s&operation=ccid" target="_blank">See Definition</a>) instead of originally proposed ID</label><br />'''  # noqa: E501
 
+        print("XXXX", self.__depId)
         self.__depositPath = Path(PathInfo().getDepositPath(self.__depId)).parent
         self.__ccReportPath = os.path.join(self.__depositPath, self.__depId, self._CC_REPORT_DIR)
         # self.__depositAssignPath = os.path.join(self.__depositPath, self.__depId, self._CC_ASSIGN_DIR)
         self.__logger = self._setupLog(log)
 
     ################################################################################################################
     # ------------------------------------------------------------------------------------------------------------
@@ -600,14 +604,15 @@
         lclDict['peptide_like_checked'] = ''
         lclDict['carbohydrate_checked'] = ''
         lclDict['lipid_checked'] = ''
         lclDict['heterogen_checked'] = ''
         lclDict['none_of_abv_checked'] = ''
 
         lclDict['alt_ccid'] = ''
+        lclDict['alt_ccid_width'] = '3'
         lclDict['dscrptr_type'] = ''
         lclDict['dscrptr_str'] = ''
         lclDict['inchi_selected'] = ''
         lclDict['smiles_selected'] = ''
         lclDict['sbmt_choice_dscrptrstr_slctd'] = 'selected="selected"'
         lclDict['sbmt_choice_sketch_slctd'] = ''
 
@@ -622,14 +627,17 @@
         ligDscrptrType = p_ccAssgnDataStr.getDpstrCcDscrptrType(p_authAssignedGrp)
         ligDscrptrStr = p_ccAssgnDataStr.getDpstrCcDscrptrStr(p_authAssignedGrp) if p_ccAssgnDataStr.getDpstrCcDscrptrStr(p_authAssignedGrp) != '?' else ""
         dpstrSubmitChoice = p_ccAssgnDataStr.getDpstrSubmitChoice(p_authAssignedGrp)
         ligName = p_ccAssgnDataStr.getDpstrCcName(p_authAssignedGrp) if p_ccAssgnDataStr.getDpstrCcName(p_authAssignedGrp) != '?' else ""
         ligFrmla = p_ccAssgnDataStr.getDpstrCcFrmla(p_authAssignedGrp) if p_ccAssgnDataStr.getDpstrCcFrmla(p_authAssignedGrp) != '?' else ""
         ligComments = p_ccAssgnDataStr.getDpstrComments(p_authAssignedGrp) if p_ccAssgnDataStr.getDpstrComments(p_authAssignedGrp) != '?' else ""
 
+        if self.__cIAppCc.get_extended_ccd_supp():
+            lclDict['alt_ccid_width'] = '5'
+
         if p_authAssignedGrp in p_hlprDict['hndle_msmtch_tophit_id_list'] and len(p_hlprDict['hndle_msmtch_tophit_id_list'][p_authAssignedGrp]) > 0:
             lclDict['dsply_addrss_msmtch_opts'] = ''
         else:
             lclDict['dsply_no_match_instrctns'] = ''
             lclDict['dsply_dscrnwlgnd'] = ''
 
         if self.__verbose and self.__debug:
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/depict/ChemCompDepict.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/depict/ChemCompDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/edit/ChemCompTableEditor.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/edit/ChemCompTableEditor.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/edit/ChemCompTableEditorDepict.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/edit/ChemCompTableEditorDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/extract/ccOps.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/extract/ccOps.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/ChemCompDataExport.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompDataExport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/ChemCompDataImport.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/ChemCompEditStore.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompEditStore.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/io/ChemCompIo.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.01"
 
 import os
 import sys
 
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 from wwpdb.io.locator.ChemRefPathInfo import ChemRefPathInfo
 
 
 class ChemCompAlignImageGenerator(object):
     """Utility Class for generating aligned ligand images
     """
@@ -40,18 +39,16 @@
         self.__sObj = self.__reqObj.getSessionObj()
         self.__sessionPath = self.__sObj.getPath()
         #
         self.__imagePath = None
 
         self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
         self.__cI = ConfigInfo(self.__siteId)
-        self.__cICommon = ConfigInfoAppCommon(self.__siteId)
         #
-        self.__ccRefPathInfo = ChemRefPathInfo(configObj=self.__cI, configCommonObj=self.__cICommon,
-                                               verbose=self.__verbose, log=self.__lfh)
+        self.__ccRefPathInfo = ChemRefPathInfo(self.__siteId, verbose=self.__verbose, log=self.__lfh)
 
     def generateImages(self, instId=None, instFile=None, hitList=None):
         if (not instId) or (not instFile):
             return
         if hitList is None:
             hitList = []
         #
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/ChemCompReports.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompReports.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 __version__ = "V0.01"
 
 import os
 import sys
 import shutil
 
 from wwpdb.apps.ccmodule.utils.ChemCompConfig import ChemCompConfig
-# from wwpdb.utils.config.ConfigInfo import ConfigInfo
 from pathlib import Path
 from wwpdb.io.locator.PathInfo import PathInfo
+from wwpdb.io.locator.ChemRefPathInfo import ChemRefPathInfo
 
 
 class ChemCompReport(object):
     """Create web report from chemical component definitions.
 
     """
     def __init__(self, reqObj, verbose=False, log=sys.stderr):
@@ -56,16 +56,17 @@
         #
         self.__ccConfig = ChemCompConfig(reqObj, verbose=self.__verbose, log=self.__lfh)
         #
         self.__reportFilePath = None
         self.__reportFileRelativePath = None
         self.__definitionId = None
         self.__definitionFilePath = None
-        # self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
+        self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
         # self.__cI = ConfigInfo(self.__siteId)
+        self.__crpi = ChemRefPathInfo(self.__siteId, verbose=verbose, log=log)
 
         context = self.__getContext()
         if context == 'standalone':
             self.__depId = 'D_0'
             self.__ccReportPath = os.path.join(self.__sessionPath, 'assign')
         elif context == 'workflow' or context == 'unknown':
             self.__ccReportPath = os.path.join(self.__sessionPath, 'assign')
@@ -109,16 +110,15 @@
     def getFilePath(self):
         return self.__definitionFilePath
 
     def __getFilePathFromId(self, ccId):
         """
         """
         idUc = str(ccId).upper()
-        fileName = idUc + ".cif"
-        self.__definitionFilePath = os.path.join(self.__ccConfig.getPath('chemCompCachePath'), idUc[0:1], idUc[0:3], fileName)
+        self.__definitionFilePath = self.__crpi.getFilePath(idUc, "CC")
         #
         if (not os.access(self.__definitionFilePath, os.R_OK)):
             return False
         return True
 
     def doReport(self, type=None, ccAssignPthMdfier=None):  # pylint: disable=redefined-builtin
         """ Generate report data -
@@ -269,14 +269,16 @@
         self.__reqObj = reqObj
         #
         self.__sObj = self.__reqObj.getSessionObj()
         self.__sessionPath = self.__sObj.getPath()
         self.__sessionRelativePath = self.__sObj.getRelativePath()
         #
         self.__ccConfig = ChemCompConfig(reqObj, verbose=self.__verbose, log=self.__lfh)
+        siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
+        self.__crpi = ChemRefPathInfo(siteId, verbose=verbose, log=log)
 
         #
         self.__reportFilePath = None
         self.__reportFileRelativePath = None
         self.__definitionId = None
         self.__definitionFilePath = None
 
@@ -295,16 +297,15 @@
 
         return True
 
     def __getFilePathFromId(self, ccId):
         """
         """
         idUc = str(ccId).upper()
-        fileName = idUc + ".cif"
-        self.__definitionFilePath = os.path.join(self.__ccConfig.getPath('chemCompCachePath'), idUc[0:1], idUc[0:3], fileName)
+        self.__definitionFilePath = self.__crpi.getFilePath(idUc, "CC")
         #
         if (not os.access(self.__definitionFilePath, os.R_OK)):
             return False
         return True
 
     def getReportPath(self):
         return self.__reportFileRelativePath
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/search/ChemCompSearch.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearch.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/search/DbSession.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/DbSession.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/utils/ChemCompConfig.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/ChemCompConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 Maintain configuration and path information for chemical component module applications.
 
 """
 
 import sys
 import os
 import os.path
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon, ConfigInfoAppCc
 
 
 class ChemCompConfig(object):
     """ Accessors for configuration and path information for chemical component module applications.
     """
 #
 #    def __init__(self,rootPath,sessionTop,archBinPath,uid, verbose=False,log=sys.stderr):
@@ -44,25 +44,26 @@
         self.__sObj = self.__reqObj.getSessionObj()
         self.__sessionPath = self.__sObj.getPath()
         self.__sessionRelativePath = self.__sObj.getRelativePath()
         self.__sessionId = self.__sObj.getId()
         #
         self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
         self.__cICommon = ConfigInfoAppCommon(self.__siteId)
+        self.__cIAppCc = ConfigInfoAppCc(self.__siteId, verbose=verbose, log=log)
         #
         # derived from the top path by convention
         #
         # JDW 2011-07-07 --- These are symbolic links in the web application top directory
         # self.__archBinPath      =  os.path.join(self.__topPath,"bin")
         # self.__archDataPath      =  os.path.join(self.__topPath,"data")
 
         # RPS 2011-11-29 --- use of above symbolic links for archBinPath and archDataPath being superseded by paths determined via calls to ConfigInfo
         self.__ccAppsBinPath = os.path.join(self.__cICommon.get_site_cc_apps_path(), "bin")
-        self.__ccDictPath = self.__cICommon.get_site_cc_dict_path()
-        self.__ccCvsPath = self.__cICommon.get_site_cc_cvs_path()
+        self.__ccDictPath = self.__cIAppCc.get_site_cc_dict_path()
+        self.__ccCvsPath = self.__cIAppCc.get_site_cc_cvs_path()
         self.__oeLicenseFilePath = self.__cICommon.get_site_cc_oe_licence()
         self.__oeDirPath = self.__cICommon.get_site_cc_oe_dir()
 
         #
         if (self.__verbose):
             self.__lfh.write("+ChemCompConfig.__init() --------------------------------------------------------------------------\n")
             self.__lfh.write("+ChemCompConfig.__init() ------ self.__ccAppsBinPath is: %s \n" % self.__ccAppsBinPath)
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,18 @@
         self._templatePath = os.path.join(self._cI.get('SITE_WEB_APPS_TOP_PATH'), 'htdocs', 'ccmodule_lite')
 
         # setting up session object
         self._setupSession(self._depId)
 
         # setting up chem comp config
         self._ccConfig = ChemCompConfig(self._reqObj, self._verbose, self._lfh)
-        self._ccRefPathInfo = ChemRefPathInfo(configObj=self._cI, configCommonObj=self._cICommon,
-                                              verbose=self._verbose, log=self._lfh)
+
+        siteId = str(self._reqObj.getValue("WWPDB_SITE_ID"))
+
+        self._ccRefPathInfo = ChemRefPathInfo(siteId, verbose=self._verbose, log=self._lfh)
         self._depositPath = Path(PathInfo().getDepositPath(self._depId)).parent
         self._ccReportPath = os.path.join(self._depositPath, self._depId, self._CC_REPORT_DIR)
         self._depositAssignPath = os.path.join(self._depositPath, self._depId, self._CC_ASSIGN_DIR)
         self._ligState = LigandAnalysisState(self._depId, self._verbose, self._lfh)
 
     def doAnalysis(self):
         self._logger.info('Starting analysis for deposition "%s"', self._depId)
@@ -250,16 +252,15 @@
             instId (str): instance ID
             authAssignmentId (str): author assigned ID
             fitTuplDict (dict): dictionary containing image related data
         Raises:
             IOError: if we were not able to read the ligand ".cif" file from
                 the ligand dict
         """
-        ccDictPrefix = self._ccConfig.getPath('chemCompCachePath')
-        chemCompCifPath = os.path.join(ccDictPrefix, topHitCcId[:1], topHitCcId, topHitCcId + '.cif')
+        chemCompCifPath = self._ccRefPathInfo.getFilePath(topHitCcId)
         refImageOutputPath = os.path.join(self._ccReportPath, topHitCcId + '.svg')
 
         if os.access(chemCompCifPath, os.R_OK):
             fitTupleDict[authAssignedId]['alignList'].append((topHitCcId, chemCompCifPath, refImageOutputPath))
         else:
             # raising here since it's expected to be able to read the ligand ".cif"
             # file from the ligand dict
@@ -271,16 +272,15 @@
 
         Args:
             ccid (str): ligand ID
 
         Returns:
             bool: True if the ligand has an entry in the dictionary, False otherwise
         """
-        ccDictPrefix = self._ccConfig.getPath('chemCompCachePath')
-        ligandEntryPath = os.path.join(ccDictPrefix, ccid[:1], ccid, ccid + '.cif')
+        ligandEntryPath = self._ccRefPathInfo.getFilePath(ccid)
 
         if not os.access(ligandEntryPath, os.R_OK):
             self._logger.warning('Ligand ID %s has no corresponding dict ref file at %s', ccid, ligandEntryPath)
 
             return False
 
         return True
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/utils/Exceptions.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/view/ChemCompView.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/view/ChemCompView.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,14 @@
 from wwpdb.apps.ccmodule.reports.ChemCompAlignImageGenerator import ChemCompAlignImageGenerator
 from wwpdb.apps.ccmodule.reports.ChemCompReports import ChemCompReport
 from wwpdb.apps.ccmodule.reports.InstanceDataGenerator import InstanceDataGenerator
 from wwpdb.apps.ccmodule.sketch.ChemCompSketch import ChemCompSketch
 from wwpdb.apps.ccmodule.sketch.ChemCompSketchDepict import ChemCompSketchDepict
 #
 from wwpdb.utils.wf.dbapi.WfTracking import WfTracking
-from wwpdb.apps.ccmodule.utils.ChemCompConfig import ChemCompConfig
 #
 from wwpdb.apps.ccmodule.io.ChemCompAssignDataStore import ChemCompAssignDataStore
 from wwpdb.apps.ccmodule.io.ChemCompDataImport import ChemCompDataImport
 from wwpdb.apps.ccmodule.io.ChemCompDataExport import ChemCompDataExport
 from wwpdb.apps.ccmodule.io.ChemCompIo import ChemCompReader
 #
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
@@ -171,14 +170,15 @@
 #
 from wwpdb.io.file.mmCIFUtil import mmCIFUtil
 #
 from wwpdb.utils.oe_util.oedepict.OeDepict import OeDepict
 from wwpdb.utils.oe_util.build.OeBuildMol import OeBuildMol
 #
 from wwpdb.io.locator.PathInfo import PathInfo
+from wwpdb.io.locator.ChemRefPathInfo import ChemRefPathInfo
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 
 
 class ChemCompWebApp(object):
     """Handle request and response object processing for the chemical component editor tool application.
 
     """
@@ -294,15 +294,14 @@
         self.__reqObj = reqObj
         self.__sObj = None
         self.__sessionId = None
         self.__sessionPath = None
         self.__rltvSessionPath = None
         self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
         self.__cI = ConfigInfo(self.__siteId)
-        self.__ccConfig = ChemCompConfig(reqObj, verbose=self.__verbose, log=self.__lfh)
         self.__modelFilePath = None
         #
         self.__pathInstncsVwTmplts = "templates/workflow_ui/instances_view"
         self.__pathSnglInstcTmplts = self.__pathInstncsVwTmplts + "/single_instance"
         self.__pathSnglInstcEditorTmplts = self.__pathSnglInstcTmplts + "/editor"
         #
         self.__appPathD = {'/service/environment/dump': '_dumpOp',
@@ -1578,16 +1577,16 @@
         instIdList = str(self.__reqObj.getValue("instidlist"))
         # instncMode = str(self.__reqObj.getValue("instncmode"))
         ccId = str(self.__reqObj.getValue("ccid")).upper()
         #
         self.__reqObj.setReturnFormat(return_format="json")
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
         #
-        pathPrefix = self.__ccConfig.getPath('chemCompCachePath')
-        validationPth = os.path.join(pathPrefix, ccId[:1], ccId, ccId + '.cif')
+        crpi = ChemRefPathInfo(siteId=self.__siteId, verbose=self.__verbose, log=self.__lfh)
+        validationPth = crpi.getFilePath(ccId, "CC")
         if (self.__verbose):
             self.__lfh.write("+ChemCompWebAppWorker._ccAssign_validateCcId() ---- validating CC ID %s against path: %s\n" % (ccId, validationPth))
         if not os.access(validationPth, os.R_OK):
             errorMessage = '"' + ccId + '" is not a valid Code.'
             rC.setError(errMsg=errorMessage)
             return rC
         #
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,27 +102,27 @@
 #
 # from wwpdb.apps.ccmodule.search.ChemCompSearch import ChemCompSearch
 # from wwpdb.apps.ccmodule.search.ChemCompSearchDepict import ChemCompSearchDepict
 # from wwpdb.apps.ccmodule.search.ChemCompSearchDb import ChemCompSearchDb
 # from wwpdb.apps.ccmodule.search.ChemCompSearchDbDepict import ChemCompSearchDbDepict
 #
 # from wwpdb.utils.wf.dbapi.WfTracking import WfTracking
-from wwpdb.apps.ccmodule.utils.ChemCompConfig import ChemCompConfig
 #
 from wwpdb.apps.ccmodule.io.ChemCompAssignDataStore import ChemCompAssignDataStore
 from wwpdb.apps.ccmodule.io.ChemCompDataExport import ChemCompDataExport
 #
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
 from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
 #
 from wwpdb.io.file.mmCIFUtil import mmCIFUtil
 
 from wwpdb.utils.wf.dbapi.WfDbApi import WfDbApi
 from wwpdb.utils.wf.dbapi.WFEtime import getTimeNow
 from wwpdb.io.locator.PathInfo import PathInfo
+from wwpdb.io.locator.ChemRefPathInfo import ChemRefPathInfo
 
 
 class ChemCompWebAppLite(object):
     """Handle request and response object processing for the chemical component lite module application.
 
     """
     def __init__(self, parameterDict=None, verbose=False, log=sys.stderr, siteId="WWPDB_DEV"):
@@ -243,15 +243,14 @@
         self.__depId = "D_0" if self.__reqObj.getValue("identifier") in [None, 'TMP_ID'] else self.__reqObj.getValue("identifier").upper()
         self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
         self.__cI = ConfigInfo(self.__siteId)
         self.__deployPath = self.__cI.get('SITE_DEPLOY_PATH')
         self.__siteSrvcUrlPathPrefix = self.__cI.get('SITE_SERVICE_URL_PATH_PREFIX', '')
         # self.__siteConfigDir = self.__cI.get('TOP_WWPDB_SITE_CONFIG_DIR')
         # self.__siteLoc = self.__cI.get('WWPDB_SITE_LOC')
-        self.__ccConfig = ChemCompConfig(reqObj, verbose=self.__verbose, log=self.__lfh)
         self.__pathInfo = PathInfo()
         self.__depositPath = Path(self.__pathInfo.getDepositPath(self.__depId)).parent
         # self.__depositAssignPath = os.path.join(self.__depositPath, self.__depId, 'assign')
         # self.__ccReportPath = os.path.join(self.__depositPath, self.__depId, 'cc_analysis')  # should we add 'cc_analysis' in a variable in site-config?
         self.__logger = self._setupLog(log)
 
         #
@@ -1130,16 +1129,17 @@
         self.__getSession()
         vldtMode = str(self.__reqObj.getValue("vldtmode"))
         ccId = str(self.__reqObj.getValue("alt_ccid")).upper()
         #
         self.__reqObj.setReturnFormat(return_format="json")
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
         #
-        pathPrefix = self.__ccConfig.getPath('chemCompCachePath')
-        validationPth = os.path.join(pathPrefix, ccId[:1], ccId, ccId + '.cif')
+
+        crpi = ChemRefPathInfo(self.__siteId, verbose=self.__verbose, log=self.__lfh)
+        validationPth = crpi.getFilePath(ccId, "CC")
         if (self.__verbose):
             self.__lfh.write("+%s.%s() ---- validating CC ID %s against path: %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, ccId, validationPth))
         if not os.access(validationPth, os.R_OK):
             errorMessage = '"' + ccId + '" is not a valid Code.'
             rC.setError(errMsg=errorMessage)
             return rC
         #
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb/apps/ccmodule/webapp/wsgi.py` & `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/wsgi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb.apps.ccmodule.egg-info/PKG-INFO` & `wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ccmodule
-Version: 0.25.dev1
+Version: 0.26
 Summary: wwPDB workflow engine utils
 Home-page: https://github.com/rcsb/py-wwpdb_apps_wf_engine_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ccmodule-0.25.dev1/wwpdb.apps.ccmodule.egg-info/SOURCES.txt` & `wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 wwpdb.apps.ccmodule.egg-info/SOURCES.txt
 wwpdb.apps.ccmodule.egg-info/dependency_links.txt
 wwpdb.apps.ccmodule.egg-info/not-zip-safe
 wwpdb.apps.ccmodule.egg-info/requires.txt
 wwpdb.apps.ccmodule.egg-info/top_level.txt
 wwpdb/apps/__init__.py
 wwpdb/apps/ccmodule/__init__.py
-wwpdb/apps/ccmodule/admin/ChemCompAdmin.py
-wwpdb/apps/ccmodule/admin/__init__.py
 wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py
 wwpdb/apps/ccmodule/chem/ChemCompAssign.py
 wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py
 wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py
 wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py
 wwpdb/apps/ccmodule/chem/__init__.py
 wwpdb/apps/ccmodule/depict/ChemCompDepict.py
@@ -26,15 +24,14 @@
 wwpdb/apps/ccmodule/extract/__init__.py
 wwpdb/apps/ccmodule/extract/ccOps.py
 wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py
 wwpdb/apps/ccmodule/io/ChemCompDataExport.py
 wwpdb/apps/ccmodule/io/ChemCompDataImport.py
 wwpdb/apps/ccmodule/io/ChemCompEditStore.py
 wwpdb/apps/ccmodule/io/ChemCompIo.py
-wwpdb/apps/ccmodule/io/PdbxChemComp.py
 wwpdb/apps/ccmodule/io/__init__.py
 wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py
 wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py
 wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py
 wwpdb/apps/ccmodule/reports/ChemCompGenImage.py
 wwpdb/apps/ccmodule/reports/ChemCompReports.py
 wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py
```

