# Comparing `tmp/wwpdb.apps.chemeditor-0.12.tar.gz` & `tmp/wwpdb.apps.chemeditor-0.12.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.chemeditor-0.12.tar", last modified: Sun May 14 15:19:03 2023, max compression
+gzip compressed data, was "wwpdb.apps.chemeditor-0.12.dev1.tar", last modified: Sun Apr  2 17:40:30 2023, max compression
```

## Comparing `wwpdb.apps.chemeditor-0.12.tar` & `wwpdb.apps.chemeditor-0.12.dev1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:19:03.738033 wwpdb.apps.chemeditor-0.12/
--rw-r--r--   0 vsts      (1001) docker     (123)      722 2023-05-14 15:19:03.738033 wwpdb.apps.chemeditor-0.12/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       53 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-05-14 15:19:03.738033 wwpdb.apps.chemeditor-0.12/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2103 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:19:03.734033 wwpdb.apps.chemeditor-0.12/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:19:03.734033 wwpdb.apps.chemeditor-0.12/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:19:03.734033 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:19:03.738033 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)     2139 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/AtomMatch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18894 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/CVSCommit.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2062 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/ChemCompHash.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9257 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/ChemEditorBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)    20819 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/ChemEditorWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2003 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/DaInternalCombineDb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2383 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/Enumeration.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4043 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/Get2D.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1881 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/GetLigand.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3819 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/SaveLigand.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4085 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/Search.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5559 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/UpdateLigand.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3471 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/Upload.py
--rw-r--r--   0 vsts      (1001) docker     (123)      889 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/Utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:17:40.000000 wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:19:03.734033 wwpdb.apps.chemeditor-0.12/wwpdb.apps.chemeditor.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      722 2023-05-14 15:19:03.000000 wwpdb.apps.chemeditor-0.12/wwpdb.apps.chemeditor.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1017 2023-05-14 15:19:03.000000 wwpdb.apps.chemeditor-0.12/wwpdb.apps.chemeditor.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 15:19:03.000000 wwpdb.apps.chemeditor-0.12/wwpdb.apps.chemeditor.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 15:18:48.000000 wwpdb.apps.chemeditor-0.12/wwpdb.apps.chemeditor.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      139 2023-05-14 15:19:03.000000 wwpdb.apps.chemeditor-0.12/wwpdb.apps.chemeditor.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-05-14 15:19:03.000000 wwpdb.apps.chemeditor-0.12/wwpdb.apps.chemeditor.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 17:40:30.859336 wwpdb.apps.chemeditor-0.12.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      727 2023-04-02 17:40:30.859336 wwpdb.apps.chemeditor-0.12.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       53 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-02 17:40:30.859336 wwpdb.apps.chemeditor-0.12.dev1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2237 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 17:40:30.847336 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 17:40:30.851336 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 17:40:30.851336 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 17:40:30.859336 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2139 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/AtomMatch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18974 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/CVSCommit.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2073 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/ChemCompHash.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8920 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/ChemEditorBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    20803 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/ChemEditorWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2003 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/DaInternalCombineDb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2383 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/Enumeration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4043 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/Get2D.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1881 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/GetLigand.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3819 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/SaveLigand.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4085 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/Search.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5559 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/UpdateLigand.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3471 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/Upload.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      889 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/Utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-02 17:39:12.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 17:40:30.851336 wwpdb.apps.chemeditor-0.12.dev1/wwpdb.apps.chemeditor.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      727 2023-04-02 17:40:30.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb.apps.chemeditor.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1017 2023-04-02 17:40:30.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb.apps.chemeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-02 17:40:30.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb.apps.chemeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-02 17:40:14.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb.apps.chemeditor.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      133 2023-04-02 17:40:30.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb.apps.chemeditor.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-02 17:40:30.000000 wwpdb.apps.chemeditor-0.12.dev1/wwpdb.apps.chemeditor.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.chemeditor-0.12/PKG-INFO` & `wwpdb.apps.chemeditor-0.12.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.chemeditor
-Version: 0.12
+Version: 0.12.dev1
 Summary: wwPDB chemical editor
 Home-page: https://github.com/rcsb/py-wwpdb_apps_chemeditor
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/AtomMatch.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/AtomMatch.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/CVSCommit.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/CVSCommit.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         self.__existingFlag = self._reqObj.getValue("existflag")
         #
         if not self.__id:
             return
         #
         self.getSandBoxFilePath(self.__id)
         self.__sourceFile = os.path.join(self._sessionPath, self.__id + ".cif")
-        self.__targetPath = self._crpi.getFileDir(self.__id, "CC")
+        self.__targetPath = os.path.join(self._ccPath, self.__id[0], self.__id)
 
     def __checkIDExisted(self):
         """ Check if Ligand ID exists
         """
         if not self.__targetPath:
             return "CVS commit failed"
         #
@@ -325,15 +325,15 @@
         parent_comp_ids = cifObj.GetSingleValue("chem_comp", "mon_nstd_parent_comp_id")
         if parent_comp_ids:
             comp_ids = parent_comp_ids.replace("\n\r", " ").replace("\n", " ").replace("\r", " ").replace(";", " ").replace(",", " ")
             for comp_id in comp_ids.split(" "):
                 if not comp_id:
                     continue
                 #
-                targetFile = self._crpi.getFilePath(comp_id, "CC")
+                targetFile = os.path.join(self._ccPath, comp_id[0], comp_id, comp_id + ".cif")
                 if (not targetFile) or (not os.access(targetFile, os.F_OK)):
                     errorMessage = "Incorrect parent compId: '" + parent_comp_ids + "'.\n\n"
                     break
                 #
             #
         #
         if noErrorFlag and synonyms and (not errorMessage):
@@ -450,41 +450,35 @@
         """ Run CVS commit
         """
         if (not sourceFilePath) or (not os.access(sourceFilePath, os.R_OK)):
             return "CVS commit failed - Cannot update nonexistent file"
         #
         targetFile = self.getSandBoxFilePath(ccId)
         textList = []
-
-        proj, rel_path = self._crpi.getCvsProjectInfo(ccId, "CC")
-
-        relDir = os.path.dirname(rel_path)
-        projFile = os.path.join(proj, rel_path)
-
         try:
             if targetFile and os.access(targetFile, os.F_OK):
-                self._cvsAdmin.checkOut(projFile)
+                self._cvsAdmin.checkOut(os.path.join(self._ccProjectName, ccId[0], ccId, ccId + ".cif"))
                 shutil.copy2(sourceFilePath, targetFile)
             else:
-                dstPath = self._crpi.getFileDir(ccId, "CC")
-                targetFile = self._crpi.getFilePath(ccId, "CC")
+                dstPath = os.path.join(self._ccPath, ccId[0], ccId)
+                targetFile = os.path.join(dstPath, ccId + ".cif")
                 if (not os.access(dstPath, os.F_OK)):
                     os.makedirs(dstPath)
-                    ok, text = self._cvsAdmin.add(proj, relDir)
+                    ok, text = self._cvsAdmin.add(self._ccProjectName, os.path.join(ccId[0], ccId))
                     if (not ok) and text:
                         textList.append(text)
                     #
                 #
                 shutil.copy2(sourceFilePath, targetFile)
-                ok, text = self._cvsAdmin.add(proj, rel_path)
+                ok, text = self._cvsAdmin.add(self._ccProjectName, os.path.join(ccId[0], ccId, ccId + ".cif"))
                 if (not ok) and text:
                     textList.append(text)
                 #
             #
-            ok, text = self._cvsAdmin.commit(proj, rel_path)
+            ok, text = self._cvsAdmin.commit(self._ccProjectName, os.path.join(ccId[0], ccId, ccId + ".cif"))
             ok = True
             if (not ok) and text:
                 textList.append(text)
             #
         except:  # noqa: E722 pylint: disable=bare-except
             textList.append("CVS commit failed - CVS update exception")
             traceback.print_exc(file=self._lfh)
```

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/ChemEditorBase.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/ChemEditorBase.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,18 +20,16 @@
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.07"
 
 import os
 import sys
 
 from wwpdb.io.cvs.CvsAdmin import CvsSandBoxAdmin
-from wwpdb.io.locator.ChemRefPathInfo import ChemRefPathInfo
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
 from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCc
 
 
 class ChemEditorBase(object):
     """  Class handle various system and C++ applications setting.
     """
 
     def __init__(self, reqObj=None, verbose=False, log=sys.stderr):
@@ -41,38 +39,32 @@
         self._sObj = None
         self._sessionId = None
         self._sessionPath = None
         self._rltvSessionPath = None
         self.__siteId = str(self._reqObj.getValue("WWPDB_SITE_ID"))
         self._cI = ConfigInfo(self.__siteId)
         self._cICommon = ConfigInfoAppCommon(self.__siteId)
-        self._cIAppCc = ConfigInfoAppCc(self.__siteId)
-        self.__sbTopPath = self._cIAppCc.get_site_refdata_top_cvs_sb_path()  # "/wwpdb_da/da_top/reference/components"
+        self.__sbTopPath = self._cICommon.get_site_refdata_top_cvs_sb_path()  # "/wwpdb_da/da_top/reference/components"
         self._ccProjectName = self._cI.get("SITE_REFDATA_PROJ_NAME_CC")  # "ligand-dict-v3"
-        self._ccPath = self._cIAppCc.get_site_cc_cvs_path()
-        self._crpi = ChemRefPathInfo(siteId=self.__siteId, verbose=self._verbose, log=self._lfh)
-
+        self._ccPath = self._cICommon.get_site_cc_cvs_path()
         #
         self.__getSession()
         #
         self._cvsAdmin = self.__setupCvs()
 
     def getSandBoxFilePath(self, ccId):
         """ Return full sandbox chemical component file path
         """
-
-        filePath = self._crpi.getFilePath(ccId, "CC")
+        filePath = os.path.join(self._ccPath, ccId[0], ccId, ccId + ".cif")
         self._lfh.write("enter ChemEditorBase.getSandBoxFilePath for ccId=%s filePath=%s\n" % (ccId, filePath))
         if os.access(filePath, os.F_OK):
             return filePath
         #
         self._lfh.write("ChemEditorBase.getSandBoxFilePath running checkOut\n")
-        proj, rel_path = self._crpi.getCvsProjectInfo(ccId, "CC")
-        fileDir = os.path.dirname(os.path.join(proj, rel_path))
-        self._cvsAdmin.checkOut(fileDir)
+        self._cvsAdmin.checkOut(os.path.join(self._ccProjectName, ccId[0], ccId))
         # self._cvsAdmin.cleanup()
         #
         if os.access(filePath, os.F_OK):
             return filePath
         #
         return ""
 
@@ -85,15 +77,15 @@
         #
         return self.getSandBoxFilePath(ccId)
 
     def _annotBashSetting(self):
         """
         """
         setting = " RCSBROOT=" + self._cICommon.get_site_annot_tools_path() + "; export RCSBROOT; " \
-                  + " COMP_PATH=" + self._cIAppCc.get_site_cc_cvs_path() + "; export COMP_PATH; " \
+                  + " COMP_PATH=" + self._cICommon.get_site_cc_cvs_path() + "; export COMP_PATH; " \
                   + " BINPATH=${RCSBROOT}/bin; export BINPATH; "
         return setting
 
     def _ccToolsBashSetting(self):
         """
         """
         setting = (" CC_TOOLS=" + os.path.join(self._cICommon.get_site_cc_apps_path(), "bin") + "; export CC_TOOLS; "
@@ -120,17 +112,17 @@
                   + " DICT_ODB_FILE=${PDBX_DICT_PATH}/${DICT_NAME}.odb; export DICT_ODB_FILE; "
         return setting
 
     def _ccDictBashSetting(self):
         """
         """
         setting = []
-        setting.append(" CC_DICT={}; export CC_DICT; ".format(self._cIAppCc.get_site_cc_dict_path()))
-        setting.append(" CC_IDX_FILE={}; export CC_IDX_FILE; ".format(self._cIAppCc.get_cc_dict_idx()))
-        setting.append(" CC_SDB_FILE={}; export CC_SDB_FILE; ".format(self._cIAppCc.get_cc_dict_serial()))
+        setting.append(" CC_DICT={}; export CC_DICT; ".format(self._cICommon.get_site_cc_dict_path()))
+        setting.append(" CC_IDX_FILE={}; export CC_IDX_FILE; ".format(self._cICommon.get_cc_dict_idx()))
+        setting.append(" CC_SDB_FILE={}; export CC_SDB_FILE; ".format(self._cICommon.get_cc_dict_serial()))
         return ''.join(setting)
 
     def _runCmd(self, cmd):
         """
         """
         self._lfh.write("running cmd=%s\n" % cmd)
         os.system(cmd)
```

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/ChemEditorWebApp.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/ChemEditorWebApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 __version__ = "V0.07"
 
 import os
 import sys
 import traceback
 
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCc
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
 from wwpdb.utils.session.WebRequest import InputRequest, ResponseContent
 
 from wwpdb.apps.chemeditor.webapp.AtomMatch import AtomMatch
 # from wwpdb.apps.chemeditor.webapp.ChemCompHash import ChemCompHash
 from wwpdb.apps.chemeditor.webapp.ChemEditorBase import ChemEditorBase
 from wwpdb.apps.chemeditor.webapp.CVSCommit import CVSCommit
 from wwpdb.apps.chemeditor.webapp.Enumeration import Enumeration
@@ -149,15 +149,15 @@
          supplied with control information from web application request
          or from a testing application.
         """
         self.__verbose = verbose
         self.__lfh = log
         self.__reqObj = reqObj
         self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
-        self.__cIAppCc = ConfigInfoAppCc(self.__siteId, verbose=verbose, log=log)
+        self.__cICommon = ConfigInfoAppCommon(self.__siteId)
         #
         self.__appPathD = {'/service/environment/dump': '_dumpOp',
                            '/service/chemeditor/get_2d': '_get2D',
                            '/service/chemeditor/upload': '_upLoad',
                            '/service/chemeditor/get_ligand': '_getLigand',
                            '/service/chemeditor/search': '_searchLigand',
                            '/service/chemeditor/atom_match': '_atomMatch',
@@ -365,15 +365,15 @@
         return rC
 
     def __getNewCodeFromList(self):
         """ Get unused Ligand Code from pre-defined list
         """
         cvsUtil = ChemEditorBase(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
         code = ''
-        filePath = os.path.join(self.__cIAppCc.get_unused_ccd_file())
+        filePath = os.path.join(self.__cICommon.get_unused_ccd_file())
         self.__lfh.write("+ChemEditorWebAppWorker.__getNewCodeFromList filePath=%s\n" % filePath)
         f = open(filePath, 'r')
         data = f.read()
         f.close()
         #
 #       cCH = ChemCompHash()
         idlist = data.split('\n')
```

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/DaInternalCombineDb.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/DaInternalCombineDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/Enumeration.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/Enumeration.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/Get2D.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/Get2D.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/GetLigand.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/GetLigand.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/SaveLigand.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/SaveLigand.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/Search.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/Search.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/UpdateLigand.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/UpdateLigand.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/Upload.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/Upload.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb/apps/chemeditor/webapp/Utils.py` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb/apps/chemeditor/webapp/Utils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb.apps.chemeditor.egg-info/PKG-INFO` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb.apps.chemeditor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.chemeditor
-Version: 0.12
+Version: 0.12.dev1
 Summary: wwPDB chemical editor
 Home-page: https://github.com/rcsb/py-wwpdb_apps_chemeditor
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.chemeditor-0.12/wwpdb.apps.chemeditor.egg-info/SOURCES.txt` & `wwpdb.apps.chemeditor-0.12.dev1/wwpdb.apps.chemeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

