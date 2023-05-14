# Comparing `tmp/xgit-python-0.3.tar.gz` & `tmp/xgit-python-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgit-python-0.3.tar", last modified: Sat Mar 25 17:32:10 2023, max compression
+gzip compressed data, was "xgit-python-0.4.tar", last modified: Sun May 14 17:55:51 2023, max compression
```

## Comparing `xgit-python-0.3.tar` & `xgit-python-0.4.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 17:32:10.526438 xgit-python-0.3/
--rw-rw-rw-   0        0        0     1105 2023-03-17 13:37:21.000000 xgit-python-0.3/LICENSE
--rw-rw-rw-   0        0        0      673 2023-03-25 17:32:10.527437 xgit-python-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-03-22 17:04:18.000000 xgit-python-0.3/README.md
--rw-rw-rw-   0        0        0     1128 2023-03-25 17:32:10.529875 xgit-python-0.3/setup.cfg
--rw-rw-rw-   0        0        0      103 2023-03-17 13:37:21.000000 xgit-python-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-25 17:32:10.492794 xgit-python-0.3/xgit/
--rw-rw-rw-   0        0        0       73 2023-03-25 17:31:57.000000 xgit-python-0.3/xgit/__init__.py
--rw-rw-rw-   0        0        0     1328 2023-03-25 13:11:28.000000 xgit-python-0.3/xgit/xgit_command.py
--rw-rw-rw-   0        0        0      841 2023-03-25 11:38:31.000000 xgit-python-0.3/xgit/xgit_filter.py
--rw-rw-rw-   0        0        0     1697 2023-03-25 17:27:25.000000 xgit-python-0.3/xgit/xgit_modify_author.py
--rw-rw-rw-   0        0        0     1742 2023-03-25 17:27:34.000000 xgit-python-0.3/xgit/xgit_modify_committer.py
--rw-rw-rw-   0        0        0     2150 2023-03-25 13:09:45.000000 xgit-python-0.3/xgit/xgit_summary.py
--rw-rw-rw-   0        0        0     1662 2023-03-23 17:07:07.000000 xgit-python-0.3/xgit/xgit_util.py
-drwxrwxrwx   0        0        0        0 2023-03-25 17:32:10.523443 xgit-python-0.3/xgit_python.egg-info/
--rw-rw-rw-   0        0        0      673 2023-03-25 17:32:10.000000 xgit-python-0.3/xgit_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-03-25 17:32:10.000000 xgit-python-0.3/xgit_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 17:32:10.000000 xgit-python-0.3/xgit_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2023-03-25 17:32:10.000000 xgit-python-0.3/xgit_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2023-03-25 17:32:10.000000 xgit-python-0.3/xgit_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-25 17:32:10.000000 xgit-python-0.3/xgit_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-25 17:32:10.000000 xgit-python-0.3/xgit_python.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-14 17:55:51.236307 xgit-python-0.4/
+-rw-rw-rw-   0        0        0     1105 2023-03-17 13:37:21.000000 xgit-python-0.4/LICENSE
+-rw-rw-rw-   0        0        0      701 2023-05-14 17:55:51.236868 xgit-python-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-03-22 17:04:18.000000 xgit-python-0.4/README.md
+-rw-rw-rw-   0        0        0     1163 2023-05-14 17:55:51.239271 xgit-python-0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 17:55:51.213364 xgit-python-0.4/xgit/
+-rw-rw-rw-   0        0        0       73 2023-05-14 16:50:27.000000 xgit-python-0.4/xgit/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-05-14 17:53:21.000000 xgit-python-0.4/xgit/xgit_command.py
+-rw-rw-rw-   0        0        0      863 2023-05-14 17:51:07.000000 xgit-python-0.4/xgit/xgit_filter.py
+-rw-rw-rw-   0        0        0     1674 2023-05-14 17:52:06.000000 xgit-python-0.4/xgit/xgit_modify_author.py
+-rw-rw-rw-   0        0        0     1753 2023-05-14 17:52:13.000000 xgit-python-0.4/xgit/xgit_modify_committer.py
+-rw-rw-rw-   0        0        0     2180 2023-05-14 17:53:54.000000 xgit-python-0.4/xgit/xgit_summary.py
+-rw-rw-rw-   0        0        0     1668 2023-04-19 12:35:01.000000 xgit-python-0.4/xgit/xgit_util.py
+drwxrwxrwx   0        0        0        0 2023-05-14 17:55:51.234082 xgit-python-0.4/xgit_python.egg-info/
+-rw-rw-rw-   0        0        0      701 2023-05-14 17:55:51.000000 xgit-python-0.4/xgit_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-05-14 17:55:51.000000 xgit-python-0.4/xgit_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 17:55:51.000000 xgit-python-0.4/xgit_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-05-14 17:55:51.000000 xgit-python-0.4/xgit_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-05-14 17:55:51.000000 xgit-python-0.4/xgit_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-14 17:55:51.000000 xgit-python-0.4/xgit_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 17:55:51.000000 xgit-python-0.4/xgit_python.egg-info/zip-safe
```

### Comparing `xgit-python-0.3/LICENSE` & `xgit-python-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xgit-python-0.3/PKG-INFO` & `xgit-python-0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: xgit-python
-Version: 0.3
+Version: 0.4
 Summary: Git tool based on GitPython.
-Home-page: https://github.com/zoumingzhe/xgit
+Home-page: https://github.com/zoumingzhe/xgit-python
 Author: mingzhe
 Author-email: zoumingzhe@qq.com
 License: MIT
-Project-URL: Source Code, https://github.com/zoumingzhe/xgit
-Project-URL: Bug Tracker, https://github.com/zoumingzhe/xgit/issues
-Project-URL: Documentation, https://github.com/zoumingzhe/xgit
+Project-URL: Source Code, https://github.com/zoumingzhe/xgit-python
+Project-URL: Bug Tracker, https://github.com/zoumingzhe/xgit-python/issues
+Project-URL: Documentation, https://github.com/zoumingzhe/xgit-python
 Keywords: git,GitPython,xgit
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `xgit-python-0.3/setup.cfg` & `xgit-python-0.4/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -8,64 +8,66 @@
 00000070: 2047 6974 2074 6f6f 6c20 6261 7365 6420   Git tool based 
 00000080: 6f6e 2047 6974 5079 7468 6f6e 2e0d 0a61  on GitPython...a
 00000090: 7574 686f 7220 3d20 6d69 6e67 7a68 650d  uthor = mingzhe.
 000000a0: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 000000b0: 7a6f 756d 696e 677a 6865 4071 712e 636f  zoumingzhe@qq.co
 000000c0: 6d0d 0a75 726c 203d 2068 7474 7073 3a2f  m..url = https:/
 000000d0: 2f67 6974 6875 622e 636f 6d2f 7a6f 756d  /github.com/zoum
-000000e0: 696e 677a 6865 2f78 6769 740d 0a6c 6f6e  ingzhe/xgit..lon
-000000f0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-00000100: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
-00000110: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000120: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-00000130: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-00000140: 6c69 6365 6e73 6520 3d20 4d49 540d 0a6c  license = MIT..l
-00000150: 6963 656e 7365 5f66 696c 6573 203d 204c  icense_files = L
-00000160: 4943 454e 5345 0d0a 706c 6174 666f 726d  ICENSE..platform
-00000170: 7320 3d20 616e 790d 0a63 6c61 7373 6966  s = any..classif
-00000180: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
-00000190: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001a0: 3a20 5079 7468 6f6e 0d0a 0950 726f 6772  : Python...Progr
-000001b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
-000001d0: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
-000001e0: 0a09 536f 7572 6365 2043 6f64 6520 3d20  ..Source Code = 
-000001f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000200: 6f6d 2f7a 6f75 6d69 6e67 7a68 652f 7867  om/zoumingzhe/xg
-00000210: 6974 0d0a 0942 7567 2054 7261 636b 6572  it...Bug Tracker
-00000220: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000230: 622e 636f 6d2f 7a6f 756d 696e 677a 6865  b.com/zoumingzhe
-00000240: 2f78 6769 742f 6973 7375 6573 0d0a 0944  /xgit/issues...D
-00000250: 6f63 756d 656e 7461 7469 6f6e 203d 2068  ocumentation = h
-00000260: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000270: 6d2f 7a6f 756d 696e 677a 6865 2f78 6769  m/zoumingzhe/xgi
-00000280: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-00000290: 7a69 705f 7361 6665 203d 2054 7275 650d  zip_safe = True.
-000002a0: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
-000002b0: 5f64 6174 6120 3d20 5472 7565 0d0a 7079  _data = True..py
-000002c0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-000002d0: 3e3d 332e 360d 0a69 6e73 7461 6c6c 5f72  >=3.6..install_r
-000002e0: 6571 7569 7265 7320 3d20 0d0a 0947 6974  equires = ...Git
-000002f0: 5079 7468 6f6e 0d0a 0978 6172 672d 7079  Python...xarg-py
-00000300: 7468 6f6e 0d0a 7061 636b 6167 6573 203d  thon..packages =
-00000310: 2066 696e 643a 0d0a 0d0a 5b6f 7074 696f   find:....[optio
-00000320: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-00000330: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
-00000340: 7320 3d20 0d0a 0978 6769 7420 3d20 7867  s = ...xgit = xg
-00000350: 6974 2e78 6769 745f 636f 6d6d 616e 643a  it.xgit_command:
-00000360: 6d61 696e 0d0a 0978 6769 742d 7375 6d6d  main...xgit-summ
-00000370: 6172 7920 3d20 7867 6974 2e78 6769 745f  ary = xgit.xgit_
-00000380: 7375 6d6d 6172 793a 6d61 696e 0d0a 0978  summary:main...x
-00000390: 6769 742d 6d6f 6469 6679 2d61 7574 686f  git-modify-autho
-000003a0: 7220 3d20 7867 6974 2e78 6769 745f 6d6f  r = xgit.xgit_mo
-000003b0: 6469 6679 5f61 7574 686f 723a 6d61 696e  dify_author:main
-000003c0: 0d0a 0978 6769 742d 6d6f 6469 6679 2d63  ...xgit-modify-c
-000003d0: 6f6d 6d69 7474 6572 203d 2078 6769 742e  ommitter = xgit.
-000003e0: 7867 6974 5f6d 6f64 6966 795f 636f 6d6d  xgit_modify_comm
-000003f0: 6974 7465 723a 6d61 696e 0d0a 0d0a 5b6f  itter:main....[o
-00000400: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-00000410: 6669 6e64 5d0d 0a69 6e63 6c75 6465 203d  find]..include =
-00000420: 2078 6769 742a 0d0a 6578 636c 7564 6520   xgit*..exclude 
-00000430: 3d20 0d0a 0974 6573 7473 0d0a 0d0a 5b65  = ...tests....[e
-00000440: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000450: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000460: 203d 2030 0d0a 0d0a                       = 0....
+000000e0: 696e 677a 6865 2f78 6769 742d 7079 7468  ingzhe/xgit-pyth
+000000f0: 6f6e 0d0a 6c6f 6e67 5f64 6573 6372 6970  on..long_descrip
+00000100: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
+00000110: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
+00000120: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
+00000130: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
+00000140: 6b64 6f77 6e0d 0a6c 6963 656e 7365 203d  kdown..license =
+00000150: 204d 4954 0d0a 6c69 6365 6e73 655f 6669   MIT..license_fi
+00000160: 6c65 7320 3d20 4c49 4345 4e53 450d 0a70  les = LICENSE..p
+00000170: 6c61 7466 6f72 6d73 203d 2061 6e79 0d0a  latforms = any..
+00000180: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+00000190: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000001a0: 6775 6167 6520 3a3a 2050 7974 686f 6e0d  guage :: Python.
+000001b0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000001c0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001d0: 203a 3a20 330d 0a70 726f 6a65 6374 5f75   :: 3..project_u
+000001e0: 726c 7320 3d20 0d0a 0953 6f75 7263 6520  rls = ...Source 
+000001f0: 436f 6465 203d 2068 7474 7073 3a2f 2f67  Code = https://g
+00000200: 6974 6875 622e 636f 6d2f 7a6f 756d 696e  ithub.com/zoumin
+00000210: 677a 6865 2f78 6769 742d 7079 7468 6f6e  gzhe/xgit-python
+00000220: 0d0a 0942 7567 2054 7261 636b 6572 203d  ...Bug Tracker =
+00000230: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000240: 636f 6d2f 7a6f 756d 696e 677a 6865 2f78  com/zoumingzhe/x
+00000250: 6769 742d 7079 7468 6f6e 2f69 7373 7565  git-python/issue
+00000260: 730d 0a09 446f 6375 6d65 6e74 6174 696f  s...Documentatio
+00000270: 6e20 3d20 6874 7470 733a 2f2f 6769 7468  n = https://gith
+00000280: 7562 2e63 6f6d 2f7a 6f75 6d69 6e67 7a68  ub.com/zoumingzh
+00000290: 652f 7867 6974 2d70 7974 686f 6e0d 0a0d  e/xgit-python...
+000002a0: 0a5b 6f70 7469 6f6e 735d 0d0a 7a69 705f  .[options]..zip_
+000002b0: 7361 6665 203d 2054 7275 650d 0a69 6e63  safe = True..inc
+000002c0: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+000002d0: 6120 3d20 5472 7565 0d0a 7079 7468 6f6e  a = True..python
+000002e0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+000002f0: 360d 0a69 6e73 7461 6c6c 5f72 6571 7569  6..install_requi
+00000300: 7265 7320 3d20 0d0a 0947 6974 5079 7468  res = ...GitPyth
+00000310: 6f6e 0d0a 0978 6172 672d 7079 7468 6f6e  on...xarg-python
+00000320: 203e 3d20 302e 350d 0a70 6163 6b61 6765   >= 0.5..package
+00000330: 7320 3d20 6669 6e64 3a0d 0a0d 0a5b 6f70  s = find:....[op
+00000340: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+00000350: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
+00000360: 6970 7473 203d 200d 0a09 7867 6974 203d  ipts = ...xgit =
+00000370: 2078 6769 742e 7867 6974 5f63 6f6d 6d61   xgit.xgit_comma
+00000380: 6e64 3a6d 6169 6e0d 0a09 7867 6974 2d73  nd:main...xgit-s
+00000390: 756d 6d61 7279 203d 2078 6769 742e 7867  ummary = xgit.xg
+000003a0: 6974 5f73 756d 6d61 7279 3a6d 6169 6e0d  it_summary:main.
+000003b0: 0a09 7867 6974 2d6d 6f64 6966 792d 6175  ..xgit-modify-au
+000003c0: 7468 6f72 203d 2078 6769 742e 7867 6974  thor = xgit.xgit
+000003d0: 5f6d 6f64 6966 795f 6175 7468 6f72 3a6d  _modify_author:m
+000003e0: 6169 6e0d 0a09 7867 6974 2d6d 6f64 6966  ain...xgit-modif
+000003f0: 792d 636f 6d6d 6974 7465 7220 3d20 7867  y-committer = xg
+00000400: 6974 2e78 6769 745f 6d6f 6469 6679 5f63  it.xgit_modify_c
+00000410: 6f6d 6d69 7474 6572 3a6d 6169 6e0d 0a0d  ommitter:main...
+00000420: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000430: 6573 2e66 696e 645d 0d0a 696e 636c 7564  es.find]..includ
+00000440: 6520 3d20 7867 6974 2a0d 0a65 7863 6c75  e = xgit*..exclu
+00000450: 6465 203d 200d 0a09 7465 7374 730d 0a0d  de = ...tests...
+00000460: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+00000470: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+00000480: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `xgit-python-0.3/xgit/xgit_command.py` & `xgit-python-0.4/xgit/xgit_command.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 #!/usr/bin/python3
 # coding=utf-8
 
 import sys
 
-from xarg import xarg
+from xarg import argp
 
-from .xgit_modify_author import add_cmd_modify_author, run_cmd_modify_author
+from .xgit_modify_author import add_cmd_modify_author
+from .xgit_modify_author import run_cmd_modify_author
 from .xgit_modify_committer import add_cmd_modify_committer
 from .xgit_modify_committer import run_cmd_modify_committer
-from .xgit_summary import add_cmd_summary, run_cmd_summary
+from .xgit_summary import add_cmd_summary
+from .xgit_summary import run_cmd_summary
 
 
 def run_sub_command(args):
     if args.debug:
-        sys.stdout.write("{}\n".format(args))
+        sys.stdout.write(f"{args}\n")
         sys.stdout.flush()
     {
         "summary": run_cmd_summary,
         "modify-author": run_cmd_modify_author,
         "modify-committer": run_cmd_modify_committer,
     }[args.sub](args)
 
 
 def main():
     try:
-        _arg = xarg(
+        _arg = argp(
             "xgit",
             description="Git tool based on GitPython",
-            epilog="For more, please visit https://github.com/zoumingzhe/xgit")
+            epilog=
+            "For more, please visit https://github.com/zoumingzhe/xgit-python")
         _arg.add_opt_on('-d', '--debug', help="show debug information")
-        _arg.add_subparsers(dest="sub", required=True)
-        add_cmd_modify_author(_arg.add_parser("modify-author"))
-        add_cmd_modify_committer(_arg.add_parser("modify-committer"))
-        add_cmd_summary(_arg.add_parser("summary"))
+        _sub = _arg.add_subparsers(dest="sub")
+        add_cmd_modify_author(_sub.add_parser("modify-author"))
+        add_cmd_modify_committer(_sub.add_parser("modify-committer"))
+        add_cmd_summary(_sub.add_parser("summary"))
         args = _arg.parse_args()
         run_sub_command(args)
     except KeyboardInterrupt:
         pass
     except Exception as e:
-        sys.stderr.write("{}\n".format(e))
+        sys.stderr.write(f"{e}\n")
         sys.stderr.flush()
```

### Comparing `xgit-python-0.3/xgit/xgit_filter.py` & `xgit-python-0.4/xgit/xgit_filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 #!/usr/bin/python3
 # coding=utf-8
 
-from xarg import xarg_parser
+from xarg import argp
 
 
-def add_cmd_filter_repo(_arg: xarg_parser):
+def add_cmd_filter_repo(_arg: argp):
     _arg.add_opt('-r',
                  '--repo',
                  type=str,
                  nargs=1,
                  default=['.'],
                  help="specify repo path")
 
 
-def add_cmd_filter_branch(_arg: xarg_parser):
+def add_cmd_filter_branch(_arg: argp):
     _arg.add_opt('-b',
                  '--branch',
                  type=str,
                  nargs=1,
                  default=[None],
                  help="specify branch")
 
 
-def add_cmd_filter_author(_arg: xarg_parser):
+def add_cmd_filter_author(_arg: argp):
     _arg.add_opt('--author',
                  type=str,
                  nargs=1,
                  default=[None],
                  help="specify author")
 
 
-def add_cmd_filter_path(_arg: xarg_parser):
-    _arg.add_pos("path", 0, type=str, help="Commit with folder or file path")
+def add_cmd_filter_path(_arg: argp):
+    _arg.add_pos("path",
+                 nargs=0,
+                 type=str,
+                 help="Commit with folder or file path")
```

### Comparing `xgit-python-0.3/xgit/xgit_modify_author.py` & `xgit-python-0.4/xgit/xgit_modify_author.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 #!/usr/bin/python3
 # coding=utf-8
 
 import sys
 
-from git import Git
-
-from xarg import xarg, xarg_parser
+from git.cmd import Git
+from xarg import argp
 
 from .xgit_filter import add_cmd_filter_repo
 
 
-def add_cmd_modify_author(_arg: xarg_parser):
+def add_cmd_modify_author(_arg: argp):
     add_cmd_filter_repo(_arg)
-    _arg.add_pos('name', 1, help="specify new author name")
-    _arg.add_pos('email', 1, help="specify new author email")
-    _arg.add_pos('old', -1, help="specify any old author name or email")
+    _arg.add_pos('name', nargs=1, help="specify new author name")
+    _arg.add_pos('email', nargs=1, help="specify new author email")
+    _arg.add_pos('old', nargs=-1, help="specify any old author name or email")
 
 
 def run_cmd_modify_author(args):
     _name = args.name[0]
     _email = args.email[0]
     _old = " ".join(['"{}"'.format(i) for i in args.old])
     _ret = Git(args.repo[0]).execute(["git", "gc"])
-    sys.stdout.write("{}\n".format(_ret))
+    sys.stdout.write(f"{_ret}\n")
     sys.stdout.flush()
     _ctx = """for old_name_or_email in {2}; do
  if [ "$GIT_AUTHOR_NAME" = "$old_name_or_email" ]; then
    export GIT_AUTHOR_NAME="{0}";
    export GIT_AUTHOR_EMAIL="{1}";
  elif [ "$GIT_AUTHOR_EMAIL" = "$old_name_or_email" ]; then
   export GIT_AUTHOR_NAME="{0}";
@@ -41,22 +40,22 @@
         "cat",
         "--force",
         "--",
         "--branches",
         "--tags",
     ]
     _ret = Git(args.repo[0]).execute(_cmd)
-    sys.stdout.write("{}\n".format(_ret))
+    sys.stdout.write(f"{_ret}\n")
     sys.stdout.flush()
 
 
 def main():
     try:
-        _arg = xarg("xgit-modify-author", description="modify author")
+        _arg = argp("xgit-modify-author", description="modify author")
         add_cmd_modify_author(_arg)
         args = _arg.parse_args()
         run_cmd_modify_author(args)
     except KeyboardInterrupt:
         pass
     except Exception as e:
-        sys.stderr.write("{}\n".format(e))
+        sys.stderr.write(f"{e}\n")
         sys.stderr.flush()
```

### Comparing `xgit-python-0.3/xgit/xgit_modify_committer.py` & `xgit-python-0.4/xgit/xgit_modify_committer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 #!/usr/bin/python3
 # coding=utf-8
 
 import sys
 
-from git import Git
-
-from xarg import xarg, xarg_parser
+from git.cmd import Git
+from xarg import argp
 
 from .xgit_filter import add_cmd_filter_repo
 
 
-def add_cmd_modify_committer(_arg: xarg_parser):
+def add_cmd_modify_committer(_arg: argp):
     add_cmd_filter_repo(_arg)
-    _arg.add_pos('name', 1, help="specify new committer name")
-    _arg.add_pos('email', 1, help="specify new committer email")
-    _arg.add_pos('old', -1, help="specify any old committer name or email")
+    _arg.add_pos('name', nargs=1, help="specify new committer name")
+    _arg.add_pos('email', nargs=1, help="specify new committer email")
+    _arg.add_pos('old',
+                 nargs=-1,
+                 help="specify any old committer name or email")
 
 
 def run_cmd_modify_committer(args):
     _name = args.name[0]
     _email = args.email[0]
     _old = " ".join(['"{}"'.format(i) for i in args.old])
     _ret = Git(args.repo[0]).execute(["git", "gc"])
-    sys.stdout.write("{}\n".format(_ret))
+    sys.stdout.write(f"{_ret}\n")
     sys.stdout.flush()
     _ctx = """for old_name_or_email in {2}; do
  if [ "$GIT_COMMITTER_NAME" = "$old_name_or_email" ]; then
    export GIT_COMMITTER_NAME="{0}";
    export GIT_COMMITTER_EMAIL="{1}";
  elif [ "$GIT_COMMITTER_EMAIL" = "$old_name_or_email" ]; then
   export GIT_COMMITTER_NAME="{0}";
@@ -41,22 +42,22 @@
         "cat",
         "--force",
         "--",
         "--branches",
         "--tags",
     ]
     _ret = Git(args.repo[0]).execute(_cmd)
-    sys.stdout.write("{}\n".format(_ret))
+    sys.stdout.write(f"{_ret}\n")
     sys.stdout.flush()
 
 
 def main():
     try:
-        _arg = xarg("xgit-modify-committer", description="modify committer")
+        _arg = argp("xgit-modify-committer", description="modify committer")
         add_cmd_modify_committer(_arg)
         args = _arg.parse_args()
         run_cmd_modify_committer(args)
     except KeyboardInterrupt:
         pass
     except Exception as e:
-        sys.stderr.write("{}\n".format(e))
+        sys.stderr.write(f"{e}\n")
         sys.stderr.flush()
```

### Comparing `xgit-python-0.3/xgit/xgit_summary.py` & `xgit-python-0.4/xgit/xgit_summary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/python3
 # coding=utf-8
 
 import sys
 
-from xarg import xarg, xarg_parser
+from xarg import argp
 
-from .xgit_filter import add_cmd_filter_repo
-from .xgit_filter import add_cmd_filter_branch
 from .xgit_filter import add_cmd_filter_author
+from .xgit_filter import add_cmd_filter_branch
 from .xgit_filter import add_cmd_filter_path
-from .xgit_util import author, committer, committed_datetime, xgit_object
+from .xgit_filter import add_cmd_filter_repo
+from .xgit_util import author
+from .xgit_util import committed_datetime
+from .xgit_util import committer
+from .xgit_util import xgit_object
 
 
-def add_cmd_summary(_arg: xarg_parser):
+def add_cmd_summary(_arg: argp):
     _arg.add_opt_on('-d', '--debug', help="show debug information")
     add_cmd_filter_repo(_arg)
     add_cmd_filter_branch(_arg)
     add_cmd_filter_author(_arg)
     add_cmd_filter_path(_arg)
     # TODO: author option and datetime option
     _arg.add_opt_on('--short', help="show prefix, default full 40-byte SHA256")
@@ -37,22 +40,22 @@
         _author = author(commit, not args.author_email)
         if args.committer or args.committer_email:
             _committer = committer(commit, not args.committer_email)
             _author = "{}, {}".format(_author, _committer)
         _summary = commit.summary
         # _message = commit.message
         _commit_info = f"{_idx}, {_hexsha}, {_datetime}, {_author}, {_summary}"
-        sys.stdout.write("{}\n".format(_commit_info))
+        sys.stdout.write(f"{_commit_info}\n")
         sys.stdout.flush()
 
 
 def main():
     try:
-        _arg = xarg("xgit-summary", description="list commit summary")
+        _arg = argp("xgit-summary", description="list commit summary")
         add_cmd_summary(_arg)
         args = _arg.parse_args()
         run_cmd_summary(args)
     except KeyboardInterrupt:
         pass
     except Exception as e:
-        sys.stderr.write("{}\n".format(e))
+        sys.stderr.write(f"{e}\n")
         sys.stderr.flush()
```

### Comparing `xgit-python-0.3/xgit/xgit_util.py` & `xgit-python-0.4/xgit/xgit_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python3
 # coding=utf-8
 
-from git import Repo
-from git import Commit
 from typing import Iterator
 
+from git import Commit
+from git.repo import Repo
+
 
 def author(commit: Commit, no_email: bool = False):
     assert type(commit) is Commit, "{} is not Commit".format(type(commit))
     assert type(no_email) is bool, "{} is not bool".format(type(no_email))
     _author = commit.author
     return _author.name if no_email else "{} <{}>".format(
         _author.name, _author.email)
```

### Comparing `xgit-python-0.3/xgit_python.egg-info/PKG-INFO` & `xgit-python-0.4/xgit_python.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: xgit-python
-Version: 0.3
+Version: 0.4
 Summary: Git tool based on GitPython.
-Home-page: https://github.com/zoumingzhe/xgit
+Home-page: https://github.com/zoumingzhe/xgit-python
 Author: mingzhe
 Author-email: zoumingzhe@qq.com
 License: MIT
-Project-URL: Source Code, https://github.com/zoumingzhe/xgit
-Project-URL: Bug Tracker, https://github.com/zoumingzhe/xgit/issues
-Project-URL: Documentation, https://github.com/zoumingzhe/xgit
+Project-URL: Source Code, https://github.com/zoumingzhe/xgit-python
+Project-URL: Bug Tracker, https://github.com/zoumingzhe/xgit-python/issues
+Project-URL: Documentation, https://github.com/zoumingzhe/xgit-python
 Keywords: git,GitPython,xgit
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

