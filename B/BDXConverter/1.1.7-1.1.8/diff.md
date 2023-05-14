# Comparing `tmp/BDXConverter-1.1.7.tar.gz` & `tmp/BDXConverter-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDXConverter-1.1.7.tar", last modified: Sun May 14 02:19:33 2023, max compression
+gzip compressed data, was "BDXConverter-1.1.8.tar", last modified: Sun May 14 02:38:15 2023, max compression
```

## Comparing `BDXConverter-1.1.7.tar` & `BDXConverter-1.1.8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.623857 BDXConverter-1.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.615857 BDXConverter-1.1.7/BDXConverter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.615857 BDXConverter-1.1.7/BDXConverter/Converter/
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Converter/Converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Converter/ErrorClassDefine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Converter/FileOperation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Converter/Signature.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.615857 BDXConverter-1.1.7/BDXConverter/General/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/General/GeneralClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/General/Operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/General/Pool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/General/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.623857 BDXConverter-1.1.7/BDXConverter/Operation/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt16XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt16YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt16ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt16ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt32XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt32YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt32ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt32ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt8XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt8YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt8ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AssignDebugData.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/CreateConstantString.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/NOP.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithBlockStates.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithNBTData.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/SetCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/SubtractXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/SubtractYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/SubtractZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/UseRuntimeIDPool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/structOfChest.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.623857 BDXConverter-1.1.7/BDXConverter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/getByte.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/getString.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/marshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/marshalNBT_OldVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/unmarshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/unmarshalNBT_OldVersion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.615857 BDXConverter-1.1.7/BDXConverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-14 02:19:33.000000 BDXConverter-1.1.7/BDXConverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-14 02:19:33.000000 BDXConverter-1.1.7/BDXConverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 02:19:33.000000 BDXConverter-1.1.7/BDXConverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 02:19:33.000000 BDXConverter-1.1.7/BDXConverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-14 02:19:33.000000 BDXConverter-1.1.7/BDXConverter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-14 02:19:33.623857 BDXConverter-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 02:19:33.623857 BDXConverter-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.097141 BDXConverter-1.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.085140 BDXConverter-1.1.8/BDXConverter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.089141 BDXConverter-1.1.8/BDXConverter/Converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Converter/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Converter/ErrorClassDefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Converter/FileOperation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Converter/Signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.089141 BDXConverter-1.1.8/BDXConverter/General/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/General/GeneralClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/General/Operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/General/Pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/General/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.093141 BDXConverter-1.1.8/BDXConverter/Operation/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt16XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt16YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt16ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt16ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt32XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt32YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt32ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt32ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt8XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt8YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddInt8ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AddZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/AssignDebugData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/CreateConstantString.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/NOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithBlockStates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithNBTData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/SetCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/SubtractXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/SubtractYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/SubtractZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/UseRuntimeIDPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/Operation/structOfChest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.093141 BDXConverter-1.1.8/BDXConverter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/getByte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/getString.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/marshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/marshalNBT_OldVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/unmarshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/BDXConverter/utils/unmarshalNBT_OldVersion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:38:15.085140 BDXConverter-1.1.8/BDXConverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-05-14 02:38:15.000000 BDXConverter-1.1.8/BDXConverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-14 02:38:15.000000 BDXConverter-1.1.8/BDXConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 02:38:15.000000 BDXConverter-1.1.8/BDXConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 02:38:15.000000 BDXConverter-1.1.8/BDXConverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-14 02:38:15.000000 BDXConverter-1.1.8/BDXConverter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-05-14 02:38:15.097141 BDXConverter-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 02:38:15.097141 BDXConverter-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-14 02:38:03.000000 BDXConverter-1.1.8/setup.py
```

### Comparing `BDXConverter-1.1.7/BDXConverter/Converter/Converter.py` & `BDXConverter-1.1.8/BDXConverter/Converter/Converter.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Converter/ErrorClassDefine.py` & `BDXConverter-1.1.8/BDXConverter/Converter/ErrorClassDefine.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Converter/FileOperation.py` & `BDXConverter-1.1.8/BDXConverter/Converter/FileOperation.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Converter/Signature.py` & `BDXConverter-1.1.8/BDXConverter/Converter/Signature.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/General/GeneralClass.py` & `BDXConverter-1.1.8/BDXConverter/General/GeneralClass.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/General/Operation.py` & `BDXConverter-1.1.8/BDXConverter/General/Operation.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/General/Pool.py` & `BDXConverter-1.1.8/BDXConverter/General/Pool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/AddInt16XValue.py` & `BDXConverter-1.1.8/BDXConverter/Operation/AddInt16XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/AddInt16YValue.py` & `BDXConverter-1.1.8/BDXConverter/Operation/AddInt16YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/AddInt16ZValue.py` & `BDXConverter-1.1.8/BDXConverter/Operation/AddInt16ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/AddInt16ZValue0.py` & `BDXConverter-1.1.8/BDXConverter/Operation/AddInt16ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/AddInt32XValue.py` & `BDXConverter-1.1.8/BDXConverter/Operation/AddInt32XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/AddInt32YValue.py` & `BDXConverter-1.1.8/BDXConverter/Operation/AddInt32YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/AddInt32ZValue.py` & `BDXConverter-1.1.8/BDXConverter/Operation/AddInt32ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/AddInt32ZValue0.py` & `BDXConverter-1.1.8/BDXConverter/Operation/AddInt32ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/AddInt8XValue.py` & `BDXConverter-1.1.8/BDXConverter/Operation/AddInt8XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/AddInt8YValue.py` & `BDXConverter-1.1.8/BDXConverter/Operation/AddInt8YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/AddInt8ZValue.py` & `BDXConverter-1.1.8/BDXConverter/Operation/AddInt8ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/AssignDebugData.py` & `BDXConverter-1.1.8/BDXConverter/Operation/AssignDebugData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/CreateConstantString.py` & `BDXConverter-1.1.8/BDXConverter/Operation/CreateConstantString.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlock.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithBlockStates.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithBlockStates.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithChestData.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithNBTData.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithNBTData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithRuntimeId.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceBlockWithRuntimeId.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlock.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py` & `BDXConverter-1.1.8/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/SetCommandBlockData.py` & `BDXConverter-1.1.8/BDXConverter/Operation/SetCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/UseRuntimeIDPool.py` & `BDXConverter-1.1.8/BDXConverter/Operation/UseRuntimeIDPool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/Operation/structOfChest.py` & `BDXConverter-1.1.8/BDXConverter/Operation/structOfChest.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/utils/marshalNBT.py` & `BDXConverter-1.1.8/BDXConverter/utils/marshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/utils/marshalNBT_OldVersion.py` & `BDXConverter-1.1.8/BDXConverter/utils/marshalNBT_OldVersion.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/utils/unmarshalNBT.py` & `BDXConverter-1.1.8/BDXConverter/utils/unmarshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter/utils/unmarshalNBT_OldVersion.py` & `BDXConverter-1.1.8/BDXConverter/utils/unmarshalNBT_OldVersion.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/BDXConverter.egg-info/PKG-INFO` & `BDXConverter-1.1.8/BDXConverter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.1.7
+Version: 1.1.8
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -204,15 +204,15 @@
         """
         ...
 ```
 
 因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
 而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
 
-目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。 
+目前 `BDX Converter` 支持了所有的操作符，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` ，当前也包含 `签名` 相关的功能。
 
 
 
 
 
 # 什么是 `BDX` 文件
 `PhoenixBuilder` 是一个用于 `网易我的世界中国版 · 基岩版租赁服` 的商业化快速建造器，而 `BDX` 文件则是此建造器用于存储 `Minecraft` 建筑结构的 `私有文件格式` 。
```

### Comparing `BDXConverter-1.1.7/BDXConverter.egg-info/SOURCES.txt` & `BDXConverter-1.1.8/BDXConverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/LICENSE` & `BDXConverter-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.7/PKG-INFO` & `BDXConverter-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.1.7
+Version: 1.1.8
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -204,15 +204,15 @@
         """
         ...
 ```
 
 因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
 而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
 
-目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。 
+目前 `BDX Converter` 支持了所有的操作符，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` ，当前也包含 `签名` 相关的功能。
 
 
 
 
 
 # 什么是 `BDX` 文件
 `PhoenixBuilder` 是一个用于 `网易我的世界中国版 · 基岩版租赁服` 的商业化快速建造器，而 `BDX` 文件则是此建造器用于存储 `Minecraft` 建筑结构的 `私有文件格式` 。
```

### Comparing `BDXConverter-1.1.7/README.md` & `BDXConverter-1.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         """
         ...
 ```
 
 因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
 而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
 
-目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。 
+目前 `BDX Converter` 支持了所有的操作符，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` ，当前也包含 `签名` 相关的功能。
 
 
 
 
 
 # 什么是 `BDX` 文件
 `PhoenixBuilder` 是一个用于 `网易我的世界中国版 · 基岩版租赁服` 的商业化快速建造器，而 `BDX` 文件则是此建造器用于存储 `Minecraft` 建筑结构的 `私有文件格式` 。
```

### Comparing `BDXConverter-1.1.7/setup.py` & `BDXConverter-1.1.8/setup.py`

 * *Files identical despite different names*

