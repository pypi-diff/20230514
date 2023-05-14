# Comparing `tmp/pyrobox-0.8.0.tar.gz` & `tmp/pyrobox-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrobox-0.8.0.tar", last modified: Fri May  5 20:56:15 2023, max compression
+gzip compressed data, was "pyrobox-0.8.1.tar", last modified: Sun May 14 20:01:07 2023, max compression
```

## Comparing `pyrobox-0.8.0.tar` & `pyrobox-0.8.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 20:56:15.065569 pyrobox-0.8.0/
--rw-rw-rw-   0        0        0     1062 2023-02-14 13:46:56.000000 pyrobox-0.8.0/LICENSE
--rw-rw-rw-   0        0        0    10318 2023-05-05 20:56:15.066567 pyrobox-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     9098 2023-04-23 13:48:06.000000 pyrobox-0.8.0/README.md
--rw-rw-rw-   0        0        0       90 2023-02-07 11:48:14.000000 pyrobox-0.8.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-05 20:56:15.055592 pyrobox-0.8.0/pyrobox.egg-info/
--rw-rw-rw-   0        0        0    10318 2023-05-05 20:56:15.000000 pyrobox-0.8.0/pyrobox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-05-05 20:56:15.000000 pyrobox-0.8.0/pyrobox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 20:56:15.000000 pyrobox-0.8.0/pyrobox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-05 20:56:15.000000 pyrobox-0.8.0/pyrobox.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-05-05 20:56:15.000000 pyrobox-0.8.0/pyrobox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 20:56:15.000000 pyrobox-0.8.0/pyrobox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1027 2023-05-05 20:56:15.069561 pyrobox-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      237 2023-03-04 18:36:12.000000 pyrobox-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 20:56:15.064574 pyrobox-0.8.0/src/
--rw-rw-rw-   0        0        0       83 2023-03-04 18:36:12.000000 pyrobox-0.8.0/src/__init__.py
--rw-rw-rw-   0        0        0       20 2023-03-04 18:36:12.000000 pyrobox-0.8.0/src/__main__.py
--rw-rw-rw-   0        0        0     1812 2023-04-19 10:26:44.000000 pyrobox-0.8.0/src/_arg_parser.py
--rw-rw-rw-   0        0        0      105 2023-04-22 14:53:08.000000 pyrobox-0.8.0/src/_exceptions.py
--rw-rw-rw-   0        0        0     8105 2023-05-05 20:50:11.000000 pyrobox-0.8.0/src/_fs_utils.py
--rw-rw-rw-   0        0        0    44160 2023-05-05 20:25:55.000000 pyrobox-0.8.0/src/_page_templates.py
--rw-rw-rw-   0        0        0     7165 2023-05-05 20:49:15.000000 pyrobox-0.8.0/src/_zipfly_manager.py
--rw-rw-rw-   0        0        0    53479 2023-05-05 20:54:03.000000 pyrobox-0.8.0/src/pyroboxCore.py
--rw-rw-rw-   0        0        0    29220 2023-05-05 20:34:07.000000 pyrobox-0.8.0/src/server.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:01:07.554375 pyrobox-0.8.1/
+-rw-rw-rw-   0        0        0     1062 2023-05-06 07:29:18.000000 pyrobox-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0    10333 2023-05-14 20:01:07.554375 pyrobox-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9098 2023-05-06 07:29:18.000000 pyrobox-0.8.1/README.md
+-rw-rw-rw-   0        0        0       90 2023-05-06 07:29:18.000000 pyrobox-0.8.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-14 20:01:07.549375 pyrobox-0.8.1/pyrobox.egg-info/
+-rw-rw-rw-   0        0        0    10333 2023-05-14 20:01:07.000000 pyrobox-0.8.1/pyrobox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-05-14 20:01:07.000000 pyrobox-0.8.1/pyrobox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 20:01:07.000000 pyrobox-0.8.1/pyrobox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-14 20:01:07.000000 pyrobox-0.8.1/pyrobox.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-05-14 20:01:07.000000 pyrobox-0.8.1/pyrobox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-14 20:01:07.000000 pyrobox-0.8.1/pyrobox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1026 2023-05-14 20:01:07.554375 pyrobox-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      237 2023-05-06 07:29:18.000000 pyrobox-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 20:01:07.553374 pyrobox-0.8.1/src/
+-rw-rw-rw-   0        0        0       83 2023-05-06 07:29:18.000000 pyrobox-0.8.1/src/__init__.py
+-rw-rw-rw-   0        0        0       20 2023-05-06 07:29:18.000000 pyrobox-0.8.1/src/__main__.py
+-rw-rw-rw-   0        0        0     1812 2023-05-06 07:29:18.000000 pyrobox-0.8.1/src/_arg_parser.py
+-rw-rw-rw-   0        0        0      105 2023-05-06 07:29:18.000000 pyrobox-0.8.1/src/_exceptions.py
+-rw-rw-rw-   0        0        0     8105 2023-05-06 07:29:18.000000 pyrobox-0.8.1/src/_fs_utils.py
+-rw-rw-rw-   0        0        0    44160 2023-05-06 07:29:18.000000 pyrobox-0.8.1/src/_page_templates.py
+-rw-rw-rw-   0        0        0     7165 2023-05-06 07:29:18.000000 pyrobox-0.8.1/src/_zipfly_manager.py
+-rw-rw-rw-   0        0        0    55114 2023-05-14 19:57:30.000000 pyrobox-0.8.1/src/pyroboxCore.py
+-rw-rw-rw-   0        0        0    29147 2023-05-14 19:57:47.000000 pyrobox-0.8.1/src/server.py
```

### Comparing `pyrobox-0.8.0/LICENSE` & `pyrobox-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrobox-0.8.0/PKG-INFO` & `pyrobox-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: pyrobox
-Version: 0.8.0
+Version: 0.8.1
 Summary: Personal DropBox for Private Network
 Home-page: https://github.com/RaSan147/pyrobox
+Author: Rasan
 Author-email: wwwqweasd147@gmail.com
 Project-URL: Bug Tracker, https://github.com/RaSan147/pyrobox/issues
 Project-URL: Documentation, https://github.com/RaSan147/pyrobox
 Project-URL: Source Code, https://github.com/RaSan147/pyrobox
 Project-URL: Release Notes, https://github.com/RaSan147/pyrobox/releases
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyrobox-0.8.0/README.md` & `pyrobox-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrobox-0.8.0/pyrobox.egg-info/PKG-INFO` & `pyrobox-0.8.1/pyrobox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: pyrobox
-Version: 0.8.0
+Version: 0.8.1
 Summary: Personal DropBox for Private Network
 Home-page: https://github.com/RaSan147/pyrobox
+Author: Rasan
 Author-email: wwwqweasd147@gmail.com
 Project-URL: Bug Tracker, https://github.com/RaSan147/pyrobox/issues
 Project-URL: Documentation, https://github.com/RaSan147/pyrobox
 Project-URL: Source Code, https://github.com/RaSan147/pyrobox
 Project-URL: Release Notes, https://github.com/RaSan147/pyrobox/releases
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyrobox-0.8.0/setup.cfg` & `pyrobox-0.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7972 6f62 6f78 0d0a 7665 7273   = pyrobox..vers
-00000020: 696f 6e20 3d20 302e 382e 300d 0a61 7574  ion = 0.8.0..aut
-00000030: 686f 7273 203d 2052 6173 616e 0d0a 6175  hors = Rasan..au
-00000040: 7468 6f72 5f65 6d61 696c 203d 2077 7777  thor_email = www
-00000050: 7177 6561 7364 3134 3740 676d 6169 6c2e  qweasd147@gmail.
-00000060: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
-00000070: 203d 2050 6572 736f 6e61 6c20 4472 6f70   = Personal Drop
-00000080: 426f 7820 666f 7220 5072 6976 6174 6520  Box for Private 
-00000090: 4e65 7477 6f72 6b0d 0a6c 6f6e 675f 6465  Network..long_de
-000000a0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
-000000b0: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
-000000c0: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
-000000d0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
-000000e0: 742f 6d61 726b 646f 776e 0d0a 6c69 6365  t/markdown..lice
-000000f0: 6e73 655f 6669 6c65 7320 3d20 4c49 4345  nse_files = LICE
-00000100: 4e53 450d 0a68 6f6d 652d 7061 6765 203d  NSE..home-page =
-00000110: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000120: 636f 6d2f 5261 5361 6e31 3437 2f70 7972  com/RaSan147/pyr
-00000130: 6f62 6f78 0d0a 7072 6f6a 6563 745f 7572  obox..project_ur
-00000140: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
-00000150: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
-00000160: 7468 7562 2e63 6f6d 2f52 6153 616e 3134  thub.com/RaSan14
-00000170: 372f 7079 726f 626f 782f 6973 7375 6573  7/pyrobox/issues
-00000180: 0d0a 0944 6f63 756d 656e 7461 7469 6f6e  ...Documentation
-00000190: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-000001a0: 622e 636f 6d2f 5261 5361 6e31 3437 2f70  b.com/RaSan147/p
-000001b0: 7972 6f62 6f78 0d0a 0953 6f75 7263 6520  yrobox...Source 
-000001c0: 436f 6465 203d 2068 7474 7073 3a2f 2f67  Code = https://g
-000001d0: 6974 6875 622e 636f 6d2f 5261 5361 6e31  ithub.com/RaSan1
-000001e0: 3437 2f70 7972 6f62 6f78 0d0a 0952 656c  47/pyrobox...Rel
-000001f0: 6561 7365 204e 6f74 6573 203d 2068 7474  ease Notes = htt
-00000200: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000210: 5261 5361 6e31 3437 2f70 7972 6f62 6f78  RaSan147/pyrobox
-00000220: 2f72 656c 6561 7365 730d 0a63 6c61 7373  /releases..class
-00000230: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
-00000240: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000250: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000260: 370d 0a09 5072 6f67 7261 6d6d 696e 6720  7...Programming 
-00000270: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000280: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
-00000290: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000002a0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000002b0: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
-000002c0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002d0: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
-000002e0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002f0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000300: 2e31 310d 0a09 4c69 6365 6e73 6520 3a3a  .11...License ::
-00000310: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-00000320: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
-00000330: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000340: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000350: 740d 0a09 546f 7069 6320 3a3a 2049 6e74  t...Topic :: Int
-00000360: 6572 6e65 7420 3a3a 2046 696c 6520 5472  ernet :: File Tr
-00000370: 616e 7366 6572 2050 726f 746f 636f 6c20  ansfer Protocol 
-00000380: 2846 5450 290d 0a09 546f 7069 6320 3a3a  (FTP)...Topic ::
-00000390: 2043 6f6d 6d75 6e69 6361 7469 6f6e 7320   Communications 
-000003a0: 3a3a 2046 696c 6520 5368 6172 696e 670d  :: File Sharing.
-000003b0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7079  ...[options]..py
-000003c0: 7468 6f6e 2d72 6571 7569 7265 7320 3d20  thon-requires = 
-000003d0: 3e3d 332e 370d 0a0d 0a5b 6567 675f 696e  >=3.7....[egg_in
-000003e0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000003f0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000400: 0a0d 0a                                  ...
+00000020: 696f 6e20 3d20 302e 382e 310d 0a61 7574  ion = 0.8.1..aut
+00000030: 686f 7220 3d20 5261 7361 6e0d 0a61 7574  hor = Rasan..aut
+00000040: 686f 725f 656d 6169 6c20 3d20 7777 7771  hor_email = wwwq
+00000050: 7765 6173 6431 3437 4067 6d61 696c 2e63  weasd147@gmail.c
+00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
+00000070: 3d20 5065 7273 6f6e 616c 2044 726f 7042  = Personal DropB
+00000080: 6f78 2066 6f72 2050 7269 7661 7465 204e  ox for Private N
+00000090: 6574 776f 726b 0d0a 6c6f 6e67 5f64 6573  etwork..long_des
+000000a0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+000000b0: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
+000000c0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
+000000d0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
+000000e0: 2f6d 6172 6b64 6f77 6e0d 0a6c 6963 656e  /markdown..licen
+000000f0: 7365 5f66 696c 6573 203d 204c 4943 454e  se_files = LICEN
+00000100: 5345 0d0a 686f 6d65 2d70 6167 6520 3d20  SE..home-page = 
+00000110: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000120: 6f6d 2f52 6153 616e 3134 372f 7079 726f  om/RaSan147/pyro
+00000130: 626f 780d 0a70 726f 6a65 6374 5f75 726c  box..project_url
+00000140: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
+00000150: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
+00000160: 6875 622e 636f 6d2f 5261 5361 6e31 3437  hub.com/RaSan147
+00000170: 2f70 7972 6f62 6f78 2f69 7373 7565 730d  /pyrobox/issues.
+00000180: 0a09 446f 6375 6d65 6e74 6174 696f 6e20  ..Documentation 
+00000190: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+000001a0: 2e63 6f6d 2f52 6153 616e 3134 372f 7079  .com/RaSan147/py
+000001b0: 726f 626f 780d 0a09 536f 7572 6365 2043  robox...Source C
+000001c0: 6f64 6520 3d20 6874 7470 733a 2f2f 6769  ode = https://gi
+000001d0: 7468 7562 2e63 6f6d 2f52 6153 616e 3134  thub.com/RaSan14
+000001e0: 372f 7079 726f 626f 780d 0a09 5265 6c65  7/pyrobox...Rele
+000001f0: 6173 6520 4e6f 7465 7320 3d20 6874 7470  ase Notes = http
+00000200: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f52  s://github.com/R
+00000210: 6153 616e 3134 372f 7079 726f 626f 782f  aSan147/pyrobox/
+00000220: 7265 6c65 6173 6573 0d0a 636c 6173 7369  releases..classi
+00000230: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
+00000240: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000250: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
+00000260: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000270: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000280: 6e20 3a3a 2033 2e38 0d0a 0950 726f 6772  n :: 3.8...Progr
+00000290: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002a0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+000002b0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000002c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002d0: 6e20 3a3a 2033 2e31 300d 0a09 5072 6f67  n :: 3.10...Prog
+000002e0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002f0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000300: 3131 0d0a 094c 6963 656e 7365 203a 3a20  11...License :: 
+00000310: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000320: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
+00000330: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000340: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00000350: 0d0a 0954 6f70 6963 203a 3a20 496e 7465  ...Topic :: Inte
+00000360: 726e 6574 203a 3a20 4669 6c65 2054 7261  rnet :: File Tra
+00000370: 6e73 6665 7220 5072 6f74 6f63 6f6c 2028  nsfer Protocol (
+00000380: 4654 5029 0d0a 0954 6f70 6963 203a 3a20  FTP)...Topic :: 
+00000390: 436f 6d6d 756e 6963 6174 696f 6e73 203a  Communications :
+000003a0: 3a20 4669 6c65 2053 6861 7269 6e67 0d0a  : File Sharing..
+000003b0: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 7974  ..[options]..pyt
+000003c0: 686f 6e2d 7265 7175 6972 6573 203d 203e  hon-requires = >
+000003d0: 3d33 2e37 0d0a 0d0a 5b65 6767 5f69 6e66  =3.7....[egg_inf
+000003e0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+000003f0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+00000400: 0d0a                                     ..
```

### Comparing `pyrobox-0.8.0/src/_arg_parser.py` & `pyrobox-0.8.1/src/_arg_parser.py`

 * *Files identical despite different names*

### Comparing `pyrobox-0.8.0/src/_fs_utils.py` & `pyrobox-0.8.1/src/_fs_utils.py`

 * *Files identical despite different names*

### Comparing `pyrobox-0.8.0/src/_page_templates.py` & `pyrobox-0.8.1/src/_page_templates.py`

 * *Files identical despite different names*

### Comparing `pyrobox-0.8.0/src/_zipfly_manager.py` & `pyrobox-0.8.1/src/_zipfly_manager.py`

 * *Files identical despite different names*

### Comparing `pyrobox-0.8.0/src/pyroboxCore.py` & `pyrobox-0.8.1/src/pyroboxCore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import traceback
 import json
 import string
 import random
 import base64
 import re
 from http import HTTPStatus
+from http.cookies import SimpleCookie
 from functools import partial
 import contextlib
 import urllib.request
 import urllib.parse
 import time
 import sys
 import socketserver
@@ -25,16 +26,16 @@
 from string import Template
 from typing import Union
 from queue import Queue
 import logging
 import atexit
 import os
 
-__version__ = "0.8.0"
 
+__version__ = "0.8.1"
 enc = "utf-8"
 __all__ = [
 	"HTTPServer", "ThreadingHTTPServer", "BaseHTTPRequestHandler",
 	"SimpleHTTPRequestHandler",
 ]
 
 
@@ -83,15 +84,15 @@
 		self.MAIN_FILE_dir = os.path.dirname(self.MAIN_FILE)
 
 		# OS DETECTION
 		self.OS = self.get_os()
 
 		# RUNNING SERVER STATS
 		self.ftp_dir = self.get_default_dir()
-		self.dev_mode = False
+		self.dev_mode = True
 		self.ASSETS = False  # if you want to use assets folder, set this to True
 		self.ASSETS_dir = os.path.join(self.MAIN_FILE_dir, "/../assets/")
 		self.reload = False
 
 		self.disabled_func = {
 			"reload": False,
 		}
@@ -129,15 +130,15 @@
 
 		self.DEFAULT_ERROR_CONTENT_TYPE = "text/html;charset=utf-8"
 
 	def clear_temp(self):
 		for i in self.temp_file:
 			try:
 				os.remove(i)
-			except:
+			except OSError:
 				pass
 
 	def get_os(self):
 		from platform import system as platform_system
 
 		out = platform_system()
 		if out == "Linux" and hasattr(sys, 'getandroidapilevel'):
@@ -191,15 +192,18 @@
 			"equal": "=",
 			"star": "*",
 			"hash": "#",
 			"dash": "-",
 			"udash": "_"
 		}
 
-	def term_width(self):
+	@staticmethod
+	def term_width():
+		""" Return CLI screen size (if not found, returns default value)
+		"""
 		return shutil.get_terminal_size()[0]
 
 	def text_box(self, *text, style="equal", sep=" "):
 		"""
 		Returns a string of text with a border around it.
 		"""
 		text = sep.join(map(str, text))
@@ -207,15 +211,19 @@
 
 		s = self.styles[style] if style in self.styles else style
 		tt = ""
 		for i in text.split('\n'):
 			tt += i.center(term_col) + '\n'
 		return (f"\n\n{s*term_col}\n{tt}{s*term_col}\n\n")
 
-	def random_string(self, length=10):
+	@staticmethod
+	def random_string(length=10):
+		"""Generates a random string
+		length : length of string
+		"""
 		letters = string.ascii_lowercase
 		return ''.join(random.choice(letters) for i in range(length))
 
 
 tools = Tools()
 config = Config()
 
@@ -237,15 +245,15 @@
 	logger.info("Reloading...\n" +
 				" ".join(
 					["RE-RUNNING: ", sys.executable,
 						sys.executable, file, *sys.argv[1:]]
 				))
 	try:
 		os.execl(sys.executable, sys.executable, file, *sys.argv[1:])
-	except:
+	except OSError:
 		traceback.print_exc()
 	sys.exit(0)
 
 
 def null(*args, **kwargs):
 	pass
 
@@ -343,22 +351,22 @@
 	The last number or both numbers may be None.
 	'''
 	if byte_range.strip() == '':
 		return None, None
 
 	m = BYTE_RANGE_RE.match(byte_range)
 	if not m:
-		raise ValueError('Invalid byte range %s' % byte_range)
+		raise ValueError(f'Invalid byte range {byte_range}')
 
 	# first, last = [x and int(x) for x in m.groups()] #
 
 	first, last = map((lambda x: int(x) if x else None), m.groups())
 
 	if last and last < first:
-		raise ValueError('Invalid byte range %s' % byte_range)
+		raise ValueError(f'Invalid byte range { byte_range}')
 	return first, last
 
 # ---------------------------x--------------------------------
 
 
 def URL_MANAGER(url: str):
 	"""
@@ -455,14 +463,18 @@
 		Return True for success, False for failure; on failure, any relevant
 		error response has already been sent back.
 
 		"""
 		self.command = ''  # set in case of error on the first line
 		self.request_version = version = self.default_request_version
 		self.close_connection = True
+		self.header_flushed = False # true when headers are flushed by self.flush_headers()
+		self.response_code_sent = False # true when response code (>=200) is sent by self.send_response()
+
+
 		requestline = str(self.raw_requestline, 'iso-8859-1')
 		requestline = requestline.rstrip('\r\n')
 		self.requestline = requestline
 		words = requestline.split()
 		if len(words) == 0:
 			return False
 
@@ -539,14 +551,22 @@
 
 		conntype = self.headers.get('Connection', "")
 		if conntype.lower() == 'close':
 			self.close_connection = True
 		elif (conntype.lower() == 'keep-alive' and
 			  self.protocol_version >= "HTTP/1.1"):
 			self.close_connection = False
+		
+		# Load cookies from request
+		# Uses standard SimpleCookie
+		# doc: https://docs.python.org/3/library/http.cookies.html
+		self.cookie = SimpleCookie()
+		self.cookie.load(self.headers.get('Cookie', ""))
+		# print(tools.text_box("Cookie: ", self.cookie))
+		
 		# Examine the headers and look for an Expect directive
 		expect = self.headers.get('Expect', "")
 		if (expect.lower() == "100-continue" and
 			self.protocol_version >= "HTTP/1.1" and
 				self.request_version >= "HTTP/1.1"):
 			if not self.handle_expect_100():
 				return False
@@ -722,14 +742,20 @@
 		"""Add the response header to the headers buffer and log the
 		response code.
 
 		Also send two standard headers with the server software
 		version and the current date.
 
 		"""
+		if self.response_code_sent:
+			return
+		
+		if not code//100 ==1: # 1xx - Informational (allowes multiple responses)
+			self.response_code_sent = True
+
 		self.log_request(code)
 		self.send_response_only(code, message)
 		self.send_header('Server', self.version_string())
 		self.send_header('Date', self.date_time_string())
 
 	def send_response_only(self, code, message=None):
 		"""Send the response header only."""
@@ -740,14 +766,23 @@
 				else:
 					message = ''
 			if not hasattr(self, '_headers_buffer'):
 				self._headers_buffer = []
 			self._headers_buffer.append(("%s %d %s\r\n" %
 				(self.protocol_version, code, message)).encode(
 				'utf-8', 'strict'))
+				
+	def send_header_string(self, lines:str):
+		"""Send a header multiline string to the headers buffer."""
+		for i in lines.split("\r\n"):
+			if not i:
+				continue
+			tag, _, msg = i.partition(":")
+			self.send_header(tag.strip(), msg.strip())
+			
 
 	def send_header(self, keyword, value):
 		"""Send a MIME header to the headers buffer."""
 		if self.request_version != 'HTTP/0.9':
 			if not hasattr(self, '_headers_buffer'):
 				self._headers_buffer = []
 			self._headers_buffer.append(
@@ -762,18 +797,27 @@
 	def end_headers(self):
 		"""Send the blank line ending the MIME headers."""
 		if self.request_version != 'HTTP/0.9':
 			self._headers_buffer.append(b"\r\n")
 			self.flush_headers()
 
 	def flush_headers(self):
+		"""Flush the headers buffer."""
+		if self.header_flushed:
+			try:
+				raise RuntimeError("Headers already flushed")
+			except RuntimeError:
+				traceback.print_exc()
+			return
 		if hasattr(self, '_headers_buffer'):
 			self.wfile.write(b"".join(self._headers_buffer))
 			self._headers_buffer = []
 
+		self.header_flushed = True
+
 	def log_request(self, code='-', size='-'):
 		"""Log an accepted request.
 
 		This is called by send_response().
 
 		"""
 		if isinstance(code, HTTPStatus):
@@ -907,17 +951,17 @@
 	server_version = "SimpleHTTP/" + __version__
 
 	if not mimetypes.inited:
 		mimetypes.init()  # try to read system mime.types
 	extensions_map = mimetypes.types_map.copy()
 	extensions_map.update({
 		'': 'application/octet-stream',  # Default
-			'.py': 'text/plain',
-			'.c': 'text/plain',
-			'.h': 'text/plain',
+			'.py': 'text/x-python',
+			'.c': 'text/x-c',
+			'.h': 'text/x-c',
 			'.css': 'text/css',
 
 			'.gz': 'application/gzip',
 			'.Z': 'application/octet-stream',
 			'.bz2': 'application/x-bzip2',
 			'.xz': 'application/x-xz',
 
@@ -944,28 +988,28 @@
 		self.directory = os.fspath(directory)
 		super().__init__(*args, **kwargs)
 		self.query = Callable_dict()
 
 	def do_GET(self):
 		"""Serve a GET request."""
 		try:
-			f = self.send_head()
+			resp = self.send_head()
 		except Exception as e:
 			traceback.print_exc()
 			self.send_error(500, str(e))
 			return
 
-		if f:
+		if resp:
 			try:
-				self.copyfile(f, self.wfile)
+				self.copyfile(resp, self.wfile)
 			except (ConnectionAbortedError, ConnectionResetError, BrokenPipeError) as e:
 				self.log_info(tools.text_box(e.__class__.__name__,
 							  e, "\nby ", self.address_string()))
 			finally:
-				f.close()
+				resp.close()
 
 	def do_(self):
 		'''incase of errored request'''
 		self.send_error(HTTPStatus.BAD_REQUEST, "Bad request.")
 
 	@staticmethod
 	def on_req(type='', url='', hasQ=(), QV={}, fragent='', url_regex='', func=null):
@@ -1013,21 +1057,21 @@
 			fragent: fragent of request
 			url_regex: url regex, the url must start and end with this regex
 
 
 		'''
 		if url_regex and not re.search("^"+url_regex+'$', self.url_path):
 				return False
-		elif url and url != self.url_path:
+		if url and url != self.url_path:
 			return False
 
 		if isinstance(hasQ, str):
 			hasQ = (hasQ,)
 
-		if hasQ and self.query(*hasQ) == False:
+		if hasQ and self.query(*hasQ) is False:
 			return False
 		if QV:
 			for k, v in QV.items():
 				if not self.query(k):
 					return False
 				if self.query[k] != v:
 					return False
@@ -1035,23 +1079,24 @@
 		if fragent and self.fragment != fragent:
 			return False
 
 		return True
 
 	def do_HEAD(self):
 		"""Serve a HEAD request."""
+		resp = None
 		try:
-			f = self.send_head()
+			resp = self.send_head()
 		except Exception as e:
 			traceback.print_exc()
 			self.send_error(500, str(e))
 			return
-
-		if f:
-			f.close()
+		finally:
+			if resp:
+				resp.close()
 
 	def do_POST(self):
 		"""Serve a POST request."""
 		self.range = None, None
 
 		path = self.translate_path(self.path)
 		# DIRECTORY DONT CONTAIN SLASH / AT END
@@ -1059,29 +1104,29 @@
 		url_path, query, fragment = self.url_path, self.query, self.fragment
 		spathsplit = self.url_path.split("/")
 
 		try:
 			for case, func in self.handlers['POST']:
 				if self.test_req(*case):
 					try:
-						f = func(self, url_path=url_path, query=query,
+						resp = func(self, url_path=url_path, query=query,
 								 fragment=fragment, path=path, spathsplit=spathsplit)
 					except PostError:
 						traceback.print_exc()
 						# break if error is raised and send BAD_REQUEST (at end of loop)
 						break
 
-					if f:
+					if resp:
 						try:
-							self.copyfile(f, self.wfile)
+							self.copyfile(resp, self.wfile)
 						except (ConnectionAbortedError, ConnectionResetError, BrokenPipeError) as e:
 							logger.info(tools.text_box(
 								e.__class__.__name__, e, "\nby ", [self.address_string()]))
 						finally:
-							f.close()
+							resp.close()
 					return
 
 			return self.send_error(HTTPStatus.BAD_REQUEST, "Invalid request.")
 
 		except (ConnectionAbortedError, ConnectionResetError, BrokenPipeError) as e:
 			logger.info(tools.text_box(e.__class__.__name__,
 						e, "\nby ", [self.address_string()]))
@@ -1089,71 +1134,76 @@
 		except Exception as e:
 			traceback.print_exc()
 			self.send_error(500, str(e))
 			return
 
 	def redirect(self, location):
 		'''redirect to location'''
-		self.send_response(HTTPStatus.FOUND)
+		print("REDIRECT ", location)
+		self.send_response(302)
 		self.send_header("Location", location)
 		self.end_headers()
 
 	def return_txt(self, code, msg, content_type="text/html; charset=utf-8"):
 		'''returns only the head to client
 		and returns a file object to be used by copyfile'''
 		self.log_debug(f'[RETURNED] {code} to client')
 		if not isinstance(msg, bytes):
 			encoded = msg.encode('utf-8', 'surrogateescape')
 		else:
 			encoded = msg
 
-		f = io.BytesIO()
-		f.write(encoded)
-		f.seek(0)
+		box = io.BytesIO()
+		box.write(encoded)
+		box.seek(0)
 
 		self.send_response(code)
-		self.send_header("Content-type", content_type)
+		self.send_header("Content-Type", content_type)
 		self.send_header("Content-Length", str(len(encoded)))
 		self.end_headers()
-		return f
+		return box
 
 	def send_txt(self, code, msg, content_type="text/html; charset=utf-8"):
 		'''sends the head and file to client'''
-		f = self.return_txt(code, msg, content_type)
+		file = self.return_txt(code, msg, content_type)
 		if self.command == "HEAD":
 			return  # to avoid sending file on get request
-		self.copyfile(f, self.wfile)
-		f.close()
+		self.copyfile(file, self.wfile)
+		file.close()
 
 	def send_text(self, code, msg, content_type="text/html; charset=utf-8"):
 		'''proxy to send_txt'''
 		self.send_txt(code, msg, content_type)
 
 	def send_json(self, obj):
 		"""send object as json
 		obj: json-able object or json.dumps() string"""
 		if not isinstance(obj, str):
 			obj = json.dumps(obj, indent=1)
-		f = self.return_txt(200, obj, content_type="application/json")
+		file = self.return_txt(200, obj, content_type="application/json")
 		if self.command == "HEAD":
 			return  # to avoid sending file on get request
-		self.copyfile(f, self.wfile)
-		f.close()
+		self.copyfile(file, self.wfile)
+		file.close()
 
-	def return_file(self, path, filename=None, download=False):
-		f = None
+	def return_file(self, path, filename=None, download=False, cache_control=""):
+		file = None
 		is_attachment = "attachment;" if (self.query("dl") or download) else ""
 
 		first, last = 0, None
 
 		try:
 			ctype = self.guess_type(path)
+			
+			# make sure texts are sent as utf-8
+			if ctype.startswith("text/"):
+				ctype += "; charset=utf-8"
 
-			f = open(path, 'rb')
-			fs = os.fstat(f.fileno())
+			file = open(path, 'rb')
+			fs = os.fstat(file.fileno())
 
 			file_len = fs[6]
 			# Use browser cache if possible
 			if ("If-Modified-Since" in self.headers
 					and "If-None-Match" not in self.headers):
 				# compare If-Modified-Since and time of last file modification
 				try:
@@ -1173,15 +1223,15 @@
 							fs.st_mtime, datetime.timezone.utc)
 						# remove microseconds, like in If-Modified-Since
 						last_modif = last_modif.replace(microsecond=0)
 
 						if last_modif <= ims:
 							self.send_response(HTTPStatus.NOT_MODIFIED)
 							self.end_headers()
-							f.close()
+							file.close()
 
 							return None
 
 			if self.use_range:
 				first = self.range[0]
 				if first is None:
 					first = 0
@@ -1190,35 +1240,38 @@
 					last = file_len - 1
 
 				if first >= file_len:  # PAUSE AND RESUME SUPPORT
 					self.send_error(416, 'Requested Range Not Satisfiable')
 					return None
 
 				self.send_response(206)
-				self.send_header('Content-Type', ctype)
 				self.send_header('Accept-Ranges', 'bytes')
 
 				response_length = last - first + 1
 
 				self.send_header('Content-Range',
-								 'bytes %s-%s/%s' % (first, last, file_len))
+								 f'bytes {first}-{last}/{file_len}')
 				self.send_header('Content-Length', str(response_length))
 
 			else:
 				self.send_response(HTTPStatus.OK)
-				self.send_header("Content-Type", ctype)
+				
 				self.send_header("Content-Length", str(file_len))
+				
+			if cache_control:
+				self.send_header("Cache-Control", cache_control)
 
 			self.send_header("Last-Modified",
 							 self.date_time_string(fs.st_mtime))
+			self.send_header("Content-Type", ctype)
 			self.send_header("Content-Disposition", is_attachment+' filename="%s"' %
 							 (os.path.basename(path) if filename is None else filename))
 			self.end_headers()
 
-			return f
+			return file
 
 		except PermissionError:
 			self.send_error(HTTPStatus.FORBIDDEN, "Permission denied")
 			return None
 
 		except OSError:
 			self.send_error(HTTPStatus.NOT_FOUND, "File not found")
@@ -1226,24 +1279,25 @@
 
 		except Exception:
 			traceback.print_exc()
 
 			# if f and not f.closed(): f.close()
 			raise
 
-	def send_file(self, path, filename=None, download=False):
+	def send_file(self, path, filename=None, download=False, cache_control=''):
 		'''sends the head and file to client'''
-		f = self.return_file(path, filename, download)
+		file = self.return_file(path, filename, download, cache_control)
 		if self.command == "HEAD":
 			return  # to avoid sending file on get request
 		try:
-			self.copyfile(f, self.wfile)
+			self.copyfile(file, self.wfile)
 		finally:
-			f.close()
-
+			file.close()
+			
+	
 	def send_head(self):
 		"""Common code for GET and HEAD commands.
 
 		This sends the response code and MIME headers.
 
 		Return value is either a file object (which has to be copied
 		to the outputfile by the caller unless the command was HEAD,
@@ -1340,21 +1394,23 @@
 
 		The only reason for overriding this would be to change
 		the block size or perhaps to replace newlines by CRLF
 		-- note however that this the default server uses this
 		to copy binary data as well.
 
 		"""
+		try:
+			# check if file readable
+			source.read(1)
+			source.seek(0)
+		except OSError as e:
+			traceback.print_exc()
+			raise e
 
 		if not self.range:
-			try:
-				source.read(1)
-			except:
-				traceback.print_exc()
-			source.seek(0)
 			shutil.copyfileobj(source, outputfile)
 
 		else:
 			# SimpleHTTPRequestHandler uses shutil.copyfileobj, which doesn't let
 			# you stop the copying before the end of the file.
 			start, stop = self.range  # set in send_head()
 			copy_byte_range(source, outputfile, start, stop)
```

### Comparing `pyrobox-0.8.0/src/server.py` & `pyrobox-0.8.1/src/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,41 +4,34 @@
 
 
 # TODO
 # ----------------------------------------------------------------
 # * ADD MORE FILE TYPES
 # * ADD SEARCH
 
+
 import html
 from string import Template
 import os
 import sys
 import posixpath
 import shutil
 
-import time
 import datetime
 
 import importlib.util
-import re
 
 import urllib.parse
 import urllib.request
 
-import threading
-
 import subprocess
-import tempfile
-import random
-import string
 import json
 from http import HTTPStatus
 
 import traceback
-import atexit
 
 from .pyroboxCore import config, logger, SimpleHTTPRequestHandler as SH_base, DealPostData as DPD, run as run_server, tools, reload_server, __version__
 
 from ._fs_utils import get_titles, dir_navigator, get_dir_size, get_dir_m_time, get_stat, get_tree_count_n_size, _get_tree_path_n_size, fmbytes, humanbytes
 from ._arg_parser import main as arg_parser
 from . import _page_templates as pt
 from ._exceptions import LimitExceed
@@ -55,14 +48,15 @@
 arg_parser(config)
 cli_args = config.parser.parse_known_args()[0]
 config.PASSWORD = cli_args.password
 
 logger.info(tools.text_box("Server Config", *({i: getattr(cli_args, i)} for i in vars(cli_args))))
 
 ###########################################
+config.dev_mode = False
 pt.pt_config.dev_mode = config.dev_mode
 
 config.MAIN_FILE = os.path.abspath(__file__)
 
 config.disabled_func.update({
 			"send2trash": False,
 			"natsort": False,
```

