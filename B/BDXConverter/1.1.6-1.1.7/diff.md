# Comparing `tmp/BDXConverter-1.1.6.tar.gz` & `tmp/BDXConverter-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDXConverter-1.1.6.tar", last modified: Sat May 13 14:43:45 2023, max compression
+gzip compressed data, was "BDXConverter-1.1.7.tar", last modified: Sun May 14 02:19:33 2023, max compression
```

## Comparing `BDXConverter-1.1.6.tar` & `BDXConverter-1.1.7.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:43:45.258452 BDXConverter-1.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:43:45.226451 BDXConverter-1.1.6/BDXConverter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:43:45.234451 BDXConverter-1.1.6/BDXConverter/Converter/
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Converter/Converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Converter/ErrorClassDefine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Converter/FileOperation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Converter/Signature.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:43:45.234451 BDXConverter-1.1.6/BDXConverter/General/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/General/GeneralClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/General/Operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/General/Pool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/General/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:43:45.250451 BDXConverter-1.1.6/BDXConverter/Operation/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddInt16XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddInt16YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddInt16ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddInt16ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddInt32XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddInt32YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddInt32ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddInt32ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddInt8XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddInt8YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddInt8ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AddZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/AssignDebugData.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/CreateConstantString.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/NOP.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlockWithBlockStates.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlockWithNBTData.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceRuntimeBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/SetCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/SubtractXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/SubtractYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/SubtractZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/UseRuntimeIDPool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/Operation/structOfChest.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:43:45.254451 BDXConverter-1.1.6/BDXConverter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/utils/getByte.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/utils/getString.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/utils/marshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/utils/marshalNBT_OldVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/utils/unmarshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/BDXConverter/utils/unmarshalNBT_OldVersion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 14:43:45.230451 BDXConverter-1.1.6/BDXConverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-13 14:43:45.000000 BDXConverter-1.1.6/BDXConverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-13 14:43:45.000000 BDXConverter-1.1.6/BDXConverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 14:43:45.000000 BDXConverter-1.1.6/BDXConverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-13 14:43:45.000000 BDXConverter-1.1.6/BDXConverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-13 14:43:45.000000 BDXConverter-1.1.6/BDXConverter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-13 14:43:45.254451 BDXConverter-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 14:43:45.258452 BDXConverter-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-13 14:43:32.000000 BDXConverter-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.623857 BDXConverter-1.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.615857 BDXConverter-1.1.7/BDXConverter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.615857 BDXConverter-1.1.7/BDXConverter/Converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Converter/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Converter/ErrorClassDefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Converter/FileOperation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Converter/Signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.615857 BDXConverter-1.1.7/BDXConverter/General/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/General/GeneralClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/General/Operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/General/Pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/General/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.623857 BDXConverter-1.1.7/BDXConverter/Operation/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt16XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt16YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt16ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt16ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt32XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt32YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt32ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt32ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt8XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt8YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddInt8ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AddZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/AssignDebugData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/CreateConstantString.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/NOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithBlockStates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithNBTData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/SetCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/SubtractXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/SubtractYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/SubtractZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/UseRuntimeIDPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/Operation/structOfChest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.623857 BDXConverter-1.1.7/BDXConverter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/getByte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/getString.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/marshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/marshalNBT_OldVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/unmarshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/BDXConverter/utils/unmarshalNBT_OldVersion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 02:19:33.615857 BDXConverter-1.1.7/BDXConverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-14 02:19:33.000000 BDXConverter-1.1.7/BDXConverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-14 02:19:33.000000 BDXConverter-1.1.7/BDXConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 02:19:33.000000 BDXConverter-1.1.7/BDXConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 02:19:33.000000 BDXConverter-1.1.7/BDXConverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-14 02:19:33.000000 BDXConverter-1.1.7/BDXConverter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-14 02:19:33.623857 BDXConverter-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 02:19:33.623857 BDXConverter-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-14 02:19:22.000000 BDXConverter-1.1.7/setup.py
```

### Comparing `BDXConverter-1.1.6/BDXConverter/Converter/Converter.py` & `BDXConverter-1.1.7/BDXConverter/Converter/Converter.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Converter/ErrorClassDefine.py` & `BDXConverter-1.1.7/BDXConverter/Converter/ErrorClassDefine.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Converter/FileOperation.py` & `BDXConverter-1.1.7/BDXConverter/Converter/FileOperation.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Converter/Signature.py` & `BDXConverter-1.1.7/BDXConverter/Converter/Signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,17 +205,14 @@
             writer.write(newWriter.seek(0, 1).to_bytes(
                 length=1, byteorder='little', signed=False))
         # write the length of the sign content
         writer.write(b'\x5a')
         # write the number of this pseudo-operation
 
     def UnMarshal(self, buffer: BytesIO) -> None:
-        """
-        Note: We don't check the signature data
-        """
         nowSeek = buffer.seek(0, 1)
         buffer.seek(-1, 2)
         if getByte(buffer, 1) != b'\x5a':
             self.signedOrNeedToSign = False
             buffer.seek(nowSeek, 0)
             return
         else:
```

### Comparing `BDXConverter-1.1.6/BDXConverter/General/GeneralClass.py` & `BDXConverter-1.1.7/BDXConverter/General/GeneralClass.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/General/Operation.py` & `BDXConverter-1.1.7/BDXConverter/General/Operation.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/General/Pool.py` & `BDXConverter-1.1.7/BDXConverter/General/Pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .GeneralClass import GeneralClass
 from .Operation import *
 
 
 def GetBDXCommandPool() -> dict[int, GeneralClass]:
     """
-    Return dict[commandId(..operationId):int, PythonClass:GeneralClass]
+    Return dict[commandId(operationId):int, PythonClass:GeneralClass]
     """
     return {
         1: CreateConstantString(),
         5: PlaceBlockWithBlockStates(),
         6: AddInt16ZValue0(),
         7: PlaceBlock(),
         8: AddZValue0(),
```

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/AddInt16XValue.py` & `BDXConverter-1.1.7/BDXConverter/Operation/AddInt16XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/AddInt16YValue.py` & `BDXConverter-1.1.7/BDXConverter/Operation/AddInt16YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/AddInt16ZValue.py` & `BDXConverter-1.1.7/BDXConverter/Operation/AddInt16ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/AddInt16ZValue0.py` & `BDXConverter-1.1.7/BDXConverter/Operation/AddInt16ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/AddInt32XValue.py` & `BDXConverter-1.1.7/BDXConverter/Operation/AddInt32XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/AddInt32YValue.py` & `BDXConverter-1.1.7/BDXConverter/Operation/AddInt32YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/AddInt32ZValue.py` & `BDXConverter-1.1.7/BDXConverter/Operation/AddInt32ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/AddInt32ZValue0.py` & `BDXConverter-1.1.7/BDXConverter/Operation/AddInt32ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/AddInt8XValue.py` & `BDXConverter-1.1.7/BDXConverter/Operation/AddInt8XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/AddInt8YValue.py` & `BDXConverter-1.1.7/BDXConverter/Operation/AddInt8YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/AddInt8ZValue.py` & `BDXConverter-1.1.7/BDXConverter/Operation/AddInt8ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/AssignDebugData.py` & `BDXConverter-1.1.7/BDXConverter/Operation/AssignDebugData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/CreateConstantString.py` & `BDXConverter-1.1.7/BDXConverter/Operation/CreateConstantString.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlock.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlockWithBlockStates.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithBlockStates.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlockWithChestData.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlockWithNBTData.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithNBTData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceBlockWithRuntimeId.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceBlockWithRuntimeId.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceRuntimeBlock.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py` & `BDXConverter-1.1.7/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/SetCommandBlockData.py` & `BDXConverter-1.1.7/BDXConverter/Operation/SetCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/UseRuntimeIDPool.py` & `BDXConverter-1.1.7/BDXConverter/Operation/UseRuntimeIDPool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/Operation/structOfChest.py` & `BDXConverter-1.1.7/BDXConverter/Operation/structOfChest.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/utils/marshalNBT.py` & `BDXConverter-1.1.7/BDXConverter/utils/marshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/utils/marshalNBT_OldVersion.py` & `BDXConverter-1.1.7/BDXConverter/utils/marshalNBT_OldVersion.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/utils/unmarshalNBT.py` & `BDXConverter-1.1.7/BDXConverter/utils/unmarshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter/utils/unmarshalNBT_OldVersion.py` & `BDXConverter-1.1.7/BDXConverter/utils/unmarshalNBT_OldVersion.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/BDXConverter.egg-info/PKG-INFO` & `BDXConverter-1.1.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: BDXConverter
-Version: 1.1.6
-Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
-Home-page: https://github.com/TriM-Organization/BDXConverter
-Author: Minecraft Muti-Media Organization
-Author-email: TriM-Organization@hotmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">BDX Converter</h1>
 <h3 align="center">一个免费开源的 BDX 文件解析器</h3>
 <br/>
 <p align="center">
 <img src="https://forthebadge.com/images/badges/built-with-love.svg">
 <p>
 
@@ -38,14 +24,16 @@
 
 
 
 # 目录
 - [目录](#目录)
 - [`BDX Converter`](#bdx-converter)
 - [注意事项](#注意事项)
+  - [兼容性](#兼容性)
+  - [签名](#签名)
 - [快速上手](#快速上手)
 - [🐍 Pypi Packages](#-pypi-packages)
 - [第三方依赖](#第三方依赖)
 - [特性](#特性)
 - [什么是 `BDX` 文件](#什么是-bdx-文件)
 - [关于 `PhoenixBuilder`](#关于-phoenixbuilder)
 - [待办列表](#待办列表)
@@ -59,17 +47,79 @@
 `BDX Converter` 是一个轻量化的纯 `Python` 实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 
 
 
 
 # 注意事项
+## 兼容性
 - 版本 `1.1.0` 不兼容之前的所有版本
 - 版本 `1.0.16` 在可视化和反可视化字典方面不兼容之前的版本
 
+## 签名
+- `BDX` 文件格式是由 `PhoenixBuilder` 所定义，签名 `BDX` 文件则必须具备 `PhoenixBuilder` 账户
+- 由于一些原因，您需要自行获取 `签名` 时的 `Prove` 和 `PrivateSigningKey` ，以下展示了获取方法。有关本项目实现的签名功能，请见 [`BDXConverter/Converter/Signature.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Signature.py)
+
+  ```python
+  """
+  import ecdsa
+  
+  peer = ecdsa.SigningKey.generate(ecdsa.NIST384p)
+  verifyingKey = peer.get_verifying_key()
+  publicKey = verifyingKey.to_string().hex()
+  
+  print(publicKey)
+  # publicKey(...)
+  """
+  # Generate a new public key to send a auth request to the romote server
+  
+  
+  """
+  The address of PhoenixBuilder Auth server is wss://api.fastbuilder.pro:2053
+  """
+  # Address of PhoenixBuilder Auth server
+  
+  
+  """
+  Golang Structure
+  type AuthRequest struct {
+      Action         string `json:"action"`
+      ServerCode     string `json:"serverCode"`
+      ServerPassword string `json:"serverPassword"`
+      Key            string `json:"publicKey"`
+      FBToken        string
+  }
+
+  Python Dictionary
+  {
+      'action': 'phoenix::login',
+      'serverCode': ...,
+      'serverPassword': ...,
+      'publicKey': ...,
+      'FBToken': ...
+  }
+  """
+  # Send an auth request to the PhoenixBuilder Auth server
+  # Note: Must use GZIP to compress data when sending
+
+
+  """
+  Python Dictionary
+  {
+      'chainInfo': ...,
+      'code': ...,
+      'message': ...,
+      'privateSigningKey': ...,
+      'prove': ...
+  }
+  """
+  # The response of the PhoenixBuilder Auth server when the request succeeds
+  ```
+  - `PhoenixBuilder Auth Server` 使用了 `Cloudflared` 来代理(加速)它的 `Websocket` 服务器，因此您无法直接使用 `Python` 的 `Websocket` 库来连接此服务器。目前尚且未找到对应的解决办法，一个替代方案是使用 `Golang` 下的 `Websocket` 库与 `PhoenixBuilder Auth Server` 建立连接
+    - 其他帮助信息另见 https://github.com/huashengdun/webssh/issues/141
 
 
 
 
 # 快速上手
 您可以利用 [`BDXConverter/Converter/FileOperation.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/FileOperation.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。
```

### Comparing `BDXConverter-1.1.6/BDXConverter.egg-info/SOURCES.txt` & `BDXConverter-1.1.7/BDXConverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/LICENSE` & `BDXConverter-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.1.6/README.md` & `BDXConverter-1.1.7/BDXConverter.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: BDXConverter
+Version: 1.1.7
+Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
+Home-page: https://github.com/TriM-Organization/BDXConverter
+Author: Minecraft Muti-Media Organization
+Author-email: TriM-Organization@hotmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 align="center">BDX Converter</h1>
 <h3 align="center">一个免费开源的 BDX 文件解析器</h3>
 <br/>
 <p align="center">
 <img src="https://forthebadge.com/images/badges/built-with-love.svg">
 <p>
 
@@ -24,14 +38,16 @@
 
 
 
 # 目录
 - [目录](#目录)
 - [`BDX Converter`](#bdx-converter)
 - [注意事项](#注意事项)
+  - [兼容性](#兼容性)
+  - [签名](#签名)
 - [快速上手](#快速上手)
 - [🐍 Pypi Packages](#-pypi-packages)
 - [第三方依赖](#第三方依赖)
 - [特性](#特性)
 - [什么是 `BDX` 文件](#什么是-bdx-文件)
 - [关于 `PhoenixBuilder`](#关于-phoenixbuilder)
 - [待办列表](#待办列表)
@@ -45,17 +61,79 @@
 `BDX Converter` 是一个轻量化的纯 `Python` 实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 
 
 
 
 # 注意事项
+## 兼容性
 - 版本 `1.1.0` 不兼容之前的所有版本
 - 版本 `1.0.16` 在可视化和反可视化字典方面不兼容之前的版本
 
+## 签名
+- `BDX` 文件格式是由 `PhoenixBuilder` 所定义，签名 `BDX` 文件则必须具备 `PhoenixBuilder` 账户
+- 由于一些原因，您需要自行获取 `签名` 时的 `Prove` 和 `PrivateSigningKey` ，以下展示了获取方法。有关本项目实现的签名功能，请见 [`BDXConverter/Converter/Signature.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Signature.py)
+
+  ```python
+  """
+  import ecdsa
+  
+  peer = ecdsa.SigningKey.generate(ecdsa.NIST384p)
+  verifyingKey = peer.get_verifying_key()
+  publicKey = verifyingKey.to_string().hex()
+  
+  print(publicKey)
+  # publicKey(...)
+  """
+  # Generate a new public key to send a auth request to the romote server
+  
+  
+  """
+  The address of PhoenixBuilder Auth server is wss://api.fastbuilder.pro:2053
+  """
+  # Address of PhoenixBuilder Auth server
+  
+  
+  """
+  Golang Structure
+  type AuthRequest struct {
+      Action         string `json:"action"`
+      ServerCode     string `json:"serverCode"`
+      ServerPassword string `json:"serverPassword"`
+      Key            string `json:"publicKey"`
+      FBToken        string
+  }
+
+  Python Dictionary
+  {
+      'action': 'phoenix::login',
+      'serverCode': ...,
+      'serverPassword': ...,
+      'publicKey': ...,
+      'FBToken': ...
+  }
+  """
+  # Send an auth request to the PhoenixBuilder Auth server
+  # Note: Must use GZIP to compress data when sending
+
+
+  """
+  Python Dictionary
+  {
+      'chainInfo': ...,
+      'code': ...,
+      'message': ...,
+      'privateSigningKey': ...,
+      'prove': ...
+  }
+  """
+  # The response of the PhoenixBuilder Auth server when the request succeeds
+  ```
+  - `PhoenixBuilder Auth Server` 使用了 `Cloudflared` 来代理(加速)它的 `Websocket` 服务器，因此您无法直接使用 `Python` 的 `Websocket` 库来连接此服务器。目前尚且未找到对应的解决办法，一个替代方案是使用 `Golang` 下的 `Websocket` 库与 `PhoenixBuilder Auth Server` 建立连接
+    - 其他帮助信息另见 https://github.com/huashengdun/webssh/issues/141
 
 
 
 
 # 快速上手
 您可以利用 [`BDXConverter/Converter/FileOperation.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/FileOperation.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。
```

### Comparing `BDXConverter-1.1.6/setup.py` & `BDXConverter-1.1.7/setup.py`

 * *Files identical despite different names*

