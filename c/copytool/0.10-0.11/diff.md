# Comparing `tmp/copytool-0.10.tar.gz` & `tmp/copytool-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copytool-0.10.tar", last modified: Sat May 13 08:08:44 2023, max compression
+gzip compressed data, was "copytool-0.11.tar", last modified: Sun May 14 21:22:35 2023, max compression
```

## Comparing `copytool-0.10.tar` & `copytool-0.11.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 08:08:44.053899 copytool-0.10/
--rw-rw-rw-   0        0        0     1148 2023-05-13 08:08:36.000000 copytool-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      274 2023-05-13 08:08:35.000000 copytool-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     1868 2023-05-13 08:08:44.053899 copytool-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1270 2023-05-13 08:03:15.000000 copytool-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 08:08:44.047915 copytool-0.10/copytool/
--rw-rw-rw-   0        0        0     1270 2023-05-13 08:03:15.000000 copytool-0.10/copytool/README.md
--rw-rw-rw-   0        0        0     7470 2023-05-13 07:55:40.000000 copytool-0.10/copytool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 08:08:44.052901 copytool-0.10/copytool/buffcall/
--rw-rw-rw-   0        0        0       30 2023-05-13 07:17:51.000000 copytool-0.10/copytool/buffcall/__init__.py
--rw-rw-rw-   0        0        0    17920 2023-05-13 07:13:40.000000 copytool-0.10/copytool/buffcall/buffercalc.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0    17920 2023-05-13 07:13:40.000000 copytool-0.10/copytool/buffercalc.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0      514 2023-05-13 03:49:46.000000 copytool-0.10/copytool/buffercalc.pyx
--rw-rw-rw-   0        0        0       69 2023-05-13 08:08:43.000000 copytool-0.10/copytool/requirements.txt
--rw-rw-rw-   0        0        0     8933 2023-05-13 08:08:43.000000 copytool-0.10/copytool/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-13 08:08:44.050906 copytool-0.10/copytool.egg-info/
--rw-rw-rw-   0        0        0     1868 2023-05-13 08:08:43.000000 copytool-0.10/copytool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-05-13 08:08:43.000000 copytool-0.10/copytool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 08:08:43.000000 copytool-0.10/copytool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-13 08:08:43.000000 copytool-0.10/copytool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-13 08:08:43.000000 copytool-0.10/copytool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-13 08:08:44.054896 copytool-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1413 2023-05-13 08:08:43.000000 copytool-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 21:22:35.357171 copytool-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-05-14 21:22:26.000000 copytool-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      274 2023-05-14 21:22:24.000000 copytool-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     1868 2023-05-14 21:22:35.357171 copytool-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1270 2023-05-13 08:11:38.000000 copytool-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 21:22:35.351186 copytool-0.11/copytool/
+-rw-rw-rw-   0        0        0     1270 2023-05-13 08:11:38.000000 copytool-0.11/copytool/README.md
+-rw-rw-rw-   0        0        0     7946 2023-05-14 21:19:43.000000 copytool-0.11/copytool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 21:22:35.356173 copytool-0.11/copytool/buffcall/
+-rw-rw-rw-   0        0        0       30 2023-05-13 08:11:38.000000 copytool-0.11/copytool/buffcall/__init__.py
+-rw-rw-rw-   0        0        0    17920 2023-05-13 08:11:38.000000 copytool-0.11/copytool/buffcall/buffercalc.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0    17920 2023-05-13 08:11:38.000000 copytool-0.11/copytool/buffercalc.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0      514 2023-05-13 08:11:38.000000 copytool-0.11/copytool/buffercalc.pyx
+-rw-rw-rw-   0        0        0       69 2023-05-14 21:22:34.000000 copytool-0.11/copytool/requirements.txt
+-rw-rw-rw-   0        0        0     8933 2023-05-14 21:22:34.000000 copytool-0.11/copytool/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-14 21:22:35.354179 copytool-0.11/copytool.egg-info/
+-rw-rw-rw-   0        0        0     1868 2023-05-14 21:22:35.000000 copytool-0.11/copytool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-05-14 21:22:35.000000 copytool-0.11/copytool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 21:22:35.000000 copytool-0.11/copytool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-14 21:22:35.000000 copytool-0.11/copytool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 21:22:35.000000 copytool-0.11/copytool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-14 21:22:35.358168 copytool-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1413 2023-05-14 21:22:34.000000 copytool-0.11/setup.py
```

### Comparing `copytool-0.10/LICENSE.rst` & `copytool-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `copytool-0.10/PKG-INFO` & `copytool-0.11/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copytool
-Version: 0.10
+Version: 0.11
 Summary: copytool copies files hell-bent for leather
 Home-page: https://github.com/hansalemaos/copytool
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: copy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `copytool-0.10/README.md` & `copytool-0.11/README.md`

 * *Files identical despite different names*

### Comparing `copytool-0.10/copytool/README.md` & `copytool-0.11/copytool/README.md`

 * *Files identical despite different names*

### Comparing `copytool-0.10/copytool/__init__.py` & `copytool-0.11/copytool/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,19 +44,22 @@
 conf = sys.modules[__name__]
 conf.tq = None
 conf.uffsfilepath = None
 try:
     O_BINARY = os.O_BINARY
 except:
     O_BINARY = 0
-READ_FLAGS = os.O_RDONLY | O_BINARY
-WRITE_FLAGS = os.O_WRONLY | os.O_CREAT | os.O_TRUNC | O_BINARY
+READ_FLAGS = os.O_RDONLY | O_BINARY #| os.O_RANDOM #| os.O_NOINHERIT | os.O_RANDOM #os.O_SEQUENTIAL #| os.O_NOINHERIT | os.O_SEQUENTIAL #| os.O_SHORT_LIVED
+WRITE_FLAGS = os.O_WRONLY | os.O_CREAT | os.O_TRUNC | O_BINARY #| os.O_RANDOM   #| os.O_NOINHERIT | os.O_RANDOM #os.O_SEQUENTIAL# os.O_NOINHERIT |  # | os.O_SHORT_LIVED  #| os.O_TEMPORARY #| os.O_SHORT_LIVED
 kernel32 = WinDLL("kernel32", use_last_error=True)
+r"""
+.\python.exe "C:\ProgramData\anaconda3\envs\dfdir\Lib\site-packages\copytool\__init__.py" --src "C:\ProgramData\anaconda3\envs" --dst "e:\envbackup1x9" --use_tqdm 1 --copy_date 1 --copy_permission 0 --overwrite 1
+"""
 
-
+# | os.O_NOINHERIT | os.O_SEQUENTIAL
 @cache
 def mkdirsall(folderfipath):
     try:
         if not os.path.exists(folderfipath):
             os.makedirs(folderfipath)
         return folderfipath
     except Exception:
@@ -141,21 +144,20 @@
 
 def copyfile(
         src: str, dst: str, copystat: bool = True, buffer: int = 1000 * 1024
 ) -> bool:
     copyok = False
     buffer = get_mu2(buffer)
     try:
-        if not copystat:
-            fin = os.open(src, READ_FLAGS)
-            stat_ = os.fstat(fin)
-            fout = os.open(dst, WRITE_FLAGS, stat_.st_mode)
-            for x in iter(lambda: os.read(fin, buffer), b""):
-                os.write(fout, x)
-            copyok = True
+        fin = os.open(src, READ_FLAGS)
+        stat_ = os.fstat(fin)
+        fout = os.open(dst, WRITE_FLAGS, stat_.st_mode)
+        for x in iter(lambda: os.read(fin, buffer), b""):
+            os.write(fout, x)
+        copyok = True
     finally:
         try:
             os.close(fout)
         except Exception:
             pass
         try:
             os.close(fin)
@@ -168,15 +170,15 @@
 
 
 @add_sysargv
 def get_all_files_on_hdd_and_copy(
         src: str = "",
         dst: str = "",
         log: str = "",
-        copy_date: int = 0,
+        copy_date: int = 1,
         copy_permission: int = 0,
         use_tqdm: int = 1,
         overwrite: int = 1,
 ):
     print(locals())
     copy_date = bool(copy_date)
     copy_permission = bool(copy_permission)
```

### Comparing `copytool-0.10/copytool/buffercalc.pyx` & `copytool-0.11/copytool/buffercalc.pyx`

 * *Files identical despite different names*

### Comparing `copytool-0.10/copytool/thirdparty.json` & `copytool-0.11/copytool/thirdparty.json`

 * *Files identical despite different names*

### Comparing `copytool-0.10/copytool.egg-info/PKG-INFO` & `copytool-0.11/copytool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copytool
-Version: 0.10
+Version: 0.11
 Summary: copytool copies files hell-bent for leather
 Home-page: https://github.com/hansalemaos/copytool
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: copy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `copytool-0.10/setup.py` & `copytool-0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''copytool copies files hell-bent for leather'''
 
 # Setting up
 setup(
     name="copytool",
     version=VERSION,
     license='MIT',
```

