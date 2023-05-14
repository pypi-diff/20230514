# Comparing `tmp/ColdTOFU-0.0.6.tar.gz` & `tmp/ColdTOFU-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "M:\TOFU\dist\.tmp-ixtgccc0\ColdTOFU-0.0.6.tar", last modified: Wed Jan  4 13:19:42 2023, max compression
+gzip compressed data, was "M:\TOFU\dist\.tmp-x826499u\ColdTOFU-0.0.7.tar", last modified: Sun May 14 04:00:32 2023, max compression
```

## Comparing `ColdTOFU-0.0.6.tar` & `ColdTOFU-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-01-04 13:19:42.082034 ColdTOFU-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-01-04 13:19:42.029060 ColdTOFU-0.0.6/ColdTOFU/
--rw-rw-rw-   0        0        0   325120 2021-03-02 14:38:17.000000 ColdTOFU-0.0.6/ColdTOFU/ATSIFIO64.dll
--rw-rw-rw-   0        0        0    13468 2023-01-01 01:58:21.000000 ColdTOFU-0.0.6/ColdTOFU/AndorSifReader.py
--rw-rw-rw-   0        0        0    20578 2023-01-04 01:23:58.000000 ColdTOFU-0.0.6/ColdTOFU/Images.py
-drwxrwxrwx   0        0        0        0 2023-01-04 13:19:42.082034 ColdTOFU-0.0.6/ColdTOFU/Physics/
--rw-rw-rw-   0        0        0      147 2022-12-14 00:17:09.000000 ColdTOFU-0.0.6/ColdTOFU/Physics/__init__.py
--rw-rw-rw-   0        0        0     1912 2021-11-11 16:31:22.000000 ColdTOFU-0.0.6/ColdTOFU/Physics/allenDeviation.py
--rw-rw-rw-   0        0        0     3139 2022-10-03 02:29:50.000000 ColdTOFU-0.0.6/ColdTOFU/Physics/basisMatrices.py
--rw-rw-rw-   0        0        0     1167 2023-01-03 00:31:50.000000 ColdTOFU-0.0.6/ColdTOFU/Physics/beams.py
--rw-rw-rw-   0        0        0     1492 2021-11-28 17:34:02.000000 ColdTOFU-0.0.6/ColdTOFU/Physics/createAndDestroy.py
--rw-rw-rw-   0        0        0     4291 2022-10-01 03:17:35.000000 ColdTOFU-0.0.6/ColdTOFU/Physics/spinInDickeBasis.py
--rw-rw-rw-   0        0        0      232 2022-10-06 00:41:22.000000 ColdTOFU-0.0.6/ColdTOFU/__init__.py
--rw-rw-rw-   0        0        0    18001 2022-10-09 16:59:46.000000 ColdTOFU-0.0.6/ColdTOFU/fits.py
--rw-rw-rw-   0        0        0     1377 2022-10-03 02:24:29.000000 ColdTOFU-0.0.6/ColdTOFU/jupyterTools.py
--rw-rw-rw-   0        0        0     7007 2022-10-03 02:02:10.000000 ColdTOFU-0.0.6/ColdTOFU/numberOfAtoms.py
--rw-rw-rw-   0        0        0     2788 2022-10-03 02:17:53.000000 ColdTOFU-0.0.6/ColdTOFU/picoMatTools.py
--rw-rw-rw-   0        0        0      106 2022-09-23 11:41:22.000000 ColdTOFU-0.0.6/ColdTOFU/rcParams.json
--rw-rw-rw-   0        0        0     2767 2022-10-03 01:55:28.000000 ColdTOFU-0.0.6/ColdTOFU/sigma.py
--rw-rw-rw-   0        0        0     9059 2022-06-23 23:15:35.000000 ColdTOFU-0.0.6/ColdTOFU/spectrum.py
-drwxrwxrwx   0        0        0        0 2023-01-04 13:19:42.039117 ColdTOFU-0.0.6/ColdTOFU.egg-info/
--rw-rw-rw-   0        0        0      906 2023-01-04 13:19:41.000000 ColdTOFU-0.0.6/ColdTOFU.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      625 2023-01-04 13:19:41.000000 ColdTOFU-0.0.6/ColdTOFU.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-04 13:19:41.000000 ColdTOFU-0.0.6/ColdTOFU.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-01-04 13:19:41.000000 ColdTOFU-0.0.6/ColdTOFU.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-10-02 01:25:04.000000 ColdTOFU-0.0.6/LICENCE
--rw-rw-rw-   0        0        0       47 2022-10-02 04:02:42.000000 ColdTOFU-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      906 2023-01-04 13:19:42.082034 ColdTOFU-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      426 2022-10-10 00:34:29.000000 ColdTOFU-0.0.6/README.md
--rw-rw-rw-   0        0        0      108 2022-10-01 11:33:37.000000 ColdTOFU-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      579 2023-01-04 13:19:42.089062 ColdTOFU-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-14 04:00:32.392000 ColdTOFU-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-14 04:00:32.325310 ColdTOFU-0.0.7/ColdTOFU/
+-rw-rw-rw-   0        0        0   325120 2021-03-02 14:38:17.000000 ColdTOFU-0.0.7/ColdTOFU/ATSIFIO64.dll
+-rw-rw-rw-   0        0        0    13468 2023-01-01 01:58:21.000000 ColdTOFU-0.0.7/ColdTOFU/AndorSifReader.py
+-rw-rw-rw-   0        0        0    20578 2023-01-04 01:23:58.000000 ColdTOFU-0.0.7/ColdTOFU/Images.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:00:32.389992 ColdTOFU-0.0.7/ColdTOFU/Physics/
+-rw-rw-rw-   0        0        0      147 2022-12-14 00:17:09.000000 ColdTOFU-0.0.7/ColdTOFU/Physics/__init__.py
+-rw-rw-rw-   0        0        0     1912 2021-11-11 16:31:22.000000 ColdTOFU-0.0.7/ColdTOFU/Physics/allenDeviation.py
+-rw-rw-rw-   0        0        0     3139 2022-10-03 02:29:50.000000 ColdTOFU-0.0.7/ColdTOFU/Physics/basisMatrices.py
+-rw-rw-rw-   0        0        0     1167 2023-01-03 00:31:50.000000 ColdTOFU-0.0.7/ColdTOFU/Physics/beams.py
+-rw-rw-rw-   0        0        0     1492 2021-11-28 17:34:02.000000 ColdTOFU-0.0.7/ColdTOFU/Physics/createAndDestroy.py
+-rw-rw-rw-   0        0        0     4291 2022-10-01 03:17:35.000000 ColdTOFU-0.0.7/ColdTOFU/Physics/spinInDickeBasis.py
+-rw-rw-rw-   0        0        0      232 2022-10-06 00:41:22.000000 ColdTOFU-0.0.7/ColdTOFU/__init__.py
+-rw-rw-rw-   0        0        0    18001 2022-10-09 16:59:46.000000 ColdTOFU-0.0.7/ColdTOFU/fits.py
+-rw-rw-rw-   0        0        0     1377 2022-10-03 02:24:29.000000 ColdTOFU-0.0.7/ColdTOFU/jupyterTools.py
+-rw-rw-rw-   0        0        0     7007 2022-10-03 02:02:10.000000 ColdTOFU-0.0.7/ColdTOFU/numberOfAtoms.py
+-rw-rw-rw-   0        0        0     2780 2023-05-14 03:51:49.000000 ColdTOFU-0.0.7/ColdTOFU/picoMatTools.py
+-rw-rw-rw-   0        0        0      106 2022-09-23 11:41:22.000000 ColdTOFU-0.0.7/ColdTOFU/rcParams.json
+-rw-rw-rw-   0        0        0     2767 2022-10-03 01:55:28.000000 ColdTOFU-0.0.7/ColdTOFU/sigma.py
+-rw-rw-rw-   0        0        0     9059 2022-06-23 23:15:35.000000 ColdTOFU-0.0.7/ColdTOFU/spectrum.py
+drwxrwxrwx   0        0        0        0 2023-05-14 04:00:32.339011 ColdTOFU-0.0.7/ColdTOFU.egg-info/
+-rw-rw-rw-   0        0        0      906 2023-05-14 04:00:32.000000 ColdTOFU-0.0.7/ColdTOFU.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      625 2023-05-14 04:00:32.000000 ColdTOFU-0.0.7/ColdTOFU.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 04:00:32.000000 ColdTOFU-0.0.7/ColdTOFU.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-14 04:00:32.000000 ColdTOFU-0.0.7/ColdTOFU.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-10-02 01:25:04.000000 ColdTOFU-0.0.7/LICENCE
+-rw-rw-rw-   0        0        0       47 2022-10-02 04:02:42.000000 ColdTOFU-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      906 2023-05-14 04:00:32.392000 ColdTOFU-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2022-10-10 00:34:29.000000 ColdTOFU-0.0.7/README.md
+-rw-rw-rw-   0        0        0      108 2022-10-01 11:33:37.000000 ColdTOFU-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      662 2023-05-14 04:00:32.395001 ColdTOFU-0.0.7/setup.cfg
```

### Comparing `ColdTOFU-0.0.6/ColdTOFU/ATSIFIO64.dll` & `ColdTOFU-0.0.7/ColdTOFU/ATSIFIO64.dll`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU/AndorSifReader.py` & `ColdTOFU-0.0.7/ColdTOFU/AndorSifReader.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU/Images.py` & `ColdTOFU-0.0.7/ColdTOFU/Images.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU/Physics/allenDeviation.py` & `ColdTOFU-0.0.7/ColdTOFU/Physics/allenDeviation.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU/Physics/basisMatrices.py` & `ColdTOFU-0.0.7/ColdTOFU/Physics/basisMatrices.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU/Physics/beams.py` & `ColdTOFU-0.0.7/ColdTOFU/Physics/beams.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU/Physics/createAndDestroy.py` & `ColdTOFU-0.0.7/ColdTOFU/Physics/createAndDestroy.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU/Physics/spinInDickeBasis.py` & `ColdTOFU-0.0.7/ColdTOFU/Physics/spinInDickeBasis.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU/fits.py` & `ColdTOFU-0.0.7/ColdTOFU/fits.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU/jupyterTools.py` & `ColdTOFU-0.0.7/ColdTOFU/jupyterTools.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU/numberOfAtoms.py` & `ColdTOFU-0.0.7/ColdTOFU/numberOfAtoms.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU/picoMatTools.py` & `ColdTOFU-0.0.7/ColdTOFU/picoMatTools.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,11 +70,11 @@
     tStep = first['Tinterval']
     N = first['Length'][0,0]
     frequencies = fftfreq(N, tStep)[0,:int(N/2)]
     inLoop = []
     for f in files[:avg]:
         data = loadmat(os.path.join(path, f))
         inLoop.append(2*abs(fft(data[channel][:,0])[:N//2]/N)**2/np.mean(data[channel][:, 0])**2)
-        inLoopRIN = np.mean(np.array(inLoop), axis=0)
-        inLoopRIN[0], inLoopRIN[-1] = inLoopRIN[0]/2, inLoopRIN[-1]/2
+    inLoopRIN = np.mean(np.array(inLoop), axis=0)
+    inLoopRIN[0], inLoopRIN[-1] = inLoopRIN[0]/2, inLoopRIN[-1]/2
     return frequencies, 10*np.log10(inLoopRIN)
```

### Comparing `ColdTOFU-0.0.6/ColdTOFU/sigma.py` & `ColdTOFU-0.0.7/ColdTOFU/sigma.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU/spectrum.py` & `ColdTOFU-0.0.7/ColdTOFU/spectrum.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/ColdTOFU.egg-info/PKG-INFO` & `ColdTOFU-0.0.7/ColdTOFU.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColdTOFU
-Version: 0.0.6
+Version: 0.0.7
 Summary: Cold Atoms Time-of-Flight Utilities
 Home-page: https://github.com/chetanmadasu/TOFU
 Author: Chetan Sriram Madasu
 Author-email: chetan.madasu@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ColdTOFU-0.0.6/ColdTOFU.egg-info/SOURCES.txt` & `ColdTOFU-0.0.7/ColdTOFU.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/LICENCE` & `ColdTOFU-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.0.6/PKG-INFO` & `ColdTOFU-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColdTOFU
-Version: 0.0.6
+Version: 0.0.7
 Summary: Cold Atoms Time-of-Flight Utilities
 Home-page: https://github.com/chetanmadasu/TOFU
 Author: Chetan Sriram Madasu
 Author-email: chetan.madasu@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ColdTOFU-0.0.6/setup.cfg` & `ColdTOFU-0.0.7/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 6f6c 6454 4f46 550d 0a76 6572   = ColdTOFU..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e36 0d0a 6175  sion = 0.0.6..au
+00000020: 7369 6f6e 203d 2030 2e30 2e37 0d0a 6175  sion = 0.0.7..au
 00000030: 7468 6f72 203d 2043 6865 7461 6e20 5372  thor = Chetan Sr
 00000040: 6972 616d 204d 6164 6173 750d 0a61 7574  iram Madasu..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6368 6574  hor_email = chet
 00000060: 616e 2e6d 6164 6173 7540 676d 6169 6c2e  an.madasu@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2043 6f6c 6420 4174 6f6d 7320 5469   = Cold Atoms Ti
 00000090: 6d65 2d6f 662d 466c 6967 6874 2055 7469  me-of-Flight Uti
@@ -13,25 +13,30 @@
 000000c0: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
 000000d0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
 000000e0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
 000000f0: 2f6d 6172 6b64 6f77 6e0d 0a75 726c 203d  /markdown..url =
 00000100: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000110: 636f 6d2f 6368 6574 616e 6d61 6461 7375  com/chetanmadasu
 00000120: 2f54 4f46 550d 0a6c 6963 656e 7365 203d  /TOFU..license =
-00000130: 204d 4954 204c 6963 656e 7365 0d0a 636c   MIT License..cl
-00000140: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
-00000150: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000160: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000170: 2033 0d0a 094c 6963 656e 7365 203a 3a20   3...License :: 
-00000180: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000190: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
-000001a0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000001b0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-000001c0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
-000001d0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-000001e0: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-000001f0: 203d 203e 3d33 2e37 0d0a 696e 636c 7564   = >=3.7..includ
-00000200: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
-00000210: 2054 7275 650d 0a0d 0a5b 6567 675f 696e   True....[egg_in
-00000220: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000230: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000240: 0a0d 0a                                  ...
+00000130: 204d 4954 204c 6963 656e 7365 0d0a 696e   MIT License..in
+00000140: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+00000150: 205b 276e 756d 7079 272c 2027 7363 6970   ['numpy', 'scip
+00000160: 7927 2c20 2770 696c 6c6f 7727 2c20 2773  y', 'pillow', 's
+00000170: 796d 7079 272c 2027 6d61 7470 6c6f 746c  ympy', 'matplotl
+00000180: 6962 272c 2027 6970 7974 686f 6e27 5d0d  ib', 'ipython'].
+00000190: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+000001a0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000001b0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001c0: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
+000001d0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+000001e0: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
+000001f0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000200: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000210: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
+00000220: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+00000230: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
+00000240: 7265 7320 3d20 3e3d 332e 370d 0a69 6e63  res = >=3.7..inc
+00000250: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+00000260: 6120 3d20 5472 7565 0d0a 0d0a 5b65 6767  a = True....[egg
+00000270: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000280: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000290: 2030 0d0a 0d0a                            0....
```

